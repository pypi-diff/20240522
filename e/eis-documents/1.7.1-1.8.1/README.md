# Comparing `tmp/eis-documents-1.7.1.tar.gz` & `tmp/eis-documents-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis-documents-1.7.1.tar", last modified: Mon Feb 12 14:38:53 2024, max compression
+gzip compressed data, was "eis-documents-1.8.1.tar", last modified: Thu Feb 22 19:51:32 2024, max compression
```

## Comparing `eis-documents-1.7.1.tar` & `eis-documents-1.8.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-12 14:38:53.206855 eis-documents-1.7.1/
--rw-r--r--   0 ricard     (501) staff       (20)      333 2024-02-12 14:38:53.206954 eis-documents-1.7.1/PKG-INFO
--rw-r--r--   0 ricard     (501) staff       (20)    14050 2024-02-12 14:25:33.000000 eis-documents-1.7.1/README.md
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-12 14:38:53.151755 eis-documents-1.7.1/eis/
--rw-r--r--   0 ricard     (501) staff       (20)        0 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/__init__.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-12 14:38:53.158367 eis-documents-1.7.1/eis/document/
--rw-r--r--   0 ricard     (501) staff       (20)      724 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/__init__.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-12 14:38:53.163541 eis-documents-1.7.1/eis/document/api/
--rw-r--r--   0 ricard     (501) staff       (20)      226 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)     5440 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/default_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    31276 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/document_templates_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    41433 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/documents_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    35537 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/docx_templates_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    30049 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/layouts_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    31551 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/product_documents_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     6402 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/search_keywords_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     7431 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/searchable_document_owners_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     7564 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api/searchable_documents_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    41630 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/api_client.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-12 14:38:53.163942 eis-documents-1.7.1/eis/document/apis/
--rw-r--r--   0 ricard     (501) staff       (20)     1047 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/apis/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)    16479 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/configuration.py
--rw-r--r--   0 ricard     (501) staff       (20)     5072 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/exceptions.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-12 14:38:53.185268 eis-documents-1.7.1/eis/document/model/
--rw-r--r--   0 ricard     (501) staff       (20)      346 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)    13833 2024-02-12 14:25:30.000000 eis-documents-1.7.1/eis/document/model/create_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11931 2024-02-12 14:25:30.000000 eis-documents-1.7.1/eis/document/model/create_doc_template_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    20279 2024-02-12 14:25:30.000000 eis-documents-1.7.1/eis/document/model/create_document_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11901 2024-02-12 14:25:30.000000 eis-documents-1.7.1/eis/document/model/create_document_sync_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11609 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/create_html_template_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    13422 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/create_layout_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11849 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/create_layout_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    17599 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/create_presigned_post_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11975 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/create_presigned_post_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11638 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/delete_layout_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12110 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/delete_product_document_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11516 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/delete_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11699 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/delete_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    15784 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/doc_template_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    19156 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/document_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11755 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/download_document_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11644 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/get_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11922 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/get_doc_template_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11526 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/get_document_download_url_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11606 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/get_docx_template_download_url_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11629 2024-02-12 14:25:31.000000 eis-documents-1.7.1/eis/document/model/get_layout_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11840 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/get_layout_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11615 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/get_product_document_download_url_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12033 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/get_product_document_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11509 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/get_signed_s3_key_url_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12884 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/grpc_create_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    13058 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/grpc_update_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    13700 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/html_template_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12219 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/inline_response200.py
--rw-r--r--   0 ricard     (501) staff       (20)    12219 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/inline_response503.py
--rw-r--r--   0 ricard     (501) staff       (20)    14955 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/layout_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12417 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12182 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_doc_templates_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12089 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_documents_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12087 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_layouts_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12160 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_product_documents_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12568 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11626 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_search_keywords_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11687 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_search_keywords_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11754 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_searchable_document_owners_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11917 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_searchable_document_owners_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12553 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_searchable_documents_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12335 2024-02-12 14:25:32.000000 eis-documents-1.7.1/eis/document/model/list_searchable_documents_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    16350 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/product_document_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13906 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/searchable_document_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11910 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/searchable_document_owner_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12497 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/shared_update_docx_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14197 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/update_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11931 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/update_doc_template_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13054 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/update_document_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11889 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/update_document_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12423 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/update_html_template_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    13784 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/update_layout_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11849 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/update_layout_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13564 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/upload_docx_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14050 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model/upload_product_document_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    82488 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/model_utils.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-12 14:38:53.185708 eis-documents-1.7.1/eis/document/models/
--rw-r--r--   0 ricard     (501) staff       (20)     5366 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/models/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)    14274 2024-02-12 14:25:33.000000 eis-documents-1.7.1/eis/document/rest.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-12 14:38:53.186664 eis-documents-1.7.1/eis_documents.egg-info/
--rw-r--r--   0 ricard     (501) staff       (20)      333 2024-02-12 14:38:53.000000 eis-documents-1.7.1/eis_documents.egg-info/PKG-INFO
--rw-r--r--   0 ricard     (501) staff       (20)     6571 2024-02-12 14:38:53.000000 eis-documents-1.7.1/eis_documents.egg-info/SOURCES.txt
--rw-r--r--   0 ricard     (501) staff       (20)        1 2024-02-12 14:38:53.000000 eis-documents-1.7.1/eis_documents.egg-info/dependency_links.txt
--rw-r--r--   0 ricard     (501) staff       (20)       32 2024-02-12 14:38:53.000000 eis-documents-1.7.1/eis_documents.egg-info/requires.txt
--rw-r--r--   0 ricard     (501) staff       (20)        4 2024-02-12 14:38:53.000000 eis-documents-1.7.1/eis_documents.egg-info/top_level.txt
--rw-r--r--   0 ricard     (501) staff       (20)      162 2024-02-12 14:38:53.207285 eis-documents-1.7.1/setup.cfg
--rw-r--r--   0 ricard     (501) staff       (20)      990 2024-02-12 14:25:33.000000 eis-documents-1.7.1/setup.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-12 14:38:53.206633 eis-documents-1.7.1/test/
--rw-r--r--   0 ricard     (501) staff       (20)      981 2024-02-12 14:25:30.000000 eis-documents-1.7.1/test/test_create_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      981 2024-02-12 14:25:30.000000 eis-documents-1.7.1/test/test_create_doc_template_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      822 2024-02-12 14:25:30.000000 eis-documents-1.7.1/test/test_create_document_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      975 2024-02-12 14:25:30.000000 eis-documents-1.7.1/test/test_create_document_sync_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      801 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_create_html_template_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      945 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_create_layout_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      924 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_create_layout_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      858 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_create_presigned_post_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      879 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_create_presigned_post_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      641 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_default_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      808 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_delete_layout_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      872 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_delete_product_document_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      765 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_delete_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      786 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_delete_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      980 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_doc_template_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      743 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_document_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1412 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_document_templates_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1671 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_documents_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1570 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_docx_templates_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      836 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_download_document_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      823 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_get_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      960 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_get_doc_template_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      901 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_get_document_download_url_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      930 2024-02-12 14:25:31.000000 eis-documents-1.7.1/test/test_get_docx_template_download_url_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      787 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_get_layout_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      903 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_get_layout_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      951 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_get_product_document_download_url_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1004 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_get_product_document_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      867 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_get_signed_s3_key_url_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1010 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_grpc_create_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1010 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_grpc_update_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      772 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_html_template_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      771 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_inline_response200.py
--rw-r--r--   0 ricard     (501) staff       (20)      771 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_inline_response503.py
--rw-r--r--   0 ricard     (501) staff       (20)      849 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_layout_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1246 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_layouts_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      830 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      974 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_doc_templates_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      939 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_documents_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      917 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_layouts_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1018 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_product_documents_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      751 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      851 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_search_keywords_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      872 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_search_keywords_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      922 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_searchable_document_owners_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1108 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_searchable_document_owners_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      886 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_searchable_documents_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1051 2024-02-12 14:25:32.000000 eis-documents-1.7.1/test/test_list_searchable_documents_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      793 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_product_document_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1470 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_product_documents_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      743 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_search_keywords_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      814 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_searchable_document_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      850 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_searchable_document_owner_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      834 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_searchable_document_owners_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_searchable_documents_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      894 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_shared_update_docx_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      981 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_update_doc_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      981 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_update_doc_template_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      822 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_update_document_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      946 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_update_document_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      801 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_update_html_template_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      945 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_update_layout_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      924 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_update_layout_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      851 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_upload_docx_template_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      872 2024-02-12 14:25:33.000000 eis-documents-1.7.1/test/test_upload_product_document_request_dto.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-22 19:51:32.264891 eis-documents-1.8.1/
+-rw-r--r--   0 ricard     (501) staff       (20)      333 2024-02-22 19:51:32.265015 eis-documents-1.8.1/PKG-INFO
+-rw-r--r--   0 ricard     (501) staff       (20)    14050 2024-02-22 19:41:14.000000 eis-documents-1.8.1/README.md
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-22 19:51:32.209933 eis-documents-1.8.1/eis/
+-rw-r--r--   0 ricard     (501) staff       (20)        0 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/__init__.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-22 19:51:32.213691 eis-documents-1.8.1/eis/document/
+-rw-r--r--   0 ricard     (501) staff       (20)      724 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/__init__.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-22 19:51:32.217820 eis-documents-1.8.1/eis/document/api/
+-rw-r--r--   0 ricard     (501) staff       (20)      226 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/__init__.py
+-rw-r--r--   0 ricard     (501) staff       (20)     5440 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/default_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    31276 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/document_templates_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    41433 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/documents_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    35537 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/docx_templates_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    30049 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/layouts_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    31551 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/product_documents_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     6402 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/search_keywords_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     7431 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/searchable_document_owners_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     7564 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api/searchable_documents_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    41630 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/api_client.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-22 19:51:32.218120 eis-documents-1.8.1/eis/document/apis/
+-rw-r--r--   0 ricard     (501) staff       (20)     1047 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/apis/__init__.py
+-rw-r--r--   0 ricard     (501) staff       (20)    16479 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/configuration.py
+-rw-r--r--   0 ricard     (501) staff       (20)     5072 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/exceptions.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-22 19:51:32.239529 eis-documents-1.8.1/eis/document/model/
+-rw-r--r--   0 ricard     (501) staff       (20)      346 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/model/__init__.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13833 2024-02-22 19:41:11.000000 eis-documents-1.8.1/eis/document/model/create_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11931 2024-02-22 19:41:11.000000 eis-documents-1.8.1/eis/document/model/create_doc_template_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    20279 2024-02-22 19:41:11.000000 eis-documents-1.8.1/eis/document/model/create_document_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11901 2024-02-22 19:41:11.000000 eis-documents-1.8.1/eis/document/model/create_document_sync_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11609 2024-02-22 19:41:11.000000 eis-documents-1.8.1/eis/document/model/create_html_template_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13422 2024-02-22 19:41:11.000000 eis-documents-1.8.1/eis/document/model/create_layout_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11849 2024-02-22 19:41:11.000000 eis-documents-1.8.1/eis/document/model/create_layout_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    17599 2024-02-22 19:41:11.000000 eis-documents-1.8.1/eis/document/model/create_presigned_post_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11975 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/create_presigned_post_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11638 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/delete_layout_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12110 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/delete_product_document_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11516 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/delete_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11699 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/delete_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    15784 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/doc_template_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    19156 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/document_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11755 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/download_document_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11644 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/get_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11922 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/get_doc_template_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11526 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/get_document_download_url_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11606 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/get_docx_template_download_url_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11629 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/get_layout_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11840 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/get_layout_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11615 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/get_product_document_download_url_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12033 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/get_product_document_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11509 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/get_signed_s3_key_url_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12884 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/grpc_create_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13058 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/grpc_update_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13700 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/html_template_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12219 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/inline_response200.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12219 2024-02-22 19:41:12.000000 eis-documents-1.8.1/eis/document/model/inline_response503.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14955 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/layout_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12417 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12182 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_doc_templates_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12089 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_documents_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12087 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_layouts_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12160 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_product_documents_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12568 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11626 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_search_keywords_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11687 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_search_keywords_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11754 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_searchable_document_owners_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11917 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_searchable_document_owners_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12553 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_searchable_documents_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12335 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/list_searchable_documents_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    17535 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/product_document_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13906 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/searchable_document_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11910 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/searchable_document_owner_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12497 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/shared_update_docx_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14197 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/update_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11931 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/update_doc_template_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13054 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/update_document_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11889 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/update_document_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12423 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/update_html_template_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13784 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/update_layout_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11849 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/update_layout_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13564 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/upload_docx_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14512 2024-02-22 19:41:13.000000 eis-documents-1.8.1/eis/document/model/upload_product_document_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    82488 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/model_utils.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-22 19:51:32.239935 eis-documents-1.8.1/eis/document/models/
+-rw-r--r--   0 ricard     (501) staff       (20)     5366 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/models/__init__.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14274 2024-02-22 19:41:14.000000 eis-documents-1.8.1/eis/document/rest.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-22 19:51:32.240977 eis-documents-1.8.1/eis_documents.egg-info/
+-rw-r--r--   0 ricard     (501) staff       (20)      333 2024-02-22 19:51:32.000000 eis-documents-1.8.1/eis_documents.egg-info/PKG-INFO
+-rw-r--r--   0 ricard     (501) staff       (20)     6571 2024-02-22 19:51:32.000000 eis-documents-1.8.1/eis_documents.egg-info/SOURCES.txt
+-rw-r--r--   0 ricard     (501) staff       (20)        1 2024-02-22 19:51:32.000000 eis-documents-1.8.1/eis_documents.egg-info/dependency_links.txt
+-rw-r--r--   0 ricard     (501) staff       (20)       32 2024-02-22 19:51:32.000000 eis-documents-1.8.1/eis_documents.egg-info/requires.txt
+-rw-r--r--   0 ricard     (501) staff       (20)        4 2024-02-22 19:51:32.000000 eis-documents-1.8.1/eis_documents.egg-info/top_level.txt
+-rw-r--r--   0 ricard     (501) staff       (20)      162 2024-02-22 19:51:32.265380 eis-documents-1.8.1/setup.cfg
+-rw-r--r--   0 ricard     (501) staff       (20)      990 2024-02-22 19:41:14.000000 eis-documents-1.8.1/setup.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-02-22 19:51:32.264645 eis-documents-1.8.1/test/
+-rw-r--r--   0 ricard     (501) staff       (20)      981 2024-02-22 19:41:11.000000 eis-documents-1.8.1/test/test_create_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      981 2024-02-22 19:41:11.000000 eis-documents-1.8.1/test/test_create_doc_template_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      822 2024-02-22 19:41:11.000000 eis-documents-1.8.1/test/test_create_document_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      975 2024-02-22 19:41:11.000000 eis-documents-1.8.1/test/test_create_document_sync_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      801 2024-02-22 19:41:11.000000 eis-documents-1.8.1/test/test_create_html_template_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      945 2024-02-22 19:41:11.000000 eis-documents-1.8.1/test/test_create_layout_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      924 2024-02-22 19:41:11.000000 eis-documents-1.8.1/test/test_create_layout_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      858 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_create_presigned_post_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      879 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_create_presigned_post_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      641 2024-02-22 19:41:14.000000 eis-documents-1.8.1/test/test_default_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      808 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_delete_layout_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      872 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_delete_product_document_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      765 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_delete_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      786 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_delete_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      980 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_doc_template_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      743 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_document_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1412 2024-02-22 19:41:14.000000 eis-documents-1.8.1/test/test_document_templates_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1671 2024-02-22 19:41:14.000000 eis-documents-1.8.1/test/test_documents_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1570 2024-02-22 19:41:14.000000 eis-documents-1.8.1/test/test_docx_templates_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      836 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_download_document_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      823 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_get_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      960 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_get_doc_template_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      901 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_get_document_download_url_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      930 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_get_docx_template_download_url_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      787 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_get_layout_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      903 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_get_layout_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      951 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_get_product_document_download_url_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1004 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_get_product_document_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      867 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_get_signed_s3_key_url_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1010 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_grpc_create_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1010 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_grpc_update_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      772 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_html_template_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      771 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_inline_response200.py
+-rw-r--r--   0 ricard     (501) staff       (20)      771 2024-02-22 19:41:12.000000 eis-documents-1.8.1/test/test_inline_response503.py
+-rw-r--r--   0 ricard     (501) staff       (20)      849 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_layout_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1246 2024-02-22 19:41:14.000000 eis-documents-1.8.1/test/test_layouts_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      830 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      974 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_doc_templates_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      939 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_documents_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      917 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_layouts_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1018 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_product_documents_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      751 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      851 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_search_keywords_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      872 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_search_keywords_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      922 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_searchable_document_owners_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1108 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_searchable_document_owners_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      886 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_searchable_documents_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1051 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_list_searchable_documents_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      793 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_product_document_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1470 2024-02-22 19:41:14.000000 eis-documents-1.8.1/test/test_product_documents_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      743 2024-02-22 19:41:14.000000 eis-documents-1.8.1/test/test_search_keywords_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      814 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_searchable_document_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      850 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_searchable_document_owner_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      834 2024-02-22 19:41:14.000000 eis-documents-1.8.1/test/test_searchable_document_owners_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      790 2024-02-22 19:41:14.000000 eis-documents-1.8.1/test/test_searchable_documents_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      894 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_shared_update_docx_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      981 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_update_doc_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      981 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_update_doc_template_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      822 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_update_document_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      946 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_update_document_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      801 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_update_html_template_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      945 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_update_layout_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      924 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_update_layout_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      851 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_upload_docx_template_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      872 2024-02-22 19:41:13.000000 eis-documents-1.8.1/test/test_upload_product_document_request_dto.py
```

### Comparing `eis-documents-1.7.1/README.md` & `eis-documents-1.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # eis-documents
 The EMIL DocumentService API description
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0
-- Package version: 1.7.1
+- Package version: 1.8.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.emil.de](https://www.emil.de)
 
 ## Requirements.
 
 Python >=3.6
 
@@ -88,15 +88,15 @@
 # Enter a context with an instance of the API client
 with eis.document.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = document_templates_api.DocumentTemplatesApi(api_client)
     create_doc_template_request_dto = CreateDocTemplateRequestDto(
         name="SEPA template",
         slug="SEPA-template",
-        layout_id=2,
+        layout_id=5,
         body_template=None,
         product_slug="car-insurance",
         label="SEPA-Lastschriftmandat",
     ) # CreateDocTemplateRequestDto | 
     authorization = "Authorization_example" # str | Bearer Token (optional)
 
     try:
```

### Comparing `eis-documents-1.7.1/eis/document/__init__.py` & `eis-documents-1.8.1/eis/document/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 1.0
     Contact: kontakt@emil.de
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.7.1"
+__version__ = "1.8.1"
 
 # import ApiClient
 from eis.document.api_client import ApiClient
 
 # import Configuration
 from eis.document.configuration import Configuration
```

### Comparing `eis-documents-1.7.1/eis/document/api/default_api.py` & `eis-documents-1.8.1/eis/document/api/default_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/api/document_templates_api.py` & `eis-documents-1.8.1/eis/document/api/document_templates_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/api/documents_api.py` & `eis-documents-1.8.1/eis/document/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/api/docx_templates_api.py` & `eis-documents-1.8.1/eis/document/api/docx_templates_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/api/layouts_api.py` & `eis-documents-1.8.1/eis/document/api/layouts_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/api/product_documents_api.py` & `eis-documents-1.8.1/eis/document/api/product_documents_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/api/search_keywords_api.py` & `eis-documents-1.8.1/eis/document/api/search_keywords_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/api/searchable_document_owners_api.py` & `eis-documents-1.8.1/eis/document/api/searchable_document_owners_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/api/searchable_documents_api.py` & `eis-documents-1.8.1/eis/document/api/searchable_documents_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/api_client.py` & `eis-documents-1.8.1/eis/document/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.7.1/python'
+        self.user_agent = 'OpenAPI-Generator/1.8.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `eis-documents-1.7.1/eis/document/apis/__init__.py` & `eis-documents-1.8.1/eis/document/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/configuration.py` & `eis-documents-1.8.1/eis/document/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.7.1".\
+               "SDK Package Version: 1.8.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `eis-documents-1.7.1/eis/document/exceptions.py` & `eis-documents-1.8.1/eis/document/exceptions.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/create_doc_template_request_dto.py` & `eis-documents-1.8.1/eis/document/model/create_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/create_doc_template_response_class.py` & `eis-documents-1.8.1/eis/document/model/create_doc_template_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/create_document_request_dto.py` & `eis-documents-1.8.1/eis/document/model/create_document_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/create_document_sync_response_class.py` & `eis-documents-1.8.1/eis/document/model/create_document_sync_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/create_html_template_dto.py` & `eis-documents-1.8.1/eis/document/model/create_html_template_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/create_layout_request_dto.py` & `eis-documents-1.8.1/eis/document/model/create_layout_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/create_layout_response_class.py` & `eis-documents-1.8.1/eis/document/model/create_layout_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/create_presigned_post_request_dto.py` & `eis-documents-1.8.1/eis/document/model/create_presigned_post_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/create_presigned_post_response_class.py` & `eis-documents-1.8.1/eis/document/model/create_presigned_post_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/delete_layout_request_dto.py` & `eis-documents-1.8.1/eis/document/model/delete_layout_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/delete_product_document_request_dto.py` & `eis-documents-1.8.1/eis/document/model/delete_product_document_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/delete_request_dto.py` & `eis-documents-1.8.1/eis/document/model/delete_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/delete_response_class.py` & `eis-documents-1.8.1/eis/document/model/delete_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/doc_template_class.py` & `eis-documents-1.8.1/eis/document/model/doc_template_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/document_class.py` & `eis-documents-1.8.1/eis/document/model/document_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/download_document_request_dto.py` & `eis-documents-1.8.1/eis/document/model/download_document_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/get_doc_template_request_dto.py` & `eis-documents-1.8.1/eis/document/model/get_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/get_doc_template_response_class.py` & `eis-documents-1.8.1/eis/document/model/get_doc_template_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/get_document_download_url_response_class.py` & `eis-documents-1.8.1/eis/document/model/get_document_download_url_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/get_docx_template_download_url_response_class.py` & `eis-documents-1.8.1/eis/document/model/get_docx_template_download_url_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/get_layout_request_dto.py` & `eis-documents-1.8.1/eis/document/model/get_layout_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/get_layout_response_class.py` & `eis-documents-1.8.1/eis/document/model/get_layout_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/get_product_document_download_url_response_class.py` & `eis-documents-1.8.1/eis/document/model/get_product_document_download_url_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/get_product_document_response_class.py` & `eis-documents-1.8.1/eis/document/model/get_product_document_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/get_signed_s3_key_url_response_class.py` & `eis-documents-1.8.1/eis/document/model/get_signed_s3_key_url_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/grpc_create_doc_template_request_dto.py` & `eis-documents-1.8.1/eis/document/model/grpc_create_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/grpc_update_doc_template_request_dto.py` & `eis-documents-1.8.1/eis/document/model/grpc_update_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/html_template_class.py` & `eis-documents-1.8.1/eis/document/model/html_template_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/inline_response200.py` & `eis-documents-1.8.1/eis/document/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/inline_response503.py` & `eis-documents-1.8.1/eis/document/model/inline_response503.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/layout_class.py` & `eis-documents-1.8.1/eis/document/model/layout_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_doc_template_request_dto.py` & `eis-documents-1.8.1/eis/document/model/list_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_doc_templates_response_class.py` & `eis-documents-1.8.1/eis/document/model/list_doc_templates_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_documents_response_class.py` & `eis-documents-1.8.1/eis/document/model/list_documents_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_layouts_response_class.py` & `eis-documents-1.8.1/eis/document/model/list_layouts_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_product_documents_response_class.py` & `eis-documents-1.8.1/eis/document/model/list_product_documents_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_request_dto.py` & `eis-documents-1.8.1/eis/document/model/list_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_search_keywords_request_dto.py` & `eis-documents-1.8.1/eis/document/model/list_search_keywords_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_search_keywords_response_class.py` & `eis-documents-1.8.1/eis/document/model/list_search_keywords_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_searchable_document_owners_request_dto.py` & `eis-documents-1.8.1/eis/document/model/list_searchable_document_owners_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_searchable_document_owners_response_class.py` & `eis-documents-1.8.1/eis/document/model/list_searchable_document_owners_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_searchable_documents_request_dto.py` & `eis-documents-1.8.1/eis/document/model/list_searchable_documents_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/list_searchable_documents_response_class.py` & `eis-documents-1.8.1/eis/document/model/list_searchable_documents_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/product_document_class.py` & `eis-documents-1.8.1/eis/document/model/product_document_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,64 +112,73 @@
                 and the value is attribute type.
         """
         return {
             'id': (float,),  # noqa: E501
             'code': (str,),  # noqa: E501
             'product_code': (str,),  # noqa: E501
             'product_version_id': (float,),  # noqa: E501
+            'slug': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             's3_key': (str,),  # noqa: E501
             'content_type': (str,),  # noqa: E501
             'entity_type': (str,),  # noqa: E501
             'product_slug': (str,),  # noqa: E501
+            'version_number': (float,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
+            'updated': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'code': 'code',  # noqa: E501
         'product_code': 'productCode',  # noqa: E501
         'product_version_id': 'productVersionId',  # noqa: E501
+        'slug': 'slug',  # noqa: E501
         'type': 'type',  # noqa: E501
         'description': 'description',  # noqa: E501
         's3_key': 's3Key',  # noqa: E501
         'content_type': 'contentType',  # noqa: E501
         'entity_type': 'entityType',  # noqa: E501
         'product_slug': 'productSlug',  # noqa: E501
+        'version_number': 'versionNumber',  # noqa: E501
         'created_at': 'createdAt',  # noqa: E501
+        'updated': 'updated',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, code, product_code, product_version_id, type, description, s3_key, content_type, entity_type, product_slug, created_at, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, code, product_code, product_version_id, slug, type, description, s3_key, content_type, entity_type, product_slug, version_number, created_at, updated, *args, **kwargs):  # noqa: E501
         """ProductDocumentClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             code (str): Unique identifier for the object.
             product_code (str): Unique identifier of the product that this object belongs to.
             product_version_id (float): Unique identifier referencing the product.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
             type (str): Type of the product document.
             description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
             s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
             content_type (str): Type of the document expressed with its file extension.
             entity_type (str): Product Document entity type.
             product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
+            version_number (float): The current version number of the product document.
             created_at (datetime): Time at which the object was created.
+            updated (datetime): Time at which the object was created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,21 +238,24 @@
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.code = code
         self.product_code = product_code
         self.product_version_id = product_version_id
+        self.slug = slug
         self.type = type
         self.description = description
         self.s3_key = s3_key
         self.content_type = content_type
         self.entity_type = entity_type
         self.product_slug = product_slug
+        self.version_number = version_number
         self.created_at = created_at
+        self.updated = updated
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -256,29 +268,32 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, code, product_code, product_version_id, type, description, s3_key, content_type, entity_type, product_slug, created_at, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, code, product_code, product_version_id, slug, type, description, s3_key, content_type, entity_type, product_slug, version_number, created_at, updated, *args, **kwargs):  # noqa: E501
         """ProductDocumentClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             code (str): Unique identifier for the object.
             product_code (str): Unique identifier of the product that this object belongs to.
             product_version_id (float): Unique identifier referencing the product.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
             type (str): Type of the product document.
             description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
             s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
             content_type (str): Type of the document expressed with its file extension.
             entity_type (str): Product Document entity type.
             product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
+            version_number (float): The current version number of the product document.
             created_at (datetime): Time at which the object was created.
+            updated (datetime): Time at which the object was created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -336,21 +351,24 @@
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.code = code
         self.product_code = product_code
         self.product_version_id = product_version_id
+        self.slug = slug
         self.type = type
         self.description = description
         self.s3_key = s3_key
         self.content_type = content_type
         self.entity_type = entity_type
         self.product_slug = product_slug
+        self.version_number = version_number
         self.created_at = created_at
+        self.updated = updated
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-documents-1.7.1/eis/document/model/searchable_document_class.py` & `eis-documents-1.8.1/eis/document/model/searchable_document_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/searchable_document_owner_class.py` & `eis-documents-1.8.1/eis/document/model/searchable_document_owner_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/shared_update_docx_template_request_dto.py` & `eis-documents-1.8.1/eis/document/model/shared_update_docx_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/update_doc_template_request_dto.py` & `eis-documents-1.8.1/eis/document/model/update_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/update_doc_template_response_class.py` & `eis-documents-1.8.1/eis/document/model/update_doc_template_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/update_document_request_dto.py` & `eis-documents-1.8.1/eis/document/model/update_document_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/update_document_response_class.py` & `eis-documents-1.8.1/eis/document/model/update_document_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/update_html_template_dto.py` & `eis-documents-1.8.1/eis/document/model/update_html_template_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/update_layout_request_dto.py` & `eis-documents-1.8.1/eis/document/model/update_layout_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/update_layout_response_class.py` & `eis-documents-1.8.1/eis/document/model/update_layout_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/upload_docx_template_request_dto.py` & `eis-documents-1.8.1/eis/document/model/upload_docx_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/model/upload_product_document_request_dto.py` & `eis-documents-1.8.1/eis/document/model/upload_product_document_request_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'content_type': (str,),  # noqa: E501
+            'slug': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'filename': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'entity_type': (str,),  # noqa: E501
             'product_slug': (str,),  # noqa: E501
             'product_version_id': (float,),  # noqa: E501
         }
@@ -102,14 +103,15 @@
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'content_type': 'contentType',  # noqa: E501
+        'slug': 'slug',  # noqa: E501
         'description': 'description',  # noqa: E501
         'filename': 'filename',  # noqa: E501
         'type': 'type',  # noqa: E501
         'entity_type': 'entityType',  # noqa: E501
         'product_slug': 'productSlug',  # noqa: E501
         'product_version_id': 'productVersionId',  # noqa: E501
     }
@@ -117,19 +119,20 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, content_type, description, filename, type, entity_type, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, content_type, slug, description, filename, type, entity_type, *args, **kwargs):  # noqa: E501
         """UploadProductDocumentRequestDto - a model defined in OpenAPI
 
         Args:
             content_type (str): Extension of the file.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
             description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
             filename (str): Name of the file the end user will see when he downloads it.
             type (str): Type of the product document.
             entity_type (str): Entity type of the product document.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -192,14 +195,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.content_type = content_type
