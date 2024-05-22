# Comparing `tmp/eolymp-0.9.8.tar.gz` & `tmp/eolymp-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eolymp-0.9.8.tar", last modified: Tue Nov 21 12:08:17 2023, max compression
+gzip compressed data, was "eolymp-0.9.9.tar", last modified: Mon Dec  4 11:48:19 2023, max compression
```

## Comparing `eolymp-0.9.8.tar` & `eolymp-0.9.9.tar`

### file list

```diff
@@ -1,457 +1,461 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.911928 eolymp-0.9.8/
--rw-r--r--   0 root         (0) root         (0)      911 2023-11-21 12:08:17.911928 eolymp-0.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2023-11-21 12:08:17.000000 eolymp-0.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.799928 eolymp-0.9.8/eolymp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.803928 eolymp-0.9.8/eolymp/acl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/acl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2478 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/acl/acl_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6121 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/acl/acl_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/acl/acl_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      842 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/acl/entitlement_service_http.py
--rw-r--r--   0 root         (0) root         (0)     2215 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/acl/entitlement_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/acl/entitlement_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.807928 eolymp-0.9.8/eolymp/annotations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/annotations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/annotations/endpoint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/annotations/endpoint_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2308 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/annotations/http_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2402 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/annotations/http_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1536 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/annotations/ratelimit_pb2.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/annotations/ratelimit_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1462 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/annotations/scope_pb2.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/annotations/scope_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.807928 eolymp-0.9.8/eolymp/apollo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/apollo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/apollo/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/apollo/events_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.807928 eolymp-0.9.8/eolymp/asset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/asset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/asset/asset_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3919 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/asset/asset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/asset/asset_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.831928 eolymp-0.9.8/eolymp/atlas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/asset_service_http.py
--rw-r--r--   0 root         (0) root         (0)     5722 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/asset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3872 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/asset_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    25624 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/atlas_http.py
--rw-r--r--   0 root         (0) root         (0)    30705 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/atlas_pb2.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/atlas_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1239 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/attachment_pb2.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/attachment_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2564 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/attachment_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/attachment_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/attachment_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1132 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/bookmark_service_http.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/bookmark_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/bookmark_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1218 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/code_template_file_pb2.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/code_template_file_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1640 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/code_template_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/code_template_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2896 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/code_template_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7639 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/code_template_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/code_template_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1166 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/configuration_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3361 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/configuration_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/configuration_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1413 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/editorial_pb2.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/editorial_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3205 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/editorial_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8288 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/editorial_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4418 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/editorial_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1859 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2046 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/library_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8485 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/library_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7990 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/library_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2806 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/problem_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/problem_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2731 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/problem_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6445 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/problem_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/problem_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2921 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/problem_solver_http.py
--rw-r--r--   0 root         (0) root         (0)     6374 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/problem_solver_pb2.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/problem_solver_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1445 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/scoring_score_pb2.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/scoring_score_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1599 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/scoring_service_http.py
--rw-r--r--   0 root         (0) root         (0)     4335 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/scoring_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/scoring_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3181 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/snapshot_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/snapshot_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1725 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/solution_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/solution_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2518 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/solution_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7906 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/solution_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6144 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/solution_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1764 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/statement_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1539 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/statement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3195 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/statement_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/statement_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5202 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/statement_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5932 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/submission_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9709 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/submission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2105 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/submission_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/submission_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6145 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/submission_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2143 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/suggestion_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/suggestion_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3524 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/suggestion_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8400 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/suggestion_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/suggestion_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1155 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_config_pb2.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_config_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1244 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_feedback_pb2.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_feedback_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1270 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_scoring_pb2.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_scoring_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     7275 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_service_http.py
--rw-r--r--   0 root         (0) root         (0)    18070 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11063 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1372 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_test_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_test_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1867 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_testset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/testing_testset_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1443 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/version_pb2.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/atlas/version_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.835928 eolymp-0.9.8/eolymp/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/auth/claims_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/auth/claims_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      493 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/auth/oauth2_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6035 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/auth/oauth2_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5486 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/auth/oauth2_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      490 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/auth/sso_service_http.py
--rw-r--r--   0 root         (0) root         (0)     2894 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/auth/sso_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/auth/sso_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.839928 eolymp-0.9.8/eolymp/cognito/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/access_key_pb2.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/access_key_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8102 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/cognito_http.py
--rw-r--r--   0 root         (0) root         (0)    25530 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/cognito_pb2.py
--rw-r--r--   0 root         (0) root         (0)    21124 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/cognito_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1375 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1170 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/quota_pb2.py
--rw-r--r--   0 root         (0) root         (0)      482 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/quota_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2297 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/cognito/user_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.843928 eolymp-0.9.8/eolymp/commerce/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1525 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/price_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1062 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/price_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1564 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/product_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1230 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/product_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      494 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/product_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7366 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/product_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4361 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/product_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2914 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/subscription_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/subscription_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      499 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/subscription_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3799 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/subscription_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2016 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/commerce/subscription_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.855928 eolymp-0.9.8/eolymp/community/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4274 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/account_service_http.py
--rw-r--r--   0 root         (0) root         (0)    11733 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/account_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7023 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/account_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2632 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/attribute_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2568 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/attribute_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7127 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/attribute_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4511 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/attribute_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2046 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/configuration_identity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/configuration_identity_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2080 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/configuration_idp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/configuration_idp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1894 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/configuration_service_http.py
--rw-r--r--   0 root         (0) root         (0)     5816 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/configuration_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/configuration_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1696 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1255 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      675 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/group_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2474 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/group_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6783 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4142 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/group_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1158 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_ghost_pb2.py
--rw-r--r--   0 root         (0) root         (0)      379 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_ghost_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2302 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4017 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_service_http.py
--rw-r--r--   0 root         (0) root         (0)    11523 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9188 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1195 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_team_pb2.py
--rw-r--r--   0 root         (0) root         (0)      469 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_team_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2124 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/member_user_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1187 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/membership_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/membership_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1415 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/membership_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2592 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/subscription_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/subscription_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1322 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/subscription_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/subscription_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/subscription_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1413 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/tier_pb2.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/tier_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1708 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/tier_service_http.py
--rw-r--r--   0 root         (0) root         (0)     4510 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/tier_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/community/tier_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.855928 eolymp-0.9.8/eolymp/content/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/content/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3542 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/content/content_service_http.py
--rw-r--r--   0 root         (0) root         (0)    10435 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/content/content_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7524 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/content/content_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1411 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/content/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/content/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1450 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/content/fragment_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/content/fragment_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.855928 eolymp-0.9.8/eolymp/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/core/http_client.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/core/oauth_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.863928 eolymp-0.9.8/eolymp/course/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/course_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1879 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/course_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2479 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/course_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7539 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/course_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5287 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/course_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2182 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1145 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_problem_pb2.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_problem_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1313 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_section_pb2.py
--rw-r--r--   0 root         (0) root         (0)      642 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_section_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5062 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_service_http.py
--rw-r--r--   0 root         (0) root         (0)    12955 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8391 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1211 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_video_pb2.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/entry_video_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2021 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/student_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/student_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3142 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/student_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8943 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/student_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5864 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/course/student_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.867928 eolymp-0.9.8/eolymp/discussion/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/discussion_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/discussion_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3064 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/discussion_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8074 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/discussion_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4433 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/discussion_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1438 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1784 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/forum_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/forum_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2478 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/forum_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6622 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/forum_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3860 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/forum_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1825 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/message_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/message_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2979 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/message_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8680 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/message_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6502 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/message_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1442 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/subscription_pb2.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/subscription_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1185 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/subscription_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3644 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/subscription_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1289 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/discussion/subscription_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.871928 eolymp-0.9.8/eolymp/ecm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ecm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ecm/content_pb2.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ecm/content_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1487 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ecm/node_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ecm/node_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.875928 eolymp-0.9.8/eolymp/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      834 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2558 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/executor_http.py
--rw-r--r--   0 root         (0) root         (0)     8384 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/executor_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5724 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/executor_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1705 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/interactor_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/interactor_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6109 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11298 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/job_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1225 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/language_pb2.py
--rw-r--r--   0 root         (0) root         (0)      565 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/language_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5233 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/report_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7802 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/report_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1290 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/runtime_pb2.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/runtime_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3472 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5875 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/status_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3640 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/task_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/task_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1565 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/usage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/usage_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1950 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/verifier_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/executor/verifier_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.875928 eolymp-0.9.8/eolymp/geography/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/geography/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/geography/country_pb2.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/geography/country_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2233 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/geography/geography_http.py
--rw-r--r--   0 root         (0) root         (0)     4943 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/geography/geography_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2558 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/geography/geography_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1252 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/geography/region_pb2.py
--rw-r--r--   0 root         (0) root         (0)      660 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/geography/region_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.879928 eolymp-0.9.8/eolymp/harmony/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/harmony/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/harmony/agreement_pb2.py
--rw-r--r--   0 root         (0) root         (0)      686 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/harmony/agreement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1727 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/harmony/consent_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/harmony/consent_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2234 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/harmony/harmony_http.py
--rw-r--r--   0 root         (0) root         (0)     4871 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/harmony/harmony_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/harmony/harmony_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.883928 eolymp-0.9.8/eolymp/helpdesk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/auto_reply_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/auto_reply_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1458 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/document_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/document_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2439 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3573 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/helpdesk_http.py
--rw-r--r--   0 root         (0) root         (0)    10284 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/helpdesk_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7297 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/helpdesk_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8600 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/support_http.py
--rw-r--r--   0 root         (0) root         (0)    19983 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/support_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/support_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3595 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/ticket_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4215 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/helpdesk/ticket_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.891928 eolymp-0.9.8/eolymp/judge/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2389 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/activity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/activity_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1461 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/announcement_pb2.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/announcement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5432 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/contest_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8095 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/contest_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3508 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    34933 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/judge_http.py
--rw-r--r--   0 root         (0) root         (0)    76253 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/judge_pb2.py
--rw-r--r--   0 root         (0) root         (0)    56765 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/judge_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1247 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/medal_pb2.py
--rw-r--r--   0 root         (0) root         (0)      395 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/medal_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2610 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/participant_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/participant_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3084 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/problem_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/problem_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1519 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/reply_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/reply_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1718 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/result_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/result_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2586 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/score_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3589 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/score_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5763 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/submission_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9124 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/submission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1557 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/template_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/template_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1768 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/ticket_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/judge/ticket_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.891928 eolymp-0.9.8/eolymp/keeper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/keeper/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1257 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/keeper/blob_pb2.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/keeper/blob_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2965 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/keeper/keeper_http.py
--rw-r--r--   0 root         (0) root         (0)     7328 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/keeper/keeper_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4406 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/keeper/keeper_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.895928 eolymp-0.9.8/eolymp/l10n/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9434 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/localization_service_http.py
--rw-r--r--   0 root         (0) root         (0)    23464 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/localization_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15558 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/localization_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1252 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/project_pb2.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/project_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1267 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/project_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/project_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2221 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/project_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1460 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/term_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/term_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1851 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/translation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/l10n/translation_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.895928 eolymp-0.9.8/eolymp/oauth2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/oauth2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/oauth2/oauth2_http.py
--rw-r--r--   0 root         (0) root         (0)     8147 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/oauth2/oauth2_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9528 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/oauth2/oauth2_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.899928 eolymp-0.9.8/eolymp/playground/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/playground/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/playground/playground_http.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/playground/playground_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/playground/playground_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2162 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/playground/run_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/playground/run_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.903928 eolymp-0.9.8/eolymp/ranker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/activity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/activity_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1258 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1165 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/format_pb2.py
--rw-r--r--   0 root         (0) root         (0)      335 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/format_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8724 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/ranker_http.py
--rw-r--r--   0 root         (0) root         (0)    21385 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/ranker_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15143 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/ranker_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4866 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/scoreboard_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8094 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/ranker/scoreboard_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.903928 eolymp-0.9.8/eolymp/resolver/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/resolver/resolver_http.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/resolver/resolver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/resolver/resolver_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.903928 eolymp-0.9.8/eolymp/taxonomy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/enum_pb2.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/enum_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6676 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/enum_service_http.py
--rw-r--r--   0 root         (0) root         (0)    15135 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/enum_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10989 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/enum_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1625 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/enum_value_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/enum_value_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1145 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/link_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/link_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/taxonomy/link_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.907928 eolymp-0.9.8/eolymp/universe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/universe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1501 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/universe/permission_pb2.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/universe/permission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2559 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/universe/space_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3499 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/universe/space_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6381 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/universe/universe_http.py
--rw-r--r--   0 root         (0) root         (0)    14509 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/universe/universe_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9821 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/universe/universe_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.907928 eolymp-0.9.8/eolymp/wellknown/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/wellknown/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/wellknown/direction_pb2.py
--rw-r--r--   0 root         (0) root         (0)      331 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/wellknown/direction_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2426 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/wellknown/errors_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/wellknown/errors_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4481 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/wellknown/expression_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/wellknown/expression_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.911928 eolymp-0.9.8/eolymp/worker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/worker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/worker/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/worker/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2649 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/worker/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/worker/job_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2751 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/worker/worker_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/worker/worker_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp/worker/worker_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 12:08:17.803928 eolymp-0.9.8/eolymp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      911 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14055 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-11-21 12:08:17.000000 eolymp-0.9.8/eolymp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-21 12:08:17.911928 eolymp-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      974 2023-11-21 12:08:17.000000 eolymp-0.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.821753 eolymp-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-12-04 11:48:19.821753 eolymp-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-12-04 11:48:19.000000 eolymp-0.9.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.709753 eolymp-0.9.9/eolymp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.713753 eolymp-0.9.9/eolymp/acl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/acl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/acl/acl_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6121 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/acl/acl_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/acl/acl_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      842 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/acl/entitlement_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/acl/entitlement_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/acl/entitlement_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/acl/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/acl/events_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.717753 eolymp-0.9.9/eolymp/annotations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/annotations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/annotations/endpoint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/annotations/endpoint_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/annotations/http_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/annotations/http_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/annotations/ratelimit_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/annotations/ratelimit_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/annotations/scope_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/annotations/scope_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.717753 eolymp-0.9.9/eolymp/apollo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/apollo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/apollo/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/apollo/events_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.717753 eolymp-0.9.9/eolymp/asset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/asset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/asset/asset_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3919 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/asset/asset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/asset/asset_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.741753 eolymp-0.9.9/eolymp/atlas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/asset_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     5722 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/asset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/asset_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    25624 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/atlas_http.py
+-rw-r--r--   0 root         (0) root         (0)    30705 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/atlas_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/atlas_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/attachment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/attachment_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/attachment_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/attachment_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/attachment_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/bookmark_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/bookmark_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/bookmark_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/code_template_file_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/code_template_file_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/code_template_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/code_template_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2896 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/code_template_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7639 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/code_template_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/code_template_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/configuration_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3361 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/configuration_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/configuration_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/editorial_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/editorial_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/editorial_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8616 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/editorial_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/editorial_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/library_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8485 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/library_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7990 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/library_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/problem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/problem_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/problem_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6445 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/problem_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/problem_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/problem_solver_http.py
+-rw-r--r--   0 root         (0) root         (0)     6374 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/problem_solver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/problem_solver_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/scoring_score_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/scoring_score_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/scoring_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/scoring_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/scoring_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/snapshot_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/snapshot_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/solution_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/solution_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/solution_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/solution_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6144 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/solution_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/statement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/statement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/statement_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8908 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/statement_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5851 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/statement_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5932 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/submission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9709 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/submission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/submission_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/submission_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6145 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/submission_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/suggestion_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/suggestion_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/suggestion_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8400 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/suggestion_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/suggestion_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_config_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_config_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_feedback_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_feedback_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_scoring_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_scoring_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     7275 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    18070 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11063 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_test_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_test_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_testset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/testing_testset_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/version_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/atlas/version_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.741753 eolymp-0.9.9/eolymp/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/auth/claims_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/auth/claims_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      493 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/auth/oauth2_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/auth/oauth2_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5486 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/auth/oauth2_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      490 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/auth/sso_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/auth/sso_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/auth/sso_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.745753 eolymp-0.9.9/eolymp/cognito/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/access_key_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/access_key_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8102 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/cognito_http.py
+-rw-r--r--   0 root         (0) root         (0)    25530 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/cognito_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21124 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/cognito_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/quota_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      482 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/quota_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/cognito/user_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.749753 eolymp-0.9.9/eolymp/commerce/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/price_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/price_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/product_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/product_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      494 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/product_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7366 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/product_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4361 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/product_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2914 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/subscription_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/subscription_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      499 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/subscription_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/subscription_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/commerce/subscription_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.761753 eolymp-0.9.9/eolymp/community/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/account_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    11733 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/account_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7023 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/account_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/attribute_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/attribute_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/attribute_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4511 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/attribute_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/configuration_identity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/configuration_identity_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/configuration_idp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/configuration_idp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/configuration_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     5816 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/configuration_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/configuration_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      675 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/group_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/group_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4142 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/group_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1158 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_ghost_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_ghost_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    11523 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9188 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_team_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      469 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_team_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/member_user_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/membership_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/membership_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/membership_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/subscription_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/subscription_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/subscription_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/subscription_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/subscription_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/tier_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/tier_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/tier_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     4510 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/tier_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/community/tier_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.765753 eolymp-0.9.9/eolymp/content/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/content/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/content/content_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    10435 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/content/content_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/content/content_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/content/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/content/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/content/fragment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/content/fragment_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.765753 eolymp-0.9.9/eolymp/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/core/http_client.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/core/oauth_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.769753 eolymp-0.9.9/eolymp/course/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/course_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/course_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2479 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/course_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7539 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/course_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5287 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/course_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_problem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_problem_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_section_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      642 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_section_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5062 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    12955 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8391 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_video_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/entry_video_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/student_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/student_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/student_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8943 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/student_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5864 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/course/student_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.777753 eolymp-0.9.9/eolymp/discussion/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/discussion_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/discussion_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/discussion_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8074 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/discussion_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/discussion_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/forum_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/forum_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/forum_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6622 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/forum_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3860 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/forum_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/message_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/message_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/message_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8680 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/message_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6502 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/message_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/subscription_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/subscription_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/subscription_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/subscription_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/discussion/subscription_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.777753 eolymp-0.9.9/eolymp/ecm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ecm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ecm/content_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ecm/content_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ecm/node_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ecm/node_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.781753 eolymp-0.9.9/eolymp/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      834 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/executor_http.py
+-rw-r--r--   0 root         (0) root         (0)     8384 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/executor_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/executor_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/interactor_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/interactor_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6109 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11298 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/job_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/language_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      565 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/language_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5233 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/report_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/report_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/runtime_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/runtime_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3472 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5875 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/status_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/task_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/task_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/usage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/usage_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/verifier_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/executor/verifier_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.785753 eolymp-0.9.9/eolymp/geography/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/geography/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/geography/country_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/geography/country_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/geography/geography_http.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/geography/geography_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/geography/geography_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/geography/region_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      660 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/geography/region_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.785753 eolymp-0.9.9/eolymp/harmony/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/harmony/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/harmony/agreement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      686 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/harmony/agreement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/harmony/consent_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/harmony/consent_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/harmony/harmony_http.py
+-rw-r--r--   0 root         (0) root         (0)     4871 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/harmony/harmony_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/harmony/harmony_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.789753 eolymp-0.9.9/eolymp/helpdesk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/auto_reply_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/auto_reply_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/document_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/document_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/helpdesk_http.py
+-rw-r--r--   0 root         (0) root         (0)    10284 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/helpdesk_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7297 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/helpdesk_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8600 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/support_http.py
+-rw-r--r--   0 root         (0) root         (0)    19983 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/support_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/support_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/ticket_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/helpdesk/ticket_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.797753 eolymp-0.9.9/eolymp/judge/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/activity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/activity_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/announcement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/announcement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5432 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/contest_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/contest_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3508 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    34933 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/judge_http.py
+-rw-r--r--   0 root         (0) root         (0)    76253 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/judge_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    56765 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/judge_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/medal_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      395 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/medal_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/participant_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/participant_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/problem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/problem_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/reply_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/reply_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/result_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/result_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/score_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/score_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5763 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/submission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9124 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/submission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/template_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/template_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/ticket_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/judge/ticket_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.801753 eolymp-0.9.9/eolymp/keeper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/keeper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/keeper/blob_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/keeper/blob_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/keeper/keeper_http.py
+-rw-r--r--   0 root         (0) root         (0)     7328 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/keeper/keeper_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/keeper/keeper_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.805753 eolymp-0.9.9/eolymp/l10n/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9434 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/localization_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    23464 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/localization_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15558 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/localization_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/project_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/project_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/project_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/project_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/project_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/term_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/term_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/translation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/l10n/translation_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.805753 eolymp-0.9.9/eolymp/oauth2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/oauth2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/oauth2/oauth2_http.py
+-rw-r--r--   0 root         (0) root         (0)     8147 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/oauth2/oauth2_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9528 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/oauth2/oauth2_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.805753 eolymp-0.9.9/eolymp/playground/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/playground/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/playground/playground_http.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/playground/playground_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/playground/playground_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/playground/run_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/playground/run_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.809753 eolymp-0.9.9/eolymp/ranker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/activity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/activity_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/format_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      335 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/format_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8724 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/ranker_http.py
+-rw-r--r--   0 root         (0) root         (0)    21385 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/ranker_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15143 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/ranker_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/scoreboard_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8094 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/ranker/scoreboard_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.809753 eolymp-0.9.9/eolymp/resolver/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/resolver/resolver_http.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/resolver/resolver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/resolver/resolver_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.813753 eolymp-0.9.9/eolymp/taxonomy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/enum_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/enum_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/enum_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    15135 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/enum_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10989 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/enum_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/enum_value_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/enum_value_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/link_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/link_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/taxonomy/link_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.813753 eolymp-0.9.9/eolymp/universe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/permission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      921 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/permission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/space_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/space_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/universe_http.py
+-rw-r--r--   0 root         (0) root         (0)    14509 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/universe_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9821 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/universe/universe_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.817753 eolymp-0.9.9/eolymp/wellknown/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/wellknown/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/wellknown/direction_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      331 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/wellknown/direction_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/wellknown/errors_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/wellknown/errors_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/wellknown/expression_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/wellknown/expression_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.817753 eolymp-0.9.9/eolymp/worker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/worker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/worker/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/worker/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/worker/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/worker/job_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/worker/worker_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/worker/worker_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp/worker/worker_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 11:48:19.709753 eolymp-0.9.9/eolymp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14167 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-12-04 11:48:19.000000 eolymp-0.9.9/eolymp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-04 11:48:19.821753 eolymp-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      974 2023-12-04 11:48:19.000000 eolymp-0.9.9/setup.py
```

### Comparing `eolymp-0.9.8/PKG-INFO` & `eolymp-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eolymp
-Version: 0.9.8
+Version: 0.9.9
 Summary: Eolymp SDK for Python
 Home-page: https://github.com/eolymp/contracts
 Author: Sergey Kolodyazhnyy
 Author-email: sergey@eolymp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eolymp-0.9.8/README.md` & `eolymp-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/acl/acl_service_http.py` & `eolymp-0.9.9/eolymp/acl/acl_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/acl/acl_service_pb2.py` & `eolymp-0.9.9/eolymp/acl/acl_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/acl/acl_service_pb2.pyi` & `eolymp-0.9.9/eolymp/acl/acl_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/acl/entitlement_service_http.py` & `eolymp-0.9.9/eolymp/acl/entitlement_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/acl/entitlement_service_pb2.py` & `eolymp-0.9.9/eolymp/acl/entitlement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/acl/entitlement_service_pb2.pyi` & `eolymp-0.9.9/eolymp/acl/entitlement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/annotations/endpoint_pb2.py` & `eolymp-0.9.9/eolymp/annotations/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/annotations/endpoint_pb2.pyi` & `eolymp-0.9.9/eolymp/annotations/endpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/annotations/http_pb2.py` & `eolymp-0.9.9/eolymp/annotations/http_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/annotations/http_pb2.pyi` & `eolymp-0.9.9/eolymp/annotations/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/annotations/ratelimit_pb2.py` & `eolymp-0.9.9/eolymp/annotations/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/annotations/ratelimit_pb2.pyi` & `eolymp-0.9.9/eolymp/annotations/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/annotations/scope_pb2.py` & `eolymp-0.9.9/eolymp/annotations/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/annotations/scope_pb2.pyi` & `eolymp-0.9.9/eolymp/annotations/scope_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/apollo/events_pb2.py` & `eolymp-0.9.9/eolymp/apollo/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/apollo/events_pb2.pyi` & `eolymp-0.9.9/eolymp/apollo/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/asset/asset_service_http.py` & `eolymp-0.9.9/eolymp/asset/asset_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/asset/asset_service_pb2.py` & `eolymp-0.9.9/eolymp/asset/asset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/asset/asset_service_pb2.pyi` & `eolymp-0.9.9/eolymp/asset/asset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/asset_service_http.py` & `eolymp-0.9.9/eolymp/atlas/asset_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/asset_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/asset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/asset_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/asset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/atlas_http.py` & `eolymp-0.9.9/eolymp/atlas/atlas_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/atlas_pb2.py` & `eolymp-0.9.9/eolymp/atlas/atlas_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/atlas_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/atlas_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/attachment_pb2.py` & `eolymp-0.9.9/eolymp/atlas/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/attachment_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/attachment_service_http.py` & `eolymp-0.9.9/eolymp/atlas/attachment_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/attachment_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/attachment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/attachment_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/attachment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/bookmark_service_http.py` & `eolymp-0.9.9/eolymp/atlas/bookmark_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/bookmark_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/bookmark_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/bookmark_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/bookmark_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/code_template_file_pb2.py` & `eolymp-0.9.9/eolymp/atlas/code_template_file_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/code_template_file_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/code_template_file_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/code_template_pb2.py` & `eolymp-0.9.9/eolymp/atlas/code_template_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/code_template_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/code_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/code_template_service_http.py` & `eolymp-0.9.9/eolymp/atlas/code_template_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/code_template_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/code_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/code_template_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/code_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/configuration_service_http.py` & `eolymp-0.9.9/eolymp/atlas/configuration_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/configuration_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/configuration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/configuration_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/configuration_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/editorial_pb2.py` & `eolymp-0.9.9/eolymp/atlas/editorial_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/editorial_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/editorial_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/editorial_service_http.py` & `eolymp-0.9.9/eolymp/atlas/editorial_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/editorial_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/editorial_service_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.atlas import editorial_pb2 as eolymp_dot_atlas_dot_editorial__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$eolymp/atlas/editorial_service.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1c\x65olymp/atlas/editorial.proto\"6\n\x13ListEditorialsInput\x12\x0e\n\x06render\x18\x01 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"M\n\x14ListEditorialsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12&\n\x05items\x18\x02 \x03(\x0b\x32\x17.eolymp.atlas.Editorial\"O\n\x16\x44\x65scribeEditorialInput\x12\x14\n\x0c\x65\x64itorial_id\x18\x02 \x01(\t\x12\x0e\n\x06render\x18\x03 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"E\n\x17\x44\x65scribeEditorialOutput\x12*\n\teditorial\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"G\n\x14LookupEditorialInput\x12\x0e\n\x06locale\x18\x02 \x01(\t\x12\x0e\n\x06render\x18\x03 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"C\n\x15LookupEditorialOutput\x12*\n\teditorial\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"C\n\x15PreviewEditorialInput\x12*\n\teditorial\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"D\n\x16PreviewEditorialOutput\x12*\n\teditorial\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"B\n\x14\x43reateEditorialInput\x12*\n\teditorial\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"-\n\x15\x43reateEditorialOutput\x12\x14\n\x0c\x65\x64itorial_id\x18\x01 \x01(\t\"X\n\x14UpdateEditorialInput\x12\x14\n\x0c\x65\x64itorial_id\x18\x02 \x01(\t\x12*\n\teditorial\x18\x03 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"\x17\n\x15UpdateEditorialOutput\",\n\x14\x44\x65leteEditorialInput\x12\x14\n\x0c\x65\x64itorial_id\x18\x02 \x01(\t\"\x17\n\x15\x44\x65leteEditorialOutput2\x8b\t\n\x10\x45\x64itorialService\x12\x99\x01\n\x0f\x43reateEditorial\x12\".eolymp.atlas.CreateEditorialInput\x1a#.eolymp.atlas.CreateEditorialOutput\"=\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\r\x1a\x0b/editorials\x12\xa8\x01\n\x0fUpdateEditorial\x12\".eolymp.atlas.UpdateEditorialInput\x1a#.eolymp.atlas.UpdateEditorialOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c\x1a\x1a/editorials/{editorial_id}\x12\xa8\x01\n\x0f\x44\x65leteEditorial\x12\".eolymp.atlas.DeleteEditorialInput\x1a#.eolymp.atlas.DeleteEditorialOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c*\x1a/editorials/{editorial_id}\x12\xad\x01\n\x11\x44\x65scribeEditorial\x12$.eolymp.atlas.DescribeEditorialInput\x1a%.eolymp.atlas.DescribeEditorialOutput\"K\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1c\x12\x1a/editorials/{editorial_id}\x12\x97\x01\n\x0fLookupEditorial\x12\".eolymp.atlas.LookupEditorialInput\x1a#.eolymp.atlas.LookupEditorialOutput\";\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0c\x12\n/editorial\x12\xa2\x01\n\x10PreviewEditorial\x12#.eolymp.atlas.PreviewEditorialInput\x1a$.eolymp.atlas.PreviewEditorialOutput\"C\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x14\"\x12/editorial/preview\x12\x95\x01\n\x0eListEditorials\x12!.eolymp.atlas.ListEditorialsInput\x1a\".eolymp.atlas.ListEditorialsOutput\"<\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\r\x12\x0b/editorialsB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$eolymp/atlas/editorial_service.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1c\x65olymp/atlas/editorial.proto\"6\n\x13ListEditorialsInput\x12\x0e\n\x06render\x18\x01 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"M\n\x14ListEditorialsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12&\n\x05items\x18\x02 \x03(\x0b\x32\x17.eolymp.atlas.Editorial\"O\n\x16\x44\x65scribeEditorialInput\x12\x14\n\x0c\x65\x64itorial_id\x18\x02 \x01(\t\x12\x0e\n\x06render\x18\x03 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"E\n\x17\x44\x65scribeEditorialOutput\x12*\n\teditorial\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"G\n\x14LookupEditorialInput\x12\x0e\n\x06locale\x18\x02 \x01(\t\x12\x0e\n\x06render\x18\x03 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"C\n\x15LookupEditorialOutput\x12*\n\teditorial\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"C\n\x15PreviewEditorialInput\x12*\n\teditorial\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"D\n\x16PreviewEditorialOutput\x12*\n\teditorial\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"B\n\x14\x43reateEditorialInput\x12*\n\teditorial\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"-\n\x15\x43reateEditorialOutput\x12\x14\n\x0c\x65\x64itorial_id\x18\x01 \x01(\t\"\xcf\x01\n\x14UpdateEditorialInput\x12\x37\n\x05patch\x18\n \x03(\x0e\x32(.eolymp.atlas.UpdateEditorialInput.Patch\x12\x14\n\x0c\x65\x64itorial_id\x18\x02 \x01(\t\x12*\n\teditorial\x18\x03 \x01(\x0b\x32\x17.eolymp.atlas.Editorial\"<\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\n\n\x06LOCALE\x10\x01\x12\x0b\n\x07\x43ONTENT\x10\x02\x12\x11\n\rDOWNLOAD_LINK\x10\x03\"\x17\n\x15UpdateEditorialOutput\",\n\x14\x44\x65leteEditorialInput\x12\x14\n\x0c\x65\x64itorial_id\x18\x02 \x01(\t\"\x17\n\x15\x44\x65leteEditorialOutput2\x8b\t\n\x10\x45\x64itorialService\x12\x99\x01\n\x0f\x43reateEditorial\x12\".eolymp.atlas.CreateEditorialInput\x1a#.eolymp.atlas.CreateEditorialOutput\"=\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\r\x1a\x0b/editorials\x12\xa8\x01\n\x0fUpdateEditorial\x12\".eolymp.atlas.UpdateEditorialInput\x1a#.eolymp.atlas.UpdateEditorialOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c\x1a\x1a/editorials/{editorial_id}\x12\xa8\x01\n\x0f\x44\x65leteEditorial\x12\".eolymp.atlas.DeleteEditorialInput\x1a#.eolymp.atlas.DeleteEditorialOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c*\x1a/editorials/{editorial_id}\x12\xad\x01\n\x11\x44\x65scribeEditorial\x12$.eolymp.atlas.DescribeEditorialInput\x1a%.eolymp.atlas.DescribeEditorialOutput\"K\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1c\x12\x1a/editorials/{editorial_id}\x12\x97\x01\n\x0fLookupEditorial\x12\".eolymp.atlas.LookupEditorialInput\x1a#.eolymp.atlas.LookupEditorialOutput\";\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0c\x12\n/editorial\x12\xa2\x01\n\x10PreviewEditorial\x12#.eolymp.atlas.PreviewEditorialInput\x1a$.eolymp.atlas.PreviewEditorialOutput\"C\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x14\"\x12/editorial/preview\x12\x95\x01\n\x0eListEditorials\x12!.eolymp.atlas.ListEditorialsInput\x1a\".eolymp.atlas.ListEditorialsOutput\"<\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\r\x12\x0b/editorialsB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.atlas.editorial_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/atlas;atlas'
@@ -55,18 +55,20 @@
   _PREVIEWEDITORIALINPUT._serialized_end=679
   _PREVIEWEDITORIALOUTPUT._serialized_start=681
   _PREVIEWEDITORIALOUTPUT._serialized_end=749
   _CREATEEDITORIALINPUT._serialized_start=751
   _CREATEEDITORIALINPUT._serialized_end=817
   _CREATEEDITORIALOUTPUT._serialized_start=819
   _CREATEEDITORIALOUTPUT._serialized_end=864
-  _UPDATEEDITORIALINPUT._serialized_start=866
-  _UPDATEEDITORIALINPUT._serialized_end=954
-  _UPDATEEDITORIALOUTPUT._serialized_start=956
-  _UPDATEEDITORIALOUTPUT._serialized_end=979
-  _DELETEEDITORIALINPUT._serialized_start=981
-  _DELETEEDITORIALINPUT._serialized_end=1025
-  _DELETEEDITORIALOUTPUT._serialized_start=1027
-  _DELETEEDITORIALOUTPUT._serialized_end=1050
-  _EDITORIALSERVICE._serialized_start=1053
-  _EDITORIALSERVICE._serialized_end=2216
+  _UPDATEEDITORIALINPUT._serialized_start=867
+  _UPDATEEDITORIALINPUT._serialized_end=1074
+  _UPDATEEDITORIALINPUT_PATCH._serialized_start=1014
+  _UPDATEEDITORIALINPUT_PATCH._serialized_end=1074
+  _UPDATEEDITORIALOUTPUT._serialized_start=1076
+  _UPDATEEDITORIALOUTPUT._serialized_end=1099
+  _DELETEEDITORIALINPUT._serialized_start=1101
+  _DELETEEDITORIALINPUT._serialized_end=1145
+  _DELETEEDITORIALOUTPUT._serialized_start=1147
+  _DELETEEDITORIALOUTPUT._serialized_end=1170
+  _EDITORIALSERVICE._serialized_start=1173
+  _EDITORIALSERVICE._serialized_end=2336
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.9.8/eolymp/atlas/editorial_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/editorial_service_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
 from eolymp.atlas import editorial_pb2 as _editorial_pb2
 from google.protobuf.internal import containers as _containers
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class CreateEditorialInput(_message.Message):
@@ -88,17 +89,25 @@
 class PreviewEditorialOutput(_message.Message):
     __slots__ = ["editorial"]
     EDITORIAL_FIELD_NUMBER: _ClassVar[int]
     editorial: _editorial_pb2.Editorial
     def __init__(self, editorial: _Optional[_Union[_editorial_pb2.Editorial, _Mapping]] = ...) -> None: ...
 
 class UpdateEditorialInput(_message.Message):
-    __slots__ = ["editorial", "editorial_id"]
+    __slots__ = ["editorial", "editorial_id", "patch"]
+    class Patch(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+    ALL: UpdateEditorialInput.Patch
+    CONTENT: UpdateEditorialInput.Patch
+    DOWNLOAD_LINK: UpdateEditorialInput.Patch
     EDITORIAL_FIELD_NUMBER: _ClassVar[int]
     EDITORIAL_ID_FIELD_NUMBER: _ClassVar[int]
+    LOCALE: UpdateEditorialInput.Patch
+    PATCH_FIELD_NUMBER: _ClassVar[int]
     editorial: _editorial_pb2.Editorial
     editorial_id: str
-    def __init__(self, editorial_id: _Optional[str] = ..., editorial: _Optional[_Union[_editorial_pb2.Editorial, _Mapping]] = ...) -> None: ...
+    patch: _containers.RepeatedScalarFieldContainer[UpdateEditorialInput.Patch]
+    def __init__(self, patch: _Optional[_Iterable[_Union[UpdateEditorialInput.Patch, str]]] = ..., editorial_id: _Optional[str] = ..., editorial: _Optional[_Union[_editorial_pb2.Editorial, _Mapping]] = ...) -> None: ...
 
 class UpdateEditorialOutput(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
```

### Comparing `eolymp-0.9.8/eolymp/atlas/events_pb2.py` & `eolymp-0.9.9/eolymp/atlas/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/events_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/library_service_http.py` & `eolymp-0.9.9/eolymp/atlas/library_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/library_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/library_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/library_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/library_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/problem_pb2.py` & `eolymp-0.9.9/eolymp/atlas/problem_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/problem_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/problem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/problem_service_http.py` & `eolymp-0.9.9/eolymp/atlas/problem_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/problem_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/problem_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/problem_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/problem_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/problem_solver_http.py` & `eolymp-0.9.9/eolymp/atlas/problem_solver_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/problem_solver_pb2.py` & `eolymp-0.9.9/eolymp/atlas/problem_solver_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/problem_solver_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/problem_solver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/scoring_score_pb2.py` & `eolymp-0.9.9/eolymp/atlas/scoring_score_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/scoring_score_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/scoring_score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/scoring_service_http.py` & `eolymp-0.9.9/eolymp/atlas/scoring_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/scoring_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/scoring_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/scoring_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/scoring_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/snapshot_pb2.py` & `eolymp-0.9.9/eolymp/atlas/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/snapshot_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/solution_pb2.py` & `eolymp-0.9.9/eolymp/atlas/solution_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/solution_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/solution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/solution_service_http.py` & `eolymp-0.9.9/eolymp/atlas/solution_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/solution_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/solution_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/solution_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/solution_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/statement_pb2.py` & `eolymp-0.9.9/eolymp/taxonomy/enum_value_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/atlas/statement.proto
+# source: eolymp/taxonomy/enum_value.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from eolymp.ecm import content_pb2 as eolymp_dot_ecm_dot_content__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x65olymp/atlas/statement.proto\x12\x0c\x65olymp.atlas\x1a\x18\x65olymp/ecm/content.proto\"\xe6\x01\n\tStatement\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x0e\n\x06locale\x18\x03 \x01(\t\x12\r\n\x05title\x18\x04 \x01(\t\x12$\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x13.eolymp.ecm.Content\x12\x15\n\rdownload_link\x18\x07 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x65 \x01(\t\x12\x0e\n\x06source\x18\x66 \x01(\t\"=\n\x06\x46ormat\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03TEX\x10\x01\x12\x0c\n\x08MARKDOWN\x10\x02\x12\x08\n\x04HTML\x10\x03\x12\x08\n\x04RICH\x10\x04\x42-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/taxonomy/enum_value.proto\x12\x0f\x65olymp.taxonomy\"\xbf\x01\n\x05Value\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07summary\x18\x03 \x01(\t\x12\x0c\n\x04\x61\x62\x62r\x18\x05 \x01(\t\x12\r\n\x05image\x18\x06 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\t\x1a\\\n\x0bTranslation\x12\x0e\n\x06locale\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x61\x62\x62r\x18\x05 \x01(\t\x12\x0f\n\x07summary\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\tB3Z1github.com/eolymp/go-sdk/eolymp/taxonomy;taxonomyb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.atlas.statement_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.taxonomy.enum_value_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/atlas;atlas'
-  _STATEMENT._serialized_start=73
-  _STATEMENT._serialized_end=303
-  _STATEMENT_FORMAT._serialized_start=242
-  _STATEMENT_FORMAT._serialized_end=303
+  DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/taxonomy;taxonomy'
+  _VALUE._serialized_start=54
+  _VALUE._serialized_end=245
+  _VALUE_TRANSLATION._serialized_start=153
+  _VALUE_TRANSLATION._serialized_end=245
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.9.8/eolymp/atlas/statement_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/statement_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from eolymp.ecm import content_pb2 as _content_pb2
-from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Statement(_message.Message):
     __slots__ = ["author", "content", "download_link", "id", "locale", "problem_id", "source", "title"]
-    class Format(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
     AUTHOR_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     DOWNLOAD_LINK_FIELD_NUMBER: _ClassVar[int]
-    HTML: Statement.Format
     ID_FIELD_NUMBER: _ClassVar[int]
     LOCALE_FIELD_NUMBER: _ClassVar[int]
-    MARKDOWN: Statement.Format
-    NONE: Statement.Format
     PROBLEM_ID_FIELD_NUMBER: _ClassVar[int]
-    RICH: Statement.Format
     SOURCE_FIELD_NUMBER: _ClassVar[int]
-    TEX: Statement.Format
     TITLE_FIELD_NUMBER: _ClassVar[int]
     author: str
     content: _content_pb2.Content
     download_link: str
     id: str
     locale: str
     problem_id: str
```

### Comparing `eolymp-0.9.8/eolymp/atlas/statement_service_http.py` & `eolymp-0.9.9/eolymp/atlas/statement_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/statement_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/statement_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.atlas import statement_pb2 as eolymp_dot_atlas_dot_statement__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$eolymp/atlas/statement_service.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1c\x65olymp/atlas/statement.proto\"J\n\x13ListStatementsInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0e\n\x06render\x18\x02 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"M\n\x14ListStatementsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12&\n\x05items\x18\x02 \x03(\x0b\x32\x17.eolymp.atlas.Statement\"c\n\x16\x44\x65scribeStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x14\n\x0cstatement_id\x18\x02 \x01(\t\x12\x0e\n\x06render\x18\x03 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"E\n\x17\x44\x65scribeStatementOutput\x12*\n\tstatement\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"[\n\x14LookupStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0e\n\x06locale\x18\x02 \x01(\t\x12\x0e\n\x06render\x18\x03 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"C\n\x15LookupStatementOutput\x12*\n\tstatement\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"W\n\x15PreviewStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12*\n\tstatement\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"D\n\x16PreviewStatementOutput\x12*\n\tstatement\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"V\n\x14\x43reateStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12*\n\tstatement\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"-\n\x15\x43reateStatementOutput\x12\x14\n\x0cstatement_id\x18\x01 \x01(\t\"l\n\x14UpdateStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x14\n\x0cstatement_id\x18\x02 \x01(\t\x12*\n\tstatement\x18\x03 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"\x17\n\x15UpdateStatementOutput\"@\n\x14\x44\x65leteStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x14\n\x0cstatement_id\x18\x02 \x01(\t\"\x17\n\x15\x44\x65leteStatementOutput2\x81\t\n\x10StatementService\x12\x99\x01\n\x0f\x43reateStatement\x12\".eolymp.atlas.CreateStatementInput\x1a#.eolymp.atlas.CreateStatementOutput\"=\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\r\x1a\x0b/statements\x12\xa8\x01\n\x0fUpdateStatement\x12\".eolymp.atlas.UpdateStatementInput\x1a#.eolymp.atlas.UpdateStatementOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c\x1a\x1a/statements/{statement_id}\x12\xa8\x01\n\x0f\x44\x65leteStatement\x12\".eolymp.atlas.DeleteStatementInput\x1a#.eolymp.atlas.DeleteStatementOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c*\x1a/statements/{statement_id}\x12\xad\x01\n\x11\x44\x65scribeStatement\x12$.eolymp.atlas.DescribeStatementInput\x1a%.eolymp.atlas.DescribeStatementOutput\"K\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1c\x12\x1a/statements/{statement_id}\x12\x97\x01\n\x0fLookupStatement\x12\".eolymp.atlas.LookupStatementInput\x1a#.eolymp.atlas.LookupStatementOutput\";\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0c\x12\n/translate\x12\x98\x01\n\x10PreviewStatement\x12#.eolymp.atlas.PreviewStatementInput\x1a$.eolymp.atlas.PreviewStatementOutput\"9\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\n\"\x08/renders\x12\x95\x01\n\x0eListStatements\x12!.eolymp.atlas.ListStatementsInput\x1a\".eolymp.atlas.ListStatementsOutput\"<\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\r\x12\x0b/statementsB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$eolymp/atlas/statement_service.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1c\x65olymp/atlas/statement.proto\"J\n\x13ListStatementsInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0e\n\x06render\x18\x02 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"M\n\x14ListStatementsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12&\n\x05items\x18\x02 \x03(\x0b\x32\x17.eolymp.atlas.Statement\"c\n\x16\x44\x65scribeStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x14\n\x0cstatement_id\x18\x02 \x01(\t\x12\x0e\n\x06render\x18\x03 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"E\n\x17\x44\x65scribeStatementOutput\x12*\n\tstatement\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"[\n\x14LookupStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0e\n\x06locale\x18\x02 \x01(\t\x12\x0e\n\x06render\x18\x03 \x01(\x08\x12\x0f\n\x07version\x18\x64 \x01(\r\"C\n\x15LookupStatementOutput\x12*\n\tstatement\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"W\n\x15PreviewStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12*\n\tstatement\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"D\n\x16PreviewStatementOutput\x12*\n\tstatement\x18\x01 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"V\n\x14\x43reateStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12*\n\tstatement\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"-\n\x15\x43reateStatementOutput\x12\x14\n\x0cstatement_id\x18\x01 \x01(\t\"\x86\x02\n\x14UpdateStatementInput\x12\x37\n\x05patch\x18\n \x03(\x0e\x32(.eolymp.atlas.UpdateStatementInput.Patch\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x14\n\x0cstatement_id\x18\x02 \x01(\t\x12*\n\tstatement\x18\x03 \x01(\x0b\x32\x17.eolymp.atlas.Statement\"_\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\n\n\x06LOCALE\x10\x01\x12\t\n\x05TITLE\x10\x02\x12\x0b\n\x07\x43ONTENT\x10\x03\x12\x11\n\rDOWNLOAD_LINK\x10\x04\x12\n\n\x06\x41UTHOR\x10\x05\x12\n\n\x06SOURCE\x10\x06\"\x17\n\x15UpdateStatementOutput\"@\n\x14\x44\x65leteStatementInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x14\n\x0cstatement_id\x18\x02 \x01(\t\"\x17\n\x15\x44\x65leteStatementOutput2\x81\t\n\x10StatementService\x12\x99\x01\n\x0f\x43reateStatement\x12\".eolymp.atlas.CreateStatementInput\x1a#.eolymp.atlas.CreateStatementOutput\"=\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\r\x1a\x0b/statements\x12\xa8\x01\n\x0fUpdateStatement\x12\".eolymp.atlas.UpdateStatementInput\x1a#.eolymp.atlas.UpdateStatementOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c\x1a\x1a/statements/{statement_id}\x12\xa8\x01\n\x0f\x44\x65leteStatement\x12\".eolymp.atlas.DeleteStatementInput\x1a#.eolymp.atlas.DeleteStatementOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c*\x1a/statements/{statement_id}\x12\xad\x01\n\x11\x44\x65scribeStatement\x12$.eolymp.atlas.DescribeStatementInput\x1a%.eolymp.atlas.DescribeStatementOutput\"K\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1c\x12\x1a/statements/{statement_id}\x12\x97\x01\n\x0fLookupStatement\x12\".eolymp.atlas.LookupStatementInput\x1a#.eolymp.atlas.LookupStatementOutput\";\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0c\x12\n/translate\x12\x98\x01\n\x10PreviewStatement\x12#.eolymp.atlas.PreviewStatementInput\x1a$.eolymp.atlas.PreviewStatementOutput\"9\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\n\"\x08/renders\x12\x95\x01\n\x0eListStatements\x12!.eolymp.atlas.ListStatementsInput\x1a\".eolymp.atlas.ListStatementsOutput\"<\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\r\x12\x0b/statementsB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.atlas.statement_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/atlas;atlas'
@@ -55,18 +55,20 @@
   _PREVIEWSTATEMENTINPUT._serialized_end=759
   _PREVIEWSTATEMENTOUTPUT._serialized_start=761
   _PREVIEWSTATEMENTOUTPUT._serialized_end=829
   _CREATESTATEMENTINPUT._serialized_start=831
   _CREATESTATEMENTINPUT._serialized_end=917
   _CREATESTATEMENTOUTPUT._serialized_start=919
   _CREATESTATEMENTOUTPUT._serialized_end=964
-  _UPDATESTATEMENTINPUT._serialized_start=966
-  _UPDATESTATEMENTINPUT._serialized_end=1074
-  _UPDATESTATEMENTOUTPUT._serialized_start=1076
-  _UPDATESTATEMENTOUTPUT._serialized_end=1099
-  _DELETESTATEMENTINPUT._serialized_start=1101
-  _DELETESTATEMENTINPUT._serialized_end=1165
-  _DELETESTATEMENTOUTPUT._serialized_start=1167
-  _DELETESTATEMENTOUTPUT._serialized_end=1190
-  _STATEMENTSERVICE._serialized_start=1193
-  _STATEMENTSERVICE._serialized_end=2346
+  _UPDATESTATEMENTINPUT._serialized_start=967
+  _UPDATESTATEMENTINPUT._serialized_end=1229
+  _UPDATESTATEMENTINPUT_PATCH._serialized_start=1134
+  _UPDATESTATEMENTINPUT_PATCH._serialized_end=1229
+  _UPDATESTATEMENTOUTPUT._serialized_start=1231
+  _UPDATESTATEMENTOUTPUT._serialized_end=1254
+  _DELETESTATEMENTINPUT._serialized_start=1256
+  _DELETESTATEMENTINPUT._serialized_end=1320
+  _DELETESTATEMENTOUTPUT._serialized_start=1322
+  _DELETESTATEMENTOUTPUT._serialized_end=1345
+  _STATEMENTSERVICE._serialized_start=1348
+  _STATEMENTSERVICE._serialized_end=2501
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.9.8/eolymp/atlas/statement_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/statement_service_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
 from eolymp.atlas import statement_pb2 as _statement_pb2
 from google.protobuf.internal import containers as _containers
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class CreateStatementInput(_message.Message):
@@ -100,19 +101,30 @@
 class PreviewStatementOutput(_message.Message):
     __slots__ = ["statement"]
     STATEMENT_FIELD_NUMBER: _ClassVar[int]
     statement: _statement_pb2.Statement
     def __init__(self, statement: _Optional[_Union[_statement_pb2.Statement, _Mapping]] = ...) -> None: ...
 
 class UpdateStatementInput(_message.Message):
-    __slots__ = ["problem_id", "statement", "statement_id"]
+    __slots__ = ["patch", "problem_id", "statement", "statement_id"]
+    class Patch(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+    ALL: UpdateStatementInput.Patch
+    AUTHOR: UpdateStatementInput.Patch
+    CONTENT: UpdateStatementInput.Patch
+    DOWNLOAD_LINK: UpdateStatementInput.Patch
+    LOCALE: UpdateStatementInput.Patch
+    PATCH_FIELD_NUMBER: _ClassVar[int]
     PROBLEM_ID_FIELD_NUMBER: _ClassVar[int]
+    SOURCE: UpdateStatementInput.Patch
     STATEMENT_FIELD_NUMBER: _ClassVar[int]
     STATEMENT_ID_FIELD_NUMBER: _ClassVar[int]
+    TITLE: UpdateStatementInput.Patch
+    patch: _containers.RepeatedScalarFieldContainer[UpdateStatementInput.Patch]
     problem_id: str
     statement: _statement_pb2.Statement
     statement_id: str
-    def __init__(self, problem_id: _Optional[str] = ..., statement_id: _Optional[str] = ..., statement: _Optional[_Union[_statement_pb2.Statement, _Mapping]] = ...) -> None: ...
+    def __init__(self, patch: _Optional[_Iterable[_Union[UpdateStatementInput.Patch, str]]] = ..., problem_id: _Optional[str] = ..., statement_id: _Optional[str] = ..., statement: _Optional[_Union[_statement_pb2.Statement, _Mapping]] = ...) -> None: ...
 
 class UpdateStatementOutput(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
```

### Comparing `eolymp-0.9.8/eolymp/atlas/submission_pb2.py` & `eolymp-0.9.9/eolymp/atlas/submission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/submission_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/submission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/submission_service_http.py` & `eolymp-0.9.9/eolymp/atlas/submission_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/submission_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/submission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/submission_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/submission_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/suggestion_pb2.py` & `eolymp-0.9.9/eolymp/atlas/suggestion_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/suggestion_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/suggestion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/suggestion_service_http.py` & `eolymp-0.9.9/eolymp/atlas/suggestion_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/suggestion_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/suggestion_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/suggestion_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/suggestion_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_config_pb2.py` & `eolymp-0.9.9/eolymp/atlas/testing_config_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_feedback_pb2.py` & `eolymp-0.9.9/eolymp/atlas/testing_feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_scoring_pb2.py` & `eolymp-0.9.9/eolymp/atlas/testing_scoring_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_service_http.py` & `eolymp-0.9.9/eolymp/atlas/testing_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_service_pb2.py` & `eolymp-0.9.9/eolymp/atlas/testing_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_service_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/testing_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_test_pb2.py` & `eolymp-0.9.9/eolymp/atlas/testing_test_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_test_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/testing_test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_testset_pb2.py` & `eolymp-0.9.9/eolymp/atlas/testing_testset_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/testing_testset_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/testing_testset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/version_pb2.py` & `eolymp-0.9.9/eolymp/atlas/version_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/atlas/version_pb2.pyi` & `eolymp-0.9.9/eolymp/atlas/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/auth/claims_pb2.py` & `eolymp-0.9.9/eolymp/auth/claims_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/auth/claims_pb2.pyi` & `eolymp-0.9.9/eolymp/auth/claims_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/auth/oauth2_service_pb2.py` & `eolymp-0.9.9/eolymp/auth/oauth2_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/auth/oauth2_service_pb2.pyi` & `eolymp-0.9.9/eolymp/auth/oauth2_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/auth/sso_service_pb2.py` & `eolymp-0.9.9/eolymp/auth/sso_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/auth/sso_service_pb2.pyi` & `eolymp-0.9.9/eolymp/auth/sso_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/access_key_pb2.py` & `eolymp-0.9.9/eolymp/cognito/access_key_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/access_key_pb2.pyi` & `eolymp-0.9.9/eolymp/cognito/access_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/cognito_http.py` & `eolymp-0.9.9/eolymp/cognito/cognito_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/cognito_pb2.py` & `eolymp-0.9.9/eolymp/cognito/cognito_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/cognito_pb2.pyi` & `eolymp-0.9.9/eolymp/cognito/cognito_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/events_pb2.py` & `eolymp-0.9.9/eolymp/cognito/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/events_pb2.pyi` & `eolymp-0.9.9/eolymp/cognito/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/quota_pb2.py` & `eolymp-0.9.9/eolymp/cognito/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/user_pb2.py` & `eolymp-0.9.9/eolymp/cognito/user_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/cognito/user_pb2.pyi` & `eolymp-0.9.9/eolymp/cognito/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/events_pb2.py` & `eolymp-0.9.9/eolymp/commerce/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/events_pb2.pyi` & `eolymp-0.9.9/eolymp/commerce/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/price_pb2.py` & `eolymp-0.9.9/eolymp/commerce/price_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/price_pb2.pyi` & `eolymp-0.9.9/eolymp/commerce/price_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/product_pb2.py` & `eolymp-0.9.9/eolymp/commerce/product_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/product_pb2.pyi` & `eolymp-0.9.9/eolymp/commerce/product_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/product_service_pb2.py` & `eolymp-0.9.9/eolymp/commerce/product_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/product_service_pb2.pyi` & `eolymp-0.9.9/eolymp/commerce/product_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/subscription_pb2.py` & `eolymp-0.9.9/eolymp/commerce/subscription_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/subscription_pb2.pyi` & `eolymp-0.9.9/eolymp/commerce/subscription_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/subscription_service_pb2.py` & `eolymp-0.9.9/eolymp/commerce/subscription_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/commerce/subscription_service_pb2.pyi` & `eolymp-0.9.9/eolymp/commerce/subscription_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/account_service_http.py` & `eolymp-0.9.9/eolymp/community/account_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/account_service_pb2.py` & `eolymp-0.9.9/eolymp/community/account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/account_service_pb2.pyi` & `eolymp-0.9.9/eolymp/community/account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/attribute_pb2.py` & `eolymp-0.9.9/eolymp/community/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/attribute_pb2.pyi` & `eolymp-0.9.9/eolymp/community/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/attribute_service_http.py` & `eolymp-0.9.9/eolymp/community/attribute_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/attribute_service_pb2.py` & `eolymp-0.9.9/eolymp/community/attribute_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/attribute_service_pb2.pyi` & `eolymp-0.9.9/eolymp/community/attribute_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/configuration_identity_pb2.py` & `eolymp-0.9.9/eolymp/community/configuration_identity_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/configuration_identity_pb2.pyi` & `eolymp-0.9.9/eolymp/community/configuration_identity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/configuration_idp_pb2.py` & `eolymp-0.9.9/eolymp/community/configuration_idp_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/configuration_idp_pb2.pyi` & `eolymp-0.9.9/eolymp/community/configuration_idp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/configuration_service_http.py` & `eolymp-0.9.9/eolymp/community/configuration_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/configuration_service_pb2.py` & `eolymp-0.9.9/eolymp/community/configuration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/configuration_service_pb2.pyi` & `eolymp-0.9.9/eolymp/community/configuration_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/events_pb2.py` & `eolymp-0.9.9/eolymp/community/events_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,22 +10,26 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.community import member_pb2 as eolymp_dot_community_dot_member__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x65olymp/community/events.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/community/member.proto\">\n\x12MemberCreatedEvent\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\">\n\x12MemberUpdatedEvent\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\">\n\x12MemberDeletedEvent\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.MemberB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x65olymp/community/events.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/community/member.proto\">\n\x12MemberCreatedEvent\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\">\n\x12MemberUpdatedEvent\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\">\n\x12MemberDeletedEvent\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"\xcf\x01\n\x12MemberChangeRecord\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12:\n\x02op\x18\x02 \x01(\x0e\x32..eolymp.community.MemberChangeRecord.Operation\x12(\n\x06member\x18\x03 \x01(\x0b\x32\x18.eolymp.community.Member\"A\n\tOperation\x12\x10\n\x0cNO_OPERATION\x10\x00\x12\n\n\x06\x43REATE\x10\x01\x12\n\n\x06UPDATE\x10\x02\x12\n\n\x06\x44\x45LETE\x10\x03\x42\x35Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.events_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
   _MEMBERCREATEDEVENT._serialized_start=82
   _MEMBERCREATEDEVENT._serialized_end=144
   _MEMBERUPDATEDEVENT._serialized_start=146
   _MEMBERUPDATEDEVENT._serialized_end=208
   _MEMBERDELETEDEVENT._serialized_start=210
   _MEMBERDELETEDEVENT._serialized_end=272
+  _MEMBERCHANGERECORD._serialized_start=275
+  _MEMBERCHANGERECORD._serialized_end=482
+  _MEMBERCHANGERECORD_OPERATION._serialized_start=417
+  _MEMBERCHANGERECORD_OPERATION._serialized_end=482
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.9.8/eolymp/community/group_pb2.py` & `eolymp-0.9.9/eolymp/community/group_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/group_pb2.pyi` & `eolymp-0.9.9/eolymp/community/group_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/group_service_http.py` & `eolymp-0.9.9/eolymp/community/group_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/group_service_pb2.py` & `eolymp-0.9.9/eolymp/community/group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/group_service_pb2.pyi` & `eolymp-0.9.9/eolymp/community/group_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/member_ghost_pb2.py` & `eolymp-0.9.9/eolymp/community/member_ghost_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/member_pb2.py` & `eolymp-0.9.9/eolymp/community/member_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/member_pb2.pyi` & `eolymp-0.9.9/eolymp/community/member_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/member_service_http.py` & `eolymp-0.9.9/eolymp/community/member_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/member_service_pb2.py` & `eolymp-0.9.9/eolymp/community/member_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/member_service_pb2.pyi` & `eolymp-0.9.9/eolymp/community/member_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/member_team_pb2.py` & `eolymp-0.9.9/eolymp/community/member_team_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/member_user_pb2.py` & `eolymp-0.9.9/eolymp/community/member_user_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/member_user_pb2.pyi` & `eolymp-0.9.9/eolymp/community/member_user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/membership_service_http.py` & `eolymp-0.9.9/eolymp/community/membership_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/membership_service_pb2.py` & `eolymp-0.9.9/eolymp/community/membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/membership_service_pb2.pyi` & `eolymp-0.9.9/eolymp/community/membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/subscription_pb2.py` & `eolymp-0.9.9/eolymp/community/subscription_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/subscription_pb2.pyi` & `eolymp-0.9.9/eolymp/community/subscription_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/subscription_service_http.py` & `eolymp-0.9.9/eolymp/community/subscription_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/subscription_service_pb2.py` & `eolymp-0.9.9/eolymp/community/subscription_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/subscription_service_pb2.pyi` & `eolymp-0.9.9/eolymp/community/subscription_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/tier_pb2.py` & `eolymp-0.9.9/eolymp/community/tier_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/tier_pb2.pyi` & `eolymp-0.9.9/eolymp/community/tier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/tier_service_http.py` & `eolymp-0.9.9/eolymp/community/tier_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/tier_service_pb2.py` & `eolymp-0.9.9/eolymp/community/tier_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/community/tier_service_pb2.pyi` & `eolymp-0.9.9/eolymp/community/tier_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/content/content_service_http.py` & `eolymp-0.9.9/eolymp/content/content_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/content/content_service_pb2.py` & `eolymp-0.9.9/eolymp/content/content_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/content/content_service_pb2.pyi` & `eolymp-0.9.9/eolymp/content/content_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/content/events_pb2.py` & `eolymp-0.9.9/eolymp/content/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/content/events_pb2.pyi` & `eolymp-0.9.9/eolymp/content/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/content/fragment_pb2.py` & `eolymp-0.9.9/eolymp/content/fragment_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/content/fragment_pb2.pyi` & `eolymp-0.9.9/eolymp/content/fragment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/core/http_client.py` & `eolymp-0.9.9/eolymp/core/http_client.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/core/oauth_client.py` & `eolymp-0.9.9/eolymp/core/oauth_client.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/course_pb2.py` & `eolymp-0.9.9/eolymp/course/course_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/course_pb2.pyi` & `eolymp-0.9.9/eolymp/course/course_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/course_service_http.py` & `eolymp-0.9.9/eolymp/course/course_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/course_service_pb2.py` & `eolymp-0.9.9/eolymp/course/course_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/course_service_pb2.pyi` & `eolymp-0.9.9/eolymp/course/course_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_pb2.py` & `eolymp-0.9.9/eolymp/course/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_pb2.pyi` & `eolymp-0.9.9/eolymp/course/entry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_problem_pb2.py` & `eolymp-0.9.9/eolymp/course/entry_problem_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_section_pb2.py` & `eolymp-0.9.9/eolymp/course/entry_section_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_section_pb2.pyi` & `eolymp-0.9.9/eolymp/course/entry_section_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_service_http.py` & `eolymp-0.9.9/eolymp/course/entry_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_service_pb2.py` & `eolymp-0.9.9/eolymp/course/entry_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_service_pb2.pyi` & `eolymp-0.9.9/eolymp/course/entry_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_video_pb2.py` & `eolymp-0.9.9/eolymp/course/entry_video_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/entry_video_pb2.pyi` & `eolymp-0.9.9/eolymp/course/entry_video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/student_pb2.py` & `eolymp-0.9.9/eolymp/course/student_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/student_pb2.pyi` & `eolymp-0.9.9/eolymp/course/student_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/student_service_http.py` & `eolymp-0.9.9/eolymp/course/student_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/student_service_pb2.py` & `eolymp-0.9.9/eolymp/course/student_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/course/student_service_pb2.pyi` & `eolymp-0.9.9/eolymp/course/student_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/discussion_pb2.py` & `eolymp-0.9.9/eolymp/discussion/discussion_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/discussion_pb2.pyi` & `eolymp-0.9.9/eolymp/discussion/discussion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/discussion_service_http.py` & `eolymp-0.9.9/eolymp/discussion/discussion_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/discussion_service_pb2.py` & `eolymp-0.9.9/eolymp/discussion/discussion_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/discussion_service_pb2.pyi` & `eolymp-0.9.9/eolymp/discussion/discussion_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/events_pb2.py` & `eolymp-0.9.9/eolymp/discussion/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/events_pb2.pyi` & `eolymp-0.9.9/eolymp/discussion/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/forum_pb2.py` & `eolymp-0.9.9/eolymp/discussion/forum_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/forum_pb2.pyi` & `eolymp-0.9.9/eolymp/discussion/forum_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/forum_service_http.py` & `eolymp-0.9.9/eolymp/discussion/forum_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/forum_service_pb2.py` & `eolymp-0.9.9/eolymp/discussion/forum_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/forum_service_pb2.pyi` & `eolymp-0.9.9/eolymp/discussion/forum_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/message_pb2.py` & `eolymp-0.9.9/eolymp/discussion/message_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/message_pb2.pyi` & `eolymp-0.9.9/eolymp/discussion/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/message_service_http.py` & `eolymp-0.9.9/eolymp/discussion/message_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/message_service_pb2.py` & `eolymp-0.9.9/eolymp/discussion/message_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/message_service_pb2.pyi` & `eolymp-0.9.9/eolymp/discussion/message_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/subscription_pb2.py` & `eolymp-0.9.9/eolymp/discussion/subscription_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/subscription_pb2.pyi` & `eolymp-0.9.9/eolymp/discussion/subscription_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/subscription_service_http.py` & `eolymp-0.9.9/eolymp/discussion/subscription_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/subscription_service_pb2.py` & `eolymp-0.9.9/eolymp/discussion/subscription_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/discussion/subscription_service_pb2.pyi` & `eolymp-0.9.9/eolymp/discussion/subscription_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ecm/content_pb2.py` & `eolymp-0.9.9/eolymp/ecm/content_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ecm/content_pb2.pyi` & `eolymp-0.9.9/eolymp/ecm/content_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ecm/node_pb2.py` & `eolymp-0.9.9/eolymp/ecm/node_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ecm/node_pb2.pyi` & `eolymp-0.9.9/eolymp/ecm/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/events_pb2.py` & `eolymp-0.9.9/eolymp/executor/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/events_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/executor_http.py` & `eolymp-0.9.9/eolymp/executor/executor_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/executor_pb2.py` & `eolymp-0.9.9/eolymp/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/executor_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/executor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/interactor_pb2.py` & `eolymp-0.9.9/eolymp/executor/interactor_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/interactor_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/interactor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/job_pb2.py` & `eolymp-0.9.9/eolymp/executor/job_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/job_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/language_pb2.py` & `eolymp-0.9.9/eolymp/executor/language_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/language_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/language_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/report_pb2.py` & `eolymp-0.9.9/eolymp/executor/report_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/report_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/runtime_pb2.py` & `eolymp-0.9.9/eolymp/executor/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/runtime_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/runtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/status_pb2.py` & `eolymp-0.9.9/eolymp/executor/status_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/status_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/task_pb2.py` & `eolymp-0.9.9/eolymp/executor/task_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/task_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/usage_pb2.py` & `eolymp-0.9.9/eolymp/executor/usage_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/usage_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/usage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/verifier_pb2.py` & `eolymp-0.9.9/eolymp/executor/verifier_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/executor/verifier_pb2.pyi` & `eolymp-0.9.9/eolymp/executor/verifier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/geography/country_pb2.py` & `eolymp-0.9.9/eolymp/geography/country_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/geography/country_pb2.pyi` & `eolymp-0.9.9/eolymp/geography/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/geography/geography_http.py` & `eolymp-0.9.9/eolymp/geography/geography_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/geography/geography_pb2.py` & `eolymp-0.9.9/eolymp/geography/geography_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/geography/geography_pb2.pyi` & `eolymp-0.9.9/eolymp/geography/geography_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/geography/region_pb2.py` & `eolymp-0.9.9/eolymp/geography/region_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/geography/region_pb2.pyi` & `eolymp-0.9.9/eolymp/geography/region_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/harmony/agreement_pb2.py` & `eolymp-0.9.9/eolymp/harmony/agreement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/harmony/agreement_pb2.pyi` & `eolymp-0.9.9/eolymp/harmony/agreement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/harmony/consent_pb2.py` & `eolymp-0.9.9/eolymp/harmony/consent_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/harmony/consent_pb2.pyi` & `eolymp-0.9.9/eolymp/harmony/consent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/harmony/harmony_http.py` & `eolymp-0.9.9/eolymp/harmony/harmony_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/harmony/harmony_pb2.py` & `eolymp-0.9.9/eolymp/harmony/harmony_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/harmony/harmony_pb2.pyi` & `eolymp-0.9.9/eolymp/harmony/harmony_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/auto_reply_pb2.py` & `eolymp-0.9.9/eolymp/helpdesk/auto_reply_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/auto_reply_pb2.pyi` & `eolymp-0.9.9/eolymp/helpdesk/auto_reply_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/document_pb2.py` & `eolymp-0.9.9/eolymp/helpdesk/document_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/document_pb2.pyi` & `eolymp-0.9.9/eolymp/helpdesk/document_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/events_pb2.py` & `eolymp-0.9.9/eolymp/helpdesk/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/events_pb2.pyi` & `eolymp-0.9.9/eolymp/helpdesk/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/helpdesk_http.py` & `eolymp-0.9.9/eolymp/helpdesk/helpdesk_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/helpdesk_pb2.py` & `eolymp-0.9.9/eolymp/helpdesk/helpdesk_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/helpdesk_pb2.pyi` & `eolymp-0.9.9/eolymp/helpdesk/helpdesk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/support_http.py` & `eolymp-0.9.9/eolymp/helpdesk/support_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/support_pb2.py` & `eolymp-0.9.9/eolymp/helpdesk/support_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/support_pb2.pyi` & `eolymp-0.9.9/eolymp/helpdesk/support_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/ticket_pb2.py` & `eolymp-0.9.9/eolymp/helpdesk/ticket_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/helpdesk/ticket_pb2.pyi` & `eolymp-0.9.9/eolymp/helpdesk/ticket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/activity_pb2.py` & `eolymp-0.9.9/eolymp/judge/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/activity_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/activity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/announcement_pb2.py` & `eolymp-0.9.9/eolymp/judge/announcement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/announcement_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/announcement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/contest_pb2.py` & `eolymp-0.9.9/eolymp/judge/contest_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/contest_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/contest_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/events_pb2.py` & `eolymp-0.9.9/eolymp/judge/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/events_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/judge_http.py` & `eolymp-0.9.9/eolymp/judge/judge_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/judge_pb2.py` & `eolymp-0.9.9/eolymp/judge/judge_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/judge_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/judge_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/medal_pb2.py` & `eolymp-0.9.9/eolymp/judge/medal_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/participant_pb2.py` & `eolymp-0.9.9/eolymp/judge/participant_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/participant_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/participant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/problem_pb2.py` & `eolymp-0.9.9/eolymp/judge/problem_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/problem_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/problem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/reply_pb2.py` & `eolymp-0.9.9/eolymp/judge/reply_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/reply_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/reply_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/result_pb2.py` & `eolymp-0.9.9/eolymp/judge/result_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/result_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/score_pb2.py` & `eolymp-0.9.9/eolymp/judge/score_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/score_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/submission_pb2.py` & `eolymp-0.9.9/eolymp/judge/submission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/submission_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/submission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/template_pb2.py` & `eolymp-0.9.9/eolymp/judge/template_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/template_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/ticket_pb2.py` & `eolymp-0.9.9/eolymp/judge/ticket_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/judge/ticket_pb2.pyi` & `eolymp-0.9.9/eolymp/judge/ticket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/keeper/blob_pb2.py` & `eolymp-0.9.9/eolymp/keeper/blob_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/keeper/blob_pb2.pyi` & `eolymp-0.9.9/eolymp/keeper/blob_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/keeper/keeper_http.py` & `eolymp-0.9.9/eolymp/keeper/keeper_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/keeper/keeper_pb2.py` & `eolymp-0.9.9/eolymp/keeper/keeper_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/keeper/keeper_pb2.pyi` & `eolymp-0.9.9/eolymp/keeper/keeper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/localization_service_http.py` & `eolymp-0.9.9/eolymp/l10n/localization_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/localization_service_pb2.py` & `eolymp-0.9.9/eolymp/l10n/localization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/localization_service_pb2.pyi` & `eolymp-0.9.9/eolymp/l10n/localization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/project_pb2.py` & `eolymp-0.9.9/eolymp/l10n/project_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/project_pb2.pyi` & `eolymp-0.9.9/eolymp/l10n/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/project_service_http.py` & `eolymp-0.9.9/eolymp/l10n/project_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/project_service_pb2.py` & `eolymp-0.9.9/eolymp/l10n/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/project_service_pb2.pyi` & `eolymp-0.9.9/eolymp/l10n/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/term_pb2.py` & `eolymp-0.9.9/eolymp/l10n/term_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/term_pb2.pyi` & `eolymp-0.9.9/eolymp/l10n/term_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/translation_pb2.py` & `eolymp-0.9.9/eolymp/l10n/translation_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/l10n/translation_pb2.pyi` & `eolymp-0.9.9/eolymp/l10n/translation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/oauth2/oauth2_pb2.py` & `eolymp-0.9.9/eolymp/oauth2/oauth2_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/oauth2/oauth2_pb2.pyi` & `eolymp-0.9.9/eolymp/oauth2/oauth2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/playground/playground_http.py` & `eolymp-0.9.9/eolymp/playground/playground_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/playground/playground_pb2.py` & `eolymp-0.9.9/eolymp/playground/playground_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/playground/playground_pb2.pyi` & `eolymp-0.9.9/eolymp/playground/playground_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/playground/run_pb2.py` & `eolymp-0.9.9/eolymp/playground/run_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/playground/run_pb2.pyi` & `eolymp-0.9.9/eolymp/playground/run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/activity_pb2.py` & `eolymp-0.9.9/eolymp/ranker/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/activity_pb2.pyi` & `eolymp-0.9.9/eolymp/ranker/activity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/events_pb2.py` & `eolymp-0.9.9/eolymp/ranker/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/events_pb2.pyi` & `eolymp-0.9.9/eolymp/ranker/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/format_pb2.py` & `eolymp-0.9.9/eolymp/ranker/format_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/ranker_http.py` & `eolymp-0.9.9/eolymp/ranker/ranker_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/ranker_pb2.py` & `eolymp-0.9.9/eolymp/ranker/ranker_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/ranker_pb2.pyi` & `eolymp-0.9.9/eolymp/ranker/ranker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/scoreboard_pb2.py` & `eolymp-0.9.9/eolymp/ranker/scoreboard_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/ranker/scoreboard_pb2.pyi` & `eolymp-0.9.9/eolymp/ranker/scoreboard_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/resolver/resolver_http.py` & `eolymp-0.9.9/eolymp/resolver/resolver_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/resolver/resolver_pb2.py` & `eolymp-0.9.9/eolymp/resolver/resolver_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/resolver/resolver_pb2.pyi` & `eolymp-0.9.9/eolymp/resolver/resolver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/taxonomy/enum_pb2.py` & `eolymp-0.9.9/eolymp/taxonomy/enum_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/taxonomy/enum_service_http.py` & `eolymp-0.9.9/eolymp/taxonomy/enum_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/taxonomy/enum_service_pb2.py` & `eolymp-0.9.9/eolymp/taxonomy/enum_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/taxonomy/enum_service_pb2.pyi` & `eolymp-0.9.9/eolymp/taxonomy/enum_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/taxonomy/enum_value_pb2.pyi` & `eolymp-0.9.9/eolymp/taxonomy/enum_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/taxonomy/link_service_http.py` & `eolymp-0.9.9/eolymp/taxonomy/link_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/taxonomy/link_service_pb2.py` & `eolymp-0.9.9/eolymp/taxonomy/link_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/taxonomy/link_service_pb2.pyi` & `eolymp-0.9.9/eolymp/taxonomy/link_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/universe/permission_pb2.py` & `eolymp-0.9.9/eolymp/universe/permission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/universe/permission_pb2.pyi` & `eolymp-0.9.9/eolymp/universe/permission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/universe/space_pb2.py` & `eolymp-0.9.9/eolymp/universe/space_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/universe/space_pb2.pyi` & `eolymp-0.9.9/eolymp/universe/space_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/universe/universe_http.py` & `eolymp-0.9.9/eolymp/universe/universe_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/universe/universe_pb2.py` & `eolymp-0.9.9/eolymp/universe/universe_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/universe/universe_pb2.pyi` & `eolymp-0.9.9/eolymp/universe/universe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/wellknown/direction_pb2.py` & `eolymp-0.9.9/eolymp/wellknown/direction_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/wellknown/errors_pb2.py` & `eolymp-0.9.9/eolymp/wellknown/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/wellknown/errors_pb2.pyi` & `eolymp-0.9.9/eolymp/wellknown/errors_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/wellknown/expression_pb2.py` & `eolymp-0.9.9/eolymp/wellknown/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/wellknown/expression_pb2.pyi` & `eolymp-0.9.9/eolymp/wellknown/expression_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/worker/events_pb2.py` & `eolymp-0.9.9/eolymp/worker/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/worker/job_pb2.py` & `eolymp-0.9.9/eolymp/worker/job_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/worker/job_pb2.pyi` & `eolymp-0.9.9/eolymp/worker/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/worker/worker_service_http.py` & `eolymp-0.9.9/eolymp/worker/worker_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/worker/worker_service_pb2.py` & `eolymp-0.9.9/eolymp/worker/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp/worker/worker_service_pb2.pyi` & `eolymp-0.9.9/eolymp/worker/worker_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.9.8/eolymp.egg-info/PKG-INFO` & `eolymp-0.9.9/eolymp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eolymp
-Version: 0.9.8
+Version: 0.9.9
 Summary: Eolymp SDK for Python
 Home-page: https://github.com/eolymp/contracts
 Author: Sergey Kolodyazhnyy
 Author-email: sergey@eolymp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eolymp-0.9.8/eolymp.egg-info/SOURCES.txt` & `eolymp-0.9.9/eolymp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 eolymp/acl/__init__.py
 eolymp/acl/acl_service_http.py
 eolymp/acl/acl_service_pb2.py
 eolymp/acl/acl_service_pb2.pyi
 eolymp/acl/entitlement_service_http.py
 eolymp/acl/entitlement_service_pb2.py
 eolymp/acl/entitlement_service_pb2.pyi
+eolymp/acl/events_pb2.py
+eolymp/acl/events_pb2.pyi
 eolymp/annotations/__init__.py
 eolymp/annotations/endpoint_pb2.py
 eolymp/annotations/endpoint_pb2.pyi
 eolymp/annotations/http_pb2.py
 eolymp/annotations/http_pb2.pyi
 eolymp/annotations/ratelimit_pb2.py
 eolymp/annotations/ratelimit_pb2.pyi
@@ -395,14 +397,16 @@
 eolymp/taxonomy/enum_service_pb2.pyi
 eolymp/taxonomy/enum_value_pb2.py
 eolymp/taxonomy/enum_value_pb2.pyi
 eolymp/taxonomy/link_service_http.py
 eolymp/taxonomy/link_service_pb2.py
 eolymp/taxonomy/link_service_pb2.pyi
 eolymp/universe/__init__.py
+eolymp/universe/events_pb2.py
+eolymp/universe/events_pb2.pyi
 eolymp/universe/permission_pb2.py
 eolymp/universe/permission_pb2.pyi
 eolymp/universe/space_pb2.py
 eolymp/universe/space_pb2.pyi
 eolymp/universe/universe_http.py
 eolymp/universe/universe_pb2.py
 eolymp/universe/universe_pb2.pyi
```

### Comparing `eolymp-0.9.8/setup.py` & `eolymp-0.9.9/setup.py`

 * *Files identical despite different names*

