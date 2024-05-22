# Comparing `tmp/pdfservices-sdk-2.3.1.tar.gz` & `tmp/pdfservices_sdk-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfservices-sdk-2.3.1.tar", last modified: Thu Mar  7 11:18:47 2024, max compression
+gzip compressed data, was "pdfservices_sdk-4.0.0.tar", last modified: Wed May 22 06:48:05 2024, max compression
```

## Comparing `pdfservices-sdk-2.3.1.tar` & `pdfservices_sdk-4.0.0.tar`

### file list

```diff
@@ -1,115 +1,360 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.271345 pdfservices-sdk-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-07 11:18:47.271345 pdfservices-sdk-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 11:18:47.271345 pdfservices-sdk-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.259345 pdfservices-sdk-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.259345 pdfservices-sdk-2.3.1/src/adobe/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.259345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.259345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.259345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/auth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/auth/service_account_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/auth/service_principal_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/client_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.259345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/exception/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/exception/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.263345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.263345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.263345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.263345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.263345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.263345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.263345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/response/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.263345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/platform_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/storage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.263345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/auth/auth_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/auth/service_account_credentials_with_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/auth/service_principal_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/auth/session_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/constants/request_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/constants/service_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/http/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/http/http_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/http/http_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/http/request_header_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/http/response_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/internal_client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/internal_execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/io/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/io/file_ref_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/service/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/util/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/util/path_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/util/validation_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/io/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/io/file_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/autotag_pdf_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/extract_pdf_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/autotag_pdf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.267345 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_element_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_pdf_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_renditions_element_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/table_structure_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-07 11:18:33.000000 pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:18:47.271345 pdfservices-sdk-2.3.1/src/pdfservices_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-07 11:18:47.000000 pdfservices-sdk-2.3.1/src/pdfservices_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-03-07 11:18:47.000000 pdfservices-sdk-2.3.1/src/pdfservices_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 11:18:47.000000 pdfservices-sdk-2.3.1/src/pdfservices_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 11:18:47.000000 pdfservices-sdk-2.3.1/src/pdfservices_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-07 11:18:47.000000 pdfservices-sdk-2.3.1/src/pdfservices_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-07 11:18:47.000000 pdfservices-sdk-2.3.1/src/pdfservices_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.283106 pdfservices_sdk-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-22 06:48:05.283106 pdfservices_sdk-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 06:48:05.283106 pdfservices_sdk-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.227106 pdfservices_sdk-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.227106 pdfservices_sdk-4.0.0/src/adobe/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.227106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.231106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.231106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/auth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/auth/service_principal_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.231106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/client_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.231106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/notifier/callback_notifier_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/notifier/notifier_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/notifier/notifier_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/notifier/notifier_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.231106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/proxy/proxy_authentication_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/proxy/proxy_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/proxy/proxy_server_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/proxy/username_password_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.231106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/exception/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.235106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.235106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.235106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.235106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.235106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.235106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/combinepdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/combinepdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/combinepdf/combine_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/combinepdf/combine_pdf_internal_asset_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.235106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/compresspdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/compresspdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/compresspdf/compress_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/compresspdf/compress_pdf_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/compresspdf/compress_pdf_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.239106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/createpdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/createpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/createpdf/create_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/createpdf/create_pdf_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/createpdf/create_pdf_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.239106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/document_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/document_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/document_generation/document_generation_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/document_generation/document_generation_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/document_generation/document_generation_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.239106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/esealpdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/esealpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/esealpdf/eseal_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/esealpdf/eseal_pdf_internal_asset_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.239106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/exportpdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/exportpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/exportpdf/export_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/exportpdf/export_pdf_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/exportpdf/export_pdf_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.239106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf/extract_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf/extract_pdf_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf/extract_pdf_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.243106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/htmltopdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/htmltopdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/htmltopdf/html_to_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/htmltopdf/html_to_pdf_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/htmltopdf/html_to_pdf_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.243106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/linearizepdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/linearizepdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/linearizepdf/linearize_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/linearizepdf/linearize_pdf_internal_asset_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.243106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/ocrpdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/ocrpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/ocrpdf/ocr_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/ocrpdf/ocr_pdf_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/ocrpdf/ocr_pdf_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.243106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/delete_page_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/page_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/page_action_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/page_action_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/page_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/page_manipulation_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/page_manipulation_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/page_manipulation_params_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pagemanipulation/rotate_page_action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.247106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdf_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdf_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdf_properties/pdf_properties_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdf_properties/pdf_properties_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdf_properties/pdf_properties_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.247106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdf_services_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdf_services_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdf_services_api/pdf_services_api_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.247106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdftoimage/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdftoimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdftoimage/pdf_to_image_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdftoimage/pdf_to_image_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/pdftoimage/pdf_to_image_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.247106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/protect_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/protect_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/protect_pdf/protect_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/protect_pdf/protect_pdf_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/protect_pdf/protect_pdf_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.247106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/remove_protection/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/remove_protection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/remove_protection/remove_protection_extenal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/remove_protection/remove_protection_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/remove_protection/remove_protection_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.247106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/splitpdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/splitpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/splitpdf/split_pdf_external_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/splitpdf/split_pdf_internal_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/splitpdf/split_pdf_params_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.247106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/response/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.251106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/response/pdf_services_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/response/pdf_services_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/response/pdf_services_api/job_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/response/pdf_services_api/pdf_services_api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/pdf_services_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/storage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.251106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/auth/auth_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/auth/service_principal_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/auth/service_token_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/auth/service_token_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/auth/session_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.251106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/constants/custom_error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/constants/operation_header_info_endpoint_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/constants/pdf_services_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/constants/request_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/constants/service_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.255106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/http/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/http/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/http/request_header_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/http/response_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.255106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/params/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/params/combine_pdf_job_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/params/page_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21248 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/pdf_services_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.255106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/asset_upload_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/enforce_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/object_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/path_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/validation_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.255106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/io/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/io/cloud_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/io/external_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/io/external_storage_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/io/stream_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdf_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdf_services_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdf_services_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdf_services_job_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdf_services_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdf_services_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.255106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.259106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/autotag_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/combine_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/compress_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/create_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/delete_pages_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/document_merge_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/eseal_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/export_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/export_pdf_to_images_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/extract_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/html_to_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/insert_pages_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/linearize_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/ocr_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/pdf_properties_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/protect_pdf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/remove_protection_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/reorder_pages_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/replace_pages_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/rotate_pages_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/jobs/split_pdf_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.263106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.263106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/autotag_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/autotag_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/autotag_pdf/autotag_pdf_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.263106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/combine_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/combine_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/combine_pdf/combine_pdf_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.263106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/compress_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/compress_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/compress_pdf/compress_pdf_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/compress_pdf/compression_level.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.263106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/CreatePDFParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.263106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/excel/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/excel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/excel/create_pdf_from_excel_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/excel/document_language.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.263106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/ppt/create_pdf_from_ppt_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/ppt/document_language.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.263106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/word/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/word/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/word/create_pdf_from_word_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/create_pdf/word/document_language.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.267106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/delete_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/delete_pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/delete_pages/delete_pages_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.267106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/documentmerge/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/documentmerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/documentmerge/document_merge_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/documentmerge/fragments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/documentmerge/output_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.267106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/RFC3161_tsa_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/appearance_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/appearance_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/csc_auth_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/csc_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/document_level_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/electronic_seal_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/field_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/field_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/signature_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/tsa_basic_auth_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/eseal/tsa_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.271107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/export_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/export_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/export_pdf/export_ocr_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/export_pdf/export_pdf_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/export_pdf/export_pdf_target_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.271107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/extract_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/extract_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/extract_pdf/extract_element_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/extract_pdf/extract_pdf_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/extract_pdf/extract_renditions_element_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/extract_pdf/table_structure_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.271107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/html_to_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/html_to_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/html_to_pdf/html_to_pdf_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/html_to_pdf/page_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.271107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/insert_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/insert_pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/insert_pages/insert_pages_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.271107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/ocr_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/ocr_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/ocr_pdf/ocr_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/ocr_pdf/ocr_supported_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/ocr_pdf/ocr_supported_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/page_ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.271107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/pdf_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/pdf_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/pdf_properties/pdf_properties_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/pdf_services_job_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.271107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/pdf_to_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/pdf_to_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/pdf_to_image/export_pdf_to_images_output_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/pdf_to_image/export_pdf_to_images_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/pdf_to_image/export_pdf_to_images_target_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.275107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/protect_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/protect_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/protect_pdf/content_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/protect_pdf/encryption_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/protect_pdf/password_protect_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/protect_pdf/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/protect_pdf/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/protect_pdf/protect_pdf_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.275107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/remove_protection/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/remove_protection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/remove_protection/remove_protection_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.275107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/reorder_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/reorder_pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/reorder_pages/reorder_pages_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.275107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/replace_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/replace_pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/replace_pages/replace_pages_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.275107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/rotate_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/rotate_pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/rotate_pages/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/rotate_pages/rotate_pages_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.275107 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/split_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/split_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/params/split_pdf/split_pdf_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.279106 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/autotag_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/combine_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/compress_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/create_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/delete_pages_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/document_merge_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/eseal_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/export_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/export_pdf_to_images_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/extract_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/html_to_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/insert_pages_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/linearize_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/ocr_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/pdf_properties_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/pdf_services_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/protect_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/remove_protection_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/reorder_pages_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/replace_page_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/rotate_pages_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/pdfjobs/result/split_pdf_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-22 06:47:53.000000 pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:48:05.283106 pdfservices_sdk-4.0.0/src/pdfservices_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-22 06:48:05.000000 pdfservices_sdk-4.0.0/src/pdfservices_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21949 2024-05-22 06:48:05.000000 pdfservices_sdk-4.0.0/src/pdfservices_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:48:05.000000 pdfservices_sdk-4.0.0/src/pdfservices_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:48:05.000000 pdfservices_sdk-4.0.0/src/pdfservices_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 06:48:05.000000 pdfservices_sdk-4.0.0/src/pdfservices_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 06:48:05.000000 pdfservices_sdk-4.0.0/src/pdfservices_sdk.egg-info/top_level.txt
```

### Comparing `pdfservices-sdk-2.3.1/setup.py` & `pdfservices_sdk-4.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pdfservices-sdk",
-    version="2.3.1",
-    author='Adobe Document Services',
+    version="4.0.0",
+    author='Adobe Acrobat Services',
     author_email='extractapi@adobe.com',
     license='Apache2',
     description="Adobe PDFServices Client Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.adobe.com/go/pdftoolsapi_doc",
     package_dir={'': 'src'},
     packages=setuptools.find_packages('src'),