+        self.slug = slug
         self.description = description
         self.filename = filename
         self.type = type
         self.entity_type = entity_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
@@ -216,19 +220,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, content_type, description, filename, type, entity_type, *args, **kwargs):  # noqa: E501
+    def __init__(self, content_type, slug, description, filename, type, entity_type, *args, **kwargs):  # noqa: E501
         """UploadProductDocumentRequestDto - a model defined in OpenAPI
 
         Args:
             content_type (str): Extension of the file.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
             description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
             filename (str): Name of the file the end user will see when he downloads it.
             type (str): Type of the product document.
             entity_type (str): Entity type of the product document.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -289,14 +294,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.content_type = content_type
+        self.slug = slug
         self.description = description
         self.filename = filename
         self.type = type
         self.entity_type = entity_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
```

### Comparing `eis-documents-1.7.1/eis/document/model_utils.py` & `eis-documents-1.8.1/eis/document/model_utils.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/models/__init__.py` & `eis-documents-1.8.1/eis/document/models/__init__.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis/document/rest.py` & `eis-documents-1.8.1/eis/document/rest.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/eis_documents.egg-info/SOURCES.txt` & `eis-documents-1.8.1/eis_documents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/setup.py` & `eis-documents-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "eis-documents"
-VERSION = "1.7.1"
+VERSION = "1.8.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `eis-documents-1.7.1/test/test_create_doc_template_request_dto.py` & `eis-documents-1.8.1/test/test_create_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_create_doc_template_response_class.py` & `eis-documents-1.8.1/test/test_create_doc_template_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_create_document_request_dto.py` & `eis-documents-1.8.1/test/test_create_document_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_create_document_sync_response_class.py` & `eis-documents-1.8.1/test/test_create_document_sync_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_create_html_template_dto.py` & `eis-documents-1.8.1/test/test_create_html_template_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_create_layout_request_dto.py` & `eis-documents-1.8.1/test/test_create_layout_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_create_layout_response_class.py` & `eis-documents-1.8.1/test/test_create_layout_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_create_presigned_post_request_dto.py` & `eis-documents-1.8.1/test/test_create_presigned_post_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_create_presigned_post_response_class.py` & `eis-documents-1.8.1/test/test_create_presigned_post_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_default_api.py` & `eis-documents-1.8.1/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_delete_layout_request_dto.py` & `eis-documents-1.8.1/test/test_delete_layout_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_delete_product_document_request_dto.py` & `eis-documents-1.8.1/test/test_delete_product_document_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_delete_request_dto.py` & `eis-documents-1.8.1/test/test_delete_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_delete_response_class.py` & `eis-documents-1.8.1/test/test_delete_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_doc_template_class.py` & `eis-documents-1.8.1/test/test_doc_template_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_document_class.py` & `eis-documents-1.8.1/test/test_document_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_document_templates_api.py` & `eis-documents-1.8.1/test/test_document_templates_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_documents_api.py` & `eis-documents-1.8.1/test/test_documents_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_docx_templates_api.py` & `eis-documents-1.8.1/test/test_docx_templates_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_download_document_request_dto.py` & `eis-documents-1.8.1/test/test_download_document_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_get_doc_template_request_dto.py` & `eis-documents-1.8.1/test/test_get_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_get_doc_template_response_class.py` & `eis-documents-1.8.1/test/test_get_doc_template_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_get_document_download_url_response_class.py` & `eis-documents-1.8.1/test/test_get_document_download_url_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_get_docx_template_download_url_response_class.py` & `eis-documents-1.8.1/test/test_get_docx_template_download_url_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_get_layout_request_dto.py` & `eis-documents-1.8.1/test/test_get_layout_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_get_layout_response_class.py` & `eis-documents-1.8.1/test/test_get_layout_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_get_product_document_download_url_response_class.py` & `eis-documents-1.8.1/test/test_get_product_document_download_url_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_get_product_document_response_class.py` & `eis-documents-1.8.1/test/test_get_product_document_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_get_signed_s3_key_url_response_class.py` & `eis-documents-1.8.1/test/test_get_signed_s3_key_url_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_grpc_create_doc_template_request_dto.py` & `eis-documents-1.8.1/test/test_grpc_create_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_grpc_update_doc_template_request_dto.py` & `eis-documents-1.8.1/test/test_grpc_update_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_html_template_class.py` & `eis-documents-1.8.1/test/test_html_template_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_inline_response200.py` & `eis-documents-1.8.1/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_inline_response503.py` & `eis-documents-1.8.1/test/test_inline_response503.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_layout_class.py` & `eis-documents-1.8.1/test/test_layout_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_layouts_api.py` & `eis-documents-1.8.1/test/test_layouts_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_doc_template_request_dto.py` & `eis-documents-1.8.1/test/test_list_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_doc_templates_response_class.py` & `eis-documents-1.8.1/test/test_list_doc_templates_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_documents_response_class.py` & `eis-documents-1.8.1/test/test_list_documents_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_layouts_response_class.py` & `eis-documents-1.8.1/test/test_list_layouts_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_product_documents_response_class.py` & `eis-documents-1.8.1/test/test_list_product_documents_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_request_dto.py` & `eis-documents-1.8.1/test/test_list_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_search_keywords_request_dto.py` & `eis-documents-1.8.1/test/test_list_search_keywords_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_search_keywords_response_class.py` & `eis-documents-1.8.1/test/test_list_search_keywords_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_searchable_document_owners_request_dto.py` & `eis-documents-1.8.1/test/test_list_searchable_document_owners_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_searchable_document_owners_response_class.py` & `eis-documents-1.8.1/test/test_list_searchable_document_owners_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_searchable_documents_request_dto.py` & `eis-documents-1.8.1/test/test_list_searchable_documents_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_list_searchable_documents_response_class.py` & `eis-documents-1.8.1/test/test_list_searchable_documents_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_product_document_class.py` & `eis-documents-1.8.1/test/test_product_document_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_product_documents_api.py` & `eis-documents-1.8.1/test/test_product_documents_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_search_keywords_api.py` & `eis-documents-1.8.1/test/test_search_keywords_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_searchable_document_class.py` & `eis-documents-1.8.1/test/test_searchable_document_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_searchable_document_owner_class.py` & `eis-documents-1.8.1/test/test_searchable_document_owner_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_searchable_document_owners_api.py` & `eis-documents-1.8.1/test/test_searchable_document_owners_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_searchable_documents_api.py` & `eis-documents-1.8.1/test/test_searchable_documents_api.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_shared_update_docx_template_request_dto.py` & `eis-documents-1.8.1/test/test_shared_update_docx_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_update_doc_template_request_dto.py` & `eis-documents-1.8.1/test/test_update_doc_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_update_doc_template_response_class.py` & `eis-documents-1.8.1/test/test_update_doc_template_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_update_document_request_dto.py` & `eis-documents-1.8.1/test/test_update_document_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_update_document_response_class.py` & `eis-documents-1.8.1/test/test_update_document_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_update_html_template_dto.py` & `eis-documents-1.8.1/test/test_update_html_template_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_update_layout_request_dto.py` & `eis-documents-1.8.1/test/test_update_layout_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_update_layout_response_class.py` & `eis-documents-1.8.1/test/test_update_layout_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_upload_docx_template_request_dto.py` & `eis-documents-1.8.1/test/test_upload_docx_template_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-documents-1.7.1/test/test_upload_product_document_request_dto.py` & `eis-documents-1.8.1/test/test_upload_product_document_request_dto.py`

 * *Files identical despite different names*

