# Comparing `tmp/eis-publicapi-1.22.1.tar.gz` & `tmp/eis-publicapi-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis-publicapi-1.22.1.tar", last modified: Wed May 22 17:33:11 2024, max compression
+gzip compressed data, was "eis-publicapi-1.6.0.tar", last modified: Sun Oct  1 20:51:13 2023, max compression
```

## Comparing `eis-publicapi-1.22.1.tar` & `eis-publicapi-1.6.0.tar`

### file list

```diff
@@ -1,187 +1,155 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:33:11.185123 eis-publicapi-1.22.1/
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-05-22 17:33:11.185123 eis-publicapi-1.22.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14165 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:33:11.165123 eis-publicapi-1.22.1/eis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:33:11.169123 eis-publicapi-1.22.1/eis/publicapi/
--rw-rw-rw-   0 root         (0) root         (0)      718 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:33:11.169123 eis-publicapi-1.22.1/eis/publicapi/api/
--rw-rw-rw-   0 root         (0) root         (0)      239 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14852 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/api/address_completions_validations_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/api/default_api.py
--rw-rw-rw-   0 root         (0) root         (0)    45336 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/api/documents_api.py
--rw-rw-rw-   0 root         (0) root         (0)    40175 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/api/leads_api.py
--rw-rw-rw-   0 root         (0) root         (0)    18326 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/api/notifications_api.py
--rw-rw-rw-   0 root         (0) root         (0)    19559 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/api/payments_setup_api.py
--rw-rw-rw-   0 root         (0) root         (0)    50023 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/api/products_api.py
--rw-rw-rw-   0 root         (0) root         (0)    41652 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:33:11.169123 eis-publicapi-1.22.1/eis/publicapi/apis/
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16467 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5057 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:33:11.177123 eis-publicapi-1.22.1/eis/publicapi/model/
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13225 2024-05-22 17:33:09.000000 eis-publicapi-1.22.1/eis/publicapi/model/address_completion_item_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11951 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/address_completion_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13471 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/address_field_score_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12227 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/calculate_product_fields_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11977 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/calculate_product_fields_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12781 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/complete_braintree_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11835 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/complete_email_verification_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11584 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/complete_email_verification_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12347 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/complete_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12109 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/complete_payment_setup_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13547 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/complete_stripe_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    19172 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_account_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11847 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_bank_account_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12164 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_custom_application_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11914 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_custom_application_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    17709 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_document_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13793 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_estimated_invoice_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13337 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_estimated_invoice_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11589 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_lead_async_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    22586 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11825 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11910 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_payment_method_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    17068 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_presigned_post_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11962 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/create_presigned_post_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    18103 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/document_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11568 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/get_custom_css_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11816 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/get_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11532 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/get_product_document_download_url_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11926 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/get_public_psp_settings_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/initiate_braintree_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11795 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/initiate_braintree_payment_setup_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12000 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/initiate_email_verification_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11584 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/initiate_email_verification_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11634 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/initiate_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12347 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/initiate_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12817 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/initiate_payment_setup_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11940 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/initiate_stripe_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12187 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/initiate_stripe_payment_setup_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12710 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/inline_response200.py
--rw-rw-rw-   0 root         (0) root         (0)    12710 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/inline_response503.py
--rw-rw-rw-   0 root         (0) root         (0)    16084 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/insured_object_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13019 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/insured_object_type_class.py
--rw-rw-rw-   0 root         (0) root         (0)    18072 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/invoice_class.py
--rw-rw-rw-   0 root         (0) root         (0)    16809 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/invoice_item_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12544 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/invoice_status_class.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/lead_account_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/lead_bank_account_class.py
--rw-rw-rw-   0 root         (0) root         (0)    17729 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/lead_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12958 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/lead_policy_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12620 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/lead_policy_object_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12075 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/list_documents_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12148 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/list_product_documents_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12057 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/list_products_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13642 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/payment_method_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12971 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/policy_object_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13030 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/policy_object_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12865 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/premium_override_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11888 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/premium_override_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    15252 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/product_class.py
--rw-rw-rw-   0 root         (0) root         (0)    16491 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/product_document_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13611 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/product_factor_for_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)    18710 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/product_field_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13406 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/product_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12826 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/send_notification_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11542 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/send_notification_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11620 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/sepa_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13023 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/structured_address_class.py
--rw-rw-rw-   0 root         (0) root         (0)    14011 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/suggested_address_details_class.py
--rw-rw-rw-   0 root         (0) root         (0)    21032 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/update_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11825 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/update_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11511 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/uploaded_document_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13937 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model/validate_address_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    82778 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/model_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:33:11.177123 eis-publicapi-1.22.1/eis/publicapi/models/
--rw-rw-rw-   0 root         (0) root         (0)     6758 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14260 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/eis/publicapi/rest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:33:11.177123 eis-publicapi-1.22.1/eis_publicapi.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-05-22 17:33:11.000000 eis-publicapi-1.22.1/eis_publicapi.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7898 2024-05-22 17:33:11.000000 eis-publicapi-1.22.1/eis_publicapi.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 17:33:11.000000 eis-publicapi-1.22.1/eis_publicapi.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-22 17:33:11.000000 eis-publicapi-1.22.1/eis_publicapi.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-22 17:33:11.000000 eis-publicapi-1.22.1/eis_publicapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-22 17:33:11.185123 eis-publicapi-1.22.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:33:11.185123 eis-publicapi-1.22.1/test/
--rw-rw-rw-   0 root         (0) root         (0)      989 2024-05-22 17:33:09.000000 eis-publicapi-1.22.1/test/test_address_completion_item_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1009 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_address_completion_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_address_completions_validations_api.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_address_field_score_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_calculate_product_fields_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_calculate_product_fields_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_complete_braintree_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_complete_email_verification_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_complete_email_verification_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_complete_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_complete_payment_setup_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_complete_stripe_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_account_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      831 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_bank_account_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_custom_application_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_custom_application_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_document_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1162 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_estimated_invoice_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_estimated_invoice_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_lead_async_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_payment_method_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_presigned_post_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_create_presigned_post_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_default_api.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_document_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1698 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_documents_api.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_get_custom_css_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_get_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_get_product_document_download_url_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_get_public_psp_settings_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_initiate_braintree_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_initiate_braintree_payment_setup_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_initiate_email_verification_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_initiate_email_verification_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_initiate_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_initiate_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_initiate_payment_setup_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_initiate_stripe_payment_setup_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_initiate_stripe_payment_setup_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_inline_response200.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_inline_response503.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_insured_object_class.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_insured_object_type_class.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_invoice_class.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_invoice_item_class.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_invoice_status_class.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_lead_account_class.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_lead_bank_account_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_lead_class.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_lead_policy_class.py
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_lead_policy_object_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_leads_api.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_list_documents_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_list_product_documents_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_list_products_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_notifications_api.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_payment_method_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_payments_setup_api.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_policy_object_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_policy_object_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_premium_override_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_premium_override_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_product_class.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_product_document_class.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_product_factor_for_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_product_field_class.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_product_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_products_api.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_send_notification_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_send_notification_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_sepa_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_structured_address_class.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_suggested_address_details_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1532 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_update_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_update_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_uploaded_document_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2024-05-22 17:33:10.000000 eis-publicapi-1.22.1/test/test_validate_address_response_class.py
+drwxr-xr-x   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:51:13.550339 eis-publicapi-1.6.0/
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11671 2023-10-01 20:51:13.550441 eis-publicapi-1.6.0/PKG-INFO
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11414 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/README.md
+drwxr-xr-x   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:51:13.516111 eis-publicapi-1.6.0/eis/
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/__init__.py
+drwxr-xr-x   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:51:13.517140 eis-publicapi-1.6.0/eis/publicapi/
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      717 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/__init__.py
+drwxr-xr-x   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:51:13.522279 eis-publicapi-1.6.0/eis/publicapi/api/
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      239 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/api/__init__.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    14671 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/api/address_completions_validations_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    28079 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/api/documents_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    22892 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/api/leads_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     6593 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/api/notifications_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    19559 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/api/payments_setup_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    43722 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/api/products_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    41651 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/api_client.py
+drwxr-xr-x   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:51:13.522447 eis-publicapi-1.6.0/eis/publicapi/apis/
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      863 2023-10-01 20:43:10.000000 eis-publicapi-1.6.0/eis/publicapi/apis/__init__.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    16466 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/configuration.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     5057 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/exceptions.py
+drwxr-xr-x   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:51:13.531848 eis-publicapi-1.6.0/eis/publicapi/model/
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      347 2023-10-01 20:43:10.000000 eis-publicapi-1.6.0/eis/publicapi/model/__init__.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13225 2023-10-01 20:43:04.000000 eis-publicapi-1.6.0/eis/publicapi/model/address_completion_item_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11951 2023-10-01 20:43:04.000000 eis-publicapi-1.6.0/eis/publicapi/model/address_completion_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13471 2023-10-01 20:43:04.000000 eis-publicapi-1.6.0/eis/publicapi/model/address_field_score_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12781 2023-10-01 20:43:04.000000 eis-publicapi-1.6.0/eis/publicapi/model/complete_braintree_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12347 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/complete_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12109 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/complete_payment_setup_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13547 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/complete_stripe_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    16800 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/create_account_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11847 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/create_bank_account_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12164 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/create_custom_application_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11914 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/create_custom_application_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    16384 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/create_document_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13793 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/create_estimated_invoice_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12668 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/create_estimated_invoice_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    16688 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/create_lead_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11825 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/eis/publicapi/model/create_lead_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    17641 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/document_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11568 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/get_custom_css_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11816 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/get_lead_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11926 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/get_public_psp_settings_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11949 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/initiate_braintree_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11795 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/initiate_braintree_payment_setup_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11634 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/initiate_lead_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12347 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/initiate_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12817 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/initiate_payment_setup_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11940 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/initiate_stripe_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12187 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/initiate_stripe_payment_setup_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    16084 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/insured_object_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13019 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/eis/publicapi/model/insured_object_type_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    18072 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/invoice_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    16295 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/invoice_item_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12544 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/invoice_status_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    15822 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/lead_account_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11884 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/lead_bank_account_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    16862 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/lead_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12958 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/lead_policy_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12127 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/lead_policy_object_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12075 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/list_documents_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12148 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/list_product_documents_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12057 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/list_products_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13642 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/payment_method_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12308 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/policy_object_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12831 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/eis/publicapi/model/premium_override_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11888 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/premium_override_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    14865 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/product_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    15358 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/product_document_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13581 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/product_factor_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    18710 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/product_field_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13406 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/product_version_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    12826 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/send_notification_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11542 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/send_notification_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13023 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/structured_address_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    14011 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/suggested_address_details_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    15482 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/update_lead_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11825 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/update_lead_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11511 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/eis/publicapi/model/uploaded_document_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    13937 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/model/validate_address_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    82474 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/model_utils.py
+drwxr-xr-x   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:51:13.532013 eis-publicapi-1.6.0/eis/publicapi/models/
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     5326 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/models/__init__.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    14260 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/eis/publicapi/rest.py
+drwxr-xr-x   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:51:13.532826 eis-publicapi-1.6.0/eis_publicapi.egg-info/
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)    11671 2023-10-01 20:51:13.000000 eis-publicapi-1.6.0/eis_publicapi.egg-info/PKG-INFO
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     6296 2023-10-01 20:51:13.000000 eis-publicapi-1.6.0/eis_publicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)        1 2023-10-01 20:51:13.000000 eis-publicapi-1.6.0/eis_publicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)       32 2023-10-01 20:51:13.000000 eis-publicapi-1.6.0/eis_publicapi.egg-info/requires.txt
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)        4 2023-10-01 20:51:13.000000 eis-publicapi-1.6.0/eis_publicapi.egg-info/top_level.txt
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      162 2023-10-01 20:51:13.550801 eis-publicapi-1.6.0/setup.cfg
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      869 2023-10-01 20:51:11.000000 eis-publicapi-1.6.0/setup.py
+drwxr-xr-x   0 thomasprovoost   (501) staff       (20)        0 2023-10-01 20:51:13.550175 eis-publicapi-1.6.0/test/
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      989 2023-10-01 20:43:04.000000 eis-publicapi-1.6.0/test/test_address_completion_item_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1009 2023-10-01 20:43:04.000000 eis-publicapi-1.6.0/test/test_address_completion_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      981 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/test/test_address_completions_validations_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      795 2023-10-01 20:43:04.000000 eis-publicapi-1.6.0/test/test_address_field_score_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      916 2023-10-01 20:43:04.000000 eis-publicapi-1.6.0/test/test_complete_braintree_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1264 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_complete_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      998 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_complete_payment_setup_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      895 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_complete_stripe_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      802 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_create_account_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      831 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_create_bank_account_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      873 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_create_custom_application_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      894 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_create_custom_application_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      809 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_create_document_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1162 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_create_estimated_invoice_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      987 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_create_estimated_invoice_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1515 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_create_lead_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      890 2023-10-01 20:43:05.000000 eis-publicapi-1.6.0/test/test_create_lead_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      730 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_document_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1182 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/test/test_documents_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      817 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_get_custom_css_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      869 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_get_lead_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      874 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_get_public_psp_settings_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      916 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_initiate_braintree_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      937 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_initiate_braintree_payment_setup_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      816 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_initiate_lead_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1264 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_initiate_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1309 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_initiate_payment_setup_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      895 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_initiate_stripe_payment_setup_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      916 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_initiate_stripe_payment_setup_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      887 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_insured_object_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      795 2023-10-01 20:43:06.000000 eis-publicapi-1.6.0/test/test_insured_object_type_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      965 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_invoice_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      752 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_invoice_item_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      766 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_invoice_status_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      752 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_lead_account_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      781 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_lead_bank_account_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1420 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_lead_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      883 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_lead_policy_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      788 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_lead_policy_object_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1075 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/test/test_leads_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      927 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_list_documents_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1006 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_list_product_documents_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      916 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_list_products_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      719 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/test/test_notifications_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      766 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_payment_method_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1066 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/test/test_payments_setup_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      795 2023-10-01 20:43:07.000000 eis-publicapi-1.6.0/test/test_policy_object_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      766 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_premium_override_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      941 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_premium_override_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      994 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_product_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      780 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_product_document_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      766 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_product_factor_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      759 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_product_field_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      773 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_product_version_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1660 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/test/test_products_api.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      823 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_send_notification_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      844 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_send_notification_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      794 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_structured_address_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      837 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_suggested_address_details_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1361 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_update_lead_request_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      890 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_update_lead_response_class.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)      773 2023-10-01 20:43:08.000000 eis-publicapi-1.6.0/test/test_uploaded_document_dto.py
+-rw-r--r--   0 thomasprovoost   (501) staff       (20)     1120 2023-10-01 20:43:09.000000 eis-publicapi-1.6.0/test/test_validate_address_response_class.py
```

### Comparing `eis-publicapi-1.22.1/README.md` & `eis-publicapi-1.6.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # eis-publicapi
 The Emil Public API description
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0
-- Package version: 1.22.1
+- Package version: 1.6.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.emil.de](https://www.emil.de)
 
 ## Requirements.
 
 Python >=3.6
 
@@ -102,86 +102,63 @@
 All URIs are relative to *https://apiv2.emil.de*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AddressCompletionsValidationsApi* | [**list_address_completions**](docs/AddressCompletionsValidationsApi.md#list_address_completions) | **GET** /publicapi/v1/addresses/completions | Retrieve the address
 *AddressCompletionsValidationsApi* | [**validate_address**](docs/AddressCompletionsValidationsApi.md#validate_address) | **GET** /publicapi/v1/addresses/validation | Retrieve the Address validation
 *DocumentsApi* | [**create_temporary_document**](docs/DocumentsApi.md#create_temporary_document) | **POST** /publicapi/v1/documents | Create the temporary document
-*DocumentsApi* | [**delete_documents**](docs/DocumentsApi.md#delete_documents) | **DELETE** /publicapi/v1/documents/{code}/lead/{leadCode} | Delete a document
 *DocumentsApi* | [**download_document**](docs/DocumentsApi.md#download_document) | **GET** /publicapi/v1/documents/download/{code} | Download a document
-*DocumentsApi* | [**download_product_document_url**](docs/DocumentsApi.md#download_product_document_url) | **GET** /publicapi/v1/documents/product/{productCode}/{code}/download-url | Get pre-signed url for downloading product document
 *DocumentsApi* | [**list_documents**](docs/DocumentsApi.md#list_documents) | **GET** /publicapi/v1/documents | List documents
 *DocumentsApi* | [**list_product_documents**](docs/DocumentsApi.md#list_product_documents) | **GET** /publicapi/v1/documents/{productCode} | List product documents
-*DocumentsApi* | [**pre_signed_post**](docs/DocumentsApi.md#pre_signed_post) | **POST** /publicapi/v1/documents/pre-signed-post | Upload documents using pre-signed URL
 *LeadsApi* | [**create_lead**](docs/LeadsApi.md#create_lead) | **POST** /publicapi/v1/leads | Create the lead
-*LeadsApi* | [**create_lead_async**](docs/LeadsApi.md#create_lead_async) | **POST** /publicapi/v1/leads-async | Create the lead asynchronously
-*LeadsApi* | [**create_lead_sync**](docs/LeadsApi.md#create_lead_sync) | **POST** /publicapi/v1/leads-sync | Create the lead synchronously
 *LeadsApi* | [**get_lead**](docs/LeadsApi.md#get_lead) | **GET** /publicapi/v1/leads/{code} | Retrieve the lead
 *LeadsApi* | [**initiate_lead**](docs/LeadsApi.md#initiate_lead) | **POST** /publicapi/v1/leads/initiate | Initiate a lead code
 *LeadsApi* | [**update_lead**](docs/LeadsApi.md#update_lead) | **PUT** /publicapi/v1/leads/{code} | Update the lead
-*LeadsApi* | [**update_lead_sync**](docs/LeadsApi.md#update_lead_sync) | **PUT** /publicapi/v1/leads-sync/{code} | Update the lead
-*NotificationsApi* | [**complete_email_verification**](docs/NotificationsApi.md#complete_email_verification) | **POST** /publicapi/v1/email-verification/complete | Complete Email Verification.
-*NotificationsApi* | [**initiate_email_verification**](docs/NotificationsApi.md#initiate_email_verification) | **POST** /publicapi/v1/email-verification/initiate | Initiate Email Verification.
 *NotificationsApi* | [**send_notification**](docs/NotificationsApi.md#send_notification) | **POST** /publicapi/v1/emails/send | Send an email.
 *PaymentsSetupApi* | [**complete_payment_setup**](docs/PaymentsSetupApi.md#complete_payment_setup) | **POST** /publicapi/v1/payment-setup/complete | Complete a payment setup
 *PaymentsSetupApi* | [**get_public_psp_config**](docs/PaymentsSetupApi.md#get_public_psp_config) | **GET** /publicapi/v1/payment-setup/get-psp-config | Get public key and psp
 *PaymentsSetupApi* | [**initiate_payment_setup**](docs/PaymentsSetupApi.md#initiate_payment_setup) | **POST** /publicapi/v1/payment-setup/initiate | Initiate a payment setup
-*ProductsApi* | [**calculate_product_fields**](docs/ProductsApi.md#calculate_product_fields) | **POST** /publicapi/v1/products/{product_code}/calculate-product-fields | Create the product fields
 *ProductsApi* | [**create_estimated_invoice**](docs/ProductsApi.md#create_estimated_invoice) | **POST** /publicapi/v1/products/{product_code}/product-invoice | Create the invoice product
 *ProductsApi* | [**custom_application**](docs/ProductsApi.md#custom_application) | **POST** /publicapi/v1/products/{product_code}/custom-application | Create the custom application
 *ProductsApi* | [**get_insured_object_types**](docs/ProductsApi.md#get_insured_object_types) | **GET** /publicapi/v1/products/{product_code}/insured-object-types | List insured object types
 *ProductsApi* | [**get_insured_objects**](docs/ProductsApi.md#get_insured_objects) | **GET** /publicapi/v1/products/{product_code}/insured-objects | List insured objects
 *ProductsApi* | [**get_product_custom_css**](docs/ProductsApi.md#get_product_custom_css) | **GET** /publicapi/v1/products/{product_code}/custom-css | Generate a custom CSS
 *ProductsApi* | [**get_product_factors**](docs/ProductsApi.md#get_product_factors) | **GET** /publicapi/v1/products/{product_code}/product-factors | List product factors
 *ProductsApi* | [**list_products**](docs/ProductsApi.md#list_products) | **GET** /publicapi/v1/products | List products
-*DefaultApi* | [**check**](docs/DefaultApi.md#check) | **GET** /publicapi/health | 
 
 
 ## Documentation For Models
 
  - [AddressCompletionItemClass](docs/AddressCompletionItemClass.md)
  - [AddressCompletionResponseClass](docs/AddressCompletionResponseClass.md)
  - [AddressFieldScoreClass](docs/AddressFieldScoreClass.md)
- - [CalculateProductFieldsRequestDto](docs/CalculateProductFieldsRequestDto.md)
- - [CalculateProductFieldsResponseClass](docs/CalculateProductFieldsResponseClass.md)
  - [CompleteBraintreePaymentSetupRequestDto](docs/CompleteBraintreePaymentSetupRequestDto.md)
- - [CompleteEmailVerificationDto](docs/CompleteEmailVerificationDto.md)
- - [CompleteEmailVerificationResponseClass](docs/CompleteEmailVerificationResponseClass.md)
  - [CompletePaymentSetupRequestDto](docs/CompletePaymentSetupRequestDto.md)
  - [CompletePaymentSetupResponseClass](docs/CompletePaymentSetupResponseClass.md)
  - [CompleteStripePaymentSetupRequestDto](docs/CompleteStripePaymentSetupRequestDto.md)
  - [CreateAccountRequestDto](docs/CreateAccountRequestDto.md)
  - [CreateBankAccountRequestDto](docs/CreateBankAccountRequestDto.md)
  - [CreateCustomApplicationRequestDto](docs/CreateCustomApplicationRequestDto.md)
  - [CreateCustomApplicationResponseClass](docs/CreateCustomApplicationResponseClass.md)
  - [CreateDocumentRequestDto](docs/CreateDocumentRequestDto.md)
  - [CreateEstimatedInvoiceRequestDto](docs/CreateEstimatedInvoiceRequestDto.md)
  - [CreateEstimatedInvoiceResponseClass](docs/CreateEstimatedInvoiceResponseClass.md)
- - [CreateLeadAsyncResponseClass](docs/CreateLeadAsyncResponseClass.md)
  - [CreateLeadRequestDto](docs/CreateLeadRequestDto.md)
  - [CreateLeadResponseClass](docs/CreateLeadResponseClass.md)
- - [CreatePaymentMethodRequestDto](docs/CreatePaymentMethodRequestDto.md)
- - [CreatePresignedPostRequestDto](docs/CreatePresignedPostRequestDto.md)
- - [CreatePresignedPostResponseClass](docs/CreatePresignedPostResponseClass.md)
  - [DocumentClass](docs/DocumentClass.md)
  - [GetCustomCssResponseClass](docs/GetCustomCssResponseClass.md)
  - [GetLeadResponseClass](docs/GetLeadResponseClass.md)
- - [GetProductDocumentDownloadUrlResponseClass](docs/GetProductDocumentDownloadUrlResponseClass.md)
  - [GetPublicPspSettingsResponseClass](docs/GetPublicPspSettingsResponseClass.md)
  - [InitiateBraintreePaymentSetupRequestDto](docs/InitiateBraintreePaymentSetupRequestDto.md)
  - [InitiateBraintreePaymentSetupResponseClass](docs/InitiateBraintreePaymentSetupResponseClass.md)
- - [InitiateEmailVerificationDto](docs/InitiateEmailVerificationDto.md)
- - [InitiateEmailVerificationResponseClass](docs/InitiateEmailVerificationResponseClass.md)
  - [InitiateLeadResponseClass](docs/InitiateLeadResponseClass.md)
  - [InitiatePaymentSetupRequestDto](docs/InitiatePaymentSetupRequestDto.md)
  - [InitiatePaymentSetupResponseClass](docs/InitiatePaymentSetupResponseClass.md)
  - [InitiateStripePaymentSetupRequestDto](docs/InitiateStripePaymentSetupRequestDto.md)
  - [InitiateStripePaymentSetupResponseClass](docs/InitiateStripePaymentSetupResponseClass.md)
- - [InlineResponse200](docs/InlineResponse200.md)
- - [InlineResponse503](docs/InlineResponse503.md)
  - [InsuredObjectClass](docs/InsuredObjectClass.md)
  - [InsuredObjectTypeClass](docs/InsuredObjectTypeClass.md)
  - [InvoiceClass](docs/InvoiceClass.md)
  - [InvoiceItemClass](docs/InvoiceItemClass.md)
  - [InvoiceStatusClass](docs/InvoiceStatusClass.md)
  - [LeadAccountClass](docs/LeadAccountClass.md)
  - [LeadBankAccountClass](docs/LeadBankAccountClass.md)
@@ -189,25 +166,23 @@
  - [LeadPolicyClass](docs/LeadPolicyClass.md)
  - [LeadPolicyObjectClass](docs/LeadPolicyObjectClass.md)
  - [ListDocumentsResponseClass](docs/ListDocumentsResponseClass.md)
  - [ListProductDocumentsResponseClass](docs/ListProductDocumentsResponseClass.md)
  - [ListProductsResponseClass](docs/ListProductsResponseClass.md)
  - [PaymentMethodClass](docs/PaymentMethodClass.md)
  - [PolicyObjectRequestDto](docs/PolicyObjectRequestDto.md)
- - [PolicyObjectResponseClass](docs/PolicyObjectResponseClass.md)
  - [PremiumOverrideDto](docs/PremiumOverrideDto.md)
  - [PremiumOverrideRequestDto](docs/PremiumOverrideRequestDto.md)
  - [ProductClass](docs/ProductClass.md)
  - [ProductDocumentClass](docs/ProductDocumentClass.md)
- - [ProductFactorForVersionClass](docs/ProductFactorForVersionClass.md)
+ - [ProductFactorClass](docs/ProductFactorClass.md)
  - [ProductFieldClass](docs/ProductFieldClass.md)
  - [ProductVersionClass](docs/ProductVersionClass.md)
  - [SendNotificationRequestDto](docs/SendNotificationRequestDto.md)
  - [SendNotificationResponseClass](docs/SendNotificationResponseClass.md)
- - [SepaDto](docs/SepaDto.md)
  - [StructuredAddressClass](docs/StructuredAddressClass.md)
  - [SuggestedAddressDetailsClass](docs/SuggestedAddressDetailsClass.md)
  - [UpdateLeadRequestDto](docs/UpdateLeadRequestDto.md)
  - [UpdateLeadResponseClass](docs/UpdateLeadResponseClass.md)
  - [UploadedDocumentDto](docs/UploadedDocumentDto.md)
  - [ValidateAddressResponseClass](docs/ValidateAddressResponseClass.md)
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/__init__.py` & `eis-publicapi-1.6.0/eis/publicapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 1.0
     Contact: kontakt@emil.de
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.22.1"
+__version__ = "1.6.0"
 
 # import ApiClient
 from eis.publicapi.api_client import ApiClient
 
 # import Configuration
 from eis.publicapi.configuration import Configuration
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/api/address_completions_validations_api.py` & `eis-publicapi-1.6.0/eis/publicapi/api/address_completions_validations_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,23 +145,18 @@
                     'house_number',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
-                    'postal_code',
                 ]
             },
             root_map={
                 'validations': {
-                    ('postal_code',): {
-                        'max_length': 10,
-                        'min_length': 4,
-                    },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'city':
                         (str,),
                     'country':
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/api/documents_api.py` & `eis-publicapi-1.6.0/eis/publicapi/api/products_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,222 +18,229 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from eis.publicapi.model.create_document_request_dto import CreateDocumentRequestDto
-from eis.publicapi.model.create_presigned_post_request_dto import CreatePresignedPostRequestDto
-from eis.publicapi.model.create_presigned_post_response_class import CreatePresignedPostResponseClass
-from eis.publicapi.model.get_product_document_download_url_response_class import GetProductDocumentDownloadUrlResponseClass
-from eis.publicapi.model.list_documents_response_class import ListDocumentsResponseClass
-from eis.publicapi.model.list_product_documents_response_class import ListProductDocumentsResponseClass
+from eis.publicapi.model.create_custom_application_request_dto import CreateCustomApplicationRequestDto
+from eis.publicapi.model.create_custom_application_response_class import CreateCustomApplicationResponseClass
+from eis.publicapi.model.create_estimated_invoice_request_dto import CreateEstimatedInvoiceRequestDto
+from eis.publicapi.model.create_estimated_invoice_response_class import CreateEstimatedInvoiceResponseClass
+from eis.publicapi.model.get_custom_css_response_class import GetCustomCssResponseClass
+from eis.publicapi.model.insured_object_class import InsuredObjectClass
+from eis.publicapi.model.insured_object_type_class import InsuredObjectTypeClass
+from eis.publicapi.model.list_products_response_class import ListProductsResponseClass
+from eis.publicapi.model.product_factor_class import ProductFactorClass
 
 
-class DocumentsApi(object):
+class ProductsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.create_temporary_document_endpoint = _Endpoint(
+        self.create_estimated_invoice_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (CreateEstimatedInvoiceResponseClass,),
                 'auth': [
                     'bearer'
                 ],
-                'endpoint_path': '/publicapi/v1/documents',
-                'operation_id': 'create_temporary_document',
+                'endpoint_path': '/publicapi/v1/products/{product_code}/product-invoice',
+                'operation_id': 'create_estimated_invoice',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'create_document_request_dto',
+                    'product_code',
+                    'create_estimated_invoice_request_dto',
                     'authorization',
                 ],
                 'required': [
-                    'create_document_request_dto',
+                    'product_code',
+                    'create_estimated_invoice_request_dto',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'create_document_request_dto':
-                        (CreateDocumentRequestDto,),
+                    'product_code':
+                        (str,),
+                    'create_estimated_invoice_request_dto':
+                        (CreateEstimatedInvoiceRequestDto,),
                     'authorization':
                         (str,),
                 },
                 'attribute_map': {
+                    'product_code': 'product_code',
                     'authorization': 'Authorization',
                 },
                 'location_map': {
-                    'create_document_request_dto': 'body',
+                    'product_code': 'path',
+                    'create_estimated_invoice_request_dto': 'body',
                     'authorization': 'header',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/json'
+                ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.delete_documents_endpoint = _Endpoint(
+        self.custom_application_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (CreateCustomApplicationResponseClass,),
                 'auth': [
                     'bearer'
                 ],
-                'endpoint_path': '/publicapi/v1/documents/{code}/lead/{leadCode}',
-                'operation_id': 'delete_documents',
-                'http_method': 'DELETE',
+                'endpoint_path': '/publicapi/v1/products/{product_code}/custom-application',
+                'operation_id': 'custom_application',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'lead_code',
-                    'code',
+                    'product_code',
+                    'create_custom_application_request_dto',
                     'authorization',
                 ],
                 'required': [
-                    'lead_code',
-                    'code',
+                    'product_code',
+                    'create_custom_application_request_dto',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'lead_code':
-                        (str,),
-                    'code':
+                    'product_code':
                         (str,),
+                    'create_custom_application_request_dto':
+                        (CreateCustomApplicationRequestDto,),
                     'authorization':
                         (str,),
                 },
                 'attribute_map': {
-                    'lead_code': 'leadCode',
-                    'code': 'code',
+                    'product_code': 'product_code',
                     'authorization': 'Authorization',
                 },
                 'location_map': {
-                    'lead_code': 'path',
-                    'code': 'path',
+                    'product_code': 'path',
+                    'create_custom_application_request_dto': 'body',
                     'authorization': 'header',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
-                'content_type': [],
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
-        self.download_document_endpoint = _Endpoint(
+        self.get_insured_object_types_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': ([InsuredObjectTypeClass],),
                 'auth': [
                     'bearer'
                 ],
-                'endpoint_path': '/publicapi/v1/documents/download/{code}',
-                'operation_id': 'download_document',
+                'endpoint_path': '/publicapi/v1/products/{product_code}/insured-object-types',
+                'operation_id': 'get_insured_object_types',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'code',
                     'authorization',
                 ],
-                'required': [
-                    'code',
-                ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'code':
-                        (str,),
                     'authorization':
                         (str,),
                 },
                 'attribute_map': {
-                    'code': 'code',
                     'authorization': 'Authorization',
                 },
                 'location_map': {
-                    'code': 'path',
                     'authorization': 'header',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/json'
+                ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.download_product_document_url_endpoint = _Endpoint(
+        self.get_insured_objects_endpoint = _Endpoint(
             settings={
-                'response_type': (GetProductDocumentDownloadUrlResponseClass,),
+                'response_type': ([InsuredObjectClass],),
                 'auth': [
                     'bearer'
                 ],
-                'endpoint_path': '/publicapi/v1/documents/product/{productCode}/{code}/download-url',
-                'operation_id': 'download_product_document_url',
+                'endpoint_path': '/publicapi/v1/products/{product_code}/insured-objects',
+                'operation_id': 'get_insured_objects',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'product_code',
-                    'code',
                     'authorization',
                 ],
                 'required': [
                     'product_code',
-                    'code',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -242,140 +249,112 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'product_code':
                         (str,),
-                    'code':
-                        (str,),
                     'authorization':
                         (str,),
                 },
                 'attribute_map': {
-                    'product_code': 'productCode',
-                    'code': 'code',
+                    'product_code': 'product_code',
                     'authorization': 'Authorization',
                 },
                 'location_map': {
                     'product_code': 'path',
-                    'code': 'path',
                     'authorization': 'header',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.list_documents_endpoint = _Endpoint(
+        self.get_product_custom_css_endpoint = _Endpoint(
             settings={
-                'response_type': (ListDocumentsResponseClass,),
+                'response_type': (GetCustomCssResponseClass,),
                 'auth': [
                     'bearer'
                 ],
-                'endpoint_path': '/publicapi/v1/documents',
-                'operation_id': 'list_documents',
+                'endpoint_path': '/publicapi/v1/products/{product_code}/custom-css',
+                'operation_id': 'get_product_custom_css',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'filter',
+                    'product_code',
                     'authorization',
-                    'page_size',
-                    'page_token',
-                    'order',
-                    'expand',
                 ],
                 'required': [
-                    'filter',
+                    'product_code',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'filter':
+                    'product_code':
                         (str,),
                     'authorization':
                         (str,),
-                    'page_size':
-                        (float,),
-                    'page_token':
-                        (str,),
-                    'order':
-                        (str,),
-                    'expand':
-                        (str,),
                 },
                 'attribute_map': {
-                    'filter': 'filter',
+                    'product_code': 'product_code',
                     'authorization': 'Authorization',
-                    'page_size': 'pageSize',
-                    'page_token': 'pageToken',
-                    'order': 'order',
-                    'expand': 'expand',
                 },
                 'location_map': {
-                    'filter': 'query',
+                    'product_code': 'path',
                     'authorization': 'header',
-                    'page_size': 'query',
-                    'page_token': 'query',
-                    'order': 'query',
-                    'expand': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.list_product_documents_endpoint = _Endpoint(
+        self.get_product_factors_endpoint = _Endpoint(
             settings={
-                'response_type': (ListProductDocumentsResponseClass,),
+                'response_type': ([ProductFactorClass],),
                 'auth': [
                     'bearer'
                 ],
-                'endpoint_path': '/publicapi/v1/documents/{productCode}',
-                'operation_id': 'list_product_documents',
+                'endpoint_path': '/publicapi/v1/products/{product_code}/product-factors',
+                'operation_id': 'get_product_factors',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'product_code',
+                    'all_values',
                     'authorization',
-                    'page_size',
-                    'page_token',
-                    'filter',
-                    'search',
-                    'order',
-                    'expand',
                 ],
                 'required': [
                     'product_code',
+                    'all_values',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -384,134 +363,138 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'product_code':
                         (str,),
+                    'all_values':
+                        (str,),
                     'authorization':
                         (str,),
-                    'page_size':
-                        (bool, date, datetime, dict, float, int, list, str, none_type,),
-                    'page_token':
-                        (bool, date, datetime, dict, float, int, list, str, none_type,),
-                    'filter':
-                        (bool, date, datetime, dict, float, int, list, str, none_type,),
-                    'search':
-                        (bool, date, datetime, dict, float, int, list, str, none_type,),
-                    'order':
-                        (bool, date, datetime, dict, float, int, list, str, none_type,),
-                    'expand':
-                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
-                    'product_code': 'productCode',
+                    'product_code': 'product_code',
+                    'all_values': 'all_values',
                     'authorization': 'Authorization',
-                    'page_size': 'pageSize',
-                    'page_token': 'pageToken',
-                    'filter': 'filter',
-                    'search': 'search',
-                    'order': 'order',
-                    'expand': 'expand',
                 },
                 'location_map': {
                     'product_code': 'path',
+                    'all_values': 'query',
                     'authorization': 'header',
-                    'page_size': 'query',
-                    'page_token': 'query',
-                    'filter': 'query',
-                    'search': 'query',
-                    'order': 'query',
-                    'expand': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.pre_signed_post_endpoint = _Endpoint(
+        self.list_products_endpoint = _Endpoint(
             settings={
-                'response_type': (CreatePresignedPostResponseClass,),
+                'response_type': (ListProductsResponseClass,),
                 'auth': [
                     'bearer'
                 ],
-                'endpoint_path': '/publicapi/v1/documents/pre-signed-post',
-                'operation_id': 'pre_signed_post',
-                'http_method': 'POST',
+                'endpoint_path': '/publicapi/v1/products',
+                'operation_id': 'list_products',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'create_presigned_post_request_dto',
                     'authorization',
+                    'page_size',
+                    'page_token',
+                    'filter',
+                    'search',
+                    'order',
+                    'expand',
                 ],
-                'required': [
-                    'create_presigned_post_request_dto',
-                ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'create_presigned_post_request_dto':
-                        (CreatePresignedPostRequestDto,),
                     'authorization':
                         (str,),
+                    'page_size':
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
+                    'page_token':
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
+                    'filter':
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
+                    'search':
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
+                    'order':
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
+                    'expand':
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'authorization': 'Authorization',
+                    'page_size': 'pageSize',
+                    'page_token': 'pageToken',
+                    'filter': 'filter',
+                    'search': 'search',
+                    'order': 'order',
+                    'expand': 'expand',
                 },
                 'location_map': {
-                    'create_presigned_post_request_dto': 'body',
                     'authorization': 'header',
+                    'page_size': 'query',
+                    'page_token': 'query',
+                    'filter': 'query',
+                    'search': 'query',
+                    'order': 'query',
+                    'expand': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
 
-    def create_temporary_document(
+    def create_estimated_invoice(
         self,
-        create_document_request_dto,
+        product_code,
+        create_estimated_invoice_request_dto,
         **kwargs
     ):
-        """Create the temporary document  # noqa: E501
+        """Create the invoice product  # noqa: E501
 
-        This will create a temporary document.  # noqa: E501
+        This will create an invoice product.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_temporary_document(create_document_request_dto, async_req=True)
+        >>> thread = api.create_estimated_invoice(product_code, create_estimated_invoice_request_dto, async_req=True)
         >>> result = thread.get()
 
         Args:
-            create_document_request_dto (CreateDocumentRequestDto):
+            product_code (str):
+            create_estimated_invoice_request_dto (CreateEstimatedInvoiceRequestDto):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -539,15 +522,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            CreateEstimatedInvoiceResponseClass
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -568,36 +551,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['create_document_request_dto'] = \
-            create_document_request_dto
-        return self.create_temporary_document_endpoint.call_with_http_info(**kwargs)
+        kwargs['product_code'] = \
+            product_code
+        kwargs['create_estimated_invoice_request_dto'] = \
+            create_estimated_invoice_request_dto
+        return self.create_estimated_invoice_endpoint.call_with_http_info(**kwargs)
 
-    def delete_documents(
+    def custom_application(
         self,
-        lead_code,
-        code,
+        product_code,
+        create_custom_application_request_dto,
         **kwargs
     ):
-        """Delete a document  # noqa: E501
+        """Create the custom application  # noqa: E501
 
-        This will delete a document for a lead by lead code and document code.Documents which were created within last 24 hours can be deleted.  # noqa: E501
+        This will create a custom application for a specific provider.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_documents(lead_code, code, async_req=True)
+        >>> thread = api.custom_application(product_code, create_custom_application_request_dto, async_req=True)
         >>> result = thread.get()
 
         Args:
-            lead_code (str):
-            code (str):
+            product_code (str):
+            create_custom_application_request_dto (CreateCustomApplicationRequestDto):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -625,15 +610,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            CreateCustomApplicationResponseClass
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -654,36 +639,33 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['lead_code'] = \
-            lead_code
-        kwargs['code'] = \
-            code
-        return self.delete_documents_endpoint.call_with_http_info(**kwargs)
+        kwargs['product_code'] = \
+            product_code
+        kwargs['create_custom_application_request_dto'] = \
+            create_custom_application_request_dto
+        return self.custom_application_endpoint.call_with_http_info(**kwargs)
 
-    def download_document(
+    def get_insured_object_types(
         self,
-        code,
         **kwargs
     ):
-        """Download a document  # noqa: E501
+        """List insured object types  # noqa: E501
 
-        Retrieves the details of the specific document that was previously created. Supply the unique document code that was returned when you created it and Emil Api will return the corresponding document file to download.  # noqa: E501
+        Returns a list of insured object types you have previously created. The insured object types are returned in sorted order, with the oldest one appearing first. For more information about pagination, read the Pagination documentation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.download_document(code, async_req=True)
+        >>> thread = api.get_insured_object_types(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            code (str):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -711,15 +693,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            [InsuredObjectTypeClass]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -740,35 +722,32 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['code'] = \
-            code
-        return self.download_document_endpoint.call_with_http_info(**kwargs)
+        return self.get_insured_object_types_endpoint.call_with_http_info(**kwargs)
 
-    def download_product_document_url(
+    def get_insured_objects(
         self,
         product_code,
-        code,
         **kwargs
     ):
-        """Get pre-signed url for downloading product document  # noqa: E501
+        """List insured objects  # noqa: E501
 
+        Returns a list of insured objects you have previously created. The insured objects are returned in sorted order, with the oldest one appearing first. For more information about pagination, read the Pagination documentation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.download_product_document_url(product_code, code, async_req=True)
+        >>> thread = api.get_insured_objects(product_code, async_req=True)
         >>> result = thread.get()
 
         Args:
             product_code (str):
-            code (str):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -796,15 +775,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetProductDocumentDownloadUrlResponseClass
+            [InsuredObjectClass]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -827,41 +806,35 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['product_code'] = \
             product_code
-        kwargs['code'] = \
-            code
-        return self.download_product_document_url_endpoint.call_with_http_info(**kwargs)
+        return self.get_insured_objects_endpoint.call_with_http_info(**kwargs)
 
-    def list_documents(
+    def get_product_custom_css(
         self,
-        filter,
+        product_code,
         **kwargs
     ):
-        """List documents  # noqa: E501
+        """Generate a custom CSS  # noqa: E501
 
-        Returns a list of documents you have previously created. The documents are returned in sorted order, with the oldest one appearing first. For more information about pagination, read the Pagination documentation.  # noqa: E501
+        This will generate a custom css for booking funnel, based on product.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_documents(filter, async_req=True)
+        >>> thread = api.get_product_custom_css(product_code, async_req=True)
         >>> result = thread.get()
 
         Args:
-            filter (str): Filter the response by one or multiple fields.     In general, fetching filtered responses will conserve bandwidth and reduce response time.
+            product_code (str):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
-            page_size (float): A limit on the number of objects to be returned.     Limit ranges between 1 and 100. Default: 10.. [optional]
-            page_token (str): A cursor for use in pagination.     pageToken is an ID that defines your place in the list.     For instance, if you make a list request and receive 100 objects and pageToken=1,     your subsequent call can include pageToken=2 in order to fetch the next page of the list.. [optional]
-            order (str): The order parameter determines how the results should be sorted according to a specified field.     It functions similarly to an SQL ORDER BY.     Sorting can be performed in either ascending (ASC) or descending (DESC) order.     Default: ASC.. [optional]
-            expand (str): Use this parameter to fetch additional information about the list items.     The expand query parameter increases the set of fields that appear in the response in     addition to the default ones.     Expanding resources can reduce the number of API calls required to accomplish a task.     However, use this with parsimony as some expanded fields can drastically increase payload size.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -886,15 +859,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            ListDocumentsResponseClass
+            GetCustomCssResponseClass
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -915,43 +888,39 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['filter'] = \
-            filter
-        return self.list_documents_endpoint.call_with_http_info(**kwargs)
+        kwargs['product_code'] = \
+            product_code
+        return self.get_product_custom_css_endpoint.call_with_http_info(**kwargs)
 
-    def list_product_documents(
+    def get_product_factors(
         self,
         product_code,
+        all_values,
         **kwargs
     ):
-        """List product documents  # noqa: E501
+        """List product factors  # noqa: E501
 
-        Returns a list of product documents you have previously created. The product documents are returned in sorted order, with the oldest one appearing first. For more information about pagination, read the Pagination documentation.  # noqa: E501
+        Returns a list of product factors you have previously created. The product factors are returned in sorted order, with the oldest one appearing first. For more information about pagination, read the Pagination documentation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_product_documents(product_code, async_req=True)
+        >>> thread = api.get_product_factors(product_code, all_values, async_req=True)
         >>> result = thread.get()
 
         Args:
             product_code (str):
+            all_values (str):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
-            page_size (bool, date, datetime, dict, float, int, list, str, none_type): A limit on the number of objects to be returned.     Limit ranges between 1 and 100. Default: 10.. [optional]
-            page_token (bool, date, datetime, dict, float, int, list, str, none_type): A cursor for use in pagination.     pageToken is an ID that defines your place in the list.     For instance, if you make a list request and receive 100 objects and pageToken=1,     your subsequent call can include pageToken=2 in order to fetch the next page of the list.. [optional]
-            filter (bool, date, datetime, dict, float, int, list, str, none_type): Filter the response by one or multiple fields.     In general, fetching filtered responses will conserve bandwidth and reduce response time.. [optional]
-            search (bool, date, datetime, dict, float, int, list, str, none_type): Search the list by any field. For instance, if you want to search by code     add code=xxx in order to fetch the result.. [optional]
-            order (bool, date, datetime, dict, float, int, list, str, none_type): The order parameter determines how the results should be sorted according to a specified field.     It functions similarly to an SQL ORDER BY.     Sorting can be performed in either ascending (ASC) or descending (DESC) order.     Default: ASC.. [optional]
-            expand (bool, date, datetime, dict, float, int, list, str, none_type): Use this parameter to fetch additional information about the list items.     The expand query parameter increases the set of fields that appear in the response in     addition to the default ones.     Expanding resources can reduce the number of API calls required to accomplish a task.     However, use this with parsimony as some expanded fields can drastically increase payload size.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -976,15 +945,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            ListProductDocumentsResponseClass
+            [ProductFactorClass]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1007,35 +976,40 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['product_code'] = \
             product_code
-        return self.list_product_documents_endpoint.call_with_http_info(**kwargs)
+        kwargs['all_values'] = \
+            all_values
+        return self.get_product_factors_endpoint.call_with_http_info(**kwargs)
 
-    def pre_signed_post(
+    def list_products(
         self,
-        create_presigned_post_request_dto,
         **kwargs
     ):
-        """Upload documents using pre-signed URL  # noqa: E501
+        """List products  # noqa: E501
 
-        This will create a URL that allows user upload its documents in Database.The URL can expire between 5 minutes and 7 days.  # noqa: E501
+        Returns a list of products you have previously created. The products are returned in sorted order, with the oldest one appearing first. For more information about pagination, read the Pagination documentation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.pre_signed_post(create_presigned_post_request_dto, async_req=True)
+        >>> thread = api.list_products(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            create_presigned_post_request_dto (CreatePresignedPostRequestDto):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
+            page_size (bool, date, datetime, dict, float, int, list, str, none_type): A limit on the number of objects to be returned.     Limit ranges between 1 and 100. Default: 10.. [optional]
+            page_token (bool, date, datetime, dict, float, int, list, str, none_type): A cursor for use in pagination.     pageToken is an ID that defines your place in the list.     For instance, if you make a list request and receive 100 objects and pageToken=1,     your subsequent call can include pageToken=2 in order to fetch the next page of the list.. [optional]
+            filter (bool, date, datetime, dict, float, int, list, str, none_type): Filter the response by one or multiple fields.     In general, fetching filtered responses will conserve bandwidth and reduce response time.. [optional]
+            search (bool, date, datetime, dict, float, int, list, str, none_type): Search the list by any field. For instance, if you want to search by code     add code=xxx in order to fetch the result.. [optional]
+            order (bool, date, datetime, dict, float, int, list, str, none_type): The order parameter determines how the results should be sorted according to a specified field.     It functions similarly to an SQL ORDER BY.     Sorting can be performed in either ascending (ASC) or descending (DESC) order.     Default: ASC.. [optional]
+            expand (bool, date, datetime, dict, float, int, list, str, none_type): You can expand product versions and insured object types list in this endpoint.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1060,15 +1034,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            CreatePresignedPostResponseClass
+            ListProductsResponseClass
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1089,11 +1063,9 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['create_presigned_post_request_dto'] = \
-            create_presigned_post_request_dto
-        return self.pre_signed_post_endpoint.call_with_http_info(**kwargs)
+        return self.list_products_endpoint.call_with_http_info(**kwargs)
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/api/leads_api.py` & `eis-publicapi-1.6.0/eis/publicapi/api/leads_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from eis.publicapi.model.create_lead_async_response_class import CreateLeadAsyncResponseClass
 from eis.publicapi.model.create_lead_request_dto import CreateLeadRequestDto
 from eis.publicapi.model.create_lead_response_class import CreateLeadResponseClass
 from eis.publicapi.model.get_lead_response_class import GetLeadResponseClass
 from eis.publicapi.model.initiate_lead_response_class import InitiateLeadResponseClass
 from eis.publicapi.model.update_lead_request_dto import UpdateLeadRequestDto
 from eis.publicapi.model.update_lead_response_class import UpdateLeadResponseClass
 
@@ -95,128 +94,14 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.create_lead_async_endpoint = _Endpoint(
-            settings={
-                'response_type': (CreateLeadAsyncResponseClass,),
-                'auth': [
-                    'bearer'
-                ],
-                'endpoint_path': '/publicapi/v1/leads-async',
-                'operation_id': 'create_lead_async',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'create_lead_request_dto',
-                    'authorization',
-                ],
-                'required': [
-                    'create_lead_request_dto',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'create_lead_request_dto':
-                        (CreateLeadRequestDto,),
-                    'authorization':
-                        (str,),
-                },
-                'attribute_map': {
-                    'authorization': 'Authorization',
-                },
-                'location_map': {
-                    'create_lead_request_dto': 'body',
-                    'authorization': 'header',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-        self.create_lead_sync_endpoint = _Endpoint(
-            settings={
-                'response_type': (CreateLeadResponseClass,),
-                'auth': [
-                    'bearer'
-                ],
-                'endpoint_path': '/publicapi/v1/leads-sync',
-                'operation_id': 'create_lead_sync',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'create_lead_request_dto',
-                    'authorization',
-                ],
-                'required': [
-                    'create_lead_request_dto',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'create_lead_request_dto':
-                        (CreateLeadRequestDto,),
-                    'authorization':
-                        (str,),
-                },
-                'attribute_map': {
-                    'authorization': 'Authorization',
-                },
-                'location_map': {
-                    'create_lead_request_dto': 'body',
-                    'authorization': 'header',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
         self.get_lead_endpoint = _Endpoint(
             settings={
                 'response_type': (GetLeadResponseClass,),
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/publicapi/v1/leads/{code}',
@@ -377,77 +262,14 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.update_lead_sync_endpoint = _Endpoint(
-            settings={
-                'response_type': (UpdateLeadResponseClass,),
-                'auth': [
-                    'bearer'
-                ],
-                'endpoint_path': '/publicapi/v1/leads-sync/{code}',
-                'operation_id': 'update_lead_sync',
-                'http_method': 'PUT',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'code',
-                    'update_lead_request_dto',
-                    'authorization',
-                ],
-                'required': [
-                    'code',
-                    'update_lead_request_dto',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'code':
-                        (str,),
-                    'update_lead_request_dto':
-                        (UpdateLeadRequestDto,),
-                    'authorization':
-                        (str,),
-                },
-                'attribute_map': {
-                    'code': 'code',
-                    'authorization': 'Authorization',
-                },
-                'location_map': {
-                    'code': 'path',
-                    'update_lead_request_dto': 'body',
-                    'authorization': 'header',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
 
     def create_lead(
         self,
         create_lead_request_dto,
         **kwargs
     ):
         """Create the lead  # noqa: E501
@@ -525,182 +347,14 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['create_lead_request_dto'] = \
             create_lead_request_dto
         return self.create_lead_endpoint.call_with_http_info(**kwargs)
 
-    def create_lead_async(
-        self,
-        create_lead_request_dto,
-        **kwargs
-    ):
-        """Create the lead asynchronously  # noqa: E501
-
-        This will send the lead to the queue for creation. Should be used when creating multiple leads     at the same time - also called 'batch processing'.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_lead_async(create_lead_request_dto, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            create_lead_request_dto (CreateLeadRequestDto):
-
-        Keyword Args:
-            authorization (str): Bearer Token. [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            CreateLeadAsyncResponseClass
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['create_lead_request_dto'] = \
-            create_lead_request_dto
-        return self.create_lead_async_endpoint.call_with_http_info(**kwargs)
-
-    def create_lead_sync(
-        self,
-        create_lead_request_dto,
-        **kwargs
-    ):
-        """Create the lead synchronously  # noqa: E501
-
-        This endpoint initiates the creation of a lead, which is the initial step in a comprehensive      workflow responsible for the creation of an account, policy, and banking information.      Unlike the standard lead creation endpoint, this variant ensures that the process waits until the entire workflow      is successfully completed before providing a response.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_lead_sync(create_lead_request_dto, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            create_lead_request_dto (CreateLeadRequestDto):
-
-        Keyword Args:
-            authorization (str): Bearer Token. [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            CreateLeadResponseClass
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['create_lead_request_dto'] = \
-            create_lead_request_dto
-        return self.create_lead_sync_endpoint.call_with_http_info(**kwargs)
-
     def get_lead(
         self,
         code,
         **kwargs
     ):
         """Retrieve the lead  # noqa: E501
 
@@ -944,95 +598,7 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
         kwargs['update_lead_request_dto'] = \
             update_lead_request_dto
         return self.update_lead_endpoint.call_with_http_info(**kwargs)
 
-    def update_lead_sync(
-        self,
-        code,
-        update_lead_request_dto,
-        **kwargs
-    ):
-        """Update the lead  # noqa: E501
-
-        Updates the specified lead by setting the values of the parameters passed. Any parameters not provided will be left unchanged.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.update_lead_sync(code, update_lead_request_dto, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            code (str): Unique identifier for the object.
-            update_lead_request_dto (UpdateLeadRequestDto):
-
-        Keyword Args:
-            authorization (str): Bearer Token. [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            UpdateLeadResponseClass
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['code'] = \
-            code
-        kwargs['update_lead_request_dto'] = \
-            update_lead_request_dto
-        return self.update_lead_sync_endpoint.call_with_http_info(**kwargs)
-
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/api/payments_setup_api.py` & `eis-publicapi-1.6.0/eis/publicapi/api/payments_setup_api.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/api_client.py` & `eis-publicapi-1.6.0/eis/publicapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.22.1/python'
+        self.user_agent = 'OpenAPI-Generator/1.6.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/apis/__init__.py` & `eis-publicapi-1.6.0/eis/publicapi/apis/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,8 +16,7 @@
 # Import APIs into API package:
 from eis.publicapi.api.address_completions_validations_api import AddressCompletionsValidationsApi
 from eis.publicapi.api.documents_api import DocumentsApi
 from eis.publicapi.api.leads_api import LeadsApi
 from eis.publicapi.api.notifications_api import NotificationsApi
 from eis.publicapi.api.payments_setup_api import PaymentsSetupApi
 from eis.publicapi.api.products_api import ProductsApi
-from eis.publicapi.api.default_api import DefaultApi
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/configuration.py` & `eis-publicapi-1.6.0/eis/publicapi/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.22.1".\
+               "SDK Package Version: 1.6.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/exceptions.py` & `eis-publicapi-1.6.0/eis/publicapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/address_completion_item_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/address_completion_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/address_completion_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/address_completion_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/address_field_score_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/address_field_score_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/calculate_product_fields_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/lead_policy_object_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.publicapi.model.policy_object_request_dto import PolicyObjectRequestDto
-    globals()['PolicyObjectRequestDto'] = PolicyObjectRequestDto
 
-
-class CalculateProductFieldsRequestDto(ModelNormal):
+class LeadPolicyObjectClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,54 +63,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'product_version_id': (float,),  # noqa: E501
-            'policy_objects': ([PolicyObjectRequestDto],),  # noqa: E501
+            'insured_object_id': (float,),  # noqa: E501
+            'data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'product_version_id': 'productVersionId',  # noqa: E501
-        'policy_objects': 'policyObjects',  # noqa: E501
+        'insured_object_id': 'insuredObjectId',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CalculateProductFieldsRequestDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, insured_object_id, data, *args, **kwargs):  # noqa: E501
+        """LeadPolicyObjectClass - a model defined in OpenAPI
+
+        Args:
+            insured_object_id (float): Unique identifier referencing the insured object.
+            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object data.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,16 +137,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            product_version_id (float): Unique identifier referencing the product version.. [optional]  # noqa: E501
-            policy_objects ([PolicyObjectRequestDto]): The policy objects to calculate product fields by.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -172,14 +168,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.insured_object_id = insured_object_id
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,16 +190,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """CalculateProductFieldsRequestDto - a model defined in OpenAPI
+    def __init__(self, insured_object_id, data, *args, **kwargs):  # noqa: E501
+        """LeadPolicyObjectClass - a model defined in OpenAPI
+
+        Args:
+            insured_object_id (float): Unique identifier referencing the insured object.
+            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object data.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,16 +228,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            product_version_id (float): Unique identifier referencing the product version.. [optional]  # noqa: E501
-            policy_objects ([PolicyObjectRequestDto]): The policy objects to calculate product fields by.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -257,14 +257,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.insured_object_id = insured_object_id
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/calculate_product_fields_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/initiate_lead_response_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.publicapi.model.policy_object_response_class import PolicyObjectResponseClass
-    globals()['PolicyObjectResponseClass'] = PolicyObjectResponseClass
 
-
-class CalculateProductFieldsResponseClass(ModelNormal):
+class InitiateLeadResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,55 +63,53 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'policy_objects': ([PolicyObjectResponseClass],),  # noqa: E501
+            'lead_code': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'policy_objects': 'policyObjects',  # noqa: E501
+        'lead_code': 'leadCode',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, policy_objects, *args, **kwargs):  # noqa: E501
-        """CalculateProductFieldsResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, lead_code, *args, **kwargs):  # noqa: E501
+        """InitiateLeadResponseClass - a model defined in OpenAPI
 
         Args:
-            policy_objects ([PolicyObjectResponseClass]): Policy objects with calculated fields.
+            lead_code (str): Unique identifier of the lead that this object belongs to.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.policy_objects = policy_objects
+        self.lead_code = lead_code
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, policy_objects, *args, **kwargs):  # noqa: E501
-        """CalculateProductFieldsResponseClass - a model defined in OpenAPI
+    def __init__(self, lead_code, *args, **kwargs):  # noqa: E501
+        """InitiateLeadResponseClass - a model defined in OpenAPI
 
         Args:
-            policy_objects ([PolicyObjectResponseClass]): Policy objects with calculated fields.
+            lead_code (str): Unique identifier of the lead that this object belongs to.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,15 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.policy_objects = policy_objects
+        self.lead_code = lead_code
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/complete_braintree_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/complete_braintree_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/complete_email_verification_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/get_custom_css_response_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class CompleteEmailVerificationDto(ModelNormal):
+class GetCustomCssResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'email': (str,),  # noqa: E501
-            'token': (str,),  # noqa: E501
+            'values': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email': 'email',  # noqa: E501
-        'token': 'token',  # noqa: E501
+        'values': 'values',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, email, token, *args, **kwargs):  # noqa: E501
-        """CompleteEmailVerificationDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, values, *args, **kwargs):  # noqa: E501
+        """GetCustomCssResponseClass - a model defined in OpenAPI
 
         Args:
-            email (str): User email
-            token (str): The confirmation token comes from an email sent to the customer.
+            values ([str]): Custom CSS setting for booking funnel.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,16 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
-        self.token = token
+        self.values = values
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, email, token, *args, **kwargs):  # noqa: E501
-        """CompleteEmailVerificationDto - a model defined in OpenAPI
+    def __init__(self, values, *args, **kwargs):  # noqa: E501
+        """GetCustomCssResponseClass - a model defined in OpenAPI
 
         Args:
-            email (str): User email
-            token (str): The confirmation token comes from an email sent to the customer.
+            values ([str]): Custom CSS setting for booking funnel.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,16 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
-        self.token = token
+        self.values = values
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/complete_email_verification_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/get_public_psp_settings_response_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class CompleteEmailVerificationResponseClass(ModelNormal):
+class GetPublicPspSettingsResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'result': (bool,),  # noqa: E501
+            'public_key': (str,),  # noqa: E501
+            'psp': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'result': 'result',  # noqa: E501
+        'public_key': 'publicKey',  # noqa: E501
+        'psp': 'psp',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, result, *args, **kwargs):  # noqa: E501
-        """CompleteEmailVerificationResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, public_key, psp, *args, **kwargs):  # noqa: E501
+        """GetPublicPspSettingsResponseClass - a model defined in OpenAPI
 
         Args:
-            result (bool): Complete verification result
+            public_key (str): Public key. Used on frontend to load the payment form component.
+            psp (str): Name of payment system provider.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +168,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.result = result
+        self.public_key = public_key
+        self.psp = psp
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +190,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, result, *args, **kwargs):  # noqa: E501
-        """CompleteEmailVerificationResponseClass - a model defined in OpenAPI
+    def __init__(self, public_key, psp, *args, **kwargs):  # noqa: E501
+        """GetPublicPspSettingsResponseClass - a model defined in OpenAPI
 
         Args:
-            result (bool): Complete verification result
+            public_key (str): Public key. Used on frontend to load the payment form component.
+            psp (str): Name of payment system provider.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +257,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.result = result
+        self.public_key = public_key
+        self.psp = psp
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/complete_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/complete_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/complete_payment_setup_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/complete_payment_setup_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/complete_stripe_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/complete_stripe_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_account_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/create_account_request_dto.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,25 +52,25 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('gender',): {
+            'MALE': "male",
+            'FEMALE': "female",
+            'UNSPECIFIED': "unspecified",
+        },
         ('title',): {
             'EMPTY': "",
             'DR.': "Dr.",
             'DR._MED.': "Dr. med.",
             'PROF._DR._MED.': "Prof. Dr. med.",
         },
-        ('gender',): {
-            'MALE': "male",
-            'FEMALE': "female",
-            'UNSPECIFIED': "unspecified",
-        },
         ('type',): {
             'PERSON': "person",
             'ORG': "org",
         },
     }
 
     validations = {
@@ -93,66 +93,77 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'title': (str,),  # noqa: E501
             'first_name': (str,),  # noqa: E501
             'last_name': (str,),  # noqa: E501
             'email': (str,),  # noqa: E501
             'gender': (str,),  # noqa: E501
             'street': (str,),  # noqa: E501
             'zip_code': (str,),  # noqa: E501
             'city': (str,),  # noqa: E501
             'house_number': (str,),  # noqa: E501
-            'birth_date': (datetime,),  # noqa: E501
             'phone': (str,),  # noqa: E501
+            'title': (str,),  # noqa: E501
+            'birth_date': (datetime,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'company_name': (str,),  # noqa: E501
             'account_number': (str,),  # noqa: E501
             'custom_fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'title': 'title',  # noqa: E501
         'first_name': 'firstName',  # noqa: E501
         'last_name': 'lastName',  # noqa: E501
         'email': 'email',  # noqa: E501
         'gender': 'gender',  # noqa: E501
         'street': 'street',  # noqa: E501
         'zip_code': 'zipCode',  # noqa: E501
         'city': 'city',  # noqa: E501
         'house_number': 'houseNumber',  # noqa: E501
-        'birth_date': 'birthDate',  # noqa: E501
         'phone': 'phone',  # noqa: E501
+        'title': 'title',  # noqa: E501
+        'birth_date': 'birthDate',  # noqa: E501
         'type': 'type',  # noqa: E501
         'company_name': 'companyName',  # noqa: E501
         'account_number': 'accountNumber',  # noqa: E501
         'custom_fields': 'customFields',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, first_name, last_name, email, gender, street, zip_code, city, house_number, phone, *args, **kwargs):  # noqa: E501
         """CreateAccountRequestDto - a model defined in OpenAPI
 
+        Args:
+            first_name (str): Customer first name
+            last_name (str): Customer last name
+            email (str): Customer email
+            gender (str): Customer gender
+            street (str): Customer street
+            zip_code (str): Customer zip code
+            city (str): Customer city
+            house_number (str): Customer house number
+            phone (str): Customer phone number
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -176,29 +187,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            title (str): Optional field to enter the honorific title you want to be called.. [optional]  # noqa: E501
-            first_name (str): The account's holder first name.     The account's first name will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            last_name (str): The account's holder first name.     The account's first name will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            email (str): The account's holder email address. It is displayed alongside the account in your dashboard       and can be useful for searching and tracking.       The account's email address will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            gender (str): The account's holder gender.     The account's gender will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            street (str): The account's holder street name.     The account's street name will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            zip_code (str): The account's holder ZIP or postal code.     The account's ZIP or postal code will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            city (str): The account's holder city, district, suburb, town, or village.     The account's city will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            house_number (str): The account's holder house number.     The account's house number will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            birth_date (datetime): The account's holder date of birth (Required for account of type person).     The account's date of birth will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            phone (str): The account's holder phone number.     The account's phone number will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            type (str): The account's type. Default value is person. [optional] if omitted the server will use the default value of "person"  # noqa: E501
-            company_name (str): The account's company name (Required for account of type org).     The account's company name will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            account_number (str): Account number.. [optional]  # noqa: E501
-            custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Optional custom fields for account. It could be included additional required/optional fields       that the account would need for specific cases.. [optional]  # noqa: E501
+            title (str): Customer honorific title. [optional]  # noqa: E501
+            birth_date (datetime): Customer birth date (Required for account of type person).. [optional]  # noqa: E501
+            type (str): Optional field to enter the type of the account.. [optional] if omitted the server will use the default value of "person"  # noqa: E501
+            company_name (str): Customer company name (Required for account of type org).. [optional]  # noqa: E501
+            account_number (str): Account number. [optional]  # noqa: E501
+            custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Custom fields could be included additional required/optional fields that the account would need for specific cases.. [optional]  # noqa: E501
             metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the account would need for specific cases.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -223,14 +225,23 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.first_name = first_name
+        self.last_name = last_name
+        self.email = email
+        self.gender = gender
+        self.street = street
+        self.zip_code = zip_code
+        self.city = city
+        self.house_number = house_number
+        self.phone = phone
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -243,17 +254,28 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, first_name, last_name, email, gender, street, zip_code, city, house_number, phone, *args, **kwargs):  # noqa: E501
         """CreateAccountRequestDto - a model defined in OpenAPI
 
+        Args:
+            first_name (str): Customer first name
+            last_name (str): Customer last name
+            email (str): Customer email
+            gender (str): Customer gender
+            street (str): Customer street
+            zip_code (str): Customer zip code
+            city (str): Customer city
+            house_number (str): Customer house number
+            phone (str): Customer phone number
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -277,29 +299,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            title (str): Optional field to enter the honorific title you want to be called.. [optional]  # noqa: E501
-            first_name (str): The account's holder first name.     The account's first name will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            last_name (str): The account's holder first name.     The account's first name will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            email (str): The account's holder email address. It is displayed alongside the account in your dashboard       and can be useful for searching and tracking.       The account's email address will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            gender (str): The account's holder gender.     The account's gender will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            street (str): The account's holder street name.     The account's street name will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            zip_code (str): The account's holder ZIP or postal code.     The account's ZIP or postal code will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            city (str): The account's holder city, district, suburb, town, or village.     The account's city will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            house_number (str): The account's holder house number.     The account's house number will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            birth_date (datetime): The account's holder date of birth (Required for account of type person).     The account's date of birth will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            phone (str): The account's holder phone number.     The account's phone number will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            type (str): The account's type. Default value is person. [optional] if omitted the server will use the default value of "person"  # noqa: E501
-            company_name (str): The account's company name (Required for account of type org).     The account's company name will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            account_number (str): Account number.. [optional]  # noqa: E501
-            custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Optional custom fields for account. It could be included additional required/optional fields       that the account would need for specific cases.. [optional]  # noqa: E501
+            title (str): Customer honorific title. [optional]  # noqa: E501
+            birth_date (datetime): Customer birth date (Required for account of type person).. [optional]  # noqa: E501
+            type (str): Optional field to enter the type of the account.. [optional] if omitted the server will use the default value of "person"  # noqa: E501
+            company_name (str): Customer company name (Required for account of type org).. [optional]  # noqa: E501
+            account_number (str): Account number. [optional]  # noqa: E501
+            custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Custom fields could be included additional required/optional fields that the account would need for specific cases.. [optional]  # noqa: E501
             metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the account would need for specific cases.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -322,14 +335,23 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.first_name = first_name
+        self.last_name = last_name
+        self.email = email
+        self.gender = gender
+        self.street = street
+        self.zip_code = zip_code
+        self.city = city
+        self.house_number = house_number
+        self.phone = phone
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_bank_account_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/create_bank_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_custom_application_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/create_custom_application_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_custom_application_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/create_custom_application_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_document_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/document_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class CreateDocumentRequestDto(ModelNormal):
+class DocumentClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,40 +52,38 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('entity_type',): {
+            'POLICY_APPLICATION': "policy_application",
+            'POLICY_CONTRACT': "policy_contract",
+            'POLICY_ADDENDUM': "policy_addendum",
+            'INITIAL_INVOICE': "initial_invoice",
+            'CORRECTION_INVOICE': "correction_invoice",
+            'RECURRING_INVOICE': "recurring_invoice",
+            'SEPA_MANDATE': "sepa_mandate",
+            'STATIC': "static",
+        },
         ('requester',): {
             'PUBLICAPI': "publicapi",
         },
         ('content_type',): {
             'PDF': "pdf",
             'JPG': "jpg",
             'PNG': "png",
             'GZ': "gz",
             'CSV': "csv",
             'DOC': "doc",
             'DOCX': "docx",
             'HTML': "html",
             'JSON': "json",
             'XML': "xml",
-            'TXT': "txt",
-            'ZIP': "zip",
-            'TAR': "tar",
-            'RAR': "rar",
-            'MP4': "MP4",
-            'MOV': "MOV",
-            'WMV': "WMV",
-            'AVI': "AVI",
-        },
-        ('engine',): {
-            'DOCX': "docx",
-            'HTML': "html",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -105,71 +103,76 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'id': (float,),  # noqa: E501
+            'code': (str,),  # noqa: E501
             'template_slug': (str,),  # noqa: E501
-            'payload': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'entity_type': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
             'requester': (str,),  # noqa: E501
+            'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            's3_key': (str,),  # noqa: E501
             'content_type': (str,),  # noqa: E501
-            'product_slug': (str,),  # noqa: E501
+            'filename': (str,),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
             'policy_code': (str,),  # noqa: E501
             'account_code': (str,),  # noqa: E501
             'entity_id': (float,),  # noqa: E501
-            'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'filename': (str,),  # noqa: E501
-            'should_skip_default_margins': (bool,),  # noqa: E501
-            'engine': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'id': 'id',  # noqa: E501
+        'code': 'code',  # noqa: E501
         'template_slug': 'templateSlug',  # noqa: E501
-        'payload': 'payload',  # noqa: E501
         'entity_type': 'entityType',  # noqa: E501
-        'description': 'description',  # noqa: E501
         'requester': 'requester',  # noqa: E501
+        'metadata': 'metadata',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        's3_key': 's3Key',  # noqa: E501
         'content_type': 'contentType',  # noqa: E501
-        'product_slug': 'productSlug',  # noqa: E501
+        'filename': 'filename',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
         'policy_code': 'policyCode',  # noqa: E501
         'account_code': 'accountCode',  # noqa: E501
         'entity_id': 'entityId',  # noqa: E501
-        'metadata': 'metadata',  # noqa: E501
-        'filename': 'filename',  # noqa: E501
-        'should_skip_default_margins': 'shouldSkipDefaultMargins',  # noqa: E501
-        'engine': 'engine',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, template_slug, payload, entity_type, description, content_type, *args, **kwargs):  # noqa: E501
-        """CreateDocumentRequestDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, code, template_slug, entity_type, metadata, description, s3_key, content_type, filename, created_at, *args, **kwargs):  # noqa: E501
+        """DocumentClass - a model defined in OpenAPI
 
         Args:
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            code (str): Unique identifier for the object.
             template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Document payload.
-            entity_type (str): Document entity type.
-            description (str): Document description.
-            content_type (str): Document type.
+            entity_type (str): Document entity type
+            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the document would need for specific cases.
+            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
+            s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
+            content_type (str): Type of the document expressed with its file extension.
+            filename (str): Document file name.
+            created_at (datetime): Time at which the object was created.
 
         Keyword Args:
-            requester (str): Document requester.. defaults to "publicapi", must be one of ["publicapi", ]  # noqa: E501
+            requester (str): Identifier of the service that requested the creation of this document.. defaults to "publicapi", must be one of ["publicapi", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -192,22 +195,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
             policy_code (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
             account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
-            entity_id (float): Unique identifier referencing the entity.. [optional]  # noqa: E501
-            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the document would need for specific cases.. [optional]  # noqa: E501
-            filename (str): Document file name.. [optional]  # noqa: E501
-            should_skip_default_margins (bool): If true, the default margins will be skipped when generating the document.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            engine (str): Type of the document engine to use to generate the document. Defaults to HTML.. [optional] if omitted the server will use the default value of "html"  # noqa: E501
+            entity_id (float): Unique identifier referencing the entity on the service the document belongs to.. [optional]  # noqa: E501
         """
 
         requester = kwargs.get('requester', "publicapi")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -232,20 +230,25 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.code = code
         self.template_slug = template_slug
-        self.payload = payload
         self.entity_type = entity_type
-        self.description = description
         self.requester = requester
+        self.metadata = metadata
+        self.description = description
+        self.s3_key = s3_key
         self.content_type = content_type
+        self.filename = filename
+        self.created_at = created_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -258,26 +261,31 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, template_slug, payload, entity_type, description, content_type, *args, **kwargs):  # noqa: E501
-        """CreateDocumentRequestDto - a model defined in OpenAPI
+    def __init__(self, id, code, template_slug, entity_type, metadata, description, s3_key, content_type, filename, created_at, *args, **kwargs):  # noqa: E501
+        """DocumentClass - a model defined in OpenAPI
 
         Args:
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            code (str): Unique identifier for the object.
             template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Document payload.
-            entity_type (str): Document entity type.
-            description (str): Document description.
-            content_type (str): Document type.
+            entity_type (str): Document entity type
+            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the document would need for specific cases.
+            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
+            s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
+            content_type (str): Type of the document expressed with its file extension.
+            filename (str): Document file name.
+            created_at (datetime): Time at which the object was created.
 
         Keyword Args:
-            requester (str): Document requester.. defaults to "publicapi", must be one of ["publicapi", ]  # noqa: E501
+            requester (str): Identifier of the service that requested the creation of this document.. defaults to "publicapi", must be one of ["publicapi", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -300,22 +308,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
             policy_code (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
             account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
-            entity_id (float): Unique identifier referencing the entity.. [optional]  # noqa: E501
-            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the document would need for specific cases.. [optional]  # noqa: E501
-            filename (str): Document file name.. [optional]  # noqa: E501
-            should_skip_default_margins (bool): If true, the default margins will be skipped when generating the document.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            engine (str): Type of the document engine to use to generate the document. Defaults to HTML.. [optional] if omitted the server will use the default value of "html"  # noqa: E501
+            entity_id (float): Unique identifier referencing the entity on the service the document belongs to.. [optional]  # noqa: E501
         """
 
         requester = kwargs.get('requester', "publicapi")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -338,20 +341,25 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.code = code
         self.template_slug = template_slug
-        self.payload = payload
         self.entity_type = entity_type
-        self.description = description
         self.requester = requester
+        self.metadata = metadata
+        self.description = description
+        self.s3_key = s3_key
         self.content_type = content_type
+        self.filename = filename
+        self.created_at = created_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_estimated_invoice_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/create_estimated_invoice_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_estimated_invoice_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/policy_object_request_dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,22 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.publicapi.model.calculate_product_fields_response_class import CalculateProductFieldsResponseClass
-    from eis.publicapi.model.invoice_class import InvoiceClass
-    globals()['CalculateProductFieldsResponseClass'] = CalculateProductFieldsResponseClass
-    globals()['InvoiceClass'] = InvoiceClass
 
-
-class CreateEstimatedInvoiceResponseClass(ModelNormal):
+class PolicyObjectRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -69,56 +63,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'invoice': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'custom': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'policy_objects': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'insured_object_id': (float,),  # noqa: E501
+            'data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'code': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'invoice': 'invoice',  # noqa: E501
-        'custom': 'custom',  # noqa: E501
-        'policy_objects': 'policyObjects',  # noqa: E501
+        'insured_object_id': 'insuredObjectId',  # noqa: E501
+        'data': 'data',  # noqa: E501
+        'code': 'code',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreateEstimatedInvoiceResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, insured_object_id, data, *args, **kwargs):  # noqa: E501
+        """PolicyObjectRequestDto - a model defined in OpenAPI
+
+        Args:
+            insured_object_id (float): Unique identifier referencing the insured object.
+            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object data.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,17 +139,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            invoice (bool, date, datetime, dict, float, int, list, str, none_type): Estimated invoice response. [optional]  # noqa: E501
-            custom ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): In some cases, custom premium calculation needs to be used.     In that case, a custom object is returned. It can hold up any kind of information. For more information,     check the general documentation.. [optional]  # noqa: E501
-            policy_objects (bool, date, datetime, dict, float, int, list, str, none_type): Calculated policy obejcts response. [optional]  # noqa: E501
+            code (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -177,14 +171,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.insured_object_id = insured_object_id
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -197,16 +193,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """CreateEstimatedInvoiceResponseClass - a model defined in OpenAPI
+    def __init__(self, insured_object_id, data, *args, **kwargs):  # noqa: E501
+        """PolicyObjectRequestDto - a model defined in OpenAPI
+
+        Args:
+            insured_object_id (float): Unique identifier referencing the insured object.
+            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object data.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -231,17 +231,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            invoice (bool, date, datetime, dict, float, int, list, str, none_type): Estimated invoice response. [optional]  # noqa: E501
-            custom ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): In some cases, custom premium calculation needs to be used.     In that case, a custom object is returned. It can hold up any kind of information. For more information,     check the general documentation.. [optional]  # noqa: E501
-            policy_objects (bool, date, datetime, dict, float, int, list, str, none_type): Calculated policy obejcts response. [optional]  # noqa: E501
+            code (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -263,14 +261,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.insured_object_id = insured_object_id
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_lead_async_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/initiate_braintree_payment_setup_response_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class CreateLeadAsyncResponseClass(ModelNormal):
+class InitiateBraintreePaymentSetupResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'code': (str,),  # noqa: E501
+            'psp_secret_token': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'code': 'code',  # noqa: E501
+        'psp_secret_token': 'pspSecretToken',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, code, *args, **kwargs):  # noqa: E501
-        """CreateLeadAsyncResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, psp_secret_token, *args, **kwargs):  # noqa: E501
+        """InitiateBraintreePaymentSetupResponseClass - a model defined in OpenAPI
 
         Args:
-            code (str): Unique identifier of the lead that this object belongs to.
+            psp_secret_token (str): Identifier used by the payment service provider to create a payment method.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.code = code
+        self.psp_secret_token = psp_secret_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, code, *args, **kwargs):  # noqa: E501
-        """CreateLeadAsyncResponseClass - a model defined in OpenAPI
+    def __init__(self, psp_secret_token, *args, **kwargs):  # noqa: E501
+        """InitiateBraintreePaymentSetupResponseClass - a model defined in OpenAPI
 
         Args:
-            code (str): Unique identifier of the lead that this object belongs to.
+            psp_secret_token (str): Identifier used by the payment service provider to create a payment method.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.code = code
+        self.psp_secret_token = psp_secret_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_lead_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/create_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_payment_method_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/list_documents_response_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from eis.publicapi.model.sepa_dto import SepaDto
-    globals()['SepaDto'] = SepaDto
+    from eis.publicapi.model.document_class import DocumentClass
+    globals()['DocumentClass'] = DocumentClass
 
 
-class CreatePaymentMethodRequestDto(ModelNormal):
+class ListDocumentsResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,18 +56,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('type',): {
-            'SEPA': "sepa",
-            'INVOICE': "invoice",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -88,40 +84,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'sepa': (SepaDto,),  # noqa: E501
+            'items': ([DocumentClass],),  # noqa: E501
+            'next_page_token': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'sepa': 'sepa',  # noqa: E501
+        'items': 'items',  # noqa: E501
+        'next_page_token': 'nextPageToken',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
-        """CreatePaymentMethodRequestDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
+        """ListDocumentsResponseClass - a model defined in OpenAPI
 
         Args:
-            type (str):
+            items ([DocumentClass]): The list of documents.
+            next_page_token (str): Next page token
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,15 +143,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sepa (SepaDto): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,15 +174,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
+        self.items = items
+        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -199,19 +196,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, type, *args, **kwargs):  # noqa: E501
-        """CreatePaymentMethodRequestDto - a model defined in OpenAPI
+    def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
+        """ListDocumentsResponseClass - a model defined in OpenAPI
 
         Args:
-            type (str):
+            items ([DocumentClass]): The list of documents.
+            next_page_token (str): Next page token
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -236,15 +234,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sepa (SepaDto): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -266,15 +263,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
+        self.items = items
+        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_presigned_post_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/product_field_class.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class CreatePresignedPostRequestDto(ModelNormal):
+class ProductFieldClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,50 +52,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('requester',): {
-            'ACCOUNTSERVICE': "accountservice",
-            'INSURANCESERVICE': "insuranceservice",
-            'BILLINGSERVICE': "billingservice",
-            'TENANTSERVICE': "tenantservice",
-            'BOOKINGFUNNEL': "bookingFunnel",
-            'PUBLICAPI': "publicapi",
-            'ADMIN': "admin",
-            'CLAIMSERVICE': "claimservice",
-            'CUSTOMERSERVICE': "customerservice",
-            'NOTIFICATIONSERVICE': "notificationservice",
-            'PAYMENTSERVICE': "paymentservice",
-            'PROCESSMANAGER': "processmanager",
-            'GDVSERVICE': "gdvservice",
-            'DOCUMENTSERVICE': "documentservice",
-        },
-        ('content_type',): {
-            'PDF': "pdf",
-            'JPG': "jpg",
-            'PNG': "png",
-            'GZ': "gz",
-            'CSV': "csv",
-            'DOC': "doc",
-            'DOCX': "docx",
-            'HTML': "html",
-            'JSON': "json",
-            'XML': "xml",
-            'TXT': "txt",
-            'ZIP': "zip",
-            'TAR': "tar",
-            'RAR': "rar",
-            'MP4': "MP4",
-            'MOV': "MOV",
-            'WMV': "WMV",
-            'AVI': "AVI",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -114,66 +78,92 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'template_slug': (str,),  # noqa: E501
-            'entity_type': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
-            'requester': (str,),  # noqa: E501
-            'content_type': (str,),  # noqa: E501
-            'iso_content_type': (str,),  # noqa: E501
-            'filename': (str,),  # noqa: E501
-            'entity_id': (float,),  # noqa: E501
-            'policy_code': (str,),  # noqa: E501
-            'account_code': (str,),  # noqa: E501
-            'lead_code': (str,),  # noqa: E501
-            'product_slug': (str,),  # noqa: E501
+            'id': (float,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'group': (str,),  # noqa: E501
+            'label': (str,),  # noqa: E501
+            'type_entity': (str,),  # noqa: E501
+            'type_id': (float,),  # noqa: E501
+            'insured_object_id': (float,),  # noqa: E501
+            'is_required': (bool,),  # noqa: E501
+            'is_hidden': (bool,),  # noqa: E501
+            'is_hidden_customer_portal': (bool,),  # noqa: E501
+            'is_editable_customer_portal': (bool,),  # noqa: E501
+            'is_system': (bool,),  # noqa: E501
+            'is_unique': (bool,),  # noqa: E501
+            'default_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'min_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'max_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
+            'updated_at': (datetime,),  # noqa: E501
+            'order': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'template_slug': 'templateSlug',  # noqa: E501
-        'entity_type': 'entityType',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'requester': 'requester',  # noqa: E501
-        'content_type': 'contentType',  # noqa: E501
-        'iso_content_type': 'isoContentType',  # noqa: E501
-        'filename': 'filename',  # noqa: E501
-        'entity_id': 'entityId',  # noqa: E501
-        'policy_code': 'policyCode',  # noqa: E501
-        'account_code': 'accountCode',  # noqa: E501
-        'lead_code': 'leadCode',  # noqa: E501
-        'product_slug': 'productSlug',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'group': 'group',  # noqa: E501
+        'label': 'label',  # noqa: E501
+        'type_entity': 'typeEntity',  # noqa: E501
+        'type_id': 'typeId',  # noqa: E501
+        'insured_object_id': 'insuredObjectId',  # noqa: E501
+        'is_required': 'isRequired',  # noqa: E501
+        'is_hidden': 'isHidden',  # noqa: E501
+        'is_hidden_customer_portal': 'isHiddenCustomerPortal',  # noqa: E501
+        'is_editable_customer_portal': 'isEditableCustomerPortal',  # noqa: E501
+        'is_system': 'isSystem',  # noqa: E501
+        'is_unique': 'isUnique',  # noqa: E501
+        'default_value': 'defaultValue',  # noqa: E501
+        'min_value': 'minValue',  # noqa: E501
+        'max_value': 'maxValue',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
+        'updated_at': 'updatedAt',  # noqa: E501
+        'order': 'order',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, template_slug, entity_type, description, requester, content_type, iso_content_type, filename, *args, **kwargs):  # noqa: E501
-        """CreatePresignedPostRequestDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, min_value, max_value, created_at, updated_at, order, *args, **kwargs):  # noqa: E501
+        """ProductFieldClass - a model defined in OpenAPI
 
         Args:
-            template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            entity_type (str): Document entity type.
-            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
-            requester (str): Identifier of the service that requested the creation of this document.
-            content_type (str): Extension of the file.
-            iso_content_type (str): Content type of the file.
-            filename (str): Name of the file the end user will see when he downloads it.
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            name (str): Product field name.
+            group (str): Product field group.
+            label (str): Product field label.
+            type_entity (str): Product field type.
+            type_id (float): Unique identifier referencing the product type.
+            insured_object_id (float): Unique identifier referencing the insured object.
+            is_required (bool): Is field required?
+            is_hidden (bool): Is field hidden on the booking funnel?
+            is_hidden_customer_portal (bool): Is field hidden on the customer portal?
+            is_editable_customer_portal (bool): Is field editable on the customer portal?
+            is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
+            is_unique (bool): Should the field value be unique across policies?
+            default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
+            min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
+            max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
+            created_at (datetime): Time at which the object was created.
+            updated_at (datetime): Time at which the object was updated.
+            order (float): Order
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -198,19 +188,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            entity_id (float): Unique identifier referencing the entity.. [optional]  # noqa: E501
-            policy_code (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
-            account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
-            lead_code (str): Unique identifier of the lead that this object belongs to.. [optional]  # noqa: E501
-            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -234,21 +219,33 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.template_slug = template_slug
-        self.entity_type = entity_type
-        self.description = description
-        self.requester = requester
-        self.content_type = content_type
-        self.iso_content_type = iso_content_type
-        self.filename = filename
+        self.id = id
+        self.name = name
+        self.group = group
+        self.label = label
+        self.type_entity = type_entity
+        self.type_id = type_id
+        self.insured_object_id = insured_object_id
+        self.is_required = is_required
+        self.is_hidden = is_hidden
+        self.is_hidden_customer_portal = is_hidden_customer_portal
+        self.is_editable_customer_portal = is_editable_customer_portal
+        self.is_system = is_system
+        self.is_unique = is_unique
+        self.default_value = default_value
+        self.min_value = min_value
+        self.max_value = max_value
+        self.created_at = created_at
+        self.updated_at = updated_at
+        self.order = order
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -261,25 +258,37 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, template_slug, entity_type, description, requester, content_type, iso_content_type, filename, *args, **kwargs):  # noqa: E501
-        """CreatePresignedPostRequestDto - a model defined in OpenAPI
+    def __init__(self, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, min_value, max_value, created_at, updated_at, order, *args, **kwargs):  # noqa: E501
+        """ProductFieldClass - a model defined in OpenAPI
 
         Args:
-            template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            entity_type (str): Document entity type.
-            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
-            requester (str): Identifier of the service that requested the creation of this document.
-            content_type (str): Extension of the file.
-            iso_content_type (str): Content type of the file.
-            filename (str): Name of the file the end user will see when he downloads it.
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            name (str): Product field name.
+            group (str): Product field group.
+            label (str): Product field label.
+            type_entity (str): Product field type.
+            type_id (float): Unique identifier referencing the product type.
+            insured_object_id (float): Unique identifier referencing the insured object.
+            is_required (bool): Is field required?
+            is_hidden (bool): Is field hidden on the booking funnel?
+            is_hidden_customer_portal (bool): Is field hidden on the customer portal?
+            is_editable_customer_portal (bool): Is field editable on the customer portal?
+            is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
+            is_unique (bool): Should the field value be unique across policies?
+            default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
+            min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
+            max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
+            created_at (datetime): Time at which the object was created.
+            updated_at (datetime): Time at which the object was updated.
+            order (float): Order
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -304,19 +313,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            entity_id (float): Unique identifier referencing the entity.. [optional]  # noqa: E501
-            policy_code (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
-            account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
-            lead_code (str): Unique identifier of the lead that this object belongs to.. [optional]  # noqa: E501
-            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -338,21 +342,33 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.template_slug = template_slug
-        self.entity_type = entity_type
-        self.description = description
-        self.requester = requester
-        self.content_type = content_type
-        self.iso_content_type = iso_content_type
-        self.filename = filename
+        self.id = id
+        self.name = name
+        self.group = group
+        self.label = label
+        self.type_entity = type_entity
+        self.type_id = type_id
+        self.insured_object_id = insured_object_id
+        self.is_required = is_required
+        self.is_hidden = is_hidden
+        self.is_hidden_customer_portal = is_hidden_customer_portal
+        self.is_editable_customer_portal = is_editable_customer_portal
+        self.is_system = is_system
+        self.is_unique = is_unique
+        self.default_value = default_value
+        self.min_value = min_value
+        self.max_value = max_value
+        self.created_at = created_at
+        self.updated_at = updated_at
+        self.order = order
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/create_presigned_post_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/lead_bank_account_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class CreatePresignedPostResponseClass(ModelNormal):
+class LeadBankAccountClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'url': (str,),  # noqa: E501
+            'account_code': (str,),  # noqa: E501
+            'iban': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'fields': 'fields',  # noqa: E501
-        'url': 'url',  # noqa: E501
+        'account_code': 'accountCode',  # noqa: E501
+        'iban': 'iban',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, fields, url, *args, **kwargs):  # noqa: E501
-        """CreatePresignedPostResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, account_code, iban, *args, **kwargs):  # noqa: E501
+        """LeadBankAccountClass - a model defined in OpenAPI
 
         Args:
-            fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Upload document fields.
-            url (str): Pre-signed Url.
+            account_code (str): Unique identifier of the account that this object belongs to.
+            iban (str): Bank account IBAN
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,16 +168,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.fields = fields
-        self.url = url
+        self.account_code = account_code
+        self.iban = iban
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +190,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, fields, url, *args, **kwargs):  # noqa: E501
-        """CreatePresignedPostResponseClass - a model defined in OpenAPI
+    def __init__(self, account_code, iban, *args, **kwargs):  # noqa: E501
+        """LeadBankAccountClass - a model defined in OpenAPI
 
         Args:
-            fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Upload document fields.
-            url (str): Pre-signed Url.
+            account_code (str): Unique identifier of the account that this object belongs to.
+            iban (str): Bank account IBAN
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,16 +257,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.fields = fields
-        self.url = url
+        self.account_code = account_code
+        self.iban = iban
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/document_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/create_document_request_dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class DocumentClass(ModelNormal):
+class CreateDocumentRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,46 +52,28 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('entity_type',): {
-            'POLICY_APPLICATION': "policy_application",
-            'POLICY_CONTRACT': "policy_contract",
-            'POLICY_ADDENDUM': "policy_addendum",
-            'INITIAL_INVOICE': "initial_invoice",
-            'CORRECTION_INVOICE': "correction_invoice",
-            'RECURRING_INVOICE': "recurring_invoice",
-            'SEPA_MANDATE': "sepa_mandate",
-            'STATIC': "static",
-        },
         ('requester',): {
             'PUBLICAPI': "publicapi",
         },
         ('content_type',): {
             'PDF': "pdf",
             'JPG': "jpg",
             'PNG': "png",
             'GZ': "gz",
             'CSV': "csv",
             'DOC': "doc",
             'DOCX': "docx",
             'HTML': "html",
             'JSON': "json",
             'XML': "xml",
-            'TXT': "txt",
-            'ZIP': "zip",
-            'TAR': "tar",
-            'RAR': "rar",
-            'MP4': "MP4",
-            'MOV': "MOV",
-            'WMV': "WMV",
-            'AVI': "AVI",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -111,79 +93,67 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (float,),  # noqa: E501
-            'code': (str,),  # noqa: E501
             'template_slug': (str,),  # noqa: E501
+            'payload': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'entity_type': (str,),  # noqa: E501
-            'requester': (str,),  # noqa: E501
-            'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'description': (str,),  # noqa: E501
-            's3_key': (str,),  # noqa: E501
+            'requester': (str,),  # noqa: E501
             'content_type': (str,),  # noqa: E501
-            'filename': (str,),  # noqa: E501
-            'lead_code': (str,),  # noqa: E501
-            'created_at': (datetime,),  # noqa: E501
+            'product_slug': (str,),  # noqa: E501
             'policy_code': (str,),  # noqa: E501
             'account_code': (str,),  # noqa: E501
             'entity_id': (float,),  # noqa: E501
+            'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'filename': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'code': 'code',  # noqa: E501
         'template_slug': 'templateSlug',  # noqa: E501
+        'payload': 'payload',  # noqa: E501
         'entity_type': 'entityType',  # noqa: E501
-        'requester': 'requester',  # noqa: E501
-        'metadata': 'metadata',  # noqa: E501
         'description': 'description',  # noqa: E501
-        's3_key': 's3Key',  # noqa: E501
+        'requester': 'requester',  # noqa: E501
         'content_type': 'contentType',  # noqa: E501
-        'filename': 'filename',  # noqa: E501
-        'lead_code': 'leadCode',  # noqa: E501
-        'created_at': 'createdAt',  # noqa: E501
+        'product_slug': 'productSlug',  # noqa: E501
         'policy_code': 'policyCode',  # noqa: E501
         'account_code': 'accountCode',  # noqa: E501
         'entity_id': 'entityId',  # noqa: E501
+        'metadata': 'metadata',  # noqa: E501
+        'filename': 'filename',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, code, template_slug, entity_type, metadata, description, s3_key, content_type, filename, lead_code, created_at, *args, **kwargs):  # noqa: E501
-        """DocumentClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, template_slug, payload, entity_type, description, content_type, *args, **kwargs):  # noqa: E501
+        """CreateDocumentRequestDto - a model defined in OpenAPI
 
         Args:
-            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            code (str): Unique identifier for the object.
             template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            entity_type (str): Document entity type
-            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the document would need for specific cases.
-            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
-            s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
-            content_type (str): Type of the document expressed with its file extension.
-            filename (str): Document file name.
-            lead_code (str): Lead
-            created_at (datetime): Time at which the object was created.
+            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Document payload.
+            entity_type (str): Document entity type.
+            description (str): Document description.
+            content_type (str): Document type.
 
         Keyword Args:
-            requester (str): Identifier of the service that requested the creation of this document.. defaults to "publicapi", must be one of ["publicapi", ]  # noqa: E501
+            requester (str): Document requester.. defaults to "publicapi", must be one of ["publicapi", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -206,17 +176,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
             policy_code (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
             account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
-            entity_id (float): Unique identifier referencing the entity on the service the document belongs to.. [optional]  # noqa: E501
+            entity_id (float): Unique identifier referencing the entity.. [optional]  # noqa: E501
+            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the document would need for specific cases.. [optional]  # noqa: E501
+            filename (str): Document file name.. [optional]  # noqa: E501
         """
 
         requester = kwargs.get('requester', "publicapi")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -241,26 +214,20 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.code = code
         self.template_slug = template_slug
+        self.payload = payload
         self.entity_type = entity_type
-        self.requester = requester
-        self.metadata = metadata
         self.description = description
-        self.s3_key = s3_key
+        self.requester = requester
         self.content_type = content_type
-        self.filename = filename
-        self.lead_code = lead_code
-        self.created_at = created_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -273,32 +240,26 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, code, template_slug, entity_type, metadata, description, s3_key, content_type, filename, lead_code, created_at, *args, **kwargs):  # noqa: E501
-        """DocumentClass - a model defined in OpenAPI
+    def __init__(self, template_slug, payload, entity_type, description, content_type, *args, **kwargs):  # noqa: E501
+        """CreateDocumentRequestDto - a model defined in OpenAPI
 
         Args:
-            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            code (str): Unique identifier for the object.
             template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            entity_type (str): Document entity type
-            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the document would need for specific cases.
-            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
-            s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
-            content_type (str): Type of the document expressed with its file extension.
-            filename (str): Document file name.
-            lead_code (str): Lead
-            created_at (datetime): Time at which the object was created.
+            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Document payload.
+            entity_type (str): Document entity type.
+            description (str): Document description.
+            content_type (str): Document type.
 
         Keyword Args:
-            requester (str): Identifier of the service that requested the creation of this document.. defaults to "publicapi", must be one of ["publicapi", ]  # noqa: E501
+            requester (str): Document requester.. defaults to "publicapi", must be one of ["publicapi", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -321,17 +282,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
             policy_code (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
             account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
-            entity_id (float): Unique identifier referencing the entity on the service the document belongs to.. [optional]  # noqa: E501
+            entity_id (float): Unique identifier referencing the entity.. [optional]  # noqa: E501
+            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Metadata contains extra information that the document would need for specific cases.. [optional]  # noqa: E501
+            filename (str): Document file name.. [optional]  # noqa: E501
         """
 
         requester = kwargs.get('requester', "publicapi")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -354,26 +318,20 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.code = code
         self.template_slug = template_slug
+        self.payload = payload
         self.entity_type = entity_type
-        self.requester = requester
-        self.metadata = metadata
         self.description = description
-        self.s3_key = s3_key
+        self.requester = requester
         self.content_type = content_type
-        self.filename = filename
-        self.lead_code = lead_code
-        self.created_at = created_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/get_custom_css_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/send_notification_response_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class GetCustomCssResponseClass(ModelNormal):
+class SendNotificationResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'values': ([str],),  # noqa: E501
+            'code': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'values': 'values',  # noqa: E501
+        'code': 'code',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, values, *args, **kwargs):  # noqa: E501
-        """GetCustomCssResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, code, *args, **kwargs):  # noqa: E501
+        """SendNotificationResponseClass - a model defined in OpenAPI
 
         Args:
-            values ([str]): Custom CSS setting for booking funnel.
+            code (str): Unique identifier for the object.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.values = values
+        self.code = code
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, values, *args, **kwargs):  # noqa: E501
-        """GetCustomCssResponseClass - a model defined in OpenAPI
+    def __init__(self, code, *args, **kwargs):  # noqa: E501
+        """SendNotificationResponseClass - a model defined in OpenAPI
 
         Args:
-            values ([str]): Custom CSS setting for booking funnel.
+            code (str): Unique identifier for the object.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.values = values
+        self.code = code
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/get_lead_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/get_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/get_product_document_download_url_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/uploaded_document_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class GetProductDocumentDownloadUrlResponseClass(ModelNormal):
+class UploadedDocumentDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'url': (str,),  # noqa: E501
+            'codes': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'url': 'url',  # noqa: E501
+        'codes': 'codes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, url, *args, **kwargs):  # noqa: E501
-        """GetProductDocumentDownloadUrlResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, codes, *args, **kwargs):  # noqa: E501
+        """UploadedDocumentDto - a model defined in OpenAPI
 
         Args:
-            url (str): Pre-signed Url
+            codes ([str]): Uploaded document codes.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.url = url
+        self.codes = codes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, url, *args, **kwargs):  # noqa: E501
-        """GetProductDocumentDownloadUrlResponseClass - a model defined in OpenAPI
+    def __init__(self, codes, *args, **kwargs):  # noqa: E501
+        """UploadedDocumentDto - a model defined in OpenAPI
 
         Args:
-            url (str): Pre-signed Url
+            codes ([str]): Uploaded document codes.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.url = url
+        self.codes = codes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/get_public_psp_settings_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/list_product_documents_response_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.publicapi.model.product_document_class import ProductDocumentClass
+    globals()['ProductDocumentClass'] = ProductDocumentClass
 
-class GetPublicPspSettingsResponseClass(ModelNormal):
+
+class ListProductDocumentsResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +67,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'public_key': (str,),  # noqa: E501
-            'psp': (str,),  # noqa: E501
+            'items': ([ProductDocumentClass],),  # noqa: E501
+            'next_page_token': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'public_key': 'publicKey',  # noqa: E501
-        'psp': 'psp',  # noqa: E501
+        'items': 'items',  # noqa: E501
+        'next_page_token': 'nextPageToken',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, public_key, psp, *args, **kwargs):  # noqa: E501
-        """GetPublicPspSettingsResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
+        """ListProductDocumentsResponseClass - a model defined in OpenAPI
 
         Args:
-            public_key (str): Public key. Used on frontend to load the payment form component.
-            psp (str): Name of payment system provider.
+            items ([ProductDocumentClass]): The list of documents.
+            next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,16 +174,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.public_key = public_key
-        self.psp = psp
+        self.items = items
+        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +196,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, public_key, psp, *args, **kwargs):  # noqa: E501
-        """GetPublicPspSettingsResponseClass - a model defined in OpenAPI
+    def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
+        """ListProductDocumentsResponseClass - a model defined in OpenAPI
 
         Args:
-            public_key (str): Public key. Used on frontend to load the payment form component.
-            psp (str): Name of payment system provider.
+            items ([ProductDocumentClass]): The list of documents.
+            next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,16 +263,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.public_key = public_key
-        self.psp = psp
+        self.items = items
+        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/initiate_braintree_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/initiate_braintree_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/initiate_braintree_payment_setup_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/initiate_stripe_payment_setup_response_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class InitiateBraintreePaymentSetupResponseClass(ModelNormal):
+class InitiateStripePaymentSetupResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -79,37 +79,40 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'psp_secret_token': (str,),  # noqa: E501
+            'psp_customer_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'psp_secret_token': 'pspSecretToken',  # noqa: E501
+        'psp_customer_id': 'pspCustomerId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, psp_secret_token, *args, **kwargs):  # noqa: E501
-        """InitiateBraintreePaymentSetupResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, psp_secret_token, psp_customer_id, *args, **kwargs):  # noqa: E501
+        """InitiateStripePaymentSetupResponseClass - a model defined in OpenAPI
 
         Args:
             psp_secret_token (str): Identifier used by the payment service provider to create a payment method.
+            psp_customer_id (str): Unique identifier for the customer on Stripe.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -166,14 +169,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.psp_secret_token = psp_secret_token
+        self.psp_customer_id = psp_customer_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +190,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, psp_secret_token, *args, **kwargs):  # noqa: E501
-        """InitiateBraintreePaymentSetupResponseClass - a model defined in OpenAPI
+    def __init__(self, psp_secret_token, psp_customer_id, *args, **kwargs):  # noqa: E501
+        """InitiateStripePaymentSetupResponseClass - a model defined in OpenAPI
 
         Args:
             psp_secret_token (str): Identifier used by the payment service provider to create a payment method.
+            psp_customer_id (str): Unique identifier for the customer on Stripe.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -253,14 +258,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.psp_secret_token = psp_secret_token
+        self.psp_customer_id = psp_customer_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/initiate_email_verification_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/initiate_stripe_payment_setup_request_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class InitiateEmailVerificationDto(ModelNormal):
+class InitiateStripePaymentSetupRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,40 +78,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'email': (str,),  # noqa: E501
-            'template_slug': (str,),  # noqa: E501
+            'lead_code': (str,),  # noqa: E501
+            'account_code': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email': 'email',  # noqa: E501
-        'template_slug': 'templateSlug',  # noqa: E501
+        'lead_code': 'leadCode',  # noqa: E501
+        'account_code': 'accountCode',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, email, *args, **kwargs):  # noqa: E501
-        """InitiateEmailVerificationDto - a model defined in OpenAPI
-
-        Args:
-            email (str): User email
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """InitiateStripePaymentSetupRequestDto - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
+            lead_code (str): Unique identifier of the lead that this object belongs to.. [optional]  # noqa: E501
+            account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,15 +166,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,19 +186,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, email, *args, **kwargs):  # noqa: E501
-        """InitiateEmailVerificationDto - a model defined in OpenAPI
-
-        Args:
-            email (str): User email
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """InitiateStripePaymentSetupRequestDto - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
+            lead_code (str): Unique identifier of the lead that this object belongs to.. [optional]  # noqa: E501
+            account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,15 +251,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/initiate_email_verification_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/update_lead_response_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.publicapi.model.lead_class import LeadClass
+    globals()['LeadClass'] = LeadClass
 
-class InitiateEmailVerificationResponseClass(ModelNormal):
+
+class UpdateLeadResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,53 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'result': (bool,),  # noqa: E501
+            'lead': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'result': 'result',  # noqa: E501
+        'lead': 'lead',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, result, *args, **kwargs):  # noqa: E501
-        """InitiateEmailVerificationResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, lead, *args, **kwargs):  # noqa: E501
+        """UpdateLeadResponseClass - a model defined in OpenAPI
 
         Args:
-            result (bool): Initiate verification result
+            lead (bool, date, datetime, dict, float, int, list, str, none_type): The list of leads.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.result = result
+        self.lead = lead
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, result, *args, **kwargs):  # noqa: E501
-        """InitiateEmailVerificationResponseClass - a model defined in OpenAPI
+    def __init__(self, lead, *args, **kwargs):  # noqa: E501
+        """UpdateLeadResponseClass - a model defined in OpenAPI
 
         Args:
-            result (bool): Initiate verification result
+            lead (bool, date, datetime, dict, float, int, list, str, none_type): The list of leads.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.result = result
+        self.lead = lead
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/initiate_lead_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/initiate_payment_setup_response_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,16 +26,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.publicapi.model.initiate_braintree_payment_setup_response_class import InitiateBraintreePaymentSetupResponseClass
+    from eis.publicapi.model.initiate_stripe_payment_setup_response_class import InitiateStripePaymentSetupResponseClass
+    globals()['InitiateBraintreePaymentSetupResponseClass'] = InitiateBraintreePaymentSetupResponseClass
+    globals()['InitiateStripePaymentSetupResponseClass'] = InitiateStripePaymentSetupResponseClass
 
-class InitiateLeadResponseClass(ModelNormal):
+
+class InitiatePaymentSetupResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,53 +69,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'lead_code': (str,),  # noqa: E501
+            'stripe': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'braintree': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'lead_code': 'leadCode',  # noqa: E501
+        'stripe': 'stripe',  # noqa: E501
+        'braintree': 'braintree',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, lead_code, *args, **kwargs):  # noqa: E501
-        """InitiateLeadResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, stripe, braintree, *args, **kwargs):  # noqa: E501
+        """InitiatePaymentSetupResponseClass - a model defined in OpenAPI
 
         Args:
-            lead_code (str): Unique identifier of the lead that this object belongs to.
+            stripe (bool, date, datetime, dict, float, int, list, str, none_type): The stripe response after creating the setup intent.
+            braintree (bool, date, datetime, dict, float, int, list, str, none_type): Braintree response after generating client token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +176,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.lead_code = lead_code
+        self.stripe = stripe
+        self.braintree = braintree
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +198,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, lead_code, *args, **kwargs):  # noqa: E501
-        """InitiateLeadResponseClass - a model defined in OpenAPI
+    def __init__(self, stripe, braintree, *args, **kwargs):  # noqa: E501
+        """InitiatePaymentSetupResponseClass - a model defined in OpenAPI
 
         Args:
-            lead_code (str): Unique identifier of the lead that this object belongs to.
+            stripe (bool, date, datetime, dict, float, int, list, str, none_type): The stripe response after creating the setup intent.
+            braintree (bool, date, datetime, dict, float, int, list, str, none_type): Braintree response after generating client token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +265,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.lead_code = lead_code
+        self.stripe = stripe
+        self.braintree = braintree
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/initiate_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/initiate_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/initiate_payment_setup_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/create_estimated_invoice_response_class.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,21 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from eis.publicapi.model.initiate_braintree_payment_setup_response_class import InitiateBraintreePaymentSetupResponseClass
-    from eis.publicapi.model.initiate_stripe_payment_setup_response_class import InitiateStripePaymentSetupResponseClass
-    globals()['InitiateBraintreePaymentSetupResponseClass'] = InitiateBraintreePaymentSetupResponseClass
-    globals()['InitiateStripePaymentSetupResponseClass'] = InitiateStripePaymentSetupResponseClass
+    from eis.publicapi.model.invoice_class import InvoiceClass
+    globals()['InvoiceClass'] = InvoiceClass
 
 
-class InitiatePaymentSetupResponseClass(ModelNormal):
+class CreateEstimatedInvoiceResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,41 +84,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'stripe': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'braintree': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'invoice': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'custom': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'stripe': 'stripe',  # noqa: E501
-        'braintree': 'braintree',  # noqa: E501
+        'invoice': 'invoice',  # noqa: E501
+        'custom': 'custom',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, stripe, braintree, *args, **kwargs):  # noqa: E501
-        """InitiatePaymentSetupResponseClass - a model defined in OpenAPI
-
-        Args:
-            stripe (bool, date, datetime, dict, float, int, list, str, none_type): The stripe response after creating the setup intent.
-            braintree (bool, date, datetime, dict, float, int, list, str, none_type): Braintree response after generating client token.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """CreateEstimatedInvoiceResponseClass - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,14 +139,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            invoice (bool, date, datetime, dict, float, int, list, str, none_type): Estimated invoice response. [optional]  # noqa: E501
+            custom ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): In some cases, custom premium calculation needs to be used.      In that case, a custom object is returned. It can hold up any kind of information. For more information,      check the general documentation.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -176,16 +172,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.stripe = stripe
-        self.braintree = braintree
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,20 +192,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, stripe, braintree, *args, **kwargs):  # noqa: E501
-        """InitiatePaymentSetupResponseClass - a model defined in OpenAPI
-
-        Args:
-            stripe (bool, date, datetime, dict, float, int, list, str, none_type): The stripe response after creating the setup intent.
-            braintree (bool, date, datetime, dict, float, int, list, str, none_type): Braintree response after generating client token.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """CreateEstimatedInvoiceResponseClass - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -236,14 +226,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            invoice (bool, date, datetime, dict, float, int, list, str, none_type): Estimated invoice response. [optional]  # noqa: E501
+            custom ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): In some cases, custom premium calculation needs to be used.      In that case, a custom object is returned. It can hold up any kind of information. For more information,      check the general documentation.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -265,16 +257,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.stripe = stripe
-        self.braintree = braintree
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/initiate_stripe_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/invoice_status_class.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class InitiateStripePaymentSetupRequestDto(ModelNormal):
+class InvoiceStatusClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,37 +78,47 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'lead_code': (str,),  # noqa: E501
-            'account_code': (str,),  # noqa: E501
+            'id': (float,),  # noqa: E501
+            'invoice_id': (float,),  # noqa: E501
+            'status': (str,),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'lead_code': 'leadCode',  # noqa: E501
-        'account_code': 'accountCode',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'invoice_id': 'invoiceId',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """InitiateStripePaymentSetupRequestDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, invoice_id, status, created_at, *args, **kwargs):  # noqa: E501
+        """InvoiceStatusClass - a model defined in OpenAPI
+
+        Args:
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            invoice_id (float): Unique identifier referencing the invoice.
+            status (str): Invoice type
+            created_at (datetime): Time at which the object was created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +143,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            lead_code (str): Unique identifier of the lead that this object belongs to.. [optional]  # noqa: E501
-            account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -166,14 +174,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.invoice_id = invoice_id
+        self.status = status
+        self.created_at = created_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,16 +198,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """InitiateStripePaymentSetupRequestDto - a model defined in OpenAPI
+    def __init__(self, id, invoice_id, status, created_at, *args, **kwargs):  # noqa: E501
+        """InvoiceStatusClass - a model defined in OpenAPI
+
+        Args:
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            invoice_id (float): Unique identifier referencing the invoice.
+            status (str): Invoice type
+            created_at (datetime): Time at which the object was created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,16 +238,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            lead_code (str): Unique identifier of the lead that this object belongs to.. [optional]  # noqa: E501
-            account_code (str): Unique identifier of the account that this object belongs to.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -251,14 +267,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.invoice_id = invoice_id
+        self.status = status
+        self.created_at = created_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/initiate_stripe_payment_setup_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/premium_override_request_dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.publicapi.model.premium_override_dto import PremiumOverrideDto
+    globals()['PremiumOverrideDto'] = PremiumOverrideDto
 
-class InitiateStripePaymentSetupResponseClass(ModelNormal):
+
+class PremiumOverrideRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'psp_secret_token': (str,),  # noqa: E501
-            'psp_customer_id': (str,),  # noqa: E501
+            'premium_overrides': ([PremiumOverrideDto],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'psp_secret_token': 'pspSecretToken',  # noqa: E501
-        'psp_customer_id': 'pspCustomerId',  # noqa: E501
+        'premium_overrides': 'premiumOverrides',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, psp_secret_token, psp_customer_id, *args, **kwargs):  # noqa: E501
-        """InitiateStripePaymentSetupResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, premium_overrides, *args, **kwargs):  # noqa: E501
+        """PremiumOverrideRequestDto - a model defined in OpenAPI
 
         Args:
-            psp_secret_token (str): Identifier used by the payment service provider to create a payment method.
-            psp_customer_id (str): Unique identifier for the customer on Stripe.
+            premium_overrides ([PremiumOverrideDto]): Premium Override.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,16 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.psp_secret_token = psp_secret_token
-        self.psp_customer_id = psp_customer_id
+        self.premium_overrides = premium_overrides
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, psp_secret_token, psp_customer_id, *args, **kwargs):  # noqa: E501
-        """InitiateStripePaymentSetupResponseClass - a model defined in OpenAPI
+    def __init__(self, premium_overrides, *args, **kwargs):  # noqa: E501
+        """PremiumOverrideRequestDto - a model defined in OpenAPI
 
         Args:
-            psp_secret_token (str): Identifier used by the payment service provider to create a payment method.
-            psp_customer_id (str): Unique identifier for the customer on Stripe.
+            premium_overrides ([PremiumOverrideDto]): Premium Override.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,16 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.psp_secret_token = psp_secret_token
-        self.psp_customer_id = psp_customer_id
+        self.premium_overrides = premium_overrides
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/inline_response200.py` & `eis-publicapi-1.6.0/eis/publicapi/model/structured_address_class.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class InlineResponse200(ModelNormal):
+class StructuredAddressClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,53 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'status': (str,),  # noqa: E501
-            'info': ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type,),  # noqa: E501
-            'error': ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type,),  # noqa: E501
-            'details': ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},),  # noqa: E501
+            'city': (str,),  # noqa: E501
+            'components': ([str],),  # noqa: E501
+            'country': (str,),  # noqa: E501
+            'house_number': (str,),  # noqa: E501
+            'postal_code': (str,),  # noqa: E501
+            'street': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'status': 'status',  # noqa: E501
-        'info': 'info',  # noqa: E501
-        'error': 'error',  # noqa: E501
-        'details': 'details',  # noqa: E501
+        'city': 'city',  # noqa: E501
+        'components': 'components',  # noqa: E501
+        'country': 'country',  # noqa: E501
+        'house_number': 'houseNumber',  # noqa: E501
+        'postal_code': 'postalCode',  # noqa: E501
+        'street': 'street',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """InlineResponse200 - a model defined in OpenAPI
+    def _from_openapi_data(cls, city, components, country, house_number, postal_code, street, *args, **kwargs):  # noqa: E501
+        """StructuredAddressClass - a model defined in OpenAPI
+
+        Args:
+            city (str): City of the address.
+            components ([str]): List of broken down address components.
+            country (str): Country of the address.
+            house_number (str): House number of the address.
+            postal_code (str): Postal code of the address.
+            street (str): Street of the address.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,18 +149,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
-            info ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type): [optional]  # noqa: E501
-            error ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type): [optional]  # noqa: E501
-            details ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -172,14 +180,20 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.city = city
+        self.components = components
+        self.country = country
+        self.house_number = house_number
+        self.postal_code = postal_code
+        self.street = street
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,16 +206,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """InlineResponse200 - a model defined in OpenAPI
+    def __init__(self, city, components, country, house_number, postal_code, street, *args, **kwargs):  # noqa: E501
+        """StructuredAddressClass - a model defined in OpenAPI
+
+        Args:
+            city (str): City of the address.
+            components ([str]): List of broken down address components.
+            country (str): Country of the address.
+            house_number (str): House number of the address.
+            postal_code (str): Postal code of the address.
+            street (str): Street of the address.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,18 +248,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
-            info ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type): [optional]  # noqa: E501
-            error ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type): [optional]  # noqa: E501
-            details ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -259,14 +277,20 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.city = city
+        self.components = components
+        self.country = country
+        self.house_number = house_number
+        self.postal_code = postal_code
+        self.street = street
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/inline_response503.py` & `eis-publicapi-1.6.0/eis/publicapi/model/payment_method_class.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class InlineResponse503(ModelNormal):
+class PaymentMethodClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,56 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'status': (str,),  # noqa: E501
-            'info': ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type,),  # noqa: E501
-            'error': ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type,),  # noqa: E501
-            'details': ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},),  # noqa: E501
+            'id': (float,),  # noqa: E501
+            'code': (str,),  # noqa: E501
+            'provider_token': (str,),  # noqa: E501
+            'psp_customer_id': (str,),  # noqa: E501
+            'psp': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'status': 'status',  # noqa: E501
-        'info': 'info',  # noqa: E501
-        'error': 'error',  # noqa: E501
-        'details': 'details',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'code': 'code',  # noqa: E501
+        'provider_token': 'providerToken',  # noqa: E501
+        'psp_customer_id': 'pspCustomerId',  # noqa: E501
+        'psp': 'psp',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """InlineResponse503 - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, code, provider_token, psp_customer_id, psp, type, created_at, *args, **kwargs):  # noqa: E501
+        """PaymentMethodClass - a model defined in OpenAPI
+
+        Args:
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            code (str): Unique identifier for the object.
+            provider_token (str): A unique identifier generated by the payment service provider for this payment method.
+            psp_customer_id (str): Customer identifier for the payment service provider.
+            psp (str): The payment service provider used by this payment method.
+            type (str): The payment method type.
+            created_at (datetime): Time at which the object was created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,18 +152,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
-            info ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type): [optional]  # noqa: E501
-            error ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type): [optional]  # noqa: E501
-            details ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -172,14 +183,21 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.code = code
+        self.provider_token = provider_token
+        self.psp_customer_id = psp_customer_id
+        self.psp = psp
+        self.type = type
+        self.created_at = created_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,16 +210,25 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """InlineResponse503 - a model defined in OpenAPI
+    def __init__(self, id, code, provider_token, psp_customer_id, psp, type, created_at, *args, **kwargs):  # noqa: E501
+        """PaymentMethodClass - a model defined in OpenAPI
+
+        Args:
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            code (str): Unique identifier for the object.
+            provider_token (str): A unique identifier generated by the payment service provider for this payment method.
+            psp_customer_id (str): Customer identifier for the payment service provider.
+            psp (str): The payment service provider used by this payment method.
+            type (str): The payment method type.
+            created_at (datetime): Time at which the object was created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,18 +253,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
-            info ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type): [optional]  # noqa: E501
-            error ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}, none_type): [optional]  # noqa: E501
-            details ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -259,14 +282,21 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.code = code
+        self.provider_token = provider_token
+        self.psp_customer_id = psp_customer_id
+        self.psp = psp
+        self.type = type
+        self.created_at = created_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/insured_object_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/insured_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/insured_object_type_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/insured_object_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/invoice_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/invoice_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/invoice_item_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/invoice_item_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,14 @@
             'tax_rate': (float,),  # noqa: E501
             'net_amount': (float,),  # noqa: E501
             'tax_amount': (float,),  # noqa: E501
             'gross_amount': (float,),  # noqa: E501
             'credit_amount': (float,),  # noqa: E501
             'billing_interval_from': (datetime,),  # noqa: E501
             'billing_interval_to': (datetime,),  # noqa: E501
-            'item_type': (str,),  # noqa: E501
-            'visibility': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -118,16 +116,14 @@
         'tax_rate': 'taxRate',  # noqa: E501
         'net_amount': 'netAmount',  # noqa: E501
         'tax_amount': 'taxAmount',  # noqa: E501
         'gross_amount': 'grossAmount',  # noqa: E501
         'credit_amount': 'creditAmount',  # noqa: E501
         'billing_interval_from': 'billingIntervalFrom',  # noqa: E501
         'billing_interval_to': 'billingIntervalTo',  # noqa: E501
-        'item_type': 'itemType',  # noqa: E501
-        'visibility': 'visibility',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -180,16 +176,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            item_type (str): Type of Premium item.. [optional]  # noqa: E501
-            visibility (str): Visibility of Premium item.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -299,16 +293,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            item_type (str): Type of Premium item.. [optional]  # noqa: E501
-            visibility (str): Visibility of Premium item.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/invoice_status_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/product_factor_class.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class InvoiceStatusClass(ModelNormal):
+class ProductFactorClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -79,46 +79,55 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'id': (float,),  # noqa: E501
-            'invoice_id': (float,),  # noqa: E501
-            'status': (str,),  # noqa: E501
+            'product_version_id': (float,),  # noqa: E501
+            'group': (str,),  # noqa: E501
+            'label': (str,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
+            'updated_at': (datetime,),  # noqa: E501
+            'values': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'invoice_id': 'invoiceId',  # noqa: E501
-        'status': 'status',  # noqa: E501
+        'product_version_id': 'productVersionId',  # noqa: E501
+        'group': 'group',  # noqa: E501
+        'label': 'label',  # noqa: E501
         'created_at': 'createdAt',  # noqa: E501
+        'updated_at': 'updatedAt',  # noqa: E501
+        'values': 'values',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, invoice_id, status, created_at, *args, **kwargs):  # noqa: E501
-        """InvoiceStatusClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, product_version_id, group, label, created_at, updated_at, values, *args, **kwargs):  # noqa: E501
+        """ProductFactorClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            invoice_id (float): Unique identifier referencing the invoice.
-            status (str): Invoice type
+            product_version_id (float): Unique identifier referencing the version of the product on which this product factor is used.
+            group (str): Product factor group.
+            label (str): Product factor label.
             created_at (datetime): Time at which the object was created.
+            updated_at (datetime): Time at which the object was updated.
+            values ([str]): Factor values.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -175,17 +184,20 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
-        self.invoice_id = invoice_id
-        self.status = status
+        self.product_version_id = product_version_id
+        self.group = group
+        self.label = label
         self.created_at = created_at
+        self.updated_at = updated_at
+        self.values = values
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,22 +210,25 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, invoice_id, status, created_at, *args, **kwargs):  # noqa: E501
-        """InvoiceStatusClass - a model defined in OpenAPI
+    def __init__(self, id, product_version_id, group, label, created_at, updated_at, values, *args, **kwargs):  # noqa: E501
+        """ProductFactorClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            invoice_id (float): Unique identifier referencing the invoice.
-            status (str): Invoice type
+            product_version_id (float): Unique identifier referencing the version of the product on which this product factor is used.
+            group (str): Product factor group.
+            label (str): Product factor label.
             created_at (datetime): Time at which the object was created.
+            updated_at (datetime): Time at which the object was updated.
+            values ([str]): Factor values.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -268,17 +283,20 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
-        self.invoice_id = invoice_id
-        self.status = status
+        self.product_version_id = product_version_id
+        self.group = group
+        self.label = label
         self.created_at = created_at
+        self.updated_at = updated_at
+        self.values = values
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/lead_account_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/lead_account_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,18 +94,18 @@
             'last_name': (str,),  # noqa: E501
             'email': (str,),  # noqa: E501
             'gender': (str,),  # noqa: E501
             'street': (str,),  # noqa: E501
             'house_number': (str,),  # noqa: E501
             'zip_code': (str,),  # noqa: E501
             'city': (str,),  # noqa: E501
+            'phone': (str,),  # noqa: E501
             'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'birth_date': (datetime,),  # noqa: E501
             'custom_fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'phone': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -116,41 +116,42 @@
         'last_name': 'lastName',  # noqa: E501
         'email': 'email',  # noqa: E501
         'gender': 'gender',  # noqa: E501
         'street': 'street',  # noqa: E501
         'house_number': 'houseNumber',  # noqa: E501
         'zip_code': 'zipCode',  # noqa: E501
         'city': 'city',  # noqa: E501
+        'phone': 'phone',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'birth_date': 'birthDate',  # noqa: E501
         'custom_fields': 'customFields',  # noqa: E501
-        'phone': 'phone',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, account_number, title, first_name, last_name, email, gender, street, house_number, zip_code, city, metadata, birth_date, custom_fields, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, account_number, title, first_name, last_name, email, gender, street, house_number, zip_code, city, phone, metadata, birth_date, custom_fields, *args, **kwargs):  # noqa: E501
         """LeadAccountClass - a model defined in OpenAPI
 
         Args:
             account_number (str): Account number
             title (str): Account honorific title
             first_name (str): Account first name
             last_name (str): Account last name
             email (str): Account email
             gender (str): Account gender
             street (str): Account street
             house_number (str): Account house number
             zip_code (str): Account zip code
             city (str): Account city
+            phone (str): Account phone number
             metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Optional metadata.
             birth_date (datetime): Customer birth date.
             custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Custom fields could be included additional required/optional fields that the account would need for specific cases.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -178,15 +179,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone (str): Account phone number. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,14 +220,15 @@
         self.last_name = last_name
         self.email = email
         self.gender = gender
         self.street = street
         self.house_number = house_number
         self.zip_code = zip_code
         self.city = city
+        self.phone = phone
         self.metadata = metadata
         self.birth_date = birth_date
         self.custom_fields = custom_fields
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
@@ -243,28 +244,29 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, account_number, title, first_name, last_name, email, gender, street, house_number, zip_code, city, metadata, birth_date, custom_fields, *args, **kwargs):  # noqa: E501
+    def __init__(self, account_number, title, first_name, last_name, email, gender, street, house_number, zip_code, city, phone, metadata, birth_date, custom_fields, *args, **kwargs):  # noqa: E501
         """LeadAccountClass - a model defined in OpenAPI
 
         Args:
             account_number (str): Account number
             title (str): Account honorific title
             first_name (str): Account first name
             last_name (str): Account last name
             email (str): Account email
             gender (str): Account gender
             street (str): Account street
             house_number (str): Account house number
             zip_code (str): Account zip code
             city (str): Account city
+            phone (str): Account phone number
             metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Optional metadata.
             birth_date (datetime): Customer birth date.
             custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Custom fields could be included additional required/optional fields that the account would need for specific cases.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -292,15 +294,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone (str): Account phone number. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -332,14 +333,15 @@
         self.last_name = last_name
         self.email = email
         self.gender = gender
         self.street = street
         self.house_number = house_number
         self.zip_code = zip_code
         self.city = city
+        self.phone = phone
         self.metadata = metadata
         self.birth_date = birth_date
         self.custom_fields = custom_fields
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/lead_bank_account_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/list_products_response_class.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.publicapi.model.product_class import ProductClass
+    globals()['ProductClass'] = ProductClass
 
-class LeadBankAccountClass(ModelNormal):
+
+class ListProductsResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +67,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'account_code': (str,),  # noqa: E501
-            'iban': (str,),  # noqa: E501
+            'items': ([ProductClass],),  # noqa: E501
+            'next_page_token': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'account_code': 'accountCode',  # noqa: E501
-        'iban': 'iban',  # noqa: E501
+        'items': 'items',  # noqa: E501
+        'next_page_token': 'nextPageToken',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, account_code, iban, *args, **kwargs):  # noqa: E501
-        """LeadBankAccountClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
+        """ListProductsResponseClass - a model defined in OpenAPI
 
         Args:
-            account_code (str): Unique identifier of the account that this object belongs to.
-            iban (str): Bank account IBAN
+            items ([ProductClass]): List of products.
+            next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,16 +174,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.account_code = account_code
-        self.iban = iban
+        self.items = items
+        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +196,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, account_code, iban, *args, **kwargs):  # noqa: E501
-        """LeadBankAccountClass - a model defined in OpenAPI
+    def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
+        """ListProductsResponseClass - a model defined in OpenAPI
 
         Args:
-            account_code (str): Unique identifier of the account that this object belongs to.
-            iban (str): Bank account IBAN
+            items ([ProductClass]): List of products.
+            next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,16 +263,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.account_code = account_code
-        self.iban = iban
+        self.items = items
+        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/lead_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/lead_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,22 +27,20 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from eis.publicapi.model.create_payment_method_request_dto import CreatePaymentMethodRequestDto
     from eis.publicapi.model.invoice_class import InvoiceClass
     from eis.publicapi.model.lead_account_class import LeadAccountClass
     from eis.publicapi.model.lead_bank_account_class import LeadBankAccountClass
     from eis.publicapi.model.lead_policy_class import LeadPolicyClass
     from eis.publicapi.model.premium_override_dto import PremiumOverrideDto
     from eis.publicapi.model.uploaded_document_dto import UploadedDocumentDto
-    globals()['CreatePaymentMethodRequestDto'] = CreatePaymentMethodRequestDto
     globals()['InvoiceClass'] = InvoiceClass
     globals()['LeadAccountClass'] = LeadAccountClass
     globals()['LeadBankAccountClass'] = LeadBankAccountClass
     globals()['LeadPolicyClass'] = LeadPolicyClass
     globals()['PremiumOverrideDto'] = PremiumOverrideDto
     globals()['UploadedDocumentDto'] = UploadedDocumentDto
 
@@ -103,15 +101,14 @@
             'id': (float,),  # noqa: E501
             'code': (str,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'account': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'policy': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'quote': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'ern': (str,),  # noqa: E501
-            'payment_method': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'updated_at': (datetime,),  # noqa: E501
             'bank_account': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'premium_overrides': ([PremiumOverrideDto],),  # noqa: E501
             'uploaded_document': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'custom_data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
@@ -125,15 +122,14 @@
         'id': 'id',  # noqa: E501
         'code': 'code',  # noqa: E501
         'status': 'status',  # noqa: E501
         'account': 'account',  # noqa: E501
         'policy': 'policy',  # noqa: E501
         'quote': 'quote',  # noqa: E501
         'ern': 'ern',  # noqa: E501
-        'payment_method': 'paymentMethod',  # noqa: E501
         'created_at': 'createdAt',  # noqa: E501
         'updated_at': 'updatedAt',  # noqa: E501
         'bank_account': 'bankAccount',  # noqa: E501
         'premium_overrides': 'premiumOverrides',  # noqa: E501
         'uploaded_document': 'uploadedDocument',  # noqa: E501
         'custom_data': 'customData',  # noqa: E501
     }
@@ -141,26 +137,25 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, code, status, account, policy, quote, ern, payment_method, created_at, updated_at, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, code, status, account, policy, quote, ern, created_at, updated_at, *args, **kwargs):  # noqa: E501
         """LeadClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             code (str): Unique identifier for the object.
             status (str): Lead status
             account (bool, date, datetime, dict, float, int, list, str, none_type): Lead account
             policy (bool, date, datetime, dict, float, int, list, str, none_type): Lead policy
             quote (bool, date, datetime, dict, float, int, list, str, none_type): Quote or price details.
             ern (str): Emil Resources Names (ERN) identifies the most specific owner of a resource.
-            payment_method (bool, date, datetime, dict, float, int, list, str, none_type): Payment method. When a payment method is provided, it needs to be handled in the workflow based on its type.
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -229,15 +224,14 @@
         self.id = id
         self.code = code
         self.status = status
         self.account = account
         self.policy = policy
         self.quote = quote
         self.ern = ern
-        self.payment_method = payment_method
         self.created_at = created_at
         self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -252,26 +246,25 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, code, status, account, policy, quote, ern, payment_method, created_at, updated_at, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, code, status, account, policy, quote, ern, created_at, updated_at, *args, **kwargs):  # noqa: E501
         """LeadClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             code (str): Unique identifier for the object.
             status (str): Lead status
             account (bool, date, datetime, dict, float, int, list, str, none_type): Lead account
             policy (bool, date, datetime, dict, float, int, list, str, none_type): Lead policy
             quote (bool, date, datetime, dict, float, int, list, str, none_type): Quote or price details.
             ern (str): Emil Resources Names (ERN) identifies the most specific owner of a resource.
-            payment_method (bool, date, datetime, dict, float, int, list, str, none_type): Payment method. When a payment method is provided, it needs to be handled in the workflow based on its type.
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -338,15 +331,14 @@
         self.id = id
         self.code = code
         self.status = status
         self.account = account
         self.policy = policy
         self.quote = quote
         self.ern = ern
-        self.payment_method = payment_method
         self.created_at = created_at
         self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/lead_policy_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/lead_policy_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/lead_policy_object_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/send_notification_request_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
 
-class LeadPolicyObjectClass(ModelNormal):
+class SendNotificationRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,43 +78,42 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'insured_object_id': (float,),  # noqa: E501
-            'data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'insured_object_name': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'template_slug': (str,),  # noqa: E501
+            'email_subject': (str,),  # noqa: E501
+            'payload': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'insured_object_id': 'insuredObjectId',  # noqa: E501
-        'data': 'data',  # noqa: E501
-        'insured_object_name': 'insuredObjectName',  # noqa: E501
+        'template_slug': 'templateSlug',  # noqa: E501
+        'email_subject': 'emailSubject',  # noqa: E501
+        'payload': 'payload',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, insured_object_id, data, *args, **kwargs):  # noqa: E501
-        """LeadPolicyObjectClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, template_slug, *args, **kwargs):  # noqa: E501
+        """SendNotificationRequestDto - a model defined in OpenAPI
 
         Args:
-            insured_object_id (float): Unique identifier referencing the insured object.
-            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object data.
+            template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,15 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            insured_object_name ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object name.. [optional]  # noqa: E501
+            email_subject (str): Subject of the email.. [optional]  # noqa: E501
+            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Payload is used by the template engine to replace all template variables with proper data.      For more information, please go to https://github.com/flosch/pongo2.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,16 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.insured_object_id = insured_object_id
-        self.data = data
+        self.template_slug = template_slug
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,20 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, insured_object_id, data, *args, **kwargs):  # noqa: E501
-        """LeadPolicyObjectClass - a model defined in OpenAPI
+    def __init__(self, template_slug, *args, **kwargs):  # noqa: E501
+        """SendNotificationRequestDto - a model defined in OpenAPI
 
         Args:
-            insured_object_id (float): Unique identifier referencing the insured object.
-            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object data.
+            template_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -231,15 +229,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            insured_object_name ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object name.. [optional]  # noqa: E501
+            email_subject (str): Subject of the email.. [optional]  # noqa: E501
+            payload ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Payload is used by the template engine to replace all template variables with proper data.      For more information, please go to https://github.com/flosch/pongo2.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -261,16 +260,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.insured_object_id = insured_object_id
-        self.data = data
+        self.template_slug = template_slug
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/list_documents_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/premium_override_dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.publicapi.model.document_class import DocumentClass
-    globals()['DocumentClass'] = DocumentClass
 
-
-class ListDocumentsResponseClass(ModelNormal):
+class PremiumOverrideDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,71 +52,85 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('type',): {
+            'TIME': "time",
+        },
+        ('unit',): {
+            'DAY': "day",
+            'WEEK': "week",
+            'MONTH': "month",
+            'YEAR': "year",
+            'ONETIMEPAYMENT': "oneTimePayment",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'items': ([DocumentClass],),  # noqa: E501
-            'next_page_token': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'unit': (str,),  # noqa: E501
+            'net_premium': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'items': 'items',  # noqa: E501
-        'next_page_token': 'nextPageToken',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'unit': 'unit',  # noqa: E501
+        'net_premium': 'netPremium',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListDocumentsResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, unit, net_premium, *args, **kwargs):  # noqa: E501
+        """PremiumOverrideDto - a model defined in OpenAPI
 
         Args:
-            items ([DocumentClass]): The list of documents.
-            next_page_token (str): Next page token
+            name (str): Name of Premium.
+            unit (str): This is unit of Premium. Premium units are determined based on day, week, month and year.
+            net_premium (float):
 
         Keyword Args:
+            type (str): Type of Premium that is based on time.. defaults to "time", must be one of ["time", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,14 +155,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
+        type = kwargs.get('type', "time")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -174,16 +185,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.items = items
-        self.next_page_token = next_page_token
+        self.name = name
+        self.type = type
+        self.unit = unit
+        self.net_premium = net_premium
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,22 +209,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListDocumentsResponseClass - a model defined in OpenAPI
+    def __init__(self, name, unit, net_premium, *args, **kwargs):  # noqa: E501
+        """PremiumOverrideDto - a model defined in OpenAPI
 
         Args:
-            items ([DocumentClass]): The list of documents.
-            next_page_token (str): Next page token
+            name (str): Name of Premium.
+            unit (str): This is unit of Premium. Premium units are determined based on day, week, month and year.
+            net_premium (float):
 
         Keyword Args:
+            type (str): Type of Premium that is based on time.. defaults to "time", must be one of ["time", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -236,14 +251,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
+        type = kwargs.get('type', "time")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -263,16 +279,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.items = items
-        self.next_page_token = next_page_token
+        self.name = name
+        self.type = type
+        self.unit = unit
+        self.net_premium = net_premium
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/list_product_documents_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/suggested_address_details_class.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.publicapi.model.product_document_class import ProductDocumentClass
-    globals()['ProductDocumentClass'] = ProductDocumentClass
 
-
-class ListProductDocumentsResponseClass(ModelNormal):
+class SuggestedAddressDetailsClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,58 +63,83 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'items': ([ProductDocumentClass],),  # noqa: E501
-            'next_page_token': (str,),  # noqa: E501
+            'label': (str,),  # noqa: E501
+            'country_code': (str,),  # noqa: E501
+            'country_name': (str,),  # noqa: E501
+            'state_code': (str,),  # noqa: E501
+            'state': (str,),  # noqa: E501
+            'city': (str,),  # noqa: E501
+            'district': (str,),  # noqa: E501
+            'street': (str,),  # noqa: E501
+            'postal_code': (str,),  # noqa: E501
+            'county_code': (str,),  # noqa: E501
+            'county': (str,),  # noqa: E501
+            'house_number': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'items': 'items',  # noqa: E501
-        'next_page_token': 'nextPageToken',  # noqa: E501
+        'label': 'label',  # noqa: E501
+        'country_code': 'countryCode',  # noqa: E501
+        'country_name': 'countryName',  # noqa: E501
+        'state_code': 'stateCode',  # noqa: E501
+        'state': 'state',  # noqa: E501
+        'city': 'city',  # noqa: E501
+        'district': 'district',  # noqa: E501
+        'street': 'street',  # noqa: E501
+        'postal_code': 'postalCode',  # noqa: E501
+        'county_code': 'countyCode',  # noqa: E501
+        'county': 'county',  # noqa: E501
+        'house_number': 'houseNumber',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListProductDocumentsResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, label, country_code, country_name, state_code, state, city, district, street, postal_code, *args, **kwargs):  # noqa: E501
+        """SuggestedAddressDetailsClass - a model defined in OpenAPI
 
         Args:
-            items ([ProductDocumentClass]): The list of documents.
-            next_page_token (str): Next page token.
+            label (str):
+            country_code (str):
+            country_name (str):
+            state_code (str):
+            state (str):
+            city (str):
+            district (str):
+            street (str):
+            postal_code (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,14 +164,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            county_code (str): [optional]  # noqa: E501
+            county (str): [optional]  # noqa: E501
+            house_number (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -174,16 +198,23 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.items = items
-        self.next_page_token = next_page_token
+        self.label = label
+        self.country_code = country_code
+        self.country_name = country_name
+        self.state_code = state_code
+        self.state = state
+        self.city = city
+        self.district = district
+        self.street = street
+        self.postal_code = postal_code
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,20 +227,27 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListProductDocumentsResponseClass - a model defined in OpenAPI
+    def __init__(self, label, country_code, country_name, state_code, state, city, district, street, postal_code, *args, **kwargs):  # noqa: E501
+        """SuggestedAddressDetailsClass - a model defined in OpenAPI
 
         Args:
-            items ([ProductDocumentClass]): The list of documents.
-            next_page_token (str): Next page token.
+            label (str):
+            country_code (str):
+            country_name (str):
+            state_code (str):
+            state (str):
+            city (str):
+            district (str):
+            street (str):
+            postal_code (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -234,14 +272,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            county_code (str): [optional]  # noqa: E501
+            county (str): [optional]  # noqa: E501
+            house_number (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -263,16 +304,23 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.items = items
-        self.next_page_token = next_page_token
+        self.label = label
+        self.country_code = country_code
+        self.country_name = country_name
+        self.state_code = state_code
+        self.state = state
+        self.city = city
+        self.district = district
+        self.street = street
+        self.postal_code = postal_code
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/list_products_response_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/product_version_class.py`

 * *Files 27% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.publicapi.model.product_class import ProductClass
-    globals()['ProductClass'] = ProductClass
 
-
-class ListProductsResponseClass(ModelNormal):
+class ProductVersionClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,69 +52,85 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('status',): {
+            'DRAFT': "draft",
+            'ACTIVE': "active",
+            'PASSIVE': "passive",
+            'ARCHIVED': "archived",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'items': ([ProductClass],),  # noqa: E501
-            'next_page_token': (str,),  # noqa: E501
+            'id': (float,),  # noqa: E501
+            'product_id': (float,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'status': (str,),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
+            'updated_at': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'items': 'items',  # noqa: E501
-        'next_page_token': 'nextPageToken',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'product_id': 'productId',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
+        'updated_at': 'updatedAt',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListProductsResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, product_id, description, status, created_at, updated_at, *args, **kwargs):  # noqa: E501
+        """ProductVersionClass - a model defined in OpenAPI
 
         Args:
-            items ([ProductClass]): List of products.
-            next_page_token (str): Next page token.
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            product_id (float): Unique identifier referencing the product.
+            description (str): Product version description.
+            status (str): Product version status.
+            created_at (datetime): Time at which the object was created.
+            updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -174,16 +186,20 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.items = items
-        self.next_page_token = next_page_token
+        self.id = id
+        self.product_id = product_id
+        self.description = description
+        self.status = status
+        self.created_at = created_at
+        self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,20 +212,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListProductsResponseClass - a model defined in OpenAPI
+    def __init__(self, id, product_id, description, status, created_at, updated_at, *args, **kwargs):  # noqa: E501
+        """ProductVersionClass - a model defined in OpenAPI
 
         Args:
-            items ([ProductClass]): List of products.
-            next_page_token (str): Next page token.
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            product_id (float): Unique identifier referencing the product.
+            description (str): Product version description.
+            status (str): Product version status.
+            created_at (datetime): Time at which the object was created.
+            updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -263,16 +283,20 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.items = items
-        self.next_page_token = next_page_token
+        self.id = id
+        self.product_id = product_id
+        self.description = description
+        self.status = status
+        self.created_at = created_at
+        self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/payment_method_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/validate_address_response_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,16 +26,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.publicapi.model.address_field_score_class import AddressFieldScoreClass
+    from eis.publicapi.model.structured_address_class import StructuredAddressClass
+    globals()['AddressFieldScoreClass'] = AddressFieldScoreClass
+    globals()['StructuredAddressClass'] = StructuredAddressClass
 
-class PaymentMethodClass(ModelNormal):
+
+class ValidateAddressResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,71 +69,67 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (float,),  # noqa: E501
-            'code': (str,),  # noqa: E501
-            'provider_token': (str,),  # noqa: E501
-            'psp_customer_id': (str,),  # noqa: E501
-            'psp': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'created_at': (datetime,),  # noqa: E501
+            'errors': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'is_address_valid': (bool,),  # noqa: E501
+            'raw_address': (str,),  # noqa: E501
+            'score': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'structured_address': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'code': 'code',  # noqa: E501
-        'provider_token': 'providerToken',  # noqa: E501
-        'psp_customer_id': 'pspCustomerId',  # noqa: E501
-        'psp': 'psp',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'created_at': 'createdAt',  # noqa: E501
+        'errors': 'errors',  # noqa: E501
+        'is_address_valid': 'isAddressValid',  # noqa: E501
+        'raw_address': 'rawAddress',  # noqa: E501
+        'score': 'score',  # noqa: E501
+        'structured_address': 'structuredAddress',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, code, provider_token, psp_customer_id, psp, type, created_at, *args, **kwargs):  # noqa: E501
-        """PaymentMethodClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, errors, is_address_valid, raw_address, score, structured_address, *args, **kwargs):  # noqa: E501
+        """ValidateAddressResponseClass - a model defined in OpenAPI
 
         Args:
-            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            code (str): Unique identifier for the object.
-            provider_token (str): A unique identifier generated by the payment service provider for this payment method.
-            psp_customer_id (str): Customer identifier for the payment service provider.
-            psp (str): The payment service provider used by this payment method.
-            type (str): The payment method type.
-            created_at (datetime): Time at which the object was created.
+            errors ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The error object for address validation!
+            is_address_valid (bool): Indicates whether the address is valid or not!
+            raw_address (str): The input address in a single line
+            score (bool, date, datetime, dict, float, int, list, str, none_type): Individual score for various parts of the address
+            structured_address (bool, date, datetime, dict, float, int, list, str, none_type): The structured address object!
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -183,21 +185,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.code = code
-        self.provider_token = provider_token
-        self.psp_customer_id = psp_customer_id
-        self.psp = psp
-        self.type = type
-        self.created_at = created_at
+        self.errors = errors
+        self.is_address_valid = is_address_valid
+        self.raw_address = raw_address
+        self.score = score
+        self.structured_address = structured_address
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -210,25 +210,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, code, provider_token, psp_customer_id, psp, type, created_at, *args, **kwargs):  # noqa: E501
-        """PaymentMethodClass - a model defined in OpenAPI
+    def __init__(self, errors, is_address_valid, raw_address, score, structured_address, *args, **kwargs):  # noqa: E501
+        """ValidateAddressResponseClass - a model defined in OpenAPI
 
         Args:
-            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            code (str): Unique identifier for the object.
-            provider_token (str): A unique identifier generated by the payment service provider for this payment method.
-            psp_customer_id (str): Customer identifier for the payment service provider.
-            psp (str): The payment service provider used by this payment method.
-            type (str): The payment method type.
-            created_at (datetime): Time at which the object was created.
+            errors ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The error object for address validation!
+            is_address_valid (bool): Indicates whether the address is valid or not!
+            raw_address (str): The input address in a single line
+            score (bool, date, datetime, dict, float, int, list, str, none_type): Individual score for various parts of the address
+            structured_address (bool, date, datetime, dict, float, int, list, str, none_type): The structured address object!
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -282,21 +280,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.code = code
-        self.provider_token = provider_token
-        self.psp_customer_id = psp_customer_id
-        self.psp = psp
-        self.type = type
-        self.created_at = created_at
+        self.errors = errors
+        self.is_address_valid = is_address_valid
+        self.raw_address = raw_address
+        self.score = score
+        self.structured_address = structured_address
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/policy_object_request_dto.py` & `eis-publicapi-1.6.0/eis/publicapi/model/product_class.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,16 +26,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.publicapi.model.insured_object_type_class import InsuredObjectTypeClass
+    from eis.publicapi.model.product_version_class import ProductVersionClass
+    globals()['InsuredObjectTypeClass'] = InsuredObjectTypeClass
+    globals()['ProductVersionClass'] = ProductVersionClass
 
-class PolicyObjectRequestDto(ModelNormal):
+
+class ProductClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +69,79 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'insured_object_id': (float,),  # noqa: E501
-            'insured_object_name': (str,),  # noqa: E501
-            'data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'id': (float,),  # noqa: E501
             'code': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'slug': (str,),  # noqa: E501
+            'insured_object_types': ([InsuredObjectTypeClass],),  # noqa: E501
+            'contract_duration_days': (float,),  # noqa: E501
+            'versions': ([ProductVersionClass],),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
+            'updated_at': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'insured_object_id': 'insuredObjectId',  # noqa: E501
-        'insured_object_name': 'insuredObjectName',  # noqa: E501
-        'data': 'data',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'code': 'code',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'slug': 'slug',  # noqa: E501
+        'insured_object_types': 'insuredObjectTypes',  # noqa: E501
+        'contract_duration_days': 'contractDurationDays',  # noqa: E501
+        'versions': 'versions',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
+        'updated_at': 'updatedAt',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PolicyObjectRequestDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, code, name, slug, insured_object_types, contract_duration_days, versions, created_at, updated_at, *args, **kwargs):  # noqa: E501
+        """ProductClass - a model defined in OpenAPI
+
+        Args:
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            code (str): Unique identifier for the object.
+            name (str): Product's name.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
+            insured_object_types ([InsuredObjectTypeClass]): Insured object types covered under product.
+            contract_duration_days (float): Contract duration in days.
+            versions ([ProductVersionClass]): Product versions.
+            created_at (datetime): Time at which the object was created.
+            updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,18 +166,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            insured_object_id (float): The id of the insured object to be used in the policy.     The insured object id will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            insured_object_name (str): Insured object name. Human readable identifier of insured object.       Can be used instead of insuredObjectId. [optional]  # noqa: E501
-            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object data.     The date will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            code (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -172,14 +197,23 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.code = code
+        self.name = name
+        self.slug = slug
+        self.insured_object_types = insured_object_types
+        self.contract_duration_days = contract_duration_days
+        self.versions = versions
+        self.created_at = created_at
+        self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,16 +226,27 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """PolicyObjectRequestDto - a model defined in OpenAPI
+    def __init__(self, id, code, name, slug, insured_object_types, contract_duration_days, versions, created_at, updated_at, *args, **kwargs):  # noqa: E501
+        """ProductClass - a model defined in OpenAPI
+
+        Args:
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            code (str): Unique identifier for the object.
+            name (str): Product's name.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
+            insured_object_types ([InsuredObjectTypeClass]): Insured object types covered under product.
+            contract_duration_days (float): Contract duration in days.
+            versions ([ProductVersionClass]): Product versions.
+            created_at (datetime): Time at which the object was created.
+            updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,18 +271,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            insured_object_id (float): The id of the insured object to be used in the policy.     The insured object id will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            insured_object_name (str): Insured object name. Human readable identifier of insured object.       Can be used instead of insuredObjectId. [optional]  # noqa: E501
-            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Insured object data.     The date will be validated if the 'validate' flag is set to true.. [optional]  # noqa: E501
-            code (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -259,14 +300,23 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.code = code
+        self.name = name
+        self.slug = slug
+        self.insured_object_types = insured_object_types
+        self.contract_duration_days = contract_duration_days
+        self.versions = versions
+        self.created_at = created_at
+        self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/product_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/product_document_class.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,22 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.publicapi.model.insured_object_type_class import InsuredObjectTypeClass
-    from eis.publicapi.model.product_version_class import ProductVersionClass
-    globals()['InsuredObjectTypeClass'] = InsuredObjectTypeClass
-    globals()['ProductVersionClass'] = ProductVersionClass
 
-
-class ProductClass(ModelNormal):
+class ProductDocumentClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,93 +52,103 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('content_type',): {
+            'PDF': "pdf",
+            'JPG': "jpg",
+            'PNG': "png",
+            'GZ': "gz",
+            'CSV': "csv",
+            'DOC': "doc",
+            'DOCX': "docx",
+            'HTML': "html",
+            'JSON': "json",
+            'XML': "xml",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'id': (float,),  # noqa: E501
             'code': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'slug': (str,),  # noqa: E501
-            'insured_object_types': ([InsuredObjectTypeClass],),  # noqa: E501
-            'contract_duration_days': (float,),  # noqa: E501
-            'versions': ([ProductVersionClass],),  # noqa: E501
+            'product_code': (str,),  # noqa: E501
+            'product_version_id': (float,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            's3_key': (str,),  # noqa: E501
+            'content_type': (str,),  # noqa: E501
+            'product_slug': (str,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
-            'updated_at': (datetime,),  # noqa: E501
-            'default_language': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'code': 'code',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'slug': 'slug',  # noqa: E501
-        'insured_object_types': 'insuredObjectTypes',  # noqa: E501
-        'contract_duration_days': 'contractDurationDays',  # noqa: E501
-        'versions': 'versions',  # noqa: E501
+        'product_code': 'productCode',  # noqa: E501
+        'product_version_id': 'productVersionId',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        's3_key': 's3Key',  # noqa: E501
+        'content_type': 'contentType',  # noqa: E501
+        'product_slug': 'productSlug',  # noqa: E501
         'created_at': 'createdAt',  # noqa: E501
-        'updated_at': 'updatedAt',  # noqa: E501
-        'default_language': 'defaultLanguage',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, code, name, slug, insured_object_types, contract_duration_days, versions, created_at, updated_at, default_language, *args, **kwargs):  # noqa: E501
-        """ProductClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, code, product_code, product_version_id, type, description, s3_key, content_type, product_slug, created_at, *args, **kwargs):  # noqa: E501
+        """ProductDocumentClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             code (str): Unique identifier for the object.
-            name (str): Product's name.
-            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            insured_object_types ([InsuredObjectTypeClass]): Insured object types covered under product.
-            contract_duration_days (float): Contract duration in days.
-            versions ([ProductVersionClass]): Product versions.
+            product_code (str): Unique identifier for the object.
+            product_version_id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            type (str):
+            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
+            s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
+            content_type (str): Type of the document expressed with its file extension.
+            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
             created_at (datetime): Time at which the object was created.
-            updated_at (datetime): Time at which the object was updated.
-            default_language (str): Default language of the product.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -202,22 +206,22 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.code = code
-        self.name = name
-        self.slug = slug
-        self.insured_object_types = insured_object_types
-        self.contract_duration_days = contract_duration_days
-        self.versions = versions
+        self.product_code = product_code
+        self.product_version_id = product_version_id
+        self.type = type
+        self.description = description
+        self.s3_key = s3_key
+        self.content_type = content_type
+        self.product_slug = product_slug
         self.created_at = created_at
-        self.updated_at = updated_at
-        self.default_language = default_language
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -230,28 +234,28 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, code, name, slug, insured_object_types, contract_duration_days, versions, created_at, updated_at, default_language, *args, **kwargs):  # noqa: E501
-        """ProductClass - a model defined in OpenAPI
+    def __init__(self, id, code, product_code, product_version_id, type, description, s3_key, content_type, product_slug, created_at, *args, **kwargs):  # noqa: E501
+        """ProductDocumentClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             code (str): Unique identifier for the object.
-            name (str): Product's name.
-            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            insured_object_types ([InsuredObjectTypeClass]): Insured object types covered under product.
-            contract_duration_days (float): Contract duration in days.
-            versions ([ProductVersionClass]): Product versions.
+            product_code (str): Unique identifier for the object.
+            product_version_id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            type (str):
+            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
+            s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
+            content_type (str): Type of the document expressed with its file extension.
+            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
             created_at (datetime): Time at which the object was created.
-            updated_at (datetime): Time at which the object was updated.
-            default_language (str): Default language of the product.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -307,22 +311,22 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.code = code
-        self.name = name
-        self.slug = slug
-        self.insured_object_types = insured_object_types
-        self.contract_duration_days = contract_duration_days
-        self.versions = versions
+        self.product_code = product_code
+        self.product_version_id = product_version_id
+        self.type = type
+        self.description = description
+        self.s3_key = s3_key
+        self.content_type = content_type
+        self.product_slug = product_slug
         self.created_at = created_at
-        self.updated_at = updated_at
-        self.default_language = default_language
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model/product_document_class.py` & `eis-publicapi-1.6.0/eis/publicapi/model/create_lead_request_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,16 +26,28 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.publicapi.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.publicapi.model.create_account_request_dto import CreateAccountRequestDto
+    from eis.publicapi.model.create_bank_account_request_dto import CreateBankAccountRequestDto
+    from eis.publicapi.model.policy_object_request_dto import PolicyObjectRequestDto
+    from eis.publicapi.model.premium_override_request_dto import PremiumOverrideRequestDto
+    from eis.publicapi.model.uploaded_document_dto import UploadedDocumentDto
+    globals()['CreateAccountRequestDto'] = CreateAccountRequestDto
+    globals()['CreateBankAccountRequestDto'] = CreateBankAccountRequestDto
+    globals()['PolicyObjectRequestDto'] = PolicyObjectRequestDto
+    globals()['PremiumOverrideRequestDto'] = PremiumOverrideRequestDto
+    globals()['UploadedDocumentDto'] = UploadedDocumentDto
 
-class ProductDocumentClass(ModelNormal):
+
+class CreateLeadRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,117 +64,87 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('content_type',): {
-            'PDF': "pdf",
-            'JPG': "jpg",
-            'PNG': "png",
-            'GZ': "gz",
-            'CSV': "csv",
-            'DOC': "doc",
-            'DOCX': "docx",
-            'HTML': "html",
-            'JSON': "json",
-            'XML': "xml",
-            'TXT': "txt",
-            'ZIP': "zip",
-            'TAR': "tar",
-            'RAR': "rar",
-            'MP4': "MP4",
-            'MOV': "MOV",
-            'WMV': "WMV",
-            'AVI': "AVI",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (float,),  # noqa: E501
-            'code': (str,),  # noqa: E501
             'product_code': (str,),  # noqa: E501
+            'policy_objects': ([PolicyObjectRequestDto],),  # noqa: E501
+            'code': (str,),  # noqa: E501
             'product_version_id': (float,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
-            's3_key': (str,),  # noqa: E501
-            'content_type': (str,),  # noqa: E501
-            'product_slug': (str,),  # noqa: E501
-            'slug': (str,),  # noqa: E501
-            'version_number': (float,),  # noqa: E501
-            'created_at': (datetime,),  # noqa: E501
+            'account': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'account_code': (str,),  # noqa: E501
+            'bank_account': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'custom_data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'uploaded_document': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'status': (str,),  # noqa: E501
+            'premium_override': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'code': 'code',  # noqa: E501
         'product_code': 'productCode',  # noqa: E501
+        'policy_objects': 'policyObjects',  # noqa: E501
+        'code': 'code',  # noqa: E501
         'product_version_id': 'productVersionId',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        's3_key': 's3Key',  # noqa: E501
-        'content_type': 'contentType',  # noqa: E501
-        'product_slug': 'productSlug',  # noqa: E501
-        'slug': 'slug',  # noqa: E501
-        'version_number': 'versionNumber',  # noqa: E501
-        'created_at': 'createdAt',  # noqa: E501
+        'account': 'account',  # noqa: E501
+        'account_code': 'accountCode',  # noqa: E501
+        'bank_account': 'bankAccount',  # noqa: E501
+        'custom_data': 'customData',  # noqa: E501
+        'uploaded_document': 'uploadedDocument',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'premium_override': 'premiumOverride',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, code, product_code, product_version_id, type, description, s3_key, content_type, product_slug, slug, version_number, created_at, *args, **kwargs):  # noqa: E501
-        """ProductDocumentClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, product_code, policy_objects, *args, **kwargs):  # noqa: E501
+        """CreateLeadRequestDto - a model defined in OpenAPI
 
         Args:
-            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            code (str): Unique identifier for the object.
-            product_code (str): Unique identifier for the object.
-            product_version_id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            type (str):
-            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
-            s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
-            content_type (str): Type of the document expressed with its file extension.
-            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            version_number (float): Version number of the document, incremented each time the document is updated.
-            created_at (datetime): Time at which the object was created.
+            product_code (str): Unique identifier of the product that this object belongs to.
+            policy_objects ([PolicyObjectRequestDto]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -187,14 +169,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            code (str): Unique identifier for the object.. [optional]  # noqa: E501
+            product_version_id (float): Unique identifier referencing the product version.. [optional]  # noqa: E501
+            account (bool, date, datetime, dict, float, int, list, str, none_type): Account. The create lead request should either contain accountCode or account.. [optional]  # noqa: E501
+            account_code (str): Account code. The create lead request should either contain accountCode or account.. [optional]  # noqa: E501
+            bank_account (bool, date, datetime, dict, float, int, list, str, none_type): Bank account details.. [optional]  # noqa: E501
+            custom_data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Custom data.. [optional]  # noqa: E501
+            uploaded_document (bool, date, datetime, dict, float, int, list, str, none_type): Codes for documents to be uploaded.. [optional]  # noqa: E501
+            status (str): Lead status. Default values are \"created\", \"approved\" and \"declined\". However, those can be extended using /lead-statuses endpoint from insuranceservice.. [optional]  # noqa: E501
+            premium_override (bool, date, datetime, dict, float, int, list, str, none_type): Premium Override.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -218,26 +209,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.code = code
         self.product_code = product_code
-        self.product_version_id = product_version_id
-        self.type = type
-        self.description = description
-        self.s3_key = s3_key
-        self.content_type = content_type
-        self.product_slug = product_slug
-        self.slug = slug
-        self.version_number = version_number
-        self.created_at = created_at
+        self.policy_objects = policy_objects
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -250,30 +231,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, code, product_code, product_version_id, type, description, s3_key, content_type, product_slug, slug, version_number, created_at, *args, **kwargs):  # noqa: E501
-        """ProductDocumentClass - a model defined in OpenAPI
+    def __init__(self, product_code, policy_objects, *args, **kwargs):  # noqa: E501
+        """CreateLeadRequestDto - a model defined in OpenAPI
 
         Args:
-            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            code (str): Unique identifier for the object.
-            product_code (str): Unique identifier for the object.
-            product_version_id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
-            type (str):
-            description (str): Description of the document. Usually a short summary about the      context in which the document is being used.
-            s3_key (str): The unique key used by Amazon Simple Storage Service (S3).
-            content_type (str): Type of the document expressed with its file extension.
-            product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
-            version_number (float): Version number of the document, incremented each time the document is updated.
-            created_at (datetime): Time at which the object was created.
+            product_code (str): Unique identifier of the product that this object belongs to.
+            policy_objects ([PolicyObjectRequestDto]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -298,14 +269,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            code (str): Unique identifier for the object.. [optional]  # noqa: E501
+            product_version_id (float): Unique identifier referencing the product version.. [optional]  # noqa: E501
+            account (bool, date, datetime, dict, float, int, list, str, none_type): Account. The create lead request should either contain accountCode or account.. [optional]  # noqa: E501
+            account_code (str): Account code. The create lead request should either contain accountCode or account.. [optional]  # noqa: E501
+            bank_account (bool, date, datetime, dict, float, int, list, str, none_type): Bank account details.. [optional]  # noqa: E501
+            custom_data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Custom data.. [optional]  # noqa: E501
+            uploaded_document (bool, date, datetime, dict, float, int, list, str, none_type): Codes for documents to be uploaded.. [optional]  # noqa: E501
+            status (str): Lead status. Default values are \"created\", \"approved\" and \"declined\". However, those can be extended using /lead-statuses endpoint from insuranceservice.. [optional]  # noqa: E501
+            premium_override (bool, date, datetime, dict, float, int, list, str, none_type): Premium Override.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -327,26 +307,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.code = code
         self.product_code = product_code
-        self.product_version_id = product_version_id
-        self.type = type
-        self.description = description
-        self.s3_key = s3_key
-        self.content_type = content_type
-        self.product_slug = product_slug
-        self.slug = slug
-        self.version_number = version_number
-        self.created_at = created_at
+        self.policy_objects = policy_objects
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/model_utils.py` & `eis-publicapi-1.6.0/eis/publicapi/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1569,20 +1569,14 @@
 
     Raises:
         ApiTypeError
     """
     results = get_required_type_classes(required_types_mixed, spec_property_naming)
     valid_classes, child_req_types_by_current_type = results
 
-    # Extend the list of valid classes with the list of child types
-    # Required to correctly handle not-empty JsonValue properties
-    child_types = list(child_req_types_by_current_type.values())
-    if len(child_types) == 1:
-        valid_classes = tuple(list(valid_classes) + list(child_types[0]))
-
     input_class_simple = get_simple_class(input_value)
     valid_type = is_valid_type(input_class_simple, valid_classes)
     if not valid_type:
         if (configuration
                 or (input_class_simple == dict
                     and dict not in valid_classes)):
             # if input_value is not valid_type try to convert it
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/models/__init__.py` & `eis-publicapi-1.6.0/eis/publicapi/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,51 +8,38 @@
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from eis.publicapi.model.address_completion_item_class import AddressCompletionItemClass
 from eis.publicapi.model.address_completion_response_class import AddressCompletionResponseClass
 from eis.publicapi.model.address_field_score_class import AddressFieldScoreClass
-from eis.publicapi.model.calculate_product_fields_request_dto import CalculateProductFieldsRequestDto
-from eis.publicapi.model.calculate_product_fields_response_class import CalculateProductFieldsResponseClass
 from eis.publicapi.model.complete_braintree_payment_setup_request_dto import CompleteBraintreePaymentSetupRequestDto
-from eis.publicapi.model.complete_email_verification_dto import CompleteEmailVerificationDto
-from eis.publicapi.model.complete_email_verification_response_class import CompleteEmailVerificationResponseClass
 from eis.publicapi.model.complete_payment_setup_request_dto import CompletePaymentSetupRequestDto
 from eis.publicapi.model.complete_payment_setup_response_class import CompletePaymentSetupResponseClass
 from eis.publicapi.model.complete_stripe_payment_setup_request_dto import CompleteStripePaymentSetupRequestDto
 from eis.publicapi.model.create_account_request_dto import CreateAccountRequestDto
 from eis.publicapi.model.create_bank_account_request_dto import CreateBankAccountRequestDto
 from eis.publicapi.model.create_custom_application_request_dto import CreateCustomApplicationRequestDto
 from eis.publicapi.model.create_custom_application_response_class import CreateCustomApplicationResponseClass
 from eis.publicapi.model.create_document_request_dto import CreateDocumentRequestDto
 from eis.publicapi.model.create_estimated_invoice_request_dto import CreateEstimatedInvoiceRequestDto
 from eis.publicapi.model.create_estimated_invoice_response_class import CreateEstimatedInvoiceResponseClass
-from eis.publicapi.model.create_lead_async_response_class import CreateLeadAsyncResponseClass
 from eis.publicapi.model.create_lead_request_dto import CreateLeadRequestDto
 from eis.publicapi.model.create_lead_response_class import CreateLeadResponseClass
-from eis.publicapi.model.create_payment_method_request_dto import CreatePaymentMethodRequestDto
-from eis.publicapi.model.create_presigned_post_request_dto import CreatePresignedPostRequestDto
-from eis.publicapi.model.create_presigned_post_response_class import CreatePresignedPostResponseClass
 from eis.publicapi.model.document_class import DocumentClass
 from eis.publicapi.model.get_custom_css_response_class import GetCustomCssResponseClass
 from eis.publicapi.model.get_lead_response_class import GetLeadResponseClass
-from eis.publicapi.model.get_product_document_download_url_response_class import GetProductDocumentDownloadUrlResponseClass
 from eis.publicapi.model.get_public_psp_settings_response_class import GetPublicPspSettingsResponseClass
 from eis.publicapi.model.initiate_braintree_payment_setup_request_dto import InitiateBraintreePaymentSetupRequestDto
 from eis.publicapi.model.initiate_braintree_payment_setup_response_class import InitiateBraintreePaymentSetupResponseClass
-from eis.publicapi.model.initiate_email_verification_dto import InitiateEmailVerificationDto
-from eis.publicapi.model.initiate_email_verification_response_class import InitiateEmailVerificationResponseClass
 from eis.publicapi.model.initiate_lead_response_class import InitiateLeadResponseClass
 from eis.publicapi.model.initiate_payment_setup_request_dto import InitiatePaymentSetupRequestDto
 from eis.publicapi.model.initiate_payment_setup_response_class import InitiatePaymentSetupResponseClass
 from eis.publicapi.model.initiate_stripe_payment_setup_request_dto import InitiateStripePaymentSetupRequestDto
 from eis.publicapi.model.initiate_stripe_payment_setup_response_class import InitiateStripePaymentSetupResponseClass
-from eis.publicapi.model.inline_response200 import InlineResponse200
-from eis.publicapi.model.inline_response503 import InlineResponse503
 from eis.publicapi.model.insured_object_class import InsuredObjectClass
 from eis.publicapi.model.insured_object_type_class import InsuredObjectTypeClass
 from eis.publicapi.model.invoice_class import InvoiceClass
 from eis.publicapi.model.invoice_item_class import InvoiceItemClass
 from eis.publicapi.model.invoice_status_class import InvoiceStatusClass
 from eis.publicapi.model.lead_account_class import LeadAccountClass
 from eis.publicapi.model.lead_bank_account_class import LeadBankAccountClass
@@ -60,24 +47,22 @@
 from eis.publicapi.model.lead_policy_class import LeadPolicyClass
 from eis.publicapi.model.lead_policy_object_class import LeadPolicyObjectClass
 from eis.publicapi.model.list_documents_response_class import ListDocumentsResponseClass
 from eis.publicapi.model.list_product_documents_response_class import ListProductDocumentsResponseClass
 from eis.publicapi.model.list_products_response_class import ListProductsResponseClass
 from eis.publicapi.model.payment_method_class import PaymentMethodClass
 from eis.publicapi.model.policy_object_request_dto import PolicyObjectRequestDto
-from eis.publicapi.model.policy_object_response_class import PolicyObjectResponseClass
 from eis.publicapi.model.premium_override_dto import PremiumOverrideDto
 from eis.publicapi.model.premium_override_request_dto import PremiumOverrideRequestDto
 from eis.publicapi.model.product_class import ProductClass
 from eis.publicapi.model.product_document_class import ProductDocumentClass
-from eis.publicapi.model.product_factor_for_version_class import ProductFactorForVersionClass
+from eis.publicapi.model.product_factor_class import ProductFactorClass
 from eis.publicapi.model.product_field_class import ProductFieldClass
 from eis.publicapi.model.product_version_class import ProductVersionClass
 from eis.publicapi.model.send_notification_request_dto import SendNotificationRequestDto
 from eis.publicapi.model.send_notification_response_class import SendNotificationResponseClass
-from eis.publicapi.model.sepa_dto import SepaDto
 from eis.publicapi.model.structured_address_class import StructuredAddressClass
 from eis.publicapi.model.suggested_address_details_class import SuggestedAddressDetailsClass
 from eis.publicapi.model.update_lead_request_dto import UpdateLeadRequestDto
 from eis.publicapi.model.update_lead_response_class import UpdateLeadResponseClass
 from eis.publicapi.model.uploaded_document_dto import UploadedDocumentDto
 from eis.publicapi.model.validate_address_response_class import ValidateAddressResponseClass
```

### Comparing `eis-publicapi-1.22.1/eis/publicapi/rest.py` & `eis-publicapi-1.6.0/eis/publicapi/rest.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/eis_publicapi.egg-info/SOURCES.txt` & `eis-publicapi-1.6.0/eis_publicapi.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,62 +6,48 @@
 eis/publicapi/api_client.py
 eis/publicapi/configuration.py
 eis/publicapi/exceptions.py
 eis/publicapi/model_utils.py
 eis/publicapi/rest.py
 eis/publicapi/api/__init__.py
 eis/publicapi/api/address_completions_validations_api.py
-eis/publicapi/api/default_api.py
 eis/publicapi/api/documents_api.py
 eis/publicapi/api/leads_api.py
 eis/publicapi/api/notifications_api.py
 eis/publicapi/api/payments_setup_api.py
 eis/publicapi/api/products_api.py
 eis/publicapi/apis/__init__.py
 eis/publicapi/model/__init__.py
 eis/publicapi/model/address_completion_item_class.py
 eis/publicapi/model/address_completion_response_class.py
 eis/publicapi/model/address_field_score_class.py
-eis/publicapi/model/calculate_product_fields_request_dto.py
-eis/publicapi/model/calculate_product_fields_response_class.py
 eis/publicapi/model/complete_braintree_payment_setup_request_dto.py
-eis/publicapi/model/complete_email_verification_dto.py
-eis/publicapi/model/complete_email_verification_response_class.py
 eis/publicapi/model/complete_payment_setup_request_dto.py
 eis/publicapi/model/complete_payment_setup_response_class.py
 eis/publicapi/model/complete_stripe_payment_setup_request_dto.py
 eis/publicapi/model/create_account_request_dto.py
 eis/publicapi/model/create_bank_account_request_dto.py
 eis/publicapi/model/create_custom_application_request_dto.py
 eis/publicapi/model/create_custom_application_response_class.py
 eis/publicapi/model/create_document_request_dto.py
 eis/publicapi/model/create_estimated_invoice_request_dto.py
 eis/publicapi/model/create_estimated_invoice_response_class.py
-eis/publicapi/model/create_lead_async_response_class.py
 eis/publicapi/model/create_lead_request_dto.py
 eis/publicapi/model/create_lead_response_class.py
-eis/publicapi/model/create_payment_method_request_dto.py
-eis/publicapi/model/create_presigned_post_request_dto.py
-eis/publicapi/model/create_presigned_post_response_class.py
 eis/publicapi/model/document_class.py
 eis/publicapi/model/get_custom_css_response_class.py
 eis/publicapi/model/get_lead_response_class.py
-eis/publicapi/model/get_product_document_download_url_response_class.py
 eis/publicapi/model/get_public_psp_settings_response_class.py
 eis/publicapi/model/initiate_braintree_payment_setup_request_dto.py
 eis/publicapi/model/initiate_braintree_payment_setup_response_class.py
-eis/publicapi/model/initiate_email_verification_dto.py
-eis/publicapi/model/initiate_email_verification_response_class.py
 eis/publicapi/model/initiate_lead_response_class.py
 eis/publicapi/model/initiate_payment_setup_request_dto.py
 eis/publicapi/model/initiate_payment_setup_response_class.py
 eis/publicapi/model/initiate_stripe_payment_setup_request_dto.py
 eis/publicapi/model/initiate_stripe_payment_setup_response_class.py
-eis/publicapi/model/inline_response200.py
-eis/publicapi/model/inline_response503.py
 eis/publicapi/model/insured_object_class.py
 eis/publicapi/model/insured_object_type_class.py
 eis/publicapi/model/invoice_class.py
 eis/publicapi/model/invoice_item_class.py
 eis/publicapi/model/invoice_status_class.py
 eis/publicapi/model/lead_account_class.py
 eis/publicapi/model/lead_bank_account_class.py
@@ -69,25 +55,23 @@
 eis/publicapi/model/lead_policy_class.py
 eis/publicapi/model/lead_policy_object_class.py
 eis/publicapi/model/list_documents_response_class.py
 eis/publicapi/model/list_product_documents_response_class.py
 eis/publicapi/model/list_products_response_class.py
 eis/publicapi/model/payment_method_class.py
 eis/publicapi/model/policy_object_request_dto.py
-eis/publicapi/model/policy_object_response_class.py
 eis/publicapi/model/premium_override_dto.py
 eis/publicapi/model/premium_override_request_dto.py
 eis/publicapi/model/product_class.py
 eis/publicapi/model/product_document_class.py
-eis/publicapi/model/product_factor_for_version_class.py
+eis/publicapi/model/product_factor_class.py
 eis/publicapi/model/product_field_class.py
 eis/publicapi/model/product_version_class.py
 eis/publicapi/model/send_notification_request_dto.py
 eis/publicapi/model/send_notification_response_class.py
-eis/publicapi/model/sepa_dto.py
 eis/publicapi/model/structured_address_class.py
 eis/publicapi/model/suggested_address_details_class.py
 eis/publicapi/model/update_lead_request_dto.py
 eis/publicapi/model/update_lead_response_class.py
 eis/publicapi/model/uploaded_document_dto.py
 eis/publicapi/model/validate_address_response_class.py
 eis/publicapi/models/__init__.py
@@ -96,53 +80,39 @@
 eis_publicapi.egg-info/dependency_links.txt
 eis_publicapi.egg-info/requires.txt
 eis_publicapi.egg-info/top_level.txt
 test/test_address_completion_item_class.py
 test/test_address_completion_response_class.py
 test/test_address_completions_validations_api.py
 test/test_address_field_score_class.py
-test/test_calculate_product_fields_request_dto.py
-test/test_calculate_product_fields_response_class.py
 test/test_complete_braintree_payment_setup_request_dto.py
-test/test_complete_email_verification_dto.py
-test/test_complete_email_verification_response_class.py
 test/test_complete_payment_setup_request_dto.py
 test/test_complete_payment_setup_response_class.py
 test/test_complete_stripe_payment_setup_request_dto.py
 test/test_create_account_request_dto.py
 test/test_create_bank_account_request_dto.py
 test/test_create_custom_application_request_dto.py
 test/test_create_custom_application_response_class.py
 test/test_create_document_request_dto.py
 test/test_create_estimated_invoice_request_dto.py
 test/test_create_estimated_invoice_response_class.py
-test/test_create_lead_async_response_class.py
 test/test_create_lead_request_dto.py
 test/test_create_lead_response_class.py
-test/test_create_payment_method_request_dto.py
-test/test_create_presigned_post_request_dto.py
-test/test_create_presigned_post_response_class.py
-test/test_default_api.py
 test/test_document_class.py
 test/test_documents_api.py
 test/test_get_custom_css_response_class.py
 test/test_get_lead_response_class.py
-test/test_get_product_document_download_url_response_class.py
 test/test_get_public_psp_settings_response_class.py
 test/test_initiate_braintree_payment_setup_request_dto.py
 test/test_initiate_braintree_payment_setup_response_class.py
-test/test_initiate_email_verification_dto.py
-test/test_initiate_email_verification_response_class.py
 test/test_initiate_lead_response_class.py
 test/test_initiate_payment_setup_request_dto.py
 test/test_initiate_payment_setup_response_class.py
 test/test_initiate_stripe_payment_setup_request_dto.py
 test/test_initiate_stripe_payment_setup_response_class.py
-test/test_inline_response200.py
-test/test_inline_response503.py
 test/test_insured_object_class.py
 test/test_insured_object_type_class.py
 test/test_invoice_class.py
 test/test_invoice_item_class.py
 test/test_invoice_status_class.py
 test/test_lead_account_class.py
 test/test_lead_bank_account_class.py
@@ -153,25 +123,23 @@
 test/test_list_documents_response_class.py
 test/test_list_product_documents_response_class.py
 test/test_list_products_response_class.py
 test/test_notifications_api.py
 test/test_payment_method_class.py
 test/test_payments_setup_api.py
 test/test_policy_object_request_dto.py
-test/test_policy_object_response_class.py
 test/test_premium_override_dto.py
 test/test_premium_override_request_dto.py
 test/test_product_class.py
 test/test_product_document_class.py
-test/test_product_factor_for_version_class.py
+test/test_product_factor_class.py
 test/test_product_field_class.py
 test/test_product_version_class.py
 test/test_products_api.py
 test/test_send_notification_request_dto.py
 test/test_send_notification_response_class.py
-test/test_sepa_dto.py
 test/test_structured_address_class.py
 test/test_suggested_address_details_class.py
 test/test_update_lead_request_dto.py
 test/test_update_lead_response_class.py
 test/test_uploaded_document_dto.py
 test/test_validate_address_response_class.py
```

### Comparing `eis-publicapi-1.22.1/test/test_address_completion_item_class.py` & `eis-publicapi-1.6.0/test/test_address_completion_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_address_completion_response_class.py` & `eis-publicapi-1.6.0/test/test_address_completion_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_address_completions_validations_api.py` & `eis-publicapi-1.6.0/test/test_address_completions_validations_api.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_address_field_score_class.py` & `eis-publicapi-1.6.0/test/test_address_field_score_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_calculate_product_fields_request_dto.py` & `eis-publicapi-1.6.0/test/test_policy_object_request_dto.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,29 +10,27 @@
 
 
 import sys
 import unittest
 
 import eis.publicapi
 from eis.publicapi.model.policy_object_request_dto import PolicyObjectRequestDto
-globals()['PolicyObjectRequestDto'] = PolicyObjectRequestDto
-from eis.publicapi.model.calculate_product_fields_request_dto import CalculateProductFieldsRequestDto
 
 
-class TestCalculateProductFieldsRequestDto(unittest.TestCase):
-    """CalculateProductFieldsRequestDto unit test stubs"""
+class TestPolicyObjectRequestDto(unittest.TestCase):
+    """PolicyObjectRequestDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCalculateProductFieldsRequestDto(self):
-        """Test CalculateProductFieldsRequestDto"""
+    def testPolicyObjectRequestDto(self):
+        """Test PolicyObjectRequestDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CalculateProductFieldsRequestDto()  # noqa: E501
+        # model = PolicyObjectRequestDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_calculate_product_fields_response_class.py` & `eis-publicapi-1.6.0/test/test_create_lead_response_class.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.policy_object_response_class import PolicyObjectResponseClass
-globals()['PolicyObjectResponseClass'] = PolicyObjectResponseClass
-from eis.publicapi.model.calculate_product_fields_response_class import CalculateProductFieldsResponseClass
+from eis.publicapi.model.lead_class import LeadClass
+globals()['LeadClass'] = LeadClass
+from eis.publicapi.model.create_lead_response_class import CreateLeadResponseClass
 
 
-class TestCalculateProductFieldsResponseClass(unittest.TestCase):
-    """CalculateProductFieldsResponseClass unit test stubs"""
+class TestCreateLeadResponseClass(unittest.TestCase):
+    """CreateLeadResponseClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCalculateProductFieldsResponseClass(self):
-        """Test CalculateProductFieldsResponseClass"""
+    def testCreateLeadResponseClass(self):
+        """Test CreateLeadResponseClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CalculateProductFieldsResponseClass()  # noqa: E501
+        # model = CreateLeadResponseClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_complete_braintree_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/test/test_complete_braintree_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_complete_email_verification_dto.py` & `eis-publicapi-1.6.0/test/test_notifications_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 
     The version of the OpenAPI document: 1.0
     Contact: kontakt@emil.de
     Generated by: https://openapi-generator.tech
 """
 
 
-import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.complete_email_verification_dto import CompleteEmailVerificationDto
+from eis.publicapi.api.notifications_api import NotificationsApi  # noqa: E501
 
 
-class TestCompleteEmailVerificationDto(unittest.TestCase):
-    """CompleteEmailVerificationDto unit test stubs"""
+class TestNotificationsApi(unittest.TestCase):
+    """NotificationsApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = NotificationsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testCompleteEmailVerificationDto(self):
-        """Test CompleteEmailVerificationDto"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CompleteEmailVerificationDto()  # noqa: E501
+    def test_send_notification(self):
+        """Test case for send_notification
+
+        Send an email.  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_complete_email_verification_response_class.py` & `eis-publicapi-1.6.0/test/test_initiate_stripe_payment_setup_response_class.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.complete_email_verification_response_class import CompleteEmailVerificationResponseClass
+from eis.publicapi.model.initiate_stripe_payment_setup_response_class import InitiateStripePaymentSetupResponseClass
 
 
-class TestCompleteEmailVerificationResponseClass(unittest.TestCase):
-    """CompleteEmailVerificationResponseClass unit test stubs"""
+class TestInitiateStripePaymentSetupResponseClass(unittest.TestCase):
+    """InitiateStripePaymentSetupResponseClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCompleteEmailVerificationResponseClass(self):
-        """Test CompleteEmailVerificationResponseClass"""
+    def testInitiateStripePaymentSetupResponseClass(self):
+        """Test InitiateStripePaymentSetupResponseClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CompleteEmailVerificationResponseClass()  # noqa: E501
+        # model = InitiateStripePaymentSetupResponseClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_complete_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/test/test_complete_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_complete_payment_setup_response_class.py` & `eis-publicapi-1.6.0/test/test_complete_payment_setup_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_complete_stripe_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/test/test_complete_stripe_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_create_account_request_dto.py` & `eis-publicapi-1.6.0/test/test_create_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_create_bank_account_request_dto.py` & `eis-publicapi-1.6.0/test/test_create_bank_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_create_custom_application_request_dto.py` & `eis-publicapi-1.6.0/test/test_create_custom_application_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_create_custom_application_response_class.py` & `eis-publicapi-1.6.0/test/test_create_custom_application_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_create_document_request_dto.py` & `eis-publicapi-1.6.0/test/test_create_document_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_create_estimated_invoice_request_dto.py` & `eis-publicapi-1.6.0/test/test_create_estimated_invoice_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_create_estimated_invoice_response_class.py` & `eis-publicapi-1.6.0/test/test_list_products_response_class.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,32 +9,30 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.calculate_product_fields_response_class import CalculateProductFieldsResponseClass
-from eis.publicapi.model.invoice_class import InvoiceClass
-globals()['CalculateProductFieldsResponseClass'] = CalculateProductFieldsResponseClass
-globals()['InvoiceClass'] = InvoiceClass
-from eis.publicapi.model.create_estimated_invoice_response_class import CreateEstimatedInvoiceResponseClass
+from eis.publicapi.model.product_class import ProductClass
+globals()['ProductClass'] = ProductClass
+from eis.publicapi.model.list_products_response_class import ListProductsResponseClass
 
 
-class TestCreateEstimatedInvoiceResponseClass(unittest.TestCase):
-    """CreateEstimatedInvoiceResponseClass unit test stubs"""
+class TestListProductsResponseClass(unittest.TestCase):
+    """ListProductsResponseClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreateEstimatedInvoiceResponseClass(self):
-        """Test CreateEstimatedInvoiceResponseClass"""
+    def testListProductsResponseClass(self):
+        """Test ListProductsResponseClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CreateEstimatedInvoiceResponseClass()  # noqa: E501
+        # model = ListProductsResponseClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_create_lead_async_response_class.py` & `eis-publicapi-1.6.0/test/test_structured_address_class.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.create_lead_async_response_class import CreateLeadAsyncResponseClass
+from eis.publicapi.model.structured_address_class import StructuredAddressClass
 
 
-class TestCreateLeadAsyncResponseClass(unittest.TestCase):
-    """CreateLeadAsyncResponseClass unit test stubs"""
+class TestStructuredAddressClass(unittest.TestCase):
+    """StructuredAddressClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreateLeadAsyncResponseClass(self):
-        """Test CreateLeadAsyncResponseClass"""
+    def testStructuredAddressClass(self):
+        """Test StructuredAddressClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CreateLeadAsyncResponseClass()  # noqa: E501
+        # model = StructuredAddressClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_create_lead_request_dto.py` & `eis-publicapi-1.6.0/test/test_create_lead_request_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 
 import sys
 import unittest
 
 import eis.publicapi
 from eis.publicapi.model.create_account_request_dto import CreateAccountRequestDto
 from eis.publicapi.model.create_bank_account_request_dto import CreateBankAccountRequestDto
-from eis.publicapi.model.create_payment_method_request_dto import CreatePaymentMethodRequestDto
 from eis.publicapi.model.policy_object_request_dto import PolicyObjectRequestDto
 from eis.publicapi.model.premium_override_request_dto import PremiumOverrideRequestDto
 from eis.publicapi.model.uploaded_document_dto import UploadedDocumentDto
 globals()['CreateAccountRequestDto'] = CreateAccountRequestDto
 globals()['CreateBankAccountRequestDto'] = CreateBankAccountRequestDto
-globals()['CreatePaymentMethodRequestDto'] = CreatePaymentMethodRequestDto
 globals()['PolicyObjectRequestDto'] = PolicyObjectRequestDto
 globals()['PremiumOverrideRequestDto'] = PremiumOverrideRequestDto
 globals()['UploadedDocumentDto'] = UploadedDocumentDto
 from eis.publicapi.model.create_lead_request_dto import CreateLeadRequestDto
 
 
 class TestCreateLeadRequestDto(unittest.TestCase):
```

### Comparing `eis-publicapi-1.22.1/test/test_create_lead_response_class.py` & `eis-publicapi-1.6.0/test/test_initiate_lead_response_class.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.lead_class import LeadClass
-globals()['LeadClass'] = LeadClass
-from eis.publicapi.model.create_lead_response_class import CreateLeadResponseClass
+from eis.publicapi.model.initiate_lead_response_class import InitiateLeadResponseClass
 
 
-class TestCreateLeadResponseClass(unittest.TestCase):
-    """CreateLeadResponseClass unit test stubs"""
+class TestInitiateLeadResponseClass(unittest.TestCase):
+    """InitiateLeadResponseClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreateLeadResponseClass(self):
-        """Test CreateLeadResponseClass"""
+    def testInitiateLeadResponseClass(self):
+        """Test InitiateLeadResponseClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CreateLeadResponseClass()  # noqa: E501
+        # model = InitiateLeadResponseClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_create_payment_method_request_dto.py` & `eis-publicapi-1.6.0/test/test_initiate_payment_setup_request_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.sepa_dto import SepaDto
-globals()['SepaDto'] = SepaDto
-from eis.publicapi.model.create_payment_method_request_dto import CreatePaymentMethodRequestDto
+from eis.publicapi.model.initiate_braintree_payment_setup_request_dto import InitiateBraintreePaymentSetupRequestDto
+from eis.publicapi.model.initiate_stripe_payment_setup_request_dto import InitiateStripePaymentSetupRequestDto
+globals()['InitiateBraintreePaymentSetupRequestDto'] = InitiateBraintreePaymentSetupRequestDto
+globals()['InitiateStripePaymentSetupRequestDto'] = InitiateStripePaymentSetupRequestDto
+from eis.publicapi.model.initiate_payment_setup_request_dto import InitiatePaymentSetupRequestDto
 
 
-class TestCreatePaymentMethodRequestDto(unittest.TestCase):
-    """CreatePaymentMethodRequestDto unit test stubs"""
+class TestInitiatePaymentSetupRequestDto(unittest.TestCase):
+    """InitiatePaymentSetupRequestDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreatePaymentMethodRequestDto(self):
-        """Test CreatePaymentMethodRequestDto"""
+    def testInitiatePaymentSetupRequestDto(self):
+        """Test InitiatePaymentSetupRequestDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CreatePaymentMethodRequestDto()  # noqa: E501
+        # model = InitiatePaymentSetupRequestDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_create_presigned_post_request_dto.py` & `eis-publicapi-1.6.0/test/test_send_notification_response_class.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.create_presigned_post_request_dto import CreatePresignedPostRequestDto
+from eis.publicapi.model.send_notification_response_class import SendNotificationResponseClass
 
 
-class TestCreatePresignedPostRequestDto(unittest.TestCase):
-    """CreatePresignedPostRequestDto unit test stubs"""
+class TestSendNotificationResponseClass(unittest.TestCase):
+    """SendNotificationResponseClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreatePresignedPostRequestDto(self):
-        """Test CreatePresignedPostRequestDto"""
+    def testSendNotificationResponseClass(self):
+        """Test SendNotificationResponseClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CreatePresignedPostRequestDto()  # noqa: E501
+        # model = SendNotificationResponseClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_create_presigned_post_response_class.py` & `eis-publicapi-1.6.0/test/test_create_estimated_invoice_response_class.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.create_presigned_post_response_class import CreatePresignedPostResponseClass
+from eis.publicapi.model.invoice_class import InvoiceClass
+globals()['InvoiceClass'] = InvoiceClass
+from eis.publicapi.model.create_estimated_invoice_response_class import CreateEstimatedInvoiceResponseClass
 
 
-class TestCreatePresignedPostResponseClass(unittest.TestCase):
-    """CreatePresignedPostResponseClass unit test stubs"""
+class TestCreateEstimatedInvoiceResponseClass(unittest.TestCase):
+    """CreateEstimatedInvoiceResponseClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreatePresignedPostResponseClass(self):
-        """Test CreatePresignedPostResponseClass"""
+    def testCreateEstimatedInvoiceResponseClass(self):
+        """Test CreateEstimatedInvoiceResponseClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CreatePresignedPostResponseClass()  # noqa: E501
+        # model = CreateEstimatedInvoiceResponseClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_default_api.py` & `eis-publicapi-1.6.0/test/test_payment_method_class.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 
     The version of the OpenAPI document: 1.0
     Contact: kontakt@emil.de
     Generated by: https://openapi-generator.tech
 """
 
 
+import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.api.default_api import DefaultApi  # noqa: E501
+from eis.publicapi.model.payment_method_class import PaymentMethodClass
 
 
-class TestDefaultApi(unittest.TestCase):
-    """DefaultApi unit test stubs"""
+class TestPaymentMethodClass(unittest.TestCase):
+    """PaymentMethodClass unit test stubs"""
 
     def setUp(self):
-        self.api = DefaultApi()  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    def test_check(self):
-        """Test case for check
-
-        """
+    def testPaymentMethodClass(self):
+        """Test PaymentMethodClass"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = PaymentMethodClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_document_class.py` & `eis-publicapi-1.6.0/test/test_document_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_documents_api.py` & `eis-publicapi-1.6.0/test/test_documents_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,52 +27,31 @@
     def test_create_temporary_document(self):
         """Test case for create_temporary_document
 
         Create the temporary document  # noqa: E501
         """
         pass
 
-    def test_delete_documents(self):
-        """Test case for delete_documents
-
-        Delete a document  # noqa: E501
-        """
-        pass
-
     def test_download_document(self):
         """Test case for download_document
 
         Download a document  # noqa: E501
         """
         pass
 
-    def test_download_product_document_url(self):
-        """Test case for download_product_document_url
-
-        Get pre-signed url for downloading product document  # noqa: E501
-        """
-        pass
-
     def test_list_documents(self):
         """Test case for list_documents
 
         List documents  # noqa: E501
         """
         pass
 
     def test_list_product_documents(self):
         """Test case for list_product_documents
 
         List product documents  # noqa: E501
         """
         pass
 
-    def test_pre_signed_post(self):
-        """Test case for pre_signed_post
-
-        Upload documents using pre-signed URL  # noqa: E501
-        """
-        pass
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_get_custom_css_response_class.py` & `eis-publicapi-1.6.0/test/test_get_custom_css_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_get_lead_response_class.py` & `eis-publicapi-1.6.0/test/test_get_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_get_public_psp_settings_response_class.py` & `eis-publicapi-1.6.0/test/test_get_public_psp_settings_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_initiate_braintree_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/test/test_initiate_braintree_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_initiate_braintree_payment_setup_response_class.py` & `eis-publicapi-1.6.0/test/test_initiate_braintree_payment_setup_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_initiate_lead_response_class.py` & `eis-publicapi-1.6.0/test/test_update_lead_response_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.initiate_lead_response_class import InitiateLeadResponseClass
+from eis.publicapi.model.lead_class import LeadClass
+globals()['LeadClass'] = LeadClass
+from eis.publicapi.model.update_lead_response_class import UpdateLeadResponseClass
 
 
-class TestInitiateLeadResponseClass(unittest.TestCase):
-    """InitiateLeadResponseClass unit test stubs"""
+class TestUpdateLeadResponseClass(unittest.TestCase):
+    """UpdateLeadResponseClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInitiateLeadResponseClass(self):
-        """Test InitiateLeadResponseClass"""
+    def testUpdateLeadResponseClass(self):
+        """Test UpdateLeadResponseClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = InitiateLeadResponseClass()  # noqa: E501
+        # model = UpdateLeadResponseClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_initiate_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/test/test_initiate_payment_setup_response_class.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.initiate_braintree_payment_setup_request_dto import InitiateBraintreePaymentSetupRequestDto
-from eis.publicapi.model.initiate_stripe_payment_setup_request_dto import InitiateStripePaymentSetupRequestDto
-globals()['InitiateBraintreePaymentSetupRequestDto'] = InitiateBraintreePaymentSetupRequestDto
-globals()['InitiateStripePaymentSetupRequestDto'] = InitiateStripePaymentSetupRequestDto
-from eis.publicapi.model.initiate_payment_setup_request_dto import InitiatePaymentSetupRequestDto
+from eis.publicapi.model.initiate_braintree_payment_setup_response_class import InitiateBraintreePaymentSetupResponseClass
+from eis.publicapi.model.initiate_stripe_payment_setup_response_class import InitiateStripePaymentSetupResponseClass
+globals()['InitiateBraintreePaymentSetupResponseClass'] = InitiateBraintreePaymentSetupResponseClass
+globals()['InitiateStripePaymentSetupResponseClass'] = InitiateStripePaymentSetupResponseClass
+from eis.publicapi.model.initiate_payment_setup_response_class import InitiatePaymentSetupResponseClass
 
 
-class TestInitiatePaymentSetupRequestDto(unittest.TestCase):
-    """InitiatePaymentSetupRequestDto unit test stubs"""
+class TestInitiatePaymentSetupResponseClass(unittest.TestCase):
+    """InitiatePaymentSetupResponseClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInitiatePaymentSetupRequestDto(self):
-        """Test InitiatePaymentSetupRequestDto"""
+    def testInitiatePaymentSetupResponseClass(self):
+        """Test InitiatePaymentSetupResponseClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = InitiatePaymentSetupRequestDto()  # noqa: E501
+        # model = InitiatePaymentSetupResponseClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_initiate_stripe_payment_setup_request_dto.py` & `eis-publicapi-1.6.0/test/test_initiate_stripe_payment_setup_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_inline_response200.py` & `eis-publicapi-1.6.0/test/test_suggested_address_details_class.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.inline_response200 import InlineResponse200
+from eis.publicapi.model.suggested_address_details_class import SuggestedAddressDetailsClass
 
 
-class TestInlineResponse200(unittest.TestCase):
-    """InlineResponse200 unit test stubs"""
+class TestSuggestedAddressDetailsClass(unittest.TestCase):
+    """SuggestedAddressDetailsClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInlineResponse200(self):
-        """Test InlineResponse200"""
+    def testSuggestedAddressDetailsClass(self):
+        """Test SuggestedAddressDetailsClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = InlineResponse200()  # noqa: E501
+        # model = SuggestedAddressDetailsClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_inline_response503.py` & `eis-publicapi-1.6.0/test/test_insured_object_class.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.inline_response503 import InlineResponse503
+from eis.publicapi.model.product_field_class import ProductFieldClass
+globals()['ProductFieldClass'] = ProductFieldClass
+from eis.publicapi.model.insured_object_class import InsuredObjectClass
 
 
-class TestInlineResponse503(unittest.TestCase):
-    """InlineResponse503 unit test stubs"""
+class TestInsuredObjectClass(unittest.TestCase):
+    """InsuredObjectClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInlineResponse503(self):
-        """Test InlineResponse503"""
+    def testInsuredObjectClass(self):
+        """Test InsuredObjectClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = InlineResponse503()  # noqa: E501
+        # model = InsuredObjectClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_insured_object_class.py` & `eis-publicapi-1.6.0/test/test_product_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.product_field_class import ProductFieldClass
-globals()['ProductFieldClass'] = ProductFieldClass
-from eis.publicapi.model.insured_object_class import InsuredObjectClass
+from eis.publicapi.model.insured_object_type_class import InsuredObjectTypeClass
+from eis.publicapi.model.product_version_class import ProductVersionClass
+globals()['InsuredObjectTypeClass'] = InsuredObjectTypeClass
+globals()['ProductVersionClass'] = ProductVersionClass
+from eis.publicapi.model.product_class import ProductClass
 
 
-class TestInsuredObjectClass(unittest.TestCase):
-    """InsuredObjectClass unit test stubs"""
+class TestProductClass(unittest.TestCase):
+    """ProductClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInsuredObjectClass(self):
-        """Test InsuredObjectClass"""
+    def testProductClass(self):
+        """Test ProductClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = InsuredObjectClass()  # noqa: E501
+        # model = ProductClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_insured_object_type_class.py` & `eis-publicapi-1.6.0/test/test_insured_object_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_invoice_class.py` & `eis-publicapi-1.6.0/test/test_invoice_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_invoice_item_class.py` & `eis-publicapi-1.6.0/test/test_invoice_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_invoice_status_class.py` & `eis-publicapi-1.6.0/test/test_invoice_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_lead_account_class.py` & `eis-publicapi-1.6.0/test/test_lead_account_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_lead_bank_account_class.py` & `eis-publicapi-1.6.0/test/test_lead_bank_account_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_lead_class.py` & `eis-publicapi-1.6.0/test/test_lead_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.create_payment_method_request_dto import CreatePaymentMethodRequestDto
 from eis.publicapi.model.invoice_class import InvoiceClass
 from eis.publicapi.model.lead_account_class import LeadAccountClass
 from eis.publicapi.model.lead_bank_account_class import LeadBankAccountClass
 from eis.publicapi.model.lead_policy_class import LeadPolicyClass
 from eis.publicapi.model.premium_override_dto import PremiumOverrideDto
 from eis.publicapi.model.uploaded_document_dto import UploadedDocumentDto
-globals()['CreatePaymentMethodRequestDto'] = CreatePaymentMethodRequestDto
 globals()['InvoiceClass'] = InvoiceClass
 globals()['LeadAccountClass'] = LeadAccountClass
 globals()['LeadBankAccountClass'] = LeadBankAccountClass
 globals()['LeadPolicyClass'] = LeadPolicyClass
 globals()['PremiumOverrideDto'] = PremiumOverrideDto
 globals()['UploadedDocumentDto'] = UploadedDocumentDto
 from eis.publicapi.model.lead_class import LeadClass
```

### Comparing `eis-publicapi-1.22.1/test/test_lead_policy_class.py` & `eis-publicapi-1.6.0/test/test_lead_policy_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_lead_policy_object_class.py` & `eis-publicapi-1.6.0/test/test_lead_policy_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_leads_api.py` & `eis-publicapi-1.6.0/test/test_leads_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,28 +27,14 @@
     def test_create_lead(self):
         """Test case for create_lead
 
         Create the lead  # noqa: E501
         """
         pass
 
-    def test_create_lead_async(self):
-        """Test case for create_lead_async
-
-        Create the lead asynchronously  # noqa: E501
-        """
-        pass
-
-    def test_create_lead_sync(self):
-        """Test case for create_lead_sync
-
-        Create the lead synchronously  # noqa: E501
-        """
-        pass
-
     def test_get_lead(self):
         """Test case for get_lead
 
         Retrieve the lead  # noqa: E501
         """
         pass
 
@@ -62,17 +48,10 @@
     def test_update_lead(self):
         """Test case for update_lead
 
         Update the lead  # noqa: E501
         """
         pass
 
-    def test_update_lead_sync(self):
-        """Test case for update_lead_sync
-
-        Update the lead  # noqa: E501
-        """
-        pass
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_list_documents_response_class.py` & `eis-publicapi-1.6.0/test/test_list_documents_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_list_product_documents_response_class.py` & `eis-publicapi-1.6.0/test/test_list_product_documents_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_list_products_response_class.py` & `eis-publicapi-1.6.0/test/test_product_document_class.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.product_class import ProductClass
-globals()['ProductClass'] = ProductClass
-from eis.publicapi.model.list_products_response_class import ListProductsResponseClass
+from eis.publicapi.model.product_document_class import ProductDocumentClass
 
 
-class TestListProductsResponseClass(unittest.TestCase):
-    """ListProductsResponseClass unit test stubs"""
+class TestProductDocumentClass(unittest.TestCase):
+    """ProductDocumentClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testListProductsResponseClass(self):
-        """Test ListProductsResponseClass"""
+    def testProductDocumentClass(self):
+        """Test ProductDocumentClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ListProductsResponseClass()  # noqa: E501
+        # model = ProductDocumentClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_notifications_api.py` & `eis-publicapi-1.6.0/test/test_payments_setup_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,43 +8,43 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import eis.publicapi
-from eis.publicapi.api.notifications_api import NotificationsApi  # noqa: E501
+from eis.publicapi.api.payments_setup_api import PaymentsSetupApi  # noqa: E501
 
 
-class TestNotificationsApi(unittest.TestCase):
-    """NotificationsApi unit test stubs"""
+class TestPaymentsSetupApi(unittest.TestCase):
+    """PaymentsSetupApi unit test stubs"""
 
     def setUp(self):
-        self.api = NotificationsApi()  # noqa: E501
+        self.api = PaymentsSetupApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_complete_email_verification(self):
-        """Test case for complete_email_verification
+    def test_complete_payment_setup(self):
+        """Test case for complete_payment_setup
 
-        Complete Email Verification.  # noqa: E501
+        Complete a payment setup  # noqa: E501
         """
         pass
 
-    def test_initiate_email_verification(self):
-        """Test case for initiate_email_verification
+    def test_get_public_psp_config(self):
+        """Test case for get_public_psp_config
 
-        Initiate Email Verification.  # noqa: E501
+        Get public key and psp  # noqa: E501
         """
         pass
 
-    def test_send_notification(self):
-        """Test case for send_notification
+    def test_initiate_payment_setup(self):
+        """Test case for initiate_payment_setup
 
-        Send an email.  # noqa: E501
+        Initiate a payment setup  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_payments_setup_api.py` & `eis-publicapi-1.6.0/test/test_product_field_class.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,46 +5,32 @@
 
     The version of the OpenAPI document: 1.0
     Contact: kontakt@emil.de
     Generated by: https://openapi-generator.tech
 """
 
 
+import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.api.payments_setup_api import PaymentsSetupApi  # noqa: E501
+from eis.publicapi.model.product_field_class import ProductFieldClass
 
 
-class TestPaymentsSetupApi(unittest.TestCase):
-    """PaymentsSetupApi unit test stubs"""
+class TestProductFieldClass(unittest.TestCase):
+    """ProductFieldClass unit test stubs"""
 
     def setUp(self):
-        self.api = PaymentsSetupApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_complete_payment_setup(self):
-        """Test case for complete_payment_setup
-
-        Complete a payment setup  # noqa: E501
-        """
         pass
 
-    def test_get_public_psp_config(self):
-        """Test case for get_public_psp_config
-
-        Get public key and psp  # noqa: E501
-        """
+    def tearDown(self):
         pass
 
-    def test_initiate_payment_setup(self):
-        """Test case for initiate_payment_setup
-
-        Initiate a payment setup  # noqa: E501
-        """
+    def testProductFieldClass(self):
+        """Test ProductFieldClass"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = ProductFieldClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_policy_object_request_dto.py` & `eis-publicapi-1.6.0/test/test_update_lead_request_dto.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,28 +9,36 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
+from eis.publicapi.model.create_account_request_dto import CreateAccountRequestDto
+from eis.publicapi.model.create_bank_account_request_dto import CreateBankAccountRequestDto
 from eis.publicapi.model.policy_object_request_dto import PolicyObjectRequestDto
+from eis.publicapi.model.uploaded_document_dto import UploadedDocumentDto
+globals()['CreateAccountRequestDto'] = CreateAccountRequestDto
+globals()['CreateBankAccountRequestDto'] = CreateBankAccountRequestDto
+globals()['PolicyObjectRequestDto'] = PolicyObjectRequestDto
+globals()['UploadedDocumentDto'] = UploadedDocumentDto
+from eis.publicapi.model.update_lead_request_dto import UpdateLeadRequestDto
 
 
-class TestPolicyObjectRequestDto(unittest.TestCase):
-    """PolicyObjectRequestDto unit test stubs"""
+class TestUpdateLeadRequestDto(unittest.TestCase):
+    """UpdateLeadRequestDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPolicyObjectRequestDto(self):
-        """Test PolicyObjectRequestDto"""
+    def testUpdateLeadRequestDto(self):
+        """Test UpdateLeadRequestDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PolicyObjectRequestDto()  # noqa: E501
+        # model = UpdateLeadRequestDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_policy_object_response_class.py` & `eis-publicapi-1.6.0/test/test_product_version_class.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.policy_object_response_class import PolicyObjectResponseClass
+from eis.publicapi.model.product_version_class import ProductVersionClass
 
 
-class TestPolicyObjectResponseClass(unittest.TestCase):
-    """PolicyObjectResponseClass unit test stubs"""
+class TestProductVersionClass(unittest.TestCase):
+    """ProductVersionClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPolicyObjectResponseClass(self):
-        """Test PolicyObjectResponseClass"""
+    def testProductVersionClass(self):
+        """Test ProductVersionClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PolicyObjectResponseClass()  # noqa: E501
+        # model = ProductVersionClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_premium_override_dto.py` & `eis-publicapi-1.6.0/test/test_premium_override_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_premium_override_request_dto.py` & `eis-publicapi-1.6.0/test/test_premium_override_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_product_class.py` & `eis-publicapi-1.6.0/test/test_product_factor_class.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,32 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.publicapi
-from eis.publicapi.model.insured_object_type_class import InsuredObjectTypeClass
-from eis.publicapi.model.product_version_class import ProductVersionClass
-globals()['InsuredObjectTypeClass'] = InsuredObjectTypeClass
-globals()['ProductVersionClass'] = ProductVersionClass
-from eis.publicapi.model.product_class import ProductClass
+from eis.publicapi.model.product_factor_class import ProductFactorClass
 
 
-class TestProductClass(unittest.TestCase):
-    """ProductClass unit test stubs"""
+class TestProductFactorClass(unittest.TestCase):
+    """ProductFactorClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProductClass(self):
-        """Test ProductClass"""
+    def testProductFactorClass(self):
+        """Test ProductFactorClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProductClass()  # noqa: E501
+        # model = ProductFactorClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-publicapi-1.22.1/test/test_products_api.py` & `eis-publicapi-1.6.0/test/test_products_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,14 @@
 
     def setUp(self):
         self.api = ProductsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_calculate_product_fields(self):
-        """Test case for calculate_product_fields
-
-        Create the product fields  # noqa: E501
-        """
-        pass
-
     def test_create_estimated_invoice(self):
         """Test case for create_estimated_invoice
 
         Create the invoice product  # noqa: E501
         """
         pass
```

### Comparing `eis-publicapi-1.22.1/test/test_send_notification_request_dto.py` & `eis-publicapi-1.6.0/test/test_send_notification_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_uploaded_document_dto.py` & `eis-publicapi-1.6.0/test/test_uploaded_document_dto.py`

 * *Files identical despite different names*

### Comparing `eis-publicapi-1.22.1/test/test_validate_address_response_class.py` & `eis-publicapi-1.6.0/test/test_validate_address_response_class.py`

 * *Files identical despite different names*