-    python_requires=">=3.6",
+    python_requires=">=3.10",
     install_requires=parse_requirements('requirements.txt', session=False),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     zip_safe=False
 )
```

### Comparing `pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/auth/credentials.py` & `pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/auth/service_principal_credentials.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-# Copyright 2021 Adobe. All rights reserved.
-# This file is licensed to you under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License. You may obtain a copy
-# of the License at http://www.apache.org/licenses/LICENSE-2.0
-# 
-# Unless required by applicable law or agreed to in writing, software distributed under
-# the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
-# OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
-
-from abc import ABC
-from adobe.pdfservices.operation.internal.util.validation_util import is_empty
-
-
-def _is_valid(value, name):
-    if is_empty(value):
-        raise ValueError(f'{name} must not be blank')
-    return value
+# Copyright 2024 Adobe
+# All Rights Reserved.
+#
+# NOTICE:  All information contained herein is, and remains
+# the property of Adobe and its suppliers, if any. The intellectual
+# and technical concepts contained herein are proprietary to Adobe
+# and its suppliers and are protected by all applicable intellectual
+# property laws, including trade secret and copyright laws.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Adobe.
+
+from adobe.pdfservices.operation.auth.credentials import Credentials
+from adobe.pdfservices.operation.internal.constants.custom_error_messages import CustomErrorMessages
+from adobe.pdfservices.operation.internal.util.enforce_types import enforce_types
+from adobe.pdfservices.operation.internal.util.string_util import StringUtil
 
 
-class Credentials(ABC):
+class ServicePrincipalCredentials(Credentials):
     """
-    Marker base class for different types of credentials. Currently it supports :class:`.ServiceAccountCredentials` and :class:`.ServicePrincipalCredentials`.
-    The factory methods within this class can be used to create instances of credentials classes.
+    Service Principal credentials allow your application to call PDF Services API. For getting the credentials,
+    `Click Here <https://www.adobe.com/go/dcsdks_credentials?ref=getStartedWithServicesSdk>`_.
     """
 
-    @staticmethod
-    def service_account_credentials_builder():
-        """ Creates a new :class:`.ServiceAccountCredentials` builder.
-
-        :return: An instance of ServiceAccountCredentials Builder.
-        :rtype: ServiceAccountCredentials.Builder
+    @enforce_types
+    def __init__(self, client_id: str, client_secret: str):
+        """
+        Constructs an instance of :samp:`ServicePrincipalCredentials`.
 
-        .. deprecated:: 2.3.0
-            Notice: JWT based service account credentials has been deprecated. Please use OAuth Server-to-Server based :class:`.ServicePrincipalCredentials`.
+        :param client_id: client ID for ServicePrincipalCredentials; can not be None or empty.
+        :type client_id: str
+        :param client_secret: client secret for ServicePrincipalCredentials; can not be None or empty.
+        :type client_secret: str
         """
-        from adobe.pdfservices.operation.auth.service_account_credentials import ServiceAccountCredentials
-        return ServiceAccountCredentials.Builder()
+        if StringUtil.is_blank(client_id):
+            raise ValueError(CustomErrorMessages.GENERIC_CAN_NOT_BE_NONE_OR_EMPTY.format("Client ID"))
+        if StringUtil.is_blank(client_secret):
+            raise ValueError(CustomErrorMessages.GENERIC_CAN_NOT_BE_NONE_OR_EMPTY.format("Client Secret"))
+
+        self.__client_id: str = client_id
+        self.__client_secret: str = client_secret
 
-    @staticmethod
-    def service_principal_credentials_builder():
-        """ Creates a new :class:`.ServicePrincipalCredentials` builder.
+    def get_client_id(self):
+        """
+        :return: Client Id
+        :rtype: str
+        """
+        return self.__client_id
 
-        :return: An instance of ServicePrincipalCredentials Builder.
-        :rtype: ServicePrincipalCredentials.Builder
+    def get_client_secret(self):
+        """
+        :return: Client Secret
+        :rtype: str
         """
-        from adobe.pdfservices.operation.auth.service_principal_credentials import ServicePrincipalCredentials
-        return ServicePrincipalCredentials.Builder()
+        return self.__client_secret
```

### Comparing `pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/client_config.py` & `pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/config/client_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-# Copyright 2021 Adobe. All rights reserved.
-# This file is licensed to you under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License. You may obtain a copy
-# of the License at http://www.apache.org/licenses/LICENSE-2.0
+# Copyright 2024 Adobe
+# All Rights Reserved.
 #
-# Unless required by applicable law or agreed to in writing, software distributed under
-# the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
-# OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# NOTICE:  All information contained herein is, and remains
+# the property of Adobe and its suppliers, if any. The intellectual
+# and technical concepts contained herein are proprietary to Adobe
+# and its suppliers and are protected by all applicable intellectual
+# property laws, including trade secret and copyright laws.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Adobe.
+
 import json
 
