# Comparing `tmp/eis-insurance-1.33.0.tar.gz` & `tmp/eis-insurance-1.33.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis-insurance-1.33.0.tar", last modified: Wed May  8 16:31:06 2024, max compression
+gzip compressed data, was "eis-insurance-1.33.1.tar", last modified: Wed May 22 16:37:42 2024, max compression
```

## Comparing `eis-insurance-1.33.0.tar` & `eis-insurance-1.33.1.tar`

### file list

```diff
@@ -1,353 +1,353 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 16:31:06.085235 eis-insurance-1.33.0/
--rw-rw-rw-   0 root         (0) root         (0)      380 2024-05-08 16:31:06.085235 eis-insurance-1.33.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    25869 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 16:31:06.041235 eis-insurance-1.33.0/eis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 16:31:06.041235 eis-insurance-1.33.0/eis/insurance/
--rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 16:31:06.045235 eis-insurance-1.33.0/eis/insurance/api/
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5447 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/default_api.py
--rw-rw-rw-   0 root         (0) root         (0)     7612 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/insured_object_types_api.py
--rw-rw-rw-   0 root         (0) root         (0)    24476 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/insured_objects_api.py
--rw-rw-rw-   0 root         (0) root         (0)    23408 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/lead_statuses_api.py
--rw-rw-rw-   0 root         (0) root         (0)    15461 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/lead_versions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    55099 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/leads_api.py
--rw-rw-rw-   0 root         (0) root         (0)    30117 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/named_ranges_api.py
--rw-rw-rw-   0 root         (0) root         (0)    70991 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/policies_api.py
--rw-rw-rw-   0 root         (0) root         (0)    36321 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/premium_formulas_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37917 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/product_factors_api.py
--rw-rw-rw-   0 root         (0) root         (0)    36949 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/product_fields_api.py
--rw-rw-rw-   0 root         (0) root         (0)    13361 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/product_versions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37898 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/products_api.py
--rw-rw-rw-   0 root         (0) root         (0)    39773 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api/status_transition_rules_api.py
--rw-rw-rw-   0 root         (0) root         (0)    41662 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 16:31:06.045235 eis-insurance-1.33.0/eis/insurance/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1354 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16484 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5074 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 16:31:06.065235 eis-insurance-1.33.0/eis/insurance/model/
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11485 2024-05-08 16:31:03.000000 eis-insurance-1.33.0/eis/insurance/model/activate_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11862 2024-05-08 16:31:03.000000 eis-insurance-1.33.0/eis/insurance/model/activate_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12128 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/calculate_custom_premium_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12924 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/calculate_premium_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12318 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/calculate_product_fields_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12421 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/clone_product_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    18487 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_account_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11866 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_bank_account_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12564 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_custom_application_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13015 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_dummy_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    14361 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_insured_object_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12009 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_insured_object_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11606 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_lead_async_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    14927 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_lead_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    21946 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11842 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11759 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_lead_status_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11947 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_lead_status_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13809 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_named_range_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_named_range_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12316 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_named_request_s3_data_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_payment_method_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    14081 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11864 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    15591 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_premium_formula_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12053 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_premium_formula_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    18650 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_product_field_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12403 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_product_field_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    14404 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_product_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11896 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_product_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12557 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_status_transition_rule_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12061 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/create_status_transition_rule_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12383 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/csv_product_factor_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11703 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/delete_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11700 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/empty_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12000 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_insured_object_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_lead_status_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11705 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_lead_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11794 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_lead_version_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11940 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_named_range_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11718 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_policy_data_by_date_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11847 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11657 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_premium_formula_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12328 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_premium_formula_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12874 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_factor_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12439 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_factor_value_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11950 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_factor_value_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12517 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_factors_for_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11871 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_factors_for_version_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11651 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_field_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12050 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_field_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12558 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11865 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12033 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12018 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_product_version_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12151 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/get_status_transition_rule_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12323 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/grouped_product_factor_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12395 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/grouped_product_factor_value_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11940 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/grouped_product_factors_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    17245 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/grpc_patch_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    22171 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/grpc_update_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12817 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/inline_response200.py
--rw-rw-rw-   0 root         (0) root         (0)    12817 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/inline_response503.py
--rw-rw-rw-   0 root         (0) root         (0)    15814 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/insured_object_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13038 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/insured_object_type_class.py
--rw-rw-rw-   0 root         (0) root         (0)    16768 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/invoice_item_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12653 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/invoice_status_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/lead_bank_account_class.py
--rw-rw-rw-   0 root         (0) root         (0)    19860 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/lead_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12384 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/lead_status_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12158 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_insured_object_types_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12131 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_insured_objects_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12100 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_lead_statuses_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12057 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_lead_versions_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12674 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_leads_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11874 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_named_ranges_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12703 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_policies_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12773 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_policy_objects_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12265 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_premium_formulas_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12149 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_product_factors_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12283 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_product_field_types_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12121 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_product_fields_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12074 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_products_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12582 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12218 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/list_status_transition_rules_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    14789 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/named_range_class.py
--rw-rw-rw-   0 root         (0) root         (0)    16739 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/patch_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11811 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/patch_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13779 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/patch_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11851 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/patch_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12492 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/patch_status_transition_rule_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12157 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/patch_status_transition_rule_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    17937 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/policy_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13748 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/policy_object_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12867 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/policy_object_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13319 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/policy_premium_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13714 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/policy_premium_item_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13763 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/policy_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)    15539 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/premium_formula_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12952 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/premium_override_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11971 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/premium_override_request_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11905 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/premium_override_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    15269 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/product_class.py
--rw-rw-rw-   0 root         (0) root         (0)    14144 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/product_factor_class.py
--rw-rw-rw-   0 root         (0) root         (0)    14246 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/product_factor_for_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13780 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/product_factor_value_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12756 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/product_factor_value_for_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)    18932 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/product_field_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12863 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/product_field_type_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13423 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/product_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11637 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/sepa_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    14945 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/shared_create_lead_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    18643 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/shared_invoice_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12997 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/eis/insurance/model/shared_lead_policy_object_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    18950 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/shared_product_field_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12804 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/shared_update_named_range_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    15971 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/shared_update_premium_formula_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    14223 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/status_transition_rule_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12263 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/store_product_factors_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/store_product_factors_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/suspend_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11859 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/suspend_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11904 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12675 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/terminate_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11863 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/terminate_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    13994 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/timeslice_class.py
--rw-rw-rw-   0 root         (0) root         (0)    14723 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_insured_object_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    21581 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11842 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12424 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_named_range_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_named_range_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    14608 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11854 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    15591 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_premium_formula_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12029 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_premium_formula_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    19144 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_product_field_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12403 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_product_field_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12771 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_product_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11874 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_product_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12417 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_product_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12027 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_product_version_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12747 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_status_transition_rule_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12160 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/update_status_transition_rule_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    11528 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/uploaded_document_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12342 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/validate_product_factors_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11860 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model/withdraw_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)    82795 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/model_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 16:31:06.069235 eis-insurance-1.33.0/eis/insurance/models/
--rw-rw-rw-   0 root         (0) root         (0)    13560 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14277 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis/insurance/rest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 16:31:06.069235 eis-insurance-1.33.0/eis_insurance.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      380 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis_insurance.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    15794 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis_insurance.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis_insurance.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis_insurance.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/eis_insurance.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-08 16:31:06.089235 eis-insurance-1.33.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      996 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 16:31:06.085235 eis-insurance-1.33.0/test/
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-05-08 16:31:03.000000 eis-insurance-1.33.0/test/test_activate_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      943 2024-05-08 16:31:03.000000 eis-insurance-1.33.0/test/test_activate_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_calculate_custom_premium_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_calculate_premium_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_calculate_product_fields_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_clone_product_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_account_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_bank_account_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_custom_application_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_dummy_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_insured_object_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_insured_object_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_lead_async_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_lead_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_lead_status_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_lead_status_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_named_range_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_named_range_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_named_request_s3_data_class.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_payment_method_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_premium_formula_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_premium_formula_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_product_field_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_product_field_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_product_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_product_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_status_transition_rule_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_create_status_transition_rule_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_csv_product_factor_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_default_api.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_delete_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_empty_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_insured_object_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_lead_status_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_lead_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_lead_version_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_named_range_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      864 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_policy_data_by_date_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_premium_formula_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_premium_formula_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_factor_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_factor_value_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1044 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_factor_value_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_factors_for_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_factors_for_version_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_field_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_field_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      919 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_product_version_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_get_status_transition_rule_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_grouped_product_factor_class.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_grouped_product_factor_value_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_grouped_product_factors_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_grpc_patch_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_grpc_update_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_inline_response200.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_inline_response503.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_insured_object_class.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_insured_object_type_class.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_insured_object_types_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_insured_objects_api.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_invoice_item_class.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_invoice_status_class.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_lead_bank_account_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_lead_class.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_lead_status_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_lead_statuses_api.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_lead_versions_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_leads_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_insured_object_types_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_insured_objects_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_lead_statuses_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_lead_versions_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_leads_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_named_ranges_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_policies_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_policy_objects_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_premium_formulas_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_product_factors_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_product_field_types_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_product_fields_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      933 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_products_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_list_status_transition_rules_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_named_range_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1347 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_named_ranges_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_patch_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_patch_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_patch_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_patch_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_patch_status_transition_rule_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_patch_status_transition_rule_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_policies_api.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_policy_class.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_policy_object_class.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_policy_object_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_policy_premium_class.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_policy_premium_item_class.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_policy_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_premium_formula_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1606 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_premium_formulas_api.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_premium_override_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_premium_override_request_class.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_premium_override_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_product_class.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_product_factor_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1043 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_product_factor_for_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_product_factor_value_class.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_product_factor_value_for_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1604 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_product_factors_api.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_product_field_class.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_product_field_type_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1543 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_product_fields_api.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_product_version_class.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_product_versions_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1453 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_products_api.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_sepa_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_shared_create_lead_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_shared_invoice_class.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-05-08 16:31:04.000000 eis-insurance-1.33.0/test/test_shared_lead_policy_object_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_shared_product_field_class.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_shared_update_named_range_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_shared_update_premium_formula_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_status_transition_rule_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_status_transition_rules_api.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_store_product_factors_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_store_product_factors_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_suspend_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_suspend_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_swap_premium_formulas_order_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_terminate_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_terminate_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_timeslice_class.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_insured_object_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1720 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_lead_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_lead_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_named_range_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_named_range_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_policy_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_policy_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_premium_formula_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_premium_formula_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_product_field_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_product_field_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_product_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_product_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_product_version_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_product_version_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_status_transition_rule_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_update_status_transition_rule_response_class.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_uploaded_document_dto.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_validate_product_factors_request_dto.py
--rw-rw-rw-   0 root         (0) root         (0)      943 2024-05-08 16:31:05.000000 eis-insurance-1.33.0/test/test_withdraw_policy_response_class.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 16:37:42.958352 eis-insurance-1.33.1/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-05-22 16:37:42.958352 eis-insurance-1.33.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    25869 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 16:37:42.910353 eis-insurance-1.33.1/eis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 16:37:42.910353 eis-insurance-1.33.1/eis/insurance/
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 16:37:42.914353 eis-insurance-1.33.1/eis/insurance/api/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/default_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7612 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/insured_object_types_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    24476 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/insured_objects_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    23408 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/lead_statuses_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    15461 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/lead_versions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    55099 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/leads_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    30117 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/named_ranges_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    70991 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/policies_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    36321 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/premium_formulas_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37917 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/product_factors_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    36949 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/product_fields_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    13361 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/product_versions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37898 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/products_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    39773 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api/status_transition_rules_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    41662 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 16:37:42.914353 eis-insurance-1.33.1/eis/insurance/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16484 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5074 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 16:37:42.934352 eis-insurance-1.33.1/eis/insurance/model/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11485 2024-05-22 16:37:40.000000 eis-insurance-1.33.1/eis/insurance/model/activate_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2024-05-22 16:37:40.000000 eis-insurance-1.33.1/eis/insurance/model/activate_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12128 2024-05-22 16:37:40.000000 eis-insurance-1.33.1/eis/insurance/model/calculate_custom_premium_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12924 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/calculate_premium_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12318 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/calculate_product_fields_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12421 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/clone_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    18487 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_account_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11866 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_bank_account_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12564 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_custom_application_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13015 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_dummy_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14361 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_insured_object_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_insured_object_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11606 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_lead_async_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14927 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_lead_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    21946 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11842 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11759 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_lead_status_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11947 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_lead_status_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13809 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12316 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_named_request_s3_data_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_payment_method_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14081 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11864 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    15591 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12053 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    18650 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12403 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14404 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11896 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12557 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12061 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/create_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12383 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/csv_product_factor_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11703 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/delete_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11700 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/empty_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12000 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_insured_object_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_lead_status_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11705 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_lead_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11794 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_lead_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11940 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11718 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_policy_data_by_date_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11847 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11657 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12328 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12874 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_factor_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12439 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_factor_value_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11950 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_factor_value_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12517 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_factors_for_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11871 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_factors_for_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11651 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12050 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12558 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11865 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12033 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12018 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_product_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12151 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/get_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12323 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/grouped_product_factor_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12395 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/grouped_product_factor_value_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11940 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/grouped_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    17245 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/grpc_patch_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    22171 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/grpc_update_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12817 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/inline_response200.py
+-rw-rw-rw-   0 root         (0) root         (0)    12817 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/inline_response503.py
+-rw-rw-rw-   0 root         (0) root         (0)    15814 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/insured_object_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13038 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/insured_object_type_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    16768 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/invoice_item_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12653 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/invoice_status_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/lead_bank_account_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    19860 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/lead_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12384 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/lead_status_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12158 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_insured_object_types_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12131 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_insured_objects_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12100 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_lead_statuses_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12057 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_lead_versions_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12674 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_leads_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11874 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_named_ranges_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12703 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_policies_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12773 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_policy_objects_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12265 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_premium_formulas_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12149 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12283 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_product_field_types_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12121 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_product_fields_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12074 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_products_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12582 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12218 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/list_status_transition_rules_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14789 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/named_range_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    16739 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/patch_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11811 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/patch_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13779 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/patch_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11851 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/patch_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12492 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/patch_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12157 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/patch_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    17937 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/policy_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13748 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/policy_object_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12867 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/policy_object_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13319 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/policy_premium_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13714 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/policy_premium_item_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13763 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/policy_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    15539 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/premium_formula_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12952 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/premium_override_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11971 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/premium_override_request_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11905 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/premium_override_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    15269 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/product_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14144 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/product_factor_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14246 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/product_factor_for_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13780 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/product_factor_value_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12756 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/product_factor_value_for_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    18932 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/product_field_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12863 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/product_field_type_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13423 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/product_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11637 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/sepa_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14945 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/shared_create_lead_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    18643 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/shared_invoice_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12997 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/shared_lead_policy_object_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    18950 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/shared_product_field_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12804 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/shared_update_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    15971 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/shared_update_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14223 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/status_transition_rule_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12263 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/store_product_factors_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/store_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/suspend_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11859 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/suspend_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11904 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/swap_premium_formulas_order_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12675 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/eis/insurance/model/terminate_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11863 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/terminate_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13994 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/timeslice_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14723 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_insured_object_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    21581 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11842 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12424 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14608 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11854 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    15591 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    19144 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12403 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12771 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11874 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12417 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12027 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_product_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12747 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12160 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/update_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11528 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/uploaded_document_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12342 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/validate_product_factors_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11860 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model/withdraw_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    82795 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/model_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 16:37:42.934352 eis-insurance-1.33.1/eis/insurance/models/
+-rw-rw-rw-   0 root         (0) root         (0)    13560 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14277 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis/insurance/rest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 16:37:42.934352 eis-insurance-1.33.1/eis_insurance.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis_insurance.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    15794 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis_insurance.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis_insurance.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis_insurance.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/eis_insurance.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-22 16:37:42.958352 eis-insurance-1.33.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      996 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 16:37:42.958352 eis-insurance-1.33.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-05-22 16:37:40.000000 eis-insurance-1.33.1/test/test_activate_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      943 2024-05-22 16:37:40.000000 eis-insurance-1.33.1/test/test_activate_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-05-22 16:37:40.000000 eis-insurance-1.33.1/test/test_calculate_custom_premium_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_calculate_premium_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_calculate_product_fields_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_clone_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_account_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_bank_account_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_custom_application_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_dummy_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_insured_object_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_insured_object_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_lead_async_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_lead_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_lead_status_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_lead_status_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_named_request_s3_data_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_payment_method_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_create_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_csv_product_factor_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_default_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_delete_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_empty_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_insured_object_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_lead_status_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_lead_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_lead_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_policy_data_by_date_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_factor_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_factor_value_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_factor_value_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_factors_for_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_factors_for_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      919 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_product_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_get_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_grouped_product_factor_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_grouped_product_factor_value_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_grouped_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_grpc_patch_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_grpc_update_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_inline_response200.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_inline_response503.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_insured_object_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_insured_object_type_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_insured_object_types_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_insured_objects_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_invoice_item_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_invoice_status_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_lead_bank_account_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_lead_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_lead_status_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_lead_statuses_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_lead_versions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_leads_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_insured_object_types_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_insured_objects_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_lead_statuses_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_lead_versions_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_leads_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_named_ranges_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_policies_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_policy_objects_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_premium_formulas_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_product_field_types_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_product_fields_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      933 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_products_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_list_status_transition_rules_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_named_range_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_named_ranges_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_patch_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_patch_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_patch_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_patch_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_patch_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_patch_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_policies_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_policy_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_policy_object_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_policy_object_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_policy_premium_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_policy_premium_item_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_policy_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_premium_formula_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_premium_formulas_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_premium_override_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_premium_override_request_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_premium_override_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_product_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_product_factor_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_product_factor_for_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_product_factor_value_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_product_factor_value_for_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1604 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_product_factors_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_product_field_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_product_field_type_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_product_fields_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_product_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_product_versions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_products_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_sepa_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_shared_create_lead_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_shared_invoice_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_shared_lead_policy_object_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_shared_product_field_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_shared_update_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_shared_update_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_status_transition_rule_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_status_transition_rules_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_store_product_factors_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_store_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_suspend_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_suspend_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-05-22 16:37:41.000000 eis-insurance-1.33.1/test/test_swap_premium_formulas_order_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_terminate_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_terminate_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_timeslice_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_insured_object_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_product_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_update_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_uploaded_document_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_validate_product_factors_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      943 2024-05-22 16:37:42.000000 eis-insurance-1.33.1/test/test_withdraw_policy_response_class.py
```

### Comparing `eis-insurance-1.33.0/README.md` & `eis-insurance-1.33.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # eis-insurance
 The EMIL InsuranceService API description
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0
-- Package version: 1.33.0
+- Package version: 1.33.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.emil.de](https://www.emil.de)
 
 ## Requirements.
 
 Python >=3.6
```

### Comparing `eis-insurance-1.33.0/eis/insurance/__init__.py` & `eis-insurance-1.33.1/eis/insurance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 1.0
     Contact: kontakt@emil.de
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.33.0"
+__version__ = "1.33.1"
 
 # import ApiClient
 from eis.insurance.api_client import ApiClient
 
 # import Configuration
 from eis.insurance.configuration import Configuration
```

### Comparing `eis-insurance-1.33.0/eis/insurance/api/default_api.py` & `eis-insurance-1.33.1/eis/insurance/api/default_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/insured_object_types_api.py` & `eis-insurance-1.33.1/eis/insurance/api/insured_object_types_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/insured_objects_api.py` & `eis-insurance-1.33.1/eis/insurance/api/insured_objects_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/lead_statuses_api.py` & `eis-insurance-1.33.1/eis/insurance/api/lead_statuses_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/lead_versions_api.py` & `eis-insurance-1.33.1/eis/insurance/api/lead_versions_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/leads_api.py` & `eis-insurance-1.33.1/eis/insurance/api/leads_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/named_ranges_api.py` & `eis-insurance-1.33.1/eis/insurance/api/named_ranges_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/policies_api.py` & `eis-insurance-1.33.1/eis/insurance/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/premium_formulas_api.py` & `eis-insurance-1.33.1/eis/insurance/api/premium_formulas_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/product_factors_api.py` & `eis-insurance-1.33.1/eis/insurance/api/product_factors_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/product_fields_api.py` & `eis-insurance-1.33.1/eis/insurance/api/product_fields_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/product_versions_api.py` & `eis-insurance-1.33.1/eis/insurance/api/product_versions_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/products_api.py` & `eis-insurance-1.33.1/eis/insurance/api/products_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api/status_transition_rules_api.py` & `eis-insurance-1.33.1/eis/insurance/api/status_transition_rules_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/api_client.py` & `eis-insurance-1.33.1/eis/insurance/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.33.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.33.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `eis-insurance-1.33.0/eis/insurance/apis/__init__.py` & `eis-insurance-1.33.1/eis/insurance/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/configuration.py` & `eis-insurance-1.33.1/eis/insurance/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.33.0".\
+               "SDK Package Version: 1.33.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `eis-insurance-1.33.0/eis/insurance/exceptions.py` & `eis-insurance-1.33.1/eis/insurance/exceptions.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/activate_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/activate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/activate_policy_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/activate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/calculate_custom_premium_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/calculate_custom_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/calculate_premium_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/calculate_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/calculate_product_fields_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/calculate_product_fields_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/clone_product_version_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/clone_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_account_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_bank_account_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_bank_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_custom_application_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_custom_application_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_dummy_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_dummy_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_insured_object_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_insured_object_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_lead_async_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_lead_async_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_lead_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_lead_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_lead_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_lead_status_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_lead_status_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_lead_status_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_named_range_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_named_range_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_named_request_s3_data_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_named_request_s3_data_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_payment_method_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_payment_method_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_policy_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_premium_formula_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_premium_formula_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_product_field_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_product_field_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_product_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_product_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_status_transition_rule_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/create_status_transition_rule_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/create_status_transition_rule_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/create_status_transition_rule_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/csv_product_factor_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/csv_product_factor_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/delete_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/delete_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/empty_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/empty_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_insured_object_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_lead_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_lead_status_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_lead_version_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/get_lead_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_lead_version_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_lead_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_named_range_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_policy_data_by_date_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/get_policy_data_by_date_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/get_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_policy_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_premium_formula_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/get_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_premium_formula_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_factor_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_factor_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_factor_value_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_factor_value_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_factor_value_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_factor_value_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_factors_for_version_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_factors_for_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_factors_for_version_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_factors_for_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_field_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_field_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_version_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_product_version_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/get_status_transition_rule_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/get_status_transition_rule_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/grouped_product_factor_class.py` & `eis-insurance-1.33.1/eis/insurance/model/grouped_product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/grouped_product_factor_value_class.py` & `eis-insurance-1.33.1/eis/insurance/model/grouped_product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/grouped_product_factors_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/grouped_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/grpc_patch_lead_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/grpc_patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/grpc_update_lead_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/grpc_update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/inline_response200.py` & `eis-insurance-1.33.1/eis/insurance/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/inline_response503.py` & `eis-insurance-1.33.1/eis/insurance/model/inline_response503.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/insured_object_class.py` & `eis-insurance-1.33.1/eis/insurance/model/insured_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/insured_object_type_class.py` & `eis-insurance-1.33.1/eis/insurance/model/insured_object_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/invoice_item_class.py` & `eis-insurance-1.33.1/eis/insurance/model/invoice_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/invoice_status_class.py` & `eis-insurance-1.33.1/eis/insurance/model/invoice_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/lead_bank_account_class.py` & `eis-insurance-1.33.1/eis/insurance/model/lead_bank_account_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/lead_class.py` & `eis-insurance-1.33.1/eis/insurance/model/lead_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/lead_status_class.py` & `eis-insurance-1.33.1/eis/insurance/model/lead_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_insured_object_types_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_insured_object_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_insured_objects_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_insured_objects_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_lead_statuses_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_lead_statuses_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_lead_versions_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_lead_versions_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_leads_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_leads_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_named_ranges_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_named_ranges_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_policies_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_policies_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_policy_objects_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_policy_objects_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_premium_formulas_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_premium_formulas_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_product_factors_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_product_field_types_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_product_field_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_product_fields_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_product_fields_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_products_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_products_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/list_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/list_status_transition_rules_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/list_status_transition_rules_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/named_range_class.py` & `eis-insurance-1.33.1/eis/insurance/model/named_range_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/patch_lead_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/patch_lead_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/patch_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/patch_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/patch_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/patch_policy_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/patch_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/patch_status_transition_rule_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/patch_status_transition_rule_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/patch_status_transition_rule_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/patch_status_transition_rule_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/policy_class.py` & `eis-insurance-1.33.1/eis/insurance/model/policy_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/policy_object_class.py` & `eis-insurance-1.33.1/eis/insurance/model/policy_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/policy_object_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/policy_premium_class.py` & `eis-insurance-1.33.1/eis/insurance/model/policy_premium_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/policy_premium_item_class.py` & `eis-insurance-1.33.1/eis/insurance/model/policy_premium_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/policy_version_class.py` & `eis-insurance-1.33.1/eis/insurance/model/policy_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/premium_formula_class.py` & `eis-insurance-1.33.1/eis/insurance/model/premium_formula_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/premium_override_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/premium_override_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/premium_override_request_class.py` & `eis-insurance-1.33.1/eis/insurance/model/premium_override_request_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/premium_override_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/premium_override_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/product_class.py` & `eis-insurance-1.33.1/eis/insurance/model/product_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/product_factor_class.py` & `eis-insurance-1.33.1/eis/insurance/model/product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/product_factor_for_version_class.py` & `eis-insurance-1.33.1/eis/insurance/model/product_factor_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/product_factor_value_class.py` & `eis-insurance-1.33.1/eis/insurance/model/product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/product_factor_value_for_version_class.py` & `eis-insurance-1.33.1/eis/insurance/model/product_factor_value_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/product_field_class.py` & `eis-insurance-1.33.1/eis/insurance/model/product_field_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/product_field_type_class.py` & `eis-insurance-1.33.1/eis/insurance/model/product_field_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/product_version_class.py` & `eis-insurance-1.33.1/eis/insurance/model/product_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/sepa_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/sepa_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/shared_create_lead_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/shared_create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/shared_invoice_class.py` & `eis-insurance-1.33.1/eis/insurance/model/shared_invoice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/shared_lead_policy_object_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/shared_lead_policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/shared_product_field_class.py` & `eis-insurance-1.33.1/eis/insurance/model/shared_product_field_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/shared_update_named_range_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/shared_update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/shared_update_premium_formula_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/shared_update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/status_transition_rule_class.py` & `eis-insurance-1.33.1/eis/insurance/model/status_transition_rule_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/store_product_factors_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/store_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/store_product_factors_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/store_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/suspend_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/suspend_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/suspend_policy_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/suspend_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/swap_premium_formulas_order_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/terminate_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/terminate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/terminate_policy_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/terminate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/timeslice_class.py` & `eis-insurance-1.33.1/eis/insurance/model/timeslice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_insured_object_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/update_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_lead_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_lead_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/update_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_named_range_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_named_range_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/update_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_policy_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/update_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_policy_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/update_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_premium_formula_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_premium_formula_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/update_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_product_field_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/update_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_product_field_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/update_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_product_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/update_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_product_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/update_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_product_version_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/update_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_product_version_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/update_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_status_transition_rule_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/update_status_transition_rule_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/update_status_transition_rule_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/update_status_transition_rule_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/uploaded_document_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/uploaded_document_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/validate_product_factors_request_dto.py` & `eis-insurance-1.33.1/eis/insurance/model/validate_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model/withdraw_policy_response_class.py` & `eis-insurance-1.33.1/eis/insurance/model/withdraw_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/model_utils.py` & `eis-insurance-1.33.1/eis/insurance/model_utils.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/models/__init__.py` & `eis-insurance-1.33.1/eis/insurance/models/__init__.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis/insurance/rest.py` & `eis-insurance-1.33.1/eis/insurance/rest.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/eis_insurance.egg-info/SOURCES.txt` & `eis-insurance-1.33.1/eis_insurance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/setup.py` & `eis-insurance-1.33.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "eis-insurance"
-VERSION = "1.33.0"
+VERSION = "1.33.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `eis-insurance-1.33.0/test/test_activate_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_activate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_activate_policy_response_class.py` & `eis-insurance-1.33.1/test/test_activate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_calculate_custom_premium_request_dto.py` & `eis-insurance-1.33.1/test/test_calculate_custom_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_calculate_premium_request_dto.py` & `eis-insurance-1.33.1/test/test_calculate_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_calculate_product_fields_request_dto.py` & `eis-insurance-1.33.1/test/test_calculate_product_fields_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_clone_product_version_request_dto.py` & `eis-insurance-1.33.1/test/test_clone_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_account_request_dto.py` & `eis-insurance-1.33.1/test/test_create_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_bank_account_request_dto.py` & `eis-insurance-1.33.1/test/test_create_bank_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_custom_application_request_dto.py` & `eis-insurance-1.33.1/test/test_create_custom_application_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_dummy_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_create_dummy_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_insured_object_request_dto.py` & `eis-insurance-1.33.1/test/test_create_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_insured_object_response_class.py` & `eis-insurance-1.33.1/test/test_create_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_lead_async_response_class.py` & `eis-insurance-1.33.1/test/test_create_lead_async_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_lead_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_lead_request_dto.py` & `eis-insurance-1.33.1/test/test_create_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_lead_response_class.py` & `eis-insurance-1.33.1/test/test_create_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_lead_status_request_dto.py` & `eis-insurance-1.33.1/test/test_create_lead_status_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_lead_status_response_class.py` & `eis-insurance-1.33.1/test/test_create_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_named_range_request_dto.py` & `eis-insurance-1.33.1/test/test_create_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_named_range_response_class.py` & `eis-insurance-1.33.1/test/test_create_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_named_request_s3_data_class.py` & `eis-insurance-1.33.1/test/test_create_named_request_s3_data_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_payment_method_request_dto.py` & `eis-insurance-1.33.1/test/test_create_payment_method_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_create_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_policy_response_class.py` & `eis-insurance-1.33.1/test/test_create_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_premium_formula_request_dto.py` & `eis-insurance-1.33.1/test/test_create_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_premium_formula_response_class.py` & `eis-insurance-1.33.1/test/test_create_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_product_field_request_dto.py` & `eis-insurance-1.33.1/test/test_create_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_product_field_response_class.py` & `eis-insurance-1.33.1/test/test_create_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_product_request_dto.py` & `eis-insurance-1.33.1/test/test_create_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_product_response_class.py` & `eis-insurance-1.33.1/test/test_create_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_status_transition_rule_request_dto.py` & `eis-insurance-1.33.1/test/test_create_status_transition_rule_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_create_status_transition_rule_response_class.py` & `eis-insurance-1.33.1/test/test_create_status_transition_rule_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_csv_product_factor_dto.py` & `eis-insurance-1.33.1/test/test_csv_product_factor_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_default_api.py` & `eis-insurance-1.33.1/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_delete_response_class.py` & `eis-insurance-1.33.1/test/test_delete_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_empty_response_class.py` & `eis-insurance-1.33.1/test/test_empty_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_insured_object_response_class.py` & `eis-insurance-1.33.1/test/test_get_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_lead_response_class.py` & `eis-insurance-1.33.1/test/test_get_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_lead_status_response_class.py` & `eis-insurance-1.33.1/test/test_get_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_lead_version_request_dto.py` & `eis-insurance-1.33.1/test/test_get_lead_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_lead_version_response_class.py` & `eis-insurance-1.33.1/test/test_get_lead_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_named_range_response_class.py` & `eis-insurance-1.33.1/test/test_get_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_policy_data_by_date_request_dto.py` & `eis-insurance-1.33.1/test/test_get_policy_data_by_date_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_get_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_policy_response_class.py` & `eis-insurance-1.33.1/test/test_get_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_premium_formula_request_dto.py` & `eis-insurance-1.33.1/test/test_get_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_premium_formula_response_class.py` & `eis-insurance-1.33.1/test/test_get_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_factor_response_class.py` & `eis-insurance-1.33.1/test/test_get_product_factor_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_factor_value_request_dto.py` & `eis-insurance-1.33.1/test/test_get_product_factor_value_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_factor_value_response_class.py` & `eis-insurance-1.33.1/test/test_get_product_factor_value_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_factors_for_version_request_dto.py` & `eis-insurance-1.33.1/test/test_get_product_factors_for_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_factors_for_version_response_class.py` & `eis-insurance-1.33.1/test/test_get_product_factors_for_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_field_request_dto.py` & `eis-insurance-1.33.1/test/test_get_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_field_response_class.py` & `eis-insurance-1.33.1/test/test_get_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_request_dto.py` & `eis-insurance-1.33.1/test/test_get_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_response_class.py` & `eis-insurance-1.33.1/test/test_get_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_version_request_dto.py` & `eis-insurance-1.33.1/test/test_get_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_product_version_response_class.py` & `eis-insurance-1.33.1/test/test_get_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_get_status_transition_rule_response_class.py` & `eis-insurance-1.33.1/test/test_get_status_transition_rule_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_grouped_product_factor_class.py` & `eis-insurance-1.33.1/test/test_grouped_product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_grouped_product_factor_value_class.py` & `eis-insurance-1.33.1/test/test_grouped_product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_grouped_product_factors_response_class.py` & `eis-insurance-1.33.1/test/test_grouped_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_grpc_patch_lead_request_dto.py` & `eis-insurance-1.33.1/test/test_grpc_patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_grpc_update_lead_request_dto.py` & `eis-insurance-1.33.1/test/test_grpc_update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_inline_response200.py` & `eis-insurance-1.33.1/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_inline_response503.py` & `eis-insurance-1.33.1/test/test_inline_response503.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_insured_object_class.py` & `eis-insurance-1.33.1/test/test_insured_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_insured_object_type_class.py` & `eis-insurance-1.33.1/test/test_insured_object_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_insured_object_types_api.py` & `eis-insurance-1.33.1/test/test_insured_object_types_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_insured_objects_api.py` & `eis-insurance-1.33.1/test/test_insured_objects_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_invoice_item_class.py` & `eis-insurance-1.33.1/test/test_invoice_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_invoice_status_class.py` & `eis-insurance-1.33.1/test/test_invoice_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_lead_bank_account_class.py` & `eis-insurance-1.33.1/test/test_lead_bank_account_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_lead_class.py` & `eis-insurance-1.33.1/test/test_lead_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_lead_status_class.py` & `eis-insurance-1.33.1/test/test_lead_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_lead_statuses_api.py` & `eis-insurance-1.33.1/test/test_lead_statuses_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_lead_versions_api.py` & `eis-insurance-1.33.1/test/test_lead_versions_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_leads_api.py` & `eis-insurance-1.33.1/test/test_leads_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_insured_object_types_response_class.py` & `eis-insurance-1.33.1/test/test_list_insured_object_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_insured_objects_response_class.py` & `eis-insurance-1.33.1/test/test_list_insured_objects_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_lead_statuses_response_class.py` & `eis-insurance-1.33.1/test/test_list_lead_statuses_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_lead_versions_response_class.py` & `eis-insurance-1.33.1/test/test_list_lead_versions_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_leads_response_class.py` & `eis-insurance-1.33.1/test/test_list_leads_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_named_ranges_response_class.py` & `eis-insurance-1.33.1/test/test_list_named_ranges_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_policies_response_class.py` & `eis-insurance-1.33.1/test/test_list_policies_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_policy_objects_response_class.py` & `eis-insurance-1.33.1/test/test_list_policy_objects_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_premium_formulas_response_class.py` & `eis-insurance-1.33.1/test/test_list_premium_formulas_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_product_factors_response_class.py` & `eis-insurance-1.33.1/test/test_list_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_product_field_types_response_class.py` & `eis-insurance-1.33.1/test/test_list_product_field_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_product_fields_response_class.py` & `eis-insurance-1.33.1/test/test_list_product_fields_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_products_response_class.py` & `eis-insurance-1.33.1/test/test_list_products_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_request_dto.py` & `eis-insurance-1.33.1/test/test_list_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_list_status_transition_rules_response_class.py` & `eis-insurance-1.33.1/test/test_list_status_transition_rules_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_named_range_class.py` & `eis-insurance-1.33.1/test/test_named_range_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_named_ranges_api.py` & `eis-insurance-1.33.1/test/test_named_ranges_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_patch_lead_request_dto.py` & `eis-insurance-1.33.1/test/test_patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_patch_lead_response_class.py` & `eis-insurance-1.33.1/test/test_patch_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_patch_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_patch_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_patch_policy_response_class.py` & `eis-insurance-1.33.1/test/test_patch_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_patch_status_transition_rule_request_dto.py` & `eis-insurance-1.33.1/test/test_patch_status_transition_rule_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_patch_status_transition_rule_response_class.py` & `eis-insurance-1.33.1/test/test_patch_status_transition_rule_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_policies_api.py` & `eis-insurance-1.33.1/test/test_policies_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_policy_class.py` & `eis-insurance-1.33.1/test/test_policy_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_policy_object_class.py` & `eis-insurance-1.33.1/test/test_policy_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_policy_object_dto.py` & `eis-insurance-1.33.1/test/test_policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_policy_premium_class.py` & `eis-insurance-1.33.1/test/test_policy_premium_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_policy_premium_item_class.py` & `eis-insurance-1.33.1/test/test_policy_premium_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_policy_version_class.py` & `eis-insurance-1.33.1/test/test_policy_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_premium_formula_class.py` & `eis-insurance-1.33.1/test/test_premium_formula_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_premium_formulas_api.py` & `eis-insurance-1.33.1/test/test_premium_formulas_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_premium_override_dto.py` & `eis-insurance-1.33.1/test/test_premium_override_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_premium_override_request_class.py` & `eis-insurance-1.33.1/test/test_premium_override_request_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_premium_override_request_dto.py` & `eis-insurance-1.33.1/test/test_premium_override_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_class.py` & `eis-insurance-1.33.1/test/test_product_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_factor_class.py` & `eis-insurance-1.33.1/test/test_product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_factor_for_version_class.py` & `eis-insurance-1.33.1/test/test_product_factor_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_factor_value_class.py` & `eis-insurance-1.33.1/test/test_product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_factor_value_for_version_class.py` & `eis-insurance-1.33.1/test/test_product_factor_value_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_factors_api.py` & `eis-insurance-1.33.1/test/test_product_factors_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_field_class.py` & `eis-insurance-1.33.1/test/test_product_field_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_field_type_class.py` & `eis-insurance-1.33.1/test/test_product_field_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_fields_api.py` & `eis-insurance-1.33.1/test/test_product_fields_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_version_class.py` & `eis-insurance-1.33.1/test/test_product_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_product_versions_api.py` & `eis-insurance-1.33.1/test/test_product_versions_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_products_api.py` & `eis-insurance-1.33.1/test/test_products_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_sepa_dto.py` & `eis-insurance-1.33.1/test/test_sepa_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_shared_create_lead_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_shared_create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_shared_invoice_class.py` & `eis-insurance-1.33.1/test/test_shared_invoice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_shared_lead_policy_object_dto.py` & `eis-insurance-1.33.1/test/test_shared_lead_policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_shared_product_field_class.py` & `eis-insurance-1.33.1/test/test_shared_product_field_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_shared_update_named_range_request_dto.py` & `eis-insurance-1.33.1/test/test_shared_update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_shared_update_premium_formula_request_dto.py` & `eis-insurance-1.33.1/test/test_shared_update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_status_transition_rule_class.py` & `eis-insurance-1.33.1/test/test_status_transition_rule_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_status_transition_rules_api.py` & `eis-insurance-1.33.1/test/test_status_transition_rules_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_store_product_factors_request_dto.py` & `eis-insurance-1.33.1/test/test_store_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_store_product_factors_response_class.py` & `eis-insurance-1.33.1/test/test_store_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_suspend_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_suspend_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_suspend_policy_response_class.py` & `eis-insurance-1.33.1/test/test_suspend_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_swap_premium_formulas_order_request_dto.py` & `eis-insurance-1.33.1/test/test_swap_premium_formulas_order_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_terminate_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_terminate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_terminate_policy_response_class.py` & `eis-insurance-1.33.1/test/test_terminate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_timeslice_class.py` & `eis-insurance-1.33.1/test/test_timeslice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_insured_object_request_dto.py` & `eis-insurance-1.33.1/test/test_update_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_lead_request_dto.py` & `eis-insurance-1.33.1/test/test_update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_lead_response_class.py` & `eis-insurance-1.33.1/test/test_update_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_named_range_request_dto.py` & `eis-insurance-1.33.1/test/test_update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_named_range_response_class.py` & `eis-insurance-1.33.1/test/test_update_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_policy_request_dto.py` & `eis-insurance-1.33.1/test/test_update_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_policy_response_class.py` & `eis-insurance-1.33.1/test/test_update_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_premium_formula_request_dto.py` & `eis-insurance-1.33.1/test/test_update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_premium_formula_response_class.py` & `eis-insurance-1.33.1/test/test_update_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_product_field_request_dto.py` & `eis-insurance-1.33.1/test/test_update_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_product_field_response_class.py` & `eis-insurance-1.33.1/test/test_update_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_product_request_dto.py` & `eis-insurance-1.33.1/test/test_update_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_product_response_class.py` & `eis-insurance-1.33.1/test/test_update_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_product_version_request_dto.py` & `eis-insurance-1.33.1/test/test_update_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_product_version_response_class.py` & `eis-insurance-1.33.1/test/test_update_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_status_transition_rule_request_dto.py` & `eis-insurance-1.33.1/test/test_update_status_transition_rule_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_update_status_transition_rule_response_class.py` & `eis-insurance-1.33.1/test/test_update_status_transition_rule_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_uploaded_document_dto.py` & `eis-insurance-1.33.1/test/test_uploaded_document_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_validate_product_factors_request_dto.py` & `eis-insurance-1.33.1/test/test_validate_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.33.0/test/test_withdraw_policy_response_class.py` & `eis-insurance-1.33.1/test/test_withdraw_policy_response_class.py`

 * *Files identical despite different names*