+from adobe.pdfservices.operation.config.proxy.proxy_server_config import ProxyServerConfig
+from adobe.pdfservices.operation.internal.constants.custom_error_messages import CustomErrorMessages
+from adobe.pdfservices.operation.internal.constants.pdf_services_uri import PDFServicesURI
 from adobe.pdfservices.operation.internal.constants.service_constants import ServiceConstants
 from adobe.pdfservices.operation.internal.util import file_utils
+from adobe.pdfservices.operation.internal.util.enforce_types import enforce_types
+from adobe.pdfservices.operation.internal.util.string_util import StringUtil
 from adobe.pdfservices.operation.region import Region
 
 
-class ClientConfig(object):
+class ClientConfig:
     """
-    Encapsulates the API request configurations
+    Encapsulates the API request configurations.
     """
+    _PDF_SERVICES = "pdfServices"
+    _PDF_SERVICES_URI = "pdfServicesUri"
     _CONNECT_TIMEOUT_KEY = "connectTimeout"
     _READ_TIMEOUT_KEY = "readTimeout"
-    _PROCESSING_TIMEOUT_KEY = "processingTimeout"
-    _PDF_SERVICES = "pdf_services"
-    _PDF_SERVICES_URI = "pdf_services_uri"
+    _PROXY_HOST = "host"
+    _PROXY_SERVER_CONFIG = "proxyServerConfig"
+    _PROXY_PORT = "port"
+    _PROXY_SCHEME = "proxyScheme"
     _REGION = "region"
+    _PROXY_CREDENTIALS = "usernamePasswordCredentials"
+    _PROXY_USERNAME = "username"
+    _PROXY_PASSWORD = "password"
+
+    @enforce_types
+    def __init__(self, *,
+                 connect_timeout: int = ServiceConstants.HTTP_CONNECT_TIMEOUT,
+                 read_timeout: int = ServiceConstants.HTTP_READ_TIMEOUT,
+                 region: Region = Region.US,
+                 proxy_server_config: ProxyServerConfig = None):
+        """
+        Constructs an instance of :samp:`ClientConfig`.
 
-    @staticmethod
-    def builder():
-        """Creates a new :class:`ClientConfig` builder.
+        :param connect_timeout: determines the timeout in milliseconds until a connection is established in the API
+            calls. Default value is 4000 milliseconds.
+        :type connect_timeout: int
+        :param read_timeout: Defines the read timeout in milliseconds, The number of milliseconds the client will \
+                wait for the server to send a response after the connection is established.\
+                Default value is 10000 milliseconds
+        :type read_timeout: int
+        :param region: Default value is US.
+        :type region: Region
+        :param proxy_server_config: Sets the configuration for proxy server.
+        :type proxy_server_config: ProxyServerConfig
+        """
+        self._connect_timeout = connect_timeout
+        self._read_timeout = read_timeout
+        self._pdf_services_uri = PDFServicesURI.get_uri_for_region(region)
+        self._proxy_server_config = proxy_server_config
 
-        :return: A ClientConfig.Builder instance.
-        :rtype: ClientConfig.Builder
+    def get_pdf_services_uri(self):
         """
-        return ClientConfig.Builder()
+        :return: The PDF Service URI used.
+        :rtype: str
+        """
+        return self._pdf_services_uri
 
-    def __init__(self):
-        return
+    def get_connect_timeout(self):
+        """
+        :return: Connect timeout.
+        :rtype: int
+        """
+        return self._connect_timeout / 1000 if self._connect_timeout else None
 
-    class Builder:
+    def get_read_timeout(self):
         """
-        Builds a :class:`ClientConfig` instance.
+        :return: Read timeout.
+        :rtype: int
         """
-        def __init__(self):
-            self._connect_timeout = ServiceConstants.HTTP_CONNECT_TIMEOUT
-            self._read_timeout = ServiceConstants.HTTP_READ_TIMEOUT
-            self._processing_timeout = ServiceConstants.HTTP_PROCESSING_TIMEOUT
-            self._pdf_services_uri = ServiceConstants.PDF_SERVICES_URI
-
-        def with_pdf_services_uri(self, pdf_services_uri: str):
-            """Sets the pdf service uri.
-
-            :param pdf_services_uri: PDF service URI.
-            :type pdf_services_uri: str
-            :return: This Builder instance to add any additional parameters.
-            :rtype: ClientConfig.Builder
-            """
-            self._pdf_services_uri = pdf_services_uri
-            return self
+        return self._read_timeout / 1000 if self._read_timeout else None
 
-        def with_region(self, region: Region):
-            """Updates the relevant value for the region.
+    def get_proxy_server_config(self):
+        """
+        :return: Proxy server config used.
+        :rtype: ProxyServerConfig
+        """
+        return self._proxy_server_config
 
-            :param region: Service region(US or EU). Default value is US.
-            :type region: Region
-            :return: This Builder instance to add any additional parameters.
-            :rtype: ClientConfig.Builder
-            """
-            self._set_pdf_services_uri_for_region(region)
-            return self
+    def validate(self):
+        """
+        Validator for the created client config.
+        """
+        if self._read_timeout <= 0:
+            raise ValueError(
+                "Invalid value for read timeout {timeout}. Must be valid integer greater than 0".format(
+                    timeout=self._read_timeout))
+
+        if self._connect_timeout <= 0:
+            raise ValueError(
+                "Invalid value for connect timeout {timeout}. Must be valid integer greater than 0".format(
+                    timeout=self._connect_timeout))
+
+        if self._proxy_server_config is not None:
+            if int(self._proxy_server_config.get_port()) <= 0:
+                raise ValueError("Invalid value for proxy port. Must be valid integer greater than 0")
 
-        def _set_pdf_services_uri_for_region(self, region: Region):
-            """Sets the pdf service uri based on the region.
+            if StringUtil.is_blank(self._proxy_server_config.get_host()):
+                raise ValueError(CustomErrorMessages.GENERIC_CAN_NOT_BE_NONE_OR_EMPTY.format("Host"))
 
-            :param region: Service region(US or EU).Default value is US.
-            :type region: Region
-            :return: Region specific pdf_services_uri
-            :rtype: str
-            """
-            if region == 'us':
-                self._pdf_services_uri = ServiceConstants.PDF_SERVICES_URI_US
-            elif region == 'eu':
-                self._pdf_services_uri = ServiceConstants.PDF_SERVICES_URI_EU
-
-        # the time it allows for the client to establish a connection to the server
-        def with_connect_timeout(self, connect_timeout: int):
-            """Sets the connect timeout. It should be greater than zero.
-
-            :param connect_timeout: determines the timeout in milliseconds until a connection is established in the \
-                API calls. Default value is 4000 milliseconds
-            :type connect_timeout: int
-            :return: This Builder instance to add any additional parameters.
-            :rtype: ClientConfig.Builder
-            """
-            self._connect_timeout = connect_timeout
-            return self
+    def from_file(self, client_config_file_path: str):
+        """
+        Sets the connect timeout and read timeout using the JSON client config file path. \
+        All the keys in the JSON structure are optional.
 
-        # the time it will wait on a response once connection is estalished
-        def with_read_timeout(self, read_timeout: int):
-            """Sets the read timeout. It should be greater than zero.
+        :param client_config_file_path: JSON client config file path
+        :type client_config_file_path: str
+        :return: This Builder instance to add any additional parameters.
+        :rtype: ClientConfig.Builder
 
-            :param read_timeout: Defines the read timeout in milliseconds, The number of milliseconds the client will \
-                wait for the server to send a response after the connection is established.\
-                Default value is 10000 milliseconds
-            :type read_timeout: int
-            :return: This Builder instance to add any additional parameters.
-            :rtype: ClientConfig.Builder
-            """
-            self._read_timeout = read_timeout
-            return self
+        JSON structure:
 
-        # the time it will wait for the operation to complete
-        def with_processing_timeout(self, processing_timeout: int):
-            """Sets the processing timeout. It should be greater than or equal to 600000 (10 minutes).
-
-            :param processing_timeout: Defines the processing timeout in milliseconds to process the documents.
-                Default value is 600000 milliseconds (10 minutes)
-            :type processing_timeout: int
-            :return: This Builder instance to add any additional parameters.
-            :rtype: ClientConfig.Builder
-            """
-            self._processing_timeout = processing_timeout
-            return self
+        .. code-block:: JSON
 
-        def from_file(self, client_config_file_path: str):
-            """
-            Sets the connect timeout and read timeout using the JSON client config file path. \
-            All the keys in the JSON structure are optional.
-
-            :param client_config_file_path: JSON client config file path
-            :type client_config_file_path: str
-            :return: This Builder instance to add any additional parameters.
-            :rtype: ClientConfig.Builder
-
-            JSON structure:
-
-            .. code-block:: JSON
-
-                {
-                    "connectTimeout": "4000",
-                    "readTimeout": "20000",
-                    "region": "eu",
-                    "processingTimeout": "600000"
-                }
-            """
+            {
+                "connectTimeout": "4000",
+                "readTimeout": "20000",
+                "proxyServerConfig": {
+                    "host": "127.0.0.1",
+                    "port": "8080",
+                    "scheme": "https",
+                    "usernamePasswordCredentials": {
+                        "username": "username",
+                        "password": "password"
+                        }
+                },
+                "region": "EU"
+            }
+        """
+        try:
             config_json_str = file_utils.read_conf_file_content(client_config_file_path)
             config_dict = json.loads(config_json_str)
+
             self._connect_timeout = int(config_dict.get(ClientConfig._CONNECT_TIMEOUT_KEY, self._connect_timeout))
+
             self._read_timeout = int(config_dict.get(ClientConfig._READ_TIMEOUT_KEY, self._read_timeout))
-            self._processing_timeout = int(config_dict.get(ClientConfig._PROCESSING_TIMEOUT_KEY,
-                                                           self._processing_timeout))
+
             region_node = config_dict.get(ClientConfig._REGION)
-            self.with_region(region_node)
+            if region_node:
+                self._pdf_services_uri = PDFServicesURI.get_uri_for_region(region_node)
+
             pdf_services_config = config_dict.get(ClientConfig._PDF_SERVICES)
             if pdf_services_config:
                 pdf_services_uri_node = pdf_services_config.get(ClientConfig._PDF_SERVICES_URI)
                 if pdf_services_uri_node:
                     self._pdf_services_uri = pdf_services_uri_node
-            return self
 
-        def build(self):
-            """
-            Returns a new :class:`ClientConfig` instance built from the current state of this builder.
-
-            :return: A ClientConfig instance.
-            :rtype: ClientConfig
-            """
-            from adobe.pdfservices.operation.internal.internal_client_config import InternalClientConfig
-            return InternalClientConfig(self._connect_timeout, self._read_timeout, self._processing_timeout,
-                                        self._pdf_services_uri)
+            proxy_server_config = config_dict.get(ClientConfig._PROXY_SERVER_CONFIG)
+            if proxy_server_config:
+                self._proxy_server_config = ProxyServerConfig("host").from_json(proxy_server_config)
+
+            return self
+        except Exception as e:
+            raise ValueError("Error while reading client config file: " + str(e))
```

### Comparing `pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/exception/exceptions.py` & `pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/exception/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# Copyright 2021 Adobe. All rights reserved.
-# This file is licensed to you under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License. You may obtain a copy
-# of the License at http://www.apache.org/licenses/LICENSE-2.0
-# 
-# Unless required by applicable law or agreed to in writing, software distributed under
-# the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
-# OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# Copyright 2024 Adobe
+# All Rights Reserved.
+#
+# NOTICE:  All information contained herein is, and remains
+# the property of Adobe and its suppliers, if any. The intellectual
+# and technical concepts contained herein are proprietary to Adobe
+# and its suppliers and are protected by all applicable intellectual
+# property laws, including trade secret and copyright laws.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Adobe.
 
 class ServiceUsageException(Exception):
     """
-    ServiceUsageError is thrown when either service usage limit has been reached or credentials quota has been exhausted.
+    ServiceUsageError is thrown when either service usage limit has been reached or credentials quota has been
+    exhausted.
     """
 
     DEFAULT_STATUS_CODE = 429
     """The default value of status code if there is no status code for this service failure."""
 
     DEFAULT_ERROR_CODE = 'UNKNOWN'
     """The default value of error code if there is no status code for this service failure."""
@@ -22,27 +25,29 @@
     def __init__(self, message, request_tracking_id, status_code=DEFAULT_STATUS_CODE, error_code=DEFAULT_ERROR_CODE):
         self.message = message
         self._request_tracking_id = request_tracking_id
         self._status_code = status_code if status_code else self.DEFAULT_STATUS_CODE
         self._error_code = error_code if error_code else self.DEFAULT_ERROR_CODE
 
     def __str__(self):
-        return "description ={description}; requestTrackingId={request_id}; statusCode={status_code}; errorCode={error_code}".format(description=self.message,
-                                                                                                                                     request_id=self.request_tracking_id,
-                                                                                                                                     status_code=self.status_code,
-                                                                                                                                     error_code=self.error_code)
+        return ("description ={description}; requestTrackingId={request_id}; statusCode={status_code}; errorCode={"
+                "error_code}").format(description=self.message,
+                                      request_id=self.request_tracking_id,
+                                      status_code=self.status_code,
+                                      error_code=self.error_code)
 
     @property
     def request_tracking_id(self):
         """ The request tracking id of the exception."""
         return self._request_tracking_id
 
     @property
     def status_code(self):
-        """ Returns the HTTP Status code or DEFAULT_STATUS_CODE if the status code doesn't adequately represent the error."""
+        """ Returns the HTTP Status code or DEFAULT_STATUS_CODE if the status code doesn't adequately represent the
+        error."""
         return self._status_code
 
     @property
     def error_code(self):
         """ Returns the detailed message of this error."""
         return self._error_code
 
@@ -59,27 +64,29 @@
     def __init__(self, message, request_tracking_id, status_code=DEFAULT_STATUS_CODE, error_code=DEFAULT_ERROR_CODE):
         self.message = message
         self._request_tracking_id = request_tracking_id
         self._status_code = status_code if status_code else self.DEFAULT_STATUS_CODE
         self._error_code = error_code if error_code else self.DEFAULT_ERROR_CODE
 
     def __str__(self):
-        return "description ={description}; requestTrackingId={request_id}; statusCode={status_code}; errorCode={error_code}".format(description=self.message,
-                                                                                                                                     request_id=self.request_tracking_id,
-                                                                                                                                     status_code=self.status_code,
-                                                                                                                                     error_code=self.error_code)
+        return ("description ={description}; requestTrackingId={request_id}; statusCode={status_code}; errorCode={"
+                "error_code}").format(description=self.message,
+                                      request_id=self.request_tracking_id,
+                                      status_code=self.status_code,
+                                      error_code=self.error_code)
 
     @property
     def request_tracking_id(self):
         """ The request tracking id of the exception."""
         return self._request_tracking_id
 
     @property
     def status_code(self):
-        """ Returns the HTTP Status code or DEFAULT_STATUS_CODE if the status code doesn't adequately represent the error."""
+        """ Returns the HTTP Status code or DEFAULT_STATUS_CODE if the status code doesn't adequately represent the
+        error."""
         return self._status_code
 
     @property
     def error_code(self):
         """ Returns the detailed message of this error."""
         return self._error_code
```

### Comparing `pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py` & `pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf/extract_pdf_params_payload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,41 @@
-# Copyright 2021 Adobe. All rights reserved.
-# This file is licensed to you under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License. You may obtain a copy
-# of the License at http://www.apache.org/licenses/LICENSE-2.0
-# 
-# Unless required by applicable law or agreed to in writing, software distributed under
-# the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
-# OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# Copyright 2024 Adobe
+# All Rights Reserved.
+#
+# NOTICE:  All information contained herein is, and remains
+# the property of Adobe and its suppliers, if any. The intellectual
+# and technical concepts contained herein are proprietary to Adobe
+# and its suppliers and are protected by all applicable intellectual
+# property laws, including trade secret and copyright laws.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Adobe.
+
 import json
-from typing import List
 
 from adobe.pdfservices.operation.internal.util.json_hint_encoder import JSONHintEncoder
-
-from adobe.pdfservices.operation.internal.api.dto.request.platform.platform_api_request import PlatformApiRequest
-from adobe.pdfservices.operation.pdfops.options.extractpdf.extract_element_type import ExtractElementType
-from adobe.pdfservices.operation.pdfops.options.extractpdf.extract_renditions_element_type import \
-    ExtractRenditionsElementType
-from adobe.pdfservices.operation.pdfops.options.extractpdf.table_structure_type import TableStructureType
-from adobe.pdfservices.operation.pdfops.options.extractpdf.extract_pdf_options import ExtractPDFOptions
+from adobe.pdfservices.operation.pdfjobs.params.extract_pdf.extract_pdf_params import ExtractPDFParams
 
 
-class ExtractPDFRequest(PlatformApiRequest):
+class ExtractPDFParamsPayload:
     json_hint = {
-        'asset_id': 'assetID',
+        'get_char_bounds': 'getCharBounds',
+        'include_styling': 'includeStyling',
         'elements_to_extract': 'elementsToExtract',
-        'renditions_to_extract': 'renditionsToExtract',
         'table_output_format': 'tableOutputFormat',
-        'extract_char_info': 'getCharBounds',
-        'include_styling_info': 'includeStyling'
+        'renditions_to_extract': 'renditionsToExtract'
     }
 
-    def __init__(self, asset_id: str = None, elements_to_extract: List[ExtractElementType] = None,
-                 renditions_to_extract: List[ExtractRenditionsElementType] = None, table_output_format: TableStructureType = None,
-                 extract_char_info: bool = None, include_styling_info: bool = None):
-        super().__init__()
-        self.asset_id = asset_id
-        self.elements_to_extract = elements_to_extract
-        self.renditions_to_extract = renditions_to_extract
-        self.table_output_format = table_output_format
-        self.extract_char_info = extract_char_info
-        self.include_styling_info = include_styling_info
-
-    @classmethod
-    def from_extract_pdf_options(cls, asset_id: str = None, extract_pdf_options: ExtractPDFOptions = None):
-        if extract_pdf_options:
-            return cls(asset_id=asset_id,
-                       elements_to_extract=extract_pdf_options.elements_to_extract,
-                       renditions_to_extract=extract_pdf_options.elements_to_extract_renditions,
-                       table_output_format=extract_pdf_options.table_output_format,
-                       extract_char_info=extract_pdf_options.get_char_info,
-                       include_styling_info=extract_pdf_options.include_styling_info)
-        else:
-            return cls(asset_id=asset_id, elements_to_extract=[ExtractElementType.TEXT])
+    def __init__(self, extract_pdf_params: ExtractPDFParams):
+        self.get_char_bounds = extract_pdf_params.get_add_char_info() \
+            if extract_pdf_params.get_add_char_info() is not None else None
+        self.include_styling = extract_pdf_params.get_styling_info() \
+            if extract_pdf_params.get_styling_info() is not None else None
+        self.elements_to_extract = extract_pdf_params.get_elements_to_extract() \
+            if extract_pdf_params.get_elements_to_extract() is not None else None
+        self.table_output_format = extract_pdf_params.get_table_structure_type().__str__() \
+            if extract_pdf_params.get_table_structure_type() is not None else None
+        self.renditions_to_extract = extract_pdf_params.get_elements_to_extract_renditions() \
+            if extract_pdf_params.get_elements_to_extract_renditions() is not None else None
 
     def to_json(self):
         return json.dumps(self, cls=JSONHintEncoder, indent=1, sort_keys=True)
```

### Comparing `pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/platform_api.py` & `pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/api/storage_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,106 @@
-# Copyright 2022 Adobe. All rights reserved.
-# This file is licensed to you under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License. You may obtain a copy
-# of the License at http://www.apache.org/licenses/LICENSE-2.0
+# Copyright 2024 Adobe
+# All Rights Reserved.
 #
-# Unless required by applicable law or agreed to in writing, software distributed under
-# the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
-# OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
-import json
+# NOTICE:  All information contained herein is, and remains
+# the property of Adobe and its suppliers, if any. The intellectual
+# and technical concepts contained herein are proprietary to Adobe
+# and its suppliers and are protected by all applicable intellectual
+# property laws, including trade secret and copyright laws.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Adobe.
+
 import logging
-from datetime import datetime
 from http import HTTPStatus
-import polling2
-from polling2 import TimeoutException
+
 import requests
 
-from adobe.pdfservices.operation.internal.api.dto.response.job_status import JobStatus
+from adobe.pdfservices.operation.exception.exceptions import ServiceApiException, SdkException
+from adobe.pdfservices.operation.internal.api.dto.request.asset_upload_uri_request import AssetUploadURIRequest
 from adobe.pdfservices.operation.internal.constants.request_key import RequestKey
-from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
-from adobe.pdfservices.operation.exception.exceptions import ServiceApiException
-from adobe.pdfservices.operation.internal.api.dto.response.platform.platform_api_response import PlatformApiResponse
 from adobe.pdfservices.operation.internal.exceptions import OperationException
-from adobe.pdfservices.operation.internal.extension_media_type_mapping import ExtensionMediaTypeMapping
-from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
+from adobe.pdfservices.operation.internal.execution_context import ExecutionContext
+from adobe.pdfservices.operation.internal.http import http_client
 from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
+from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
 from adobe.pdfservices.operation.internal.http.request_header_const import DefaultHeaders
-from adobe.pdfservices.operation.internal.http import http_client
-from adobe.pdfservices.operation.internal.internal_execution_context import InternalExecutionContext
-from adobe.pdfservices.operation.internal.api.dto.request.platform.platform_api_request import PlatformApiRequest
+from adobe.pdfservices.operation.pdf_services_media_type import PDFServicesMediaType
 
 
-class PlatformApi:
-    operation = '/operation/'
-    PROCESSING_TIMEOUT_STATUS_CODE = 0
+class StorageApi:
+    assets = "/assets"
 
     @staticmethod
-    def submit_job(context: InternalExecutionContext, platform_api_request: PlatformApiRequest, operation_endpoint: str,
-                   x_request_id: str, operation_header_info: str):
-        http_request = HttpRequest(http_method=HttpMethod.POST,
-                                   request_key=RequestKey.PLATFORM,
-                                   url=context.client_config.get_pdf_services_uri() + PlatformApi.operation +
-                                       operation_endpoint, data=platform_api_request.to_json(),
-                                   headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id,
-                                            DefaultHeaders.X_DCSDK_OPS_INFO_HEADER_NAME: operation_header_info,
-                                            DefaultHeaders.CONTENT_TYPE_HEADER_NAME: ExtensionMediaTypeMapping.JSON.mime_type},
-
-                                   authenticator=context.authenticator,
-                                   connect_timeout=context.client_config.get_connect_timeout(),
-                                   read_timeout=context.client_config.get_read_timeout())
-        response = http_client.process_request(http_request=http_request,
-                                               success_status_codes=[HTTPStatus.CREATED],
-                                               error_response_handler=PlatformApi.handle_error_response)
-        return response.headers.get('location')
+    def upload_to_cloud(context: ExecutionContext, uri: str, input_stream, media_type):
+        try:
+            http_request = HttpRequest(http_method=HttpMethod.PUT,
+                                       request_key=RequestKey.UPLOAD,
+                                       url=uri,
+                                       data=input_stream,
+                                       headers={DefaultHeaders.CONTENT_TYPE_HEADER_NAME: media_type},
+                                       connect_timeout=context.client_config.get_connect_timeout(),
+                                       read_timeout=context.client_config.get_read_timeout(),
+                                       proxies=context.client_config.get_proxy_server_config())
+            response = http_client.process_request(http_request=http_request,
+                                                   success_status_codes=[HTTPStatus.ACCEPTED, HTTPStatus.OK],
+                                                   error_response_handler=StorageApi.handle_error_response)
+
+            logging.debug(f'Asset upload response {response}')
+
+            return response
+        except FileNotFoundError as fe:
+            raise fe
+        except IOError as io:
+            raise SdkException(f'Unexpected error while uploading file {io}')
+
+    @staticmethod
+    def get_upload_uri(context: ExecutionContext, media_type: str, x_request_id: str):
+
+        try:
+            asset_upload_uri_request = AssetUploadURIRequest(media_type)
+
+            http_request = HttpRequest(http_method=HttpMethod.POST,
+                                       request_key=RequestKey.PLATFORM,
+                                       url=context.client_config.get_pdf_services_uri() + StorageApi.assets,
+                                       data=asset_upload_uri_request.to_json(),
+                                       headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id,
+                                                DefaultHeaders.CONTENT_TYPE_HEADER_NAME: PDFServicesMediaType.JSON.mime_type},
+                                       authenticator=context.authenticator,
+                                       connect_timeout=context.client_config.get_connect_timeout(),
+                                       read_timeout=context.client_config.get_read_timeout(),
+                                       proxies=context.client_config.get_proxy_server_config())
+
+            response = http_client.process_request(http_request=http_request,
+                                                   success_status_codes=[HTTPStatus.ACCEPTED, HTTPStatus.OK],
+                                                   error_response_handler=StorageApi.handle_error_response)
+            return response
+
+        except OperationException as oex:
+            raise ServiceApiException(message=oex.error_message, error_code=oex.error_code,
+                                      request_tracking_id=oex.request_tracking_id, status_code=oex.status_code)
 
     @staticmethod
-    def status_poll(context: InternalExecutionContext, location: str, x_request_id: str):
-        def is_correct_response(response):
-            content = json.loads(response.content)
-            status = content.get('status')
-            if status == JobStatus.FAILED:
-                job_error_response = PlatformApiResponse(status,content.get('error')).get_error_response()
-                raise ServiceApiException(job_error_response.get('message'), ResponseUtil.
-                                          get_request_tracking_id_from_response(response, False), job_error_response
-                                          .get('status'), job_error_response.get('code'))
-            return status == JobStatus.DONE
-
-        start_time = datetime.now()
-        http_request = HttpRequest(http_method=HttpMethod.GET,
-                                   request_key=RequestKey.STATUS,
-                                   url=location,
-                                   headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id},
-                                   authenticator=context.authenticator,
-                                   connect_timeout=context.client_config.get_connect_timeout(),
-                                   read_timeout=context.client_config.get_read_timeout(),
-                                   retryable=True)
+    def get_download_uri(context: ExecutionContext, asset_id: str, x_request_id: str):
 
         try:
-            response = polling2.poll(
-                lambda: http_client.process_request(http_request=http_request,
-                                                    success_status_codes=[HTTPStatus.OK, HTTPStatus.ACCEPTED],
-                                                    error_response_handler=PlatformApi.handle_error_response),
-                check_success=is_correct_response,
-                step=1,
-                timeout=context.client_config.get_processing_timeout()
-            )
-            logging.debug(f'Total processing time, Latency(ms): {(datetime.now() - start_time).microseconds / 1000}')
+            http_request = HttpRequest(http_method=HttpMethod.GET,
+                                       request_key=RequestKey.PLATFORM,
+                                       url=context.client_config.get_pdf_services_uri() + StorageApi.assets + "/" + asset_id,
+                                       headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id},
+                                       authenticator=context.authenticator,
+                                       connect_timeout=context.client_config.get_connect_timeout(),
+                                       read_timeout=context.client_config.get_read_timeout(),
+                                       proxies=context.client_config.get_proxy_server_config())
+
+            response = http_client.process_request(http_request=http_request,
+                                                   success_status_codes=[HTTPStatus.ACCEPTED, HTTPStatus.OK],
+                                                   error_response_handler=StorageApi.handle_error_response)
             return response
-        except TimeoutException:
-            logging.error("Processing Timeout reached. Something's wrong, file operation took too long")
-            raise OperationException(message="Operation execution has timed out!", error_message="Processing Timeout reached", request_tracking_id=x_request_id
-                                     ,status_code=PlatformApi.PROCESSING_TIMEOUT_STATUS_CODE)
 
+        except OperationException as oex:
+            raise ServiceApiException(message=oex.error_message, error_code=oex.error_code,
+                                      request_tracking_id=oex.request_tracking_id, status_code=oex.status_code)
 
     @staticmethod
     def handle_error_response(response: requests.Response):
         pass
```

### Comparing `pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/api/storage_api.py` & `pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/auth/service_principal_authenticator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,112 @@
-# Copyright 2022 Adobe. All rights reserved.
-# This file is licensed to you under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License. You may obtain a copy
-# of the License at http://www.apache.org/licenses/LICENSE-2.0
+# Copyright 2024 Adobe
+# All Rights Reserved.
 #
-# Unless required by applicable law or agreed to in writing, software distributed under
-# the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
-# OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# NOTICE:  All information contained herein is, and remains
+# the property of Adobe and its suppliers, if any. The intellectual
+# and technical concepts contained herein are proprietary to Adobe
+# and its suppliers and are protected by all applicable intellectual
+# property laws, including trade secret and copyright laws.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Adobe.
 
+import json
 import logging
+import sys
+import threading
 from datetime import datetime
 from http import HTTPStatus
 
-import requests
+from adobe.pdfservices.operation.auth.service_principal_credentials import ServicePrincipalCredentials
+from adobe.pdfservices.operation.exception.exceptions import SdkException, ServiceApiException
+from adobe.pdfservices.operation.internal.auth.authenticator import Authenticator
+from adobe.pdfservices.operation.internal.auth.session_token import SessionToken
 from adobe.pdfservices.operation.internal.constants.request_key import RequestKey
+from adobe.pdfservices.operation.internal.constants.service_constants import custom_error_messages
 from adobe.pdfservices.operation.internal.exceptions import OperationException
-from adobe.pdfservices.operation.exception.exceptions import ServiceApiException, SdkException
-from adobe.pdfservices.operation.io.file_ref import FileRef
-from adobe.pdfservices.operation.internal.internal_execution_context import InternalExecutionContext
-from adobe.pdfservices.operation.internal.extension_media_type_mapping import ExtensionMediaTypeMapping
-from adobe.pdfservices.operation.internal.http.request_header_const import DefaultHeaders
 from adobe.pdfservices.operation.internal.http import http_client
 from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
 from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
-from adobe.pdfservices.operation.internal.api.dto.request.asset_upload_uri_request import AssetUploadURIRequest
+from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
 
 
-class StorageApi:
-
-    assets = "/assets"
-
-    @staticmethod
-    def upload_to_cloud(context: InternalExecutionContext, uri: str, source_file_ref: FileRef):
-        try:
-            http_request = HttpRequest(http_method=HttpMethod.PUT,
-                                       request_key=RequestKey.UPLOAD,
-                                       url=uri,
-                                       data=source_file_ref.get_as_stream(),
-                                       headers={DefaultHeaders.CONTENT_TYPE_HEADER_NAME: source_file_ref.get_media_type(
-                                       )},
-                                       connect_timeout=context.client_config.get_connect_timeout(),
-                                       read_timeout=context.client_config.get_read_timeout())
-            response = http_client.process_request(http_request=http_request,
-                                                   success_status_codes=[HTTPStatus.ACCEPTED, HTTPStatus.OK],
-                                                   error_response_handler=StorageApi.handle_error_response)
-
-            logging.debug(f'Asset upload response {response}')
-
-            return response
-        except FileNotFoundError as fe:
-            raise fe
-        except IOError as io:
-            raise SdkException(f'Unexpected error while uploading file {io}')
-
-    @staticmethod
-    def get_upload_uri(context: InternalExecutionContext, media_type: str, x_request_id: str):
+class ServicePrincipalAuthenticator(Authenticator):
+    """
+        Authenticator for OAuth Server-to-Server based Service Principal credentials
+    """
+    token: SessionToken = None
+    service_principal_configuration: ServicePrincipalCredentials
+    token_endpoint = ''
+
+    def __init__(self, service_principal_configuration, client_config):
+        self.service_principal_configuration = service_principal_configuration
+        self.token_endpoint = client_config.get_pdf_services_uri()
+        self._logger = logging.getLogger(__name__)
+        self.proxy_server_config = client_config.get_proxy_server_config()
+
+        # thread locking to avoid refreshing token multiple times in multi threaded cases
+        self.lock = threading.Lock()
+
+    def session_token(self):
+        """ Access token for the PDF Services API """
+        with self.lock:
+            if self.token:
+                if self.time_to_expire() > 2:
+                    return self.token
+            self._logger.debug(
+                "Refreshing access token with creation time: {creation_time} minutes".format(
+                    creation_time=datetime.now()))
+            return self.refresh_token()
+
+    def time_to_expire(self):
+        """ Time remaining in minutes till token expiry """
+        return int((self.token.expired_at.timestamp() - datetime.now().timestamp()) / 60)
+
+    def refresh_token(self):
+        """ Refreshes the access token sent to PDF Services API """
+        url = "{token_endpoint}/{ims_proxy_token_endpoint}".format(
+            token_endpoint=self.token_endpoint,
+            ims_proxy_token_endpoint='token'
+        )
+        access_token_request_payload = {"client_id": self.service_principal_configuration.get_client_id(),
+                                        "client_secret": self.service_principal_configuration.get_client_secret()}
 
         try:
-            assetUploadURIRequest = AssetUploadURIRequest(media_type)
-
-            http_request = HttpRequest(http_method=HttpMethod.POST,
-                                       request_key=RequestKey.PLATFORM,
-                                       url=context.client_config.get_pdf_services_uri() + StorageApi.assets,
-                                       data=assetUploadURIRequest.to_json(),
-                                       headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id,
-                                                DefaultHeaders.CONTENT_TYPE_HEADER_NAME: ExtensionMediaTypeMapping.JSON.mime_type}
-                                       , authenticator=context.authenticator,
-                                       connect_timeout=context.client_config.get_connect_timeout(),
-                                       read_timeout=context.client_config.get_read_timeout())
-
-            response = http_client.process_request(http_request=http_request,
-                                                   success_status_codes=[HTTPStatus.ACCEPTED, HTTPStatus.OK],
-                                                   error_response_handler=StorageApi.handle_error_response)
-            return response
-
-        except OperationException as oex:
-            raise ServiceApiException(message=oex.error_message, error_code=oex.error_code,
-                                      request_tracking_id=oex.request_tracking_id, status_code=oex.status_code)
-
-    @staticmethod
-    def handle_error_response(response: requests.Response):
-        pass
-
-    @staticmethod
-    def download_and_save_file(context: InternalExecutionContext, uri: str,
-                               destination_path: str):
-
-        start_time = datetime.now()
-        http_request = HttpRequest(http_method=HttpMethod.GET,
-                                   request_key=RequestKey.DOWNLOAD,
-                                   headers={},
-                                   url=uri,
-                                   connect_timeout=context.client_config.get_connect_timeout(),
-                                   read_timeout=context.client_config.get_read_timeout())
-
-        response = http_client.process_request(http_request=http_request,
-                                               success_status_codes=[HTTPStatus.OK, HTTPStatus.ACCEPTED],
-                                               error_response_handler=StorageApi.handle_error_response)
-        logging.debug(f'Upload Operation Latency(ms): {(datetime.now() - start_time).microseconds / 1000}')
-
-        logging.info(f'Downloading file to {destination_path}')
-
-        file = FileRef.create_from_local_file(destination_path)
-        with open(destination_path, 'wb') as f:
-            f.write(response.content)
-        return file
-
-
+            http_request = HttpRequest(http_method=HttpMethod.POST, request_key=RequestKey.AUTHN, url=url,
+                                       data=access_token_request_payload, headers={},
+                                       proxies=self.proxy_server_config)
+            response = http_client.process_request(http_request=http_request, success_status_codes=[HTTPStatus.OK],
+                                                   error_response_handler=self.handle_ims_failure)
+
+            content = json.loads(response.content)
+            self.token = SessionToken(content['access_token'], content['expires_in'] * 1000)
+        except ServiceApiException as ex:
+            raise ex
+        except Exception:
+            raise SdkException("Exception in fetching access token", sys.exc_info())
+        return self.token
+
+    def get_api_key(self):
+        """ API key for Service Principle credentials """
+        return self.service_principal_configuration.get_client_id()
+
+    def handle_ims_failure(self, response):
+        """ Handling of IMS failure during call to PDF Services API """
+
+        self._logger.error(
+            "IMS call failed with status code {error_code}".format(error_code=response.status_code))
+        content = json.loads(response.content)
+        # When error is returned with no description
+        if not content.get("error_description", None) or content["error_description"].isspace():
+            content["error_description"] = content.get("error", None)
+        # Special handling for invalid token and certificate expiry cases
+        if "invalid_token" == content.get("error", None):
+            if "Could not match signature to any of the bindings" == content.get("error_description", None):
+                content["error_description"] = custom_error_messages["imsCertificateExpiredErrorMessage"]
+            else:
+                content["error_description"] = custom_error_messages["imsInvalidTokenGenericErrorMessage"]
+        raise OperationException(message="Error response received for IMS request",
+                                 status_code=response.status_code,
+                                 error_code=content.get("error", None),
+                                 error_message=content.get("error_description", None),
+                                 request_tracking_id=ResponseUtil.get_request_tracking_id_from_response(response, True))
```

### Comparing `pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/http/http_client.py` & `pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/http/http_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,112 @@
-# Copyright 2021 Adobe. All rights reserved.
-# This file is licensed to you under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License. You may obtain a copy
-# of the License at http://www.apache.org/licenses/LICENSE-2.0
+# Copyright 2024 Adobe
+# All Rights Reserved.
 #
-# Unless required by applicable law or agreed to in writing, software distributed under
-# the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
-# OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# NOTICE:  All information contained herein is, and remains
+# the property of Adobe and its suppliers, if any. The intellectual
+# and technical concepts contained herein are proprietary to Adobe
+# and its suppliers and are protected by all applicable intellectual
+# property laws, including trade secret and copyright laws.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Adobe.
+
 import logging
 import sys
 from typing import Callable, List
 
 import requests
 
 from adobe.pdfservices.operation.exception.exceptions import SdkException
-from adobe.pdfservices.operation.internal.http.request_header_const import DefaultHeaders
-from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
 from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
 from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
+from adobe.pdfservices.operation.internal.http.request_header_const import DefaultHeaders
+from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
 
 _logger = logging.getLogger(__name__)
 
 
 def process_request(http_request: HttpRequest, success_status_codes: List,
                     error_response_handler: Callable[[requests.Response], None]):
     _append_default_headers(http_request.headers)
     if http_request.authenticator:
         # get token and append auth header
         access_token = http_request.authenticator.session_token().access_token
         http_request.headers[DefaultHeaders.AUTHORIZATION_HEADER_NAME] = "Bearer " + access_token
         http_request.headers[DefaultHeaders.X_API_KEY_HEADER_NAME] = http_request.authenticator.get_api_key()
 
     # retry the request if it fails with 401 and specific error code
-    while (True):
+    while True:
         response = _execute_request(http_request)
         if _handle_response_and_retry(response, success_status_codes,
-                                      error_response_handler, not http_request.authenticator, http_request.request_key) and http_request.retryable:
+                                      error_response_handler, not http_request.authenticator,
+                                      http_request.request_key) and http_request.retryable:
             _force_authenticate(http_request)
             # Only single retry is required in case of token expiry
             http_request.retryable = False
         else:
             return response
 
 
 def _append_default_headers(headers: dict):
     # Set SDK Info header
     headers[DefaultHeaders.DC_APP_INFO_HEADER_KEY] = "{lang}-{name}-{version}".format(lang="python",
                                                                                       name='pdfservices-sdk',
-                                                                                      version='2.3.1')
+                                                                                      version='4.0.0')
     headers[DefaultHeaders.ACCEPT_HEADER_NAME] = DefaultHeaders.JSON_TXT_CONTENT_TYPE
 
 
 def _execute_request(http_request: HttpRequest):
     response = None
     timeout = (http_request.connect_timeout, http_request.read_timeout)
     try:
         if http_request.method == HttpMethod.POST:
             if http_request.data:
                 response = requests.post(url=http_request.url,
                                          data=http_request.data,
                                          headers=http_request.headers,
-                                         timeout=timeout)
+                                         timeout=timeout,
+                                         proxies=http_request.proxies.proxy_config_map() if
+                                         http_request.proxies is not None else None)
             elif http_request.files:
                 response = requests.post(url=http_request.url,
                                          files=http_request.files,
                                          headers=http_request.headers,
-                                         timeout=timeout)
+                                         timeout=timeout,
+                                         proxies=http_request.proxies.proxy_config_map() if
+                                         http_request.proxies is not None else None)
                 for key, val in http_request.files.items():
                     if hasattr(val[1], 'close'):
                         val[1].close()
         elif http_request.method == HttpMethod.GET:
             response = requests.get(url=http_request.url, allow_redirects=True, headers=http_request.headers,
-                                    timeout=timeout)
+                                    timeout=timeout,
+                                    proxies=http_request.proxies.proxy_config_map() if
+                                    http_request.proxies is not None else None)
         elif http_request.method == HttpMethod.PUT:
             response = requests.put(url=http_request.url, data=http_request.data, headers=http_request.headers,
-                                    timeout=timeout)
+                                    timeout=timeout,
+                                    proxies=http_request.proxies.proxy_config_map() if
+                                    http_request.proxies is not None else None)
+        elif http_request.method == HttpMethod.DELETE:
+            response = requests.delete(url=http_request.url, headers=http_request.headers, timeout=timeout,
+                                       proxies=http_request.proxies.proxy_config_map() if
+                                       http_request.proxies is not None else None)
 
     except Exception as e:
         raise SdkException("Request could not be completed. Possible cause attached!", sys.exc_info())
     return response
 
 
 def _force_authenticate(http_request: HttpRequest):
     _logger.debug("Re-authenticate as access_token is expired")
     access_token = http_request.authenticator.refresh_token().access_token
     http_request.headers[DefaultHeaders.AUTHORIZATION_HEADER_NAME] = "Bearer " + access_token
 
 
-def _handle_response_and_retry(response: requests.Response, success_status_codes, error_response_handler, is_ims_api, request_key: str):
+def _handle_response_and_retry(response: requests.Response, success_status_codes, error_response_handler, is_ims_api,
+                               request_key: str):
     if response.status_code not in success_status_codes:
         _logger.debug(
             "Failure response code {error_code} encountered from backend".format(error_code=response.status_code))
         should_retry = ResponseUtil.handle_api_failures(response, request_key, is_ims_api)
         return should_retry if should_retry else error_response_handler(response)
```

### Comparing `pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/http/http_request.py` & `pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/http/http_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-# Copyright 2021 Adobe. All rights reserved.
-# This file is licensed to you under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License. You may obtain a copy
-# of the License at http://www.apache.org/licenses/LICENSE-2.0
+# Copyright 2024 Adobe
+# All Rights Reserved.
 #
-# Unless required by applicable law or agreed to in writing, software distributed under
-# the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
-# OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# NOTICE:  All information contained herein is, and remains
+# the property of Adobe and its suppliers, if any. The intellectual
+# and technical concepts contained herein are proprietary to Adobe
+# and its suppliers and are protected by all applicable intellectual
+# property laws, including trade secret and copyright laws.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Adobe.
+
+from adobe.pdfservices.operation.config.proxy.proxy_server_config import ProxyServerConfig
 from adobe.pdfservices.operation.internal.auth.authenticator import Authenticator
 from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
 
 
 class HttpRequest:
 
     # (url, data/files, headers, authenticator (if none its not authenticated), socket_timeout, connect_timeout)
     def __init__(self, http_method: HttpMethod, request_key: str, url: str, headers: dict, data=None, files=None,
-                 authenticator: Authenticator = None, read_timeout=None, connect_timeout=None, retryable:bool=False):
+                 authenticator: Authenticator = None, read_timeout=None, connect_timeout=None, retryable: bool = False,
+                 proxies: ProxyServerConfig = None):
         self.method = http_method
         self.request_key = request_key
         self.url = url
         self.headers = headers
         self.data = data
         self.files = files
         self.authenticator = authenticator
         self.read_timeout = read_timeout
         self.connect_timeout = connect_timeout
         self.retryable = retryable
+        self.proxies = proxies
```

### Comparing `pdfservices-sdk-2.3.1/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py` & `pdfservices_sdk-4.0.0/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# Copyright 2021 Adobe. All rights reserved.
-# This file is licensed to you under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License. You may obtain a copy
-# of the License at http://www.apache.org/licenses/LICENSE-2.0
-# 
-# Unless required by applicable law or agreed to in writing, software distributed under
-# the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
-# OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# Copyright 2024 Adobe
+# All Rights Reserved.
+#
+# NOTICE:  All information contained herein is, and remains
+# the property of Adobe and its suppliers, if any. The intellectual
+# and technical concepts contained herein are proprietary to Adobe
+# and its suppliers and are protected by all applicable intellectual
+# property laws, including trade secret and copyright laws.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Adobe.
 
 import json
 
 
 class JSONHintEncoder(json.JSONEncoder):
     def default(self, obj):
         if hasattr(obj, 'json_hint'):
@@ -33,16 +35,16 @@
                     dict_to_return[dict_field] = result
                 else:
                     if field_val is not None:
                         dict_to_return[dict_field] = json.loads(json.dumps(field_val, cls=JSONHintEncoder))
             return dict_to_return
         return json.JSONEncoder.default(self, obj)
 
-class JSONHintDecoder:
 
+class JSONHintDecoder:
 
     @staticmethod
     def rev(dct):
         result = {}
         for key, val in dct.items():
             cls_type = str
             rev_key = val
```

