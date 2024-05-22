# Comparing `tmp/mercoa-0.3.7.tar.gz` & `tmp/mercoa-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.3.7.tar", max compression
+gzip compressed data, was "mercoa-0.3.8.tar", max compression
```

## Comparing `mercoa-0.3.7.tar` & `mercoa-0.3.8.tar`

### file list

```diff
@@ -1,256 +1,257 @@
--rw-r--r--   0        0        0     1930 2023-12-19 23:38:42.999119 mercoa-0.3.7/README.md
--rw-r--r--   0        0        0      399 2023-12-19 23:38:42.999119 mercoa-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    10739 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/__init__.py
--rw-r--r--   0        0        0     3241 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/client.py
--rw-r--r--   0        0        0      519 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      426 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1381 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      157 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/py.typed
--rw-r--r--   0        0        0    10834 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     5038 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0     1083 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0     1069 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      724 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      657 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      237 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
--rw-r--r--   0        0        0      221 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/errors/auth_header_missing_error.py
--rw-r--r--   0        0        0      222 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/errors/forbidden.py
--rw-r--r--   0        0        0      230 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/errors/invalid_postal_code.py
--rw-r--r--   0        0        0      235 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/errors/invalid_state_or_province.py
--rw-r--r--   0        0        0      221 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/errors/not_found.py
--rw-r--r--   0        0        0      225 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/errors/unauthorized.py
--rw-r--r--   0        0        0      226 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/errors/unimplemented.py
--rw-r--r--   0        0        0      469 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1216 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      947 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0     1117 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      973 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      980 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      441 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/types/order_direction.py
--rw-r--r--   0        0        0      978 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      979 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0     1161 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    61621 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0     1216 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/__init__.py
--rw-r--r--   0        0        0      228 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/approval_policy/__init__.py
--rw-r--r--   0        0        0    24087 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/approval_policy/client.py
--rw-r--r--   0        0        0      305 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
--rw-r--r--   0        0        0      242 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
--rw-r--r--   0        0        0      248 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/counterparty/__init__.py
--rw-r--r--   0        0        0    32782 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/counterparty/client.py
--rw-r--r--   0        0        0      645 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/__init__.py
--rw-r--r--   0        0        0    13551 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/client.py
--rw-r--r--   0        0        0      822 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/__init__.py
--rw-r--r--   0        0        0     1220 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/codat_company_creation_request.py
--rw-r--r--   0        0        0      969 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/codat_company_response.py
--rw-r--r--   0        0        0      582 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/external_accounting_system_company_creation_request.py
--rw-r--r--   0        0        0      539 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/external_accounting_system_company_response.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/invoice/__init__.py
--rw-r--r--   0        0        0    29660 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/invoice/client.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/metadata/__init__.py
--rw-r--r--   0        0        0    17495 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/metadata/client.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/notification_policy/__init__.py
--rw-r--r--   0        0        0    14058 2023-12-19 23:38:42.999119 mercoa-0.3.7/src/mercoa/resources/entity/resources/notification_policy/client.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    33780 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/payment_method/client.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/representative/__init__.py
--rw-r--r--   0        0        0    18722 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/representative/client.py
--rw-r--r--   0        0        0      175 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/user/__init__.py
--rw-r--r--   0        0        0    27162 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/user/client.py
--rw-r--r--   0        0        0      166 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/user/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/user/resources/notification_policy/__init__.py
--rw-r--r--   0        0        0    14647 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/user/resources/notifications/__init__.py
--rw-r--r--   0        0        0    13184 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity/resources/user/resources/notifications/client.py
--rw-r--r--   0        0        0     3588 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/__init__.py
--rw-r--r--   0        0        0      378 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/errors/__init__.py
--rw-r--r--   0        0        0      224 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/errors/entity_error.py
--rw-r--r--   0        0        0      241 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/errors/entity_foreign_id_already_exists.py
--rw-r--r--   0        0        0      225 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/errors/invalid_tax_id.py
--rw-r--r--   0        0        0      234 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/errors/token_generation_failed.py
--rw-r--r--   0        0        0     5049 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/__init__.py
--rw-r--r--   0        0        0      487 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/account_type.py
--rw-r--r--   0        0        0      972 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/amount_trigger.py
--rw-r--r--   0        0        0       88 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/approval_policy_id.py
--rw-r--r--   0        0        0     1497 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/approval_policy_request.py
--rw-r--r--   0        0        0     1172 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/approval_policy_response.py
--rw-r--r--   0        0        0     1203 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
--rw-r--r--   0        0        0     1086 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/approver_rule.py
--rw-r--r--   0        0        0     2354 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/business_profile_request.py
--rw-r--r--   0        0        0     1727 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/business_type.py
--rw-r--r--   0        0        0      498 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/counterparty_network_type.py
--rw-r--r--   0        0        0     1302 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/counterparty_response.py
--rw-r--r--   0        0        0      930 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/ein.py
--rw-r--r--   0        0        0     1019 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
--rw-r--r--   0        0        0     1019 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_add_payors_request.py
--rw-r--r--   0        0        0      999 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_hide_payees_request.py
--rw-r--r--   0        0        0      999 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_hide_payors_request.py
--rw-r--r--   0        0        0       80 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_id.py
--rw-r--r--   0        0        0      908 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_metadata_response.py
--rw-r--r--   0        0        0      486 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_onboarding_link_type.py
--rw-r--r--   0        0        0     2511 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_request.py
--rw-r--r--   0        0        0     2463 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_status.py
--rw-r--r--   0        0        0     2602 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_update_request.py
--rw-r--r--   0        0        0       84 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_user_id.py
--rw-r--r--   0        0        0     1298 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_user_request.py
--rw-r--r--   0        0        0     1342 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_user_response.py
--rw-r--r--   0        0        0     1164 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_with_payment_method_response.py
--rw-r--r--   0        0        0     1417 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/find_counterparties_response.py
--rw-r--r--   0        0        0     1433 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/find_entity_response.py
--rw-r--r--   0        0        0     1460 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/find_notification_response.py
--rw-r--r--   0        0        0      784 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/identifier_list.py
--rw-r--r--   0        0        0     1495 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/individual_profile_request.py
--rw-r--r--   0        0        0     1329 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/individual_profile_response.py
--rw-r--r--   0        0        0     1042 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/metadata_trigger.py
--rw-r--r--   0        0        0       86 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/notification_id.py
--rw-r--r--   0        0        0     1311 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/notification_policy_request.py
--rw-r--r--   0        0        0     1342 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/notification_policy_response.py
--rw-r--r--   0        0        0     1409 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/notification_response.py
--rw-r--r--   0        0        0     2126 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/notification_type.py
--rw-r--r--   0        0        0     1281 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/profile_request.py
--rw-r--r--   0        0        0     1278 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/profile_response.py
--rw-r--r--   0        0        0       88 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/representative_id.py
--rw-r--r--   0        0        0     1493 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/representative_request.py
--rw-r--r--   0        0        0     1662 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/representative_response.py
--rw-r--r--   0        0        0     1581 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/responsibilities.py
--rw-r--r--   0        0        0      418 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/rule.py
--rw-r--r--   0        0        0      884 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/tax_id.py
--rw-r--r--   0        0        0     1176 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_entity_options.py
--rw-r--r--   0        0        0     1181 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py
--rw-r--r--   0        0        0     1748 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_options.py
--rw-r--r--   0        0        0     1086 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_pages_options.py
--rw-r--r--   0        0        0      980 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_style_options.py
--rw-r--r--   0        0        0     1161 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py
--rw-r--r--   0        0        0      950 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/trigger.py
--rw-r--r--   0        0        0     1066 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/user_notification_policy_response.py
--rw-r--r--   0        0        0      627 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/vendor_network.py
--rw-r--r--   0        0        0     1010 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/entity_types/types/vendor_trigger.py
--rw-r--r--   0        0        0      163 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    52914 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      154 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice/resources/approval/__init__.py
--rw-r--r--   0        0        0    10313 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice/resources/approval/client.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice/resources/comment/__init__.py
--rw-r--r--   0        0        0    21112 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice/resources/comment/client.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice/resources/document/__init__.py
--rw-r--r--   0        0        0     5041 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice/resources/document/client.py
--rw-r--r--   0        0        0     1328 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/__init__.py
--rw-r--r--   0        0        0      430 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/errors/__init__.py
--rw-r--r--   0        0        0      235 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/errors/duplicate_invoice_number.py
--rw-r--r--   0        0        0      225 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/errors/invoice_error.py
--rw-r--r--   0        0        0      230 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/errors/invoice_query_error.py
--rw-r--r--   0        0        0      231 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/errors/invoice_status_error.py
--rw-r--r--   0        0        0      227 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/errors/vendor_not_found.py
--rw-r--r--   0        0        0     1641 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/__init__.py
--rw-r--r--   0        0        0     1136 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/approval_request.py
--rw-r--r--   0        0        0     1685 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/approval_slot.py
--rw-r--r--   0        0        0     1266 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py
--rw-r--r--   0        0        0       86 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/approval_slot_id.py
--rw-r--r--   0        0        0      631 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/approver_action.py
--rw-r--r--   0        0        0     1107 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/associated_approval_action.py
--rw-r--r--   0        0        0       81 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/comment_id.py
--rw-r--r--   0        0        0     1057 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/comment_request.py
--rw-r--r--   0        0        0     1525 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/comment_response.py
--rw-r--r--   0        0        0      974 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/document_response.py
--rw-r--r--   0        0        0     1440 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/find_invoice_response.py
--rw-r--r--   0        0        0     1273 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_failure_type.py
--rw-r--r--   0        0        0     1698 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_fees_response.py
--rw-r--r--   0        0        0       81 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_id.py
--rw-r--r--   0        0        0     2195 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1933 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
--rw-r--r--   0        0        0     1195 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
--rw-r--r--   0        0        0     1367 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
--rw-r--r--   0        0        0     4796 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_request.py
--rw-r--r--   0        0        0     5397 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_response.py
--rw-r--r--   0        0        0     1623 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_status.py
--rw-r--r--   0        0        0      302 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0    10772 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      127 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/ocr/errors/__init__.py
--rw-r--r--   0        0        0      223 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/ocr/errors/ocr_failure.py
--rw-r--r--   0        0        0      367 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1047 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/ocr/types/cloud_mailin_attachment.py
--rw-r--r--   0        0        0     1173 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/ocr/types/cloud_mailin_envelope.py
--rw-r--r--   0        0        0     1171 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/ocr/types/cloud_mailin_request.py
--rw-r--r--   0        0        0     1381 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      157 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0    17026 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0      148 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization/resources/notification_configuration/__init__.py
--rw-r--r--   0        0        0    17642 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization/resources/notification_configuration/client.py
--rw-r--r--   0        0        0     2209 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/__init__.py
--rw-r--r--   0        0        0     3242 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/__init__.py
--rw-r--r--   0        0        0     1471 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/business_onboarding_options.py
--rw-r--r--   0        0        0      961 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/codat_provider_request.py
--rw-r--r--   0        0        0     1071 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/color_scheme_request.py
--rw-r--r--   0        0        0     1072 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/color_scheme_response.py
--rw-r--r--   0        0        0     1104 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_log_response.py
--rw-r--r--   0        0        0     1055 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_provider_request.py
--rw-r--r--   0        0        0     1059 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_provider_response.py
--rw-r--r--   0        0        0      785 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_sender_provider.py
--rw-r--r--   0        0        0     1175 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_sender_request.py
--rw-r--r--   0        0        0     1167 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_sender_response.py
--rw-r--r--   0        0        0      539 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/external_accounting_system_provider_request.py
--rw-r--r--   0        0        0     1301 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/individual_onboarding_options.py
--rw-r--r--   0        0        0      897 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py
--rw-r--r--   0        0        0     1031 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py
--rw-r--r--   0        0        0     2043 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/metadata_schema.py
--rw-r--r--   0        0        0     2460 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/metadata_show_conditions.py
--rw-r--r--   0        0        0      912 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/metadata_type.py
--rw-r--r--   0        0        0      751 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/notification_configuration_request.py
--rw-r--r--   0        0        0      757 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/notification_configuration_response.py
--rw-r--r--   0        0        0      910 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/onboarding_option.py
--rw-r--r--   0        0        0     1343 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/onboarding_options_request.py
--rw-r--r--   0        0        0     1276 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/onboarding_options_response.py
--rw-r--r--   0        0        0       86 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/organization_id.py
--rw-r--r--   0        0        0     2312 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/organization_request.py
--rw-r--r--   0        0        0     2192 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/organization_response.py
--rw-r--r--   0        0        0     1587 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_methods_request.py
--rw-r--r--   0        0        0     1593 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_methods_response.py
--rw-r--r--   0        0        0      972 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1270 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_rail_request.py
--rw-r--r--   0        0        0      870 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_rail_response.py
--rw-r--r--   0        0        0       65 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0    20898 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0     2506 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/__init__.py
--rw-r--r--   0        0        0      152 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/errors/__init__.py
--rw-r--r--   0        0        0      231 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/errors/payment_method_error.py
--rw-r--r--   0        0        0     3289 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/__init__.py
--rw-r--r--   0        0        0     1532 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_account_request.py
--rw-r--r--   0        0        0     1383 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_account_response.py
--rw-r--r--   0        0        0     1064 2023-12-19 23:38:43.003119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_account_update_request.py
--rw-r--r--   0        0        0      960 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_type.py
--rw-r--r--   0        0        0      819 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/card_brand.py
--rw-r--r--   0        0        0     1336 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/card_request.py
--rw-r--r--   0        0        0     1325 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/card_response.py
--rw-r--r--   0        0        0      750 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/card_type.py
--rw-r--r--   0        0        0     1347 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/check_request.py
--rw-r--r--   0        0        0     1351 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/check_response.py
--rw-r--r--   0        0        0    22179 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/currency_code.py
--rw-r--r--   0        0        0     1699 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1849 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
--rw-r--r--   0        0        0     1770 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
--rw-r--r--   0        0        0     1588 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_base_request.py
--rw-r--r--   0        0        0     1634 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_base_response.py
--rw-r--r--   0        0        0       87 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_id.py
--rw-r--r--   0        0        0     1372 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_request.py
--rw-r--r--   0        0        0     1406 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_response.py
--rw-r--r--   0        0        0     2047 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
--rw-r--r--   0        0        0     1417 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1670 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1804 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
--rw-r--r--   0        0        0     1229 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_type.py
--rw-r--r--   0        0        0     1490 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
--rw-r--r--   0        0        0     1143 2023-12-19 23:38:43.007119 mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/plaid_link_request.py
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1930 2023-12-21 23:38:21.479988 mercoa-0.3.8/README.md
+-rw-r--r--   0        0        0      399 2023-12-21 23:38:21.483988 mercoa-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0    11057 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     3241 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/client.py
+-rw-r--r--   0        0        0      519 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1381 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      157 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/py.typed
+-rw-r--r--   0        0        0    11152 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     5038 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0     1083 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0     1069 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      724 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      657 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      237 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
+-rw-r--r--   0        0        0      221 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/errors/auth_header_missing_error.py
+-rw-r--r--   0        0        0      222 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/errors/forbidden.py
+-rw-r--r--   0        0        0      230 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/errors/invalid_postal_code.py
+-rw-r--r--   0        0        0      235 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/errors/invalid_state_or_province.py
+-rw-r--r--   0        0        0      221 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/errors/not_found.py
+-rw-r--r--   0        0        0      225 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/errors/unauthorized.py
+-rw-r--r--   0        0        0      226 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/errors/unimplemented.py
+-rw-r--r--   0        0        0      469 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1216 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      947 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0     1117 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      973 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      980 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      441 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/types/order_direction.py
+-rw-r--r--   0        0        0      978 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      979 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0     1161 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    61621 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0     1216 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/__init__.py
+-rw-r--r--   0        0        0      228 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/approval_policy/__init__.py
+-rw-r--r--   0        0        0    24087 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/approval_policy/client.py
+-rw-r--r--   0        0        0      305 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
+-rw-r--r--   0        0        0      242 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
+-rw-r--r--   0        0        0      248 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0    32782 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/counterparty/client.py
+-rw-r--r--   0        0        0      645 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/__init__.py
+-rw-r--r--   0        0        0    13551 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/client.py
+-rw-r--r--   0        0        0      822 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/__init__.py
+-rw-r--r--   0        0        0     1220 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/codat_company_creation_request.py
+-rw-r--r--   0        0        0      969 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/codat_company_response.py
+-rw-r--r--   0        0        0      582 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/external_accounting_system_company_creation_request.py
+-rw-r--r--   0        0        0      539 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/external_accounting_system_company_response.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    29660 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/invoice/client.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/metadata/__init__.py
+-rw-r--r--   0        0        0    17495 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/metadata/client.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/notification_policy/__init__.py
+-rw-r--r--   0        0        0    14058 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/notification_policy/client.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    38532 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/payment_method/client.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/representative/__init__.py
+-rw-r--r--   0        0        0    18722 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/representative/client.py
+-rw-r--r--   0        0        0      175 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/user/__init__.py
+-rw-r--r--   0        0        0    27162 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/user/client.py
+-rw-r--r--   0        0        0      166 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/user/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/user/resources/notification_policy/__init__.py
+-rw-r--r--   0        0        0    14647 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/user/resources/notifications/__init__.py
+-rw-r--r--   0        0        0    13184 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity/resources/user/resources/notifications/client.py
+-rw-r--r--   0        0        0     3588 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/__init__.py
+-rw-r--r--   0        0        0      378 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/errors/__init__.py
+-rw-r--r--   0        0        0      224 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/errors/entity_error.py
+-rw-r--r--   0        0        0      241 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/errors/entity_foreign_id_already_exists.py
+-rw-r--r--   0        0        0      225 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/errors/invalid_tax_id.py
+-rw-r--r--   0        0        0      234 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/errors/token_generation_failed.py
+-rw-r--r--   0        0        0     5049 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/account_type.py
+-rw-r--r--   0        0        0      972 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/amount_trigger.py
+-rw-r--r--   0        0        0       88 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/approval_policy_id.py
+-rw-r--r--   0        0        0     1497 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/approval_policy_request.py
+-rw-r--r--   0        0        0     1172 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/approval_policy_response.py
+-rw-r--r--   0        0        0     1203 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
+-rw-r--r--   0        0        0     1086 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/approver_rule.py
+-rw-r--r--   0        0        0     2354 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/business_profile_request.py
+-rw-r--r--   0        0        0     1727 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/business_type.py
+-rw-r--r--   0        0        0      498 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/counterparty_network_type.py
+-rw-r--r--   0        0        0     1302 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/counterparty_response.py
+-rw-r--r--   0        0        0      930 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/ein.py
+-rw-r--r--   0        0        0     1019 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
+-rw-r--r--   0        0        0     1019 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_add_payors_request.py
+-rw-r--r--   0        0        0      999 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_hide_payees_request.py
+-rw-r--r--   0        0        0      999 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_hide_payors_request.py
+-rw-r--r--   0        0        0       80 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_id.py
+-rw-r--r--   0        0        0      908 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_metadata_response.py
+-rw-r--r--   0        0        0      486 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_onboarding_link_type.py
+-rw-r--r--   0        0        0     2511 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_request.py
+-rw-r--r--   0        0        0     2463 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_status.py
+-rw-r--r--   0        0        0     2602 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_update_request.py
+-rw-r--r--   0        0        0       84 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_user_id.py
+-rw-r--r--   0        0        0     1298 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_user_request.py
+-rw-r--r--   0        0        0     1342 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_user_response.py
+-rw-r--r--   0        0        0     1164 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_with_payment_method_response.py
+-rw-r--r--   0        0        0     1417 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/find_counterparties_response.py
+-rw-r--r--   0        0        0     1433 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/find_entity_response.py
+-rw-r--r--   0        0        0     1460 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/find_notification_response.py
+-rw-r--r--   0        0        0      784 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/identifier_list.py
+-rw-r--r--   0        0        0     1495 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1329 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/individual_profile_response.py
+-rw-r--r--   0        0        0     1042 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/metadata_trigger.py
+-rw-r--r--   0        0        0       86 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/notification_id.py
+-rw-r--r--   0        0        0     1311 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/notification_policy_request.py
+-rw-r--r--   0        0        0     1342 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/notification_policy_response.py
+-rw-r--r--   0        0        0     1409 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/notification_response.py
+-rw-r--r--   0        0        0     2126 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/notification_type.py
+-rw-r--r--   0        0        0     1281 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/profile_request.py
+-rw-r--r--   0        0        0     1278 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/profile_response.py
+-rw-r--r--   0        0        0       88 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/representative_id.py
+-rw-r--r--   0        0        0     1493 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/representative_request.py
+-rw-r--r--   0        0        0     1662 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/representative_response.py
+-rw-r--r--   0        0        0     1581 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/responsibilities.py
+-rw-r--r--   0        0        0      418 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/rule.py
+-rw-r--r--   0        0        0      884 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/tax_id.py
+-rw-r--r--   0        0        0     1176 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_entity_options.py
+-rw-r--r--   0        0        0      977 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py
+-rw-r--r--   0        0        0     1748 2023-12-21 23:38:21.483988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_options.py
+-rw-r--r--   0        0        0     1086 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_pages_options.py
+-rw-r--r--   0        0        0      980 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_style_options.py
+-rw-r--r--   0        0        0     1161 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py
+-rw-r--r--   0        0        0      950 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/trigger.py
+-rw-r--r--   0        0        0     1066 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/user_notification_policy_response.py
+-rw-r--r--   0        0        0      627 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/vendor_network.py
+-rw-r--r--   0        0        0     1010 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/entity_types/types/vendor_trigger.py
+-rw-r--r--   0        0        0      163 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    52914 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      154 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice/resources/approval/__init__.py
+-rw-r--r--   0        0        0    10313 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice/resources/approval/client.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice/resources/comment/__init__.py
+-rw-r--r--   0        0        0    21112 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice/resources/comment/client.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice/resources/document/__init__.py
+-rw-r--r--   0        0        0     5041 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice/resources/document/client.py
+-rw-r--r--   0        0        0     1328 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/__init__.py
+-rw-r--r--   0        0        0      430 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/errors/__init__.py
+-rw-r--r--   0        0        0      235 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/errors/duplicate_invoice_number.py
+-rw-r--r--   0        0        0      225 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/errors/invoice_error.py
+-rw-r--r--   0        0        0      230 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/errors/invoice_query_error.py
+-rw-r--r--   0        0        0      231 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/errors/invoice_status_error.py
+-rw-r--r--   0        0        0      227 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/errors/vendor_not_found.py
+-rw-r--r--   0        0        0     1641 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/__init__.py
+-rw-r--r--   0        0        0     1136 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/approval_request.py
+-rw-r--r--   0        0        0     1685 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/approval_slot.py
+-rw-r--r--   0        0        0     1266 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py
+-rw-r--r--   0        0        0       86 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/approval_slot_id.py
+-rw-r--r--   0        0        0      631 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/approver_action.py
+-rw-r--r--   0        0        0     1107 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/associated_approval_action.py
+-rw-r--r--   0        0        0       81 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/comment_id.py
+-rw-r--r--   0        0        0     1057 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/comment_request.py
+-rw-r--r--   0        0        0     1525 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/comment_response.py
+-rw-r--r--   0        0        0      974 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/document_response.py
+-rw-r--r--   0        0        0     1440 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/find_invoice_response.py
+-rw-r--r--   0        0        0     1273 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_failure_type.py
+-rw-r--r--   0        0        0     1698 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_fees_response.py
+-rw-r--r--   0        0        0       81 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_id.py
+-rw-r--r--   0        0        0     2195 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1933 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     1195 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0     1367 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
+-rw-r--r--   0        0        0     4796 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_request.py
+-rw-r--r--   0        0        0     5397 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_response.py
+-rw-r--r--   0        0        0     1623 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_status.py
+-rw-r--r--   0        0        0      302 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0    10772 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      127 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/ocr/errors/__init__.py
+-rw-r--r--   0        0        0      223 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/ocr/errors/ocr_failure.py
+-rw-r--r--   0        0        0      367 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1047 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/ocr/types/cloud_mailin_attachment.py
+-rw-r--r--   0        0        0     1173 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/ocr/types/cloud_mailin_envelope.py
+-rw-r--r--   0        0        0     1171 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/ocr/types/cloud_mailin_request.py
+-rw-r--r--   0        0        0     1381 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      157 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0    17026 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0      148 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization/resources/notification_configuration/__init__.py
+-rw-r--r--   0        0        0    17642 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization/resources/notification_configuration/client.py
+-rw-r--r--   0        0        0     2209 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/__init__.py
+-rw-r--r--   0        0        0     3242 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/__init__.py
+-rw-r--r--   0        0        0     1471 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/business_onboarding_options.py
+-rw-r--r--   0        0        0      961 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/codat_provider_request.py
+-rw-r--r--   0        0        0     1071 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/color_scheme_request.py
+-rw-r--r--   0        0        0     1072 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/color_scheme_response.py
+-rw-r--r--   0        0        0     1104 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_log_response.py
+-rw-r--r--   0        0        0     1055 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_provider_request.py
+-rw-r--r--   0        0        0     1059 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_provider_response.py
+-rw-r--r--   0        0        0      785 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1175 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_sender_request.py
+-rw-r--r--   0        0        0     1167 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_sender_response.py
+-rw-r--r--   0        0        0      539 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/external_accounting_system_provider_request.py
+-rw-r--r--   0        0        0     1301 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/individual_onboarding_options.py
+-rw-r--r--   0        0        0      897 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py
+-rw-r--r--   0        0        0     1031 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py
+-rw-r--r--   0        0        0     2043 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/metadata_schema.py
+-rw-r--r--   0        0        0     2460 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/metadata_show_conditions.py
+-rw-r--r--   0        0        0      912 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/metadata_type.py
+-rw-r--r--   0        0        0      751 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/notification_configuration_request.py
+-rw-r--r--   0        0        0      757 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/notification_configuration_response.py
+-rw-r--r--   0        0        0      910 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/onboarding_option.py
+-rw-r--r--   0        0        0     1343 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/onboarding_options_request.py
+-rw-r--r--   0        0        0     1276 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/onboarding_options_response.py
+-rw-r--r--   0        0        0       86 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/organization_id.py
+-rw-r--r--   0        0        0     2312 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/organization_request.py
+-rw-r--r--   0        0        0     2192 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/organization_response.py
+-rw-r--r--   0        0        0     1587 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1593 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_methods_response.py
+-rw-r--r--   0        0        0      972 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1270 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_rail_request.py
+-rw-r--r--   0        0        0      870 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_rail_response.py
+-rw-r--r--   0        0        0       65 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0    20898 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0     2824 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/__init__.py
+-rw-r--r--   0        0        0      152 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/errors/__init__.py
+-rw-r--r--   0        0        0      231 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/errors/payment_method_error.py
+-rw-r--r--   0        0        0     3647 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/__init__.py
+-rw-r--r--   0        0        0     1532 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_account_request.py
+-rw-r--r--   0        0        0     1383 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_account_response.py
+-rw-r--r--   0        0        0     1064 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_account_update_request.py
+-rw-r--r--   0        0        0      960 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_type.py
+-rw-r--r--   0        0        0      819 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/card_brand.py
+-rw-r--r--   0        0        0     1336 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/card_request.py
+-rw-r--r--   0        0        0     1325 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/card_type.py
+-rw-r--r--   0        0        0     1347 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/check_request.py
+-rw-r--r--   0        0        0     1351 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/check_response.py
+-rw-r--r--   0        0        0    22179 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/currency_code.py
+-rw-r--r--   0        0        0     1699 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1849 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0     1770 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
+-rw-r--r--   0        0        0     1058 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_balance_response.py
+-rw-r--r--   0        0        0     1588 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_base_request.py
+-rw-r--r--   0        0        0     1634 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_base_response.py
+-rw-r--r--   0        0        0       87 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_id.py
+-rw-r--r--   0        0        0     1722 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_request.py
+-rw-r--r--   0        0        0     1748 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_response.py
+-rw-r--r--   0        0        0     2047 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0     1417 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1670 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1804 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0     1400 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_type.py
+-rw-r--r--   0        0        0     1773 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
+-rw-r--r--   0        0        0     1143 2023-12-21 23:38:21.487988 mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/plaid_link_request.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.3.8/PKG-INFO
```

### Comparing `mercoa-0.3.7/README.md` & `mercoa-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,55 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .resources import (
-    AccountType,
+from . import (
+    bank_lookup,
+    commons,
+    entity,
+    entity_types,
+    invoice,
+    invoice_types,
+    ocr,
+    organization,
+    organization_types,
+    payment_method_schema,
+    payment_method_types,
+)
+from .bank_lookup import BankAddress, BankLookupResponse
+from .commons import (
     Address,
+    AuthHeaderMalformedError,
+    AuthHeaderMissingError,
+    BirthDate,
+    Forbidden,
+    FullName,
+    IndividualGovernmentId,
+    InvalidPostalCode,
+    InvalidStateOrProvince,
+    Itin,
+    NotFound,
+    OrderDirection,
+    PhoneNumber,
+    Ssn,
+    Unauthorized,
+    Unimplemented,
+)
+from .entity_types import (
+    AccountType,
     AmountTrigger,
     ApprovalPolicyId,
     ApprovalPolicyRequest,
     ApprovalPolicyResponse,
     ApprovalPolicyUpdateRequest,
-    ApprovalRequest,
-    ApprovalSlot,
-    ApprovalSlotAssignment,
-    ApprovalSlotId,
-    ApproverAction,
     ApproverRule,
-    AssociatedApprovalAction,
-    AuthHeaderMalformedError,
-    AuthHeaderMissingError,
-    BankAccountRequest,
-    BankAccountResponse,
-    BankAccountUpdateRequest,
-    BankAddress,
-    BankLookupResponse,
-    BankStatus,
-    BankType,
-    BirthDate,
-    BusinessOnboardingOptions,
     BusinessProfileRequest,
     BusinessProfileResponse,
     BusinessType,
-    CardBrand,
-    CardRequest,
-    CardResponse,
-    CardType,
-    CheckRequest,
-    CheckResponse,
-    CloudMailinAttachment,
-    CloudMailinEnvelope,
-    CloudMailinRequest,
-    CodatProviderRequest,
-    ColorSchemeRequest,
-    ColorSchemeResponse,
-    CommentId,
-    CommentRequest,
-    CommentResponse,
     CounterpartyNetworkType,
     CounterpartyResponse,
-    CurrencyCode,
-    CustomPaymentMethodRequest,
-    CustomPaymentMethodResponse,
-    CustomPaymentMethodUpdateRequest,
-    DocumentResponse,
-    DuplicateInvoiceNumber,
     Ein,
-    EmailLogResponse,
-    EmailProviderRequest,
-    EmailProviderResponse,
-    EmailSenderProvider,
-    EmailSenderRequest,
-    EmailSenderResponse,
     EntityAddPayeesRequest,
     EntityAddPayorsRequest,
     EntityError,
     EntityForeignIdAlreadyExists,
     EntityHidePayeesRequest,
     EntityHidePayorsRequest,
     EntityId,
@@ -72,144 +59,165 @@
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
     EntityUserId,
     EntityUserRequest,
     EntityUserResponse,
     EntityWithPaymentMethodResponse,
-    ExternalAccountingSystemProviderRequest,
-    ExternalAccountingSystemProviderRequest_Codat,
     FindCounterpartiesResponse,
     FindEntityResponse,
-    FindInvoiceResponse,
     FindNotificationResponse,
-    Forbidden,
-    FullName,
     IdentifierList,
     IdentifierList_RolesList,
     IdentifierList_UserList,
-    IndividualGovernmentId,
-    IndividualOnboardingOptions,
     IndividualProfileRequest,
     IndividualProfileResponse,
-    InvalidPostalCode,
-    InvalidStateOrProvince,
     InvalidTaxId,
+    MetadataTrigger,
+    NotificationId,
+    NotificationPolicyRequest,
+    NotificationPolicyResponse,
+    NotificationResponse,
+    NotificationType,
+    ProfileRequest,
+    ProfileResponse,
+    RepresentativeId,
+    RepresentativeRequest,
+    RepresentativeResponse,
+    Responsibilities,
+    Rule,
+    Rule_Approver,
+    TaxId,
+    TokenGenerationEntityOptions,
+    TokenGenerationFailed,
+    TokenGenerationInvoiceOptions,
+    TokenGenerationOptions,
+    TokenGenerationPagesOptions,
+    TokenGenerationStyleOptions,
+    TokenGenerationVendorOptions,
+    Trigger,
+    Trigger_Amount,
+    Trigger_Metadata,
+    Trigger_Vendor,
+    UserNotificationPolicyResponse,
+    VendorNetwork,
+    VendorTrigger,
+)
+from .invoice_types import (
+    ApprovalRequest,
+    ApprovalSlot,
+    ApprovalSlotAssignment,
+    ApprovalSlotId,
+    ApproverAction,
+    AssociatedApprovalAction,
+    CommentId,
+    CommentRequest,
+    CommentResponse,
+    DocumentResponse,
+    DuplicateInvoiceNumber,
+    FindInvoiceResponse,
     InvoiceError,
     InvoiceFailureType,
     InvoiceFeesResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
-    InvoiceNotificationConfigurationRequest,
-    InvoiceNotificationConfigurationResponse,
     InvoiceOrderByField,
     InvoiceQueryError,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     InvoiceStatusError,
-    Itin,
+    VendorNotFound,
+)
+from .ocr import CloudMailinAttachment, CloudMailinEnvelope, CloudMailinRequest, OcrFailure, OcrResponse
+from .organization_types import (
+    BusinessOnboardingOptions,
+    CodatProviderRequest,
+    ColorSchemeRequest,
+    ColorSchemeResponse,
+    EmailLogResponse,
+    EmailProviderRequest,
+    EmailProviderResponse,
+    EmailSenderProvider,
+    EmailSenderRequest,
+    EmailSenderResponse,
+    ExternalAccountingSystemProviderRequest,
+    ExternalAccountingSystemProviderRequest_Codat,
+    IndividualOnboardingOptions,
+    InvoiceNotificationConfigurationRequest,
+    InvoiceNotificationConfigurationResponse,
     MetadataSchema,
     MetadataShowConditions,
-    MetadataTrigger,
     MetadataType,
-    NotFound,
     NotificationConfigurationRequest,
     NotificationConfigurationRequest_Invoice,
     NotificationConfigurationResponse,
     NotificationConfigurationResponse_Invoice,
-    NotificationId,
-    NotificationPolicyRequest,
-    NotificationPolicyResponse,
-    NotificationResponse,
-    NotificationType,
-    OcrFailure,
-    OcrResponse,
     OnboardingOption,
     OnboardingOptionsRequest,
     OnboardingOptionsResponse,
-    OrderDirection,
     OrganizationId,
     OrganizationRequest,
     OrganizationResponse,
+    PaymentMethodsRequest,
+    PaymentMethodsResponse,
+    PaymentRailMarkup,
+    PaymentRailMarkupType,
+    PaymentRailRequest,
+    PaymentRailResponse,
+)
+from .payment_method_types import (
+    BankAccountRequest,
+    BankAccountResponse,
+    BankAccountUpdateRequest,
+    BankStatus,
+    BankType,
+    CardBrand,
+    CardRequest,
+    CardResponse,
+    CardType,
+    CheckRequest,
+    CheckResponse,
+    CurrencyCode,
+    CustomPaymentMethodRequest,
+    CustomPaymentMethodResponse,
+    CustomPaymentMethodUpdateRequest,
+    PaymentMethodBalanceResponse,
     PaymentMethodBaseRequest,
     PaymentMethodBaseResponse,
     PaymentMethodError,
     PaymentMethodId,
     PaymentMethodRequest,
     PaymentMethodRequest_BankAccount,
     PaymentMethodRequest_Card,
     PaymentMethodRequest_Check,
     PaymentMethodRequest_Custom,
+    PaymentMethodRequest_OffPlatform,
     PaymentMethodResponse,
     PaymentMethodResponse_BankAccount,
     PaymentMethodResponse_Card,
     PaymentMethodResponse_Check,
     PaymentMethodResponse_Custom,
+    PaymentMethodResponse_OffPlatform,
     PaymentMethodSchemaField,
     PaymentMethodSchemaFieldType,
     PaymentMethodSchemaId,
     PaymentMethodSchemaRequest,
     PaymentMethodSchemaResponse,
     PaymentMethodType,
     PaymentMethodUpdateRequest,
     PaymentMethodUpdateRequest_BankAccount,
     PaymentMethodUpdateRequest_Card,
     PaymentMethodUpdateRequest_Check,
     PaymentMethodUpdateRequest_Custom,
-    PaymentMethodsRequest,
-    PaymentMethodsResponse,
-    PaymentRailMarkup,
-    PaymentRailMarkupType,
-    PaymentRailRequest,
-    PaymentRailResponse,
-    PhoneNumber,
+    PaymentMethodUpdateRequest_OffPlatform,
     PlaidLinkRequest,
-    ProfileRequest,
-    ProfileResponse,
-    RepresentativeId,
-    RepresentativeRequest,
-    RepresentativeResponse,
-    Responsibilities,
-    Rule,
-    Rule_Approver,
-    Ssn,
-    TaxId,
-    TokenGenerationEntityOptions,
-    TokenGenerationFailed,
-    TokenGenerationInvoiceOptions,
-    TokenGenerationOptions,
-    TokenGenerationPagesOptions,
-    TokenGenerationStyleOptions,
-    TokenGenerationVendorOptions,
-    Trigger,
-    Trigger_Amount,
-    Trigger_Metadata,
-    Trigger_Vendor,
-    Unauthorized,
-    Unimplemented,
-    UserNotificationPolicyResponse,
-    VendorNetwork,
-    VendorNotFound,
-    VendorTrigger,
-    bank_lookup,
-    commons,
-    entity,
-    entity_types,
-    invoice,
-    invoice_types,
-    ocr,
-    organization,
-    organization_types,
-    payment_method_schema,
-    payment_method_types,
 )
-from .environment import MercoaEnvironment
 
 __all__ = [
     "AccountType",
     "Address",
     "AmountTrigger",
     "ApprovalPolicyId",
     "ApprovalPolicyRequest",
@@ -313,15 +321,14 @@
     "InvoiceOrderByField",
     "InvoiceQueryError",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "InvoiceStatusError",
     "Itin",
-    "MercoaEnvironment",
     "MetadataSchema",
     "MetadataShowConditions",
     "MetadataTrigger",
     "MetadataType",
     "NotFound",
     "NotificationConfigurationRequest",
     "NotificationConfigurationRequest_Invoice",
@@ -337,39 +344,43 @@
     "OnboardingOption",
     "OnboardingOptionsRequest",
     "OnboardingOptionsResponse",
     "OrderDirection",
     "OrganizationId",
     "OrganizationRequest",
     "OrganizationResponse",
+    "PaymentMethodBalanceResponse",
     "PaymentMethodBaseRequest",
     "PaymentMethodBaseResponse",
     "PaymentMethodError",
     "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodRequest_BankAccount",
     "PaymentMethodRequest_Card",
     "PaymentMethodRequest_Check",
     "PaymentMethodRequest_Custom",
+    "PaymentMethodRequest_OffPlatform",
     "PaymentMethodResponse",
     "PaymentMethodResponse_BankAccount",
     "PaymentMethodResponse_Card",
     "PaymentMethodResponse_Check",
     "PaymentMethodResponse_Custom",
+    "PaymentMethodResponse_OffPlatform",
     "PaymentMethodSchemaField",
     "PaymentMethodSchemaFieldType",
     "PaymentMethodSchemaId",
     "PaymentMethodSchemaRequest",
     "PaymentMethodSchemaResponse",
     "PaymentMethodType",
     "PaymentMethodUpdateRequest",
     "PaymentMethodUpdateRequest_BankAccount",
     "PaymentMethodUpdateRequest_Card",
     "PaymentMethodUpdateRequest_Check",
     "PaymentMethodUpdateRequest_Custom",
+    "PaymentMethodUpdateRequest_OffPlatform",
     "PaymentMethodsRequest",
     "PaymentMethodsResponse",
     "PaymentRailMarkup",
     "PaymentRailMarkupType",
     "PaymentRailRequest",
     "PaymentRailResponse",
     "PhoneNumber",
```

### Comparing `mercoa-0.3.7/src/mercoa/client.py` & `mercoa-0.3.8/src/mercoa/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/core/__init__.py` & `mercoa-0.3.8/src/mercoa/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/core/client_wrapper.py` & `mercoa-0.3.8/src/mercoa/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._token = token
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "mercoa",
-            "X-Fern-SDK-Version": "v0.3.7",
+            "X-Fern-SDK-Version": "v0.3.8",
         }
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
         if isinstance(self._token, str):
             return self._token
```

### Comparing `mercoa-0.3.7/src/mercoa/core/datetime_utils.py` & `mercoa-0.3.8/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.3.8/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/__init__.py` & `mercoa-0.3.8/src/mercoa/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from . import (
-    bank_lookup,
-    commons,
-    entity,
-    entity_types,
-    invoice,
-    invoice_types,
-    ocr,
-    organization,
-    organization_types,
-    payment_method_schema,
-    payment_method_types,
-)
-from .bank_lookup import BankAddress, BankLookupResponse
-from .commons import (
-    Address,
-    AuthHeaderMalformedError,
-    AuthHeaderMissingError,
-    BirthDate,
-    Forbidden,
-    FullName,
-    IndividualGovernmentId,
-    InvalidPostalCode,
-    InvalidStateOrProvince,
-    Itin,
-    NotFound,
-    OrderDirection,
-    PhoneNumber,
-    Ssn,
-    Unauthorized,
-    Unimplemented,
-)
-from .entity_types import (
+from .resources import (
     AccountType,
+    Address,
     AmountTrigger,
     ApprovalPolicyId,
     ApprovalPolicyRequest,
     ApprovalPolicyResponse,
     ApprovalPolicyUpdateRequest,
+    ApprovalRequest,
+    ApprovalSlot,
+    ApprovalSlotAssignment,
+    ApprovalSlotId,
+    ApproverAction,
     ApproverRule,
+    AssociatedApprovalAction,
+    AuthHeaderMalformedError,
+    AuthHeaderMissingError,
+    BankAccountRequest,
+    BankAccountResponse,
+    BankAccountUpdateRequest,
+    BankAddress,
+    BankLookupResponse,
+    BankStatus,
+    BankType,
+    BirthDate,
+    BusinessOnboardingOptions,
     BusinessProfileRequest,
     BusinessProfileResponse,
     BusinessType,
+    CardBrand,
+    CardRequest,
+    CardResponse,
+    CardType,
+    CheckRequest,
+    CheckResponse,
+    CloudMailinAttachment,
+    CloudMailinEnvelope,
+    CloudMailinRequest,
+    CodatProviderRequest,
+    ColorSchemeRequest,
+    ColorSchemeResponse,
+    CommentId,
+    CommentRequest,
+    CommentResponse,
     CounterpartyNetworkType,
     CounterpartyResponse,
+    CurrencyCode,
+    CustomPaymentMethodRequest,
+    CustomPaymentMethodResponse,
+    CustomPaymentMethodUpdateRequest,
+    DocumentResponse,
+    DuplicateInvoiceNumber,
     Ein,
+    EmailLogResponse,
+    EmailProviderRequest,
+    EmailProviderResponse,
+    EmailSenderProvider,
+    EmailSenderRequest,
+    EmailSenderResponse,
     EntityAddPayeesRequest,
     EntityAddPayorsRequest,
     EntityError,
     EntityForeignIdAlreadyExists,
     EntityHidePayeesRequest,
     EntityHidePayorsRequest,
     EntityId,
@@ -59,161 +72,148 @@
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
     EntityUserId,
     EntityUserRequest,
     EntityUserResponse,
     EntityWithPaymentMethodResponse,
+    ExternalAccountingSystemProviderRequest,
+    ExternalAccountingSystemProviderRequest_Codat,
     FindCounterpartiesResponse,
     FindEntityResponse,
+    FindInvoiceResponse,
     FindNotificationResponse,
+    Forbidden,
+    FullName,
     IdentifierList,
     IdentifierList_RolesList,
     IdentifierList_UserList,
+    IndividualGovernmentId,
+    IndividualOnboardingOptions,
     IndividualProfileRequest,
     IndividualProfileResponse,
+    InvalidPostalCode,
+    InvalidStateOrProvince,
     InvalidTaxId,
-    MetadataTrigger,
-    NotificationId,
-    NotificationPolicyRequest,
-    NotificationPolicyResponse,
-    NotificationResponse,
-    NotificationType,
-    ProfileRequest,
-    ProfileResponse,
-    RepresentativeId,
-    RepresentativeRequest,
-    RepresentativeResponse,
-    Responsibilities,
-    Rule,
-    Rule_Approver,
-    TaxId,
-    TokenGenerationEntityOptions,
-    TokenGenerationFailed,
-    TokenGenerationInvoiceOptions,
-    TokenGenerationOptions,
-    TokenGenerationPagesOptions,
-    TokenGenerationStyleOptions,
-    TokenGenerationVendorOptions,
-    Trigger,
-    Trigger_Amount,
-    Trigger_Metadata,
-    Trigger_Vendor,
-    UserNotificationPolicyResponse,
-    VendorNetwork,
-    VendorTrigger,
-)
-from .invoice_types import (
-    ApprovalRequest,
-    ApprovalSlot,
-    ApprovalSlotAssignment,
-    ApprovalSlotId,
-    ApproverAction,
-    AssociatedApprovalAction,
-    CommentId,
-    CommentRequest,
-    CommentResponse,
-    DocumentResponse,
-    DuplicateInvoiceNumber,
-    FindInvoiceResponse,
     InvoiceError,
     InvoiceFailureType,
     InvoiceFeesResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
+    InvoiceNotificationConfigurationRequest,
+    InvoiceNotificationConfigurationResponse,
     InvoiceOrderByField,
     InvoiceQueryError,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     InvoiceStatusError,
-    VendorNotFound,
-)
-from .ocr import CloudMailinAttachment, CloudMailinEnvelope, CloudMailinRequest, OcrFailure, OcrResponse
-from .organization_types import (
-    BusinessOnboardingOptions,
-    CodatProviderRequest,
-    ColorSchemeRequest,
-    ColorSchemeResponse,
-    EmailLogResponse,
-    EmailProviderRequest,
-    EmailProviderResponse,
-    EmailSenderProvider,
-    EmailSenderRequest,
-    EmailSenderResponse,
-    ExternalAccountingSystemProviderRequest,
-    ExternalAccountingSystemProviderRequest_Codat,
-    IndividualOnboardingOptions,
-    InvoiceNotificationConfigurationRequest,
-    InvoiceNotificationConfigurationResponse,
+    Itin,
     MetadataSchema,
     MetadataShowConditions,
+    MetadataTrigger,
     MetadataType,
+    NotFound,
     NotificationConfigurationRequest,
     NotificationConfigurationRequest_Invoice,
     NotificationConfigurationResponse,
     NotificationConfigurationResponse_Invoice,
+    NotificationId,
+    NotificationPolicyRequest,
+    NotificationPolicyResponse,
+    NotificationResponse,
+    NotificationType,
+    OcrFailure,
+    OcrResponse,
     OnboardingOption,
     OnboardingOptionsRequest,
     OnboardingOptionsResponse,
+    OrderDirection,
     OrganizationId,
     OrganizationRequest,
     OrganizationResponse,
-    PaymentMethodsRequest,
-    PaymentMethodsResponse,
-    PaymentRailMarkup,
-    PaymentRailMarkupType,
-    PaymentRailRequest,
-    PaymentRailResponse,
-)
-from .payment_method_types import (
-    BankAccountRequest,
-    BankAccountResponse,
-    BankAccountUpdateRequest,
-    BankStatus,
-    BankType,
-    CardBrand,
-    CardRequest,
-    CardResponse,
-    CardType,
-    CheckRequest,
-    CheckResponse,
-    CurrencyCode,
-    CustomPaymentMethodRequest,
-    CustomPaymentMethodResponse,
-    CustomPaymentMethodUpdateRequest,
+    PaymentMethodBalanceResponse,
     PaymentMethodBaseRequest,
     PaymentMethodBaseResponse,
     PaymentMethodError,
     PaymentMethodId,
     PaymentMethodRequest,
     PaymentMethodRequest_BankAccount,
     PaymentMethodRequest_Card,
     PaymentMethodRequest_Check,
     PaymentMethodRequest_Custom,
+    PaymentMethodRequest_OffPlatform,
     PaymentMethodResponse,
     PaymentMethodResponse_BankAccount,
     PaymentMethodResponse_Card,
     PaymentMethodResponse_Check,
     PaymentMethodResponse_Custom,
+    PaymentMethodResponse_OffPlatform,
     PaymentMethodSchemaField,
     PaymentMethodSchemaFieldType,
     PaymentMethodSchemaId,
     PaymentMethodSchemaRequest,
     PaymentMethodSchemaResponse,
     PaymentMethodType,
     PaymentMethodUpdateRequest,
     PaymentMethodUpdateRequest_BankAccount,
     PaymentMethodUpdateRequest_Card,
     PaymentMethodUpdateRequest_Check,
     PaymentMethodUpdateRequest_Custom,
+    PaymentMethodUpdateRequest_OffPlatform,
+    PaymentMethodsRequest,
+    PaymentMethodsResponse,
+    PaymentRailMarkup,
+    PaymentRailMarkupType,
+    PaymentRailRequest,
+    PaymentRailResponse,
+    PhoneNumber,
     PlaidLinkRequest,
+    ProfileRequest,
+    ProfileResponse,
+    RepresentativeId,
+    RepresentativeRequest,
+    RepresentativeResponse,
+    Responsibilities,
+    Rule,
+    Rule_Approver,
+    Ssn,
+    TaxId,
+    TokenGenerationEntityOptions,
+    TokenGenerationFailed,
+    TokenGenerationInvoiceOptions,
+    TokenGenerationOptions,
+    TokenGenerationPagesOptions,
+    TokenGenerationStyleOptions,
+    TokenGenerationVendorOptions,
+    Trigger,
+    Trigger_Amount,
+    Trigger_Metadata,
+    Trigger_Vendor,
+    Unauthorized,
+    Unimplemented,
+    UserNotificationPolicyResponse,
+    VendorNetwork,
+    VendorNotFound,
+    VendorTrigger,
+    bank_lookup,
+    commons,
+    entity,
+    entity_types,
+    invoice,
+    invoice_types,
+    ocr,
+    organization,
+    organization_types,
+    payment_method_schema,
+    payment_method_types,
 )
+from .environment import MercoaEnvironment
 
 __all__ = [
     "AccountType",
     "Address",
     "AmountTrigger",
     "ApprovalPolicyId",
     "ApprovalPolicyRequest",
@@ -317,14 +317,15 @@
     "InvoiceOrderByField",
     "InvoiceQueryError",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "InvoiceStatusError",
     "Itin",
+    "MercoaEnvironment",
     "MetadataSchema",
     "MetadataShowConditions",
     "MetadataTrigger",
     "MetadataType",
     "NotFound",
     "NotificationConfigurationRequest",
     "NotificationConfigurationRequest_Invoice",
@@ -340,39 +341,43 @@
     "OnboardingOption",
     "OnboardingOptionsRequest",
     "OnboardingOptionsResponse",
     "OrderDirection",
     "OrganizationId",
     "OrganizationRequest",
     "OrganizationResponse",
+    "PaymentMethodBalanceResponse",
     "PaymentMethodBaseRequest",
     "PaymentMethodBaseResponse",
     "PaymentMethodError",
     "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodRequest_BankAccount",
     "PaymentMethodRequest_Card",
     "PaymentMethodRequest_Check",
     "PaymentMethodRequest_Custom",
+    "PaymentMethodRequest_OffPlatform",
     "PaymentMethodResponse",
     "PaymentMethodResponse_BankAccount",
     "PaymentMethodResponse_Card",
     "PaymentMethodResponse_Check",
     "PaymentMethodResponse_Custom",
+    "PaymentMethodResponse_OffPlatform",
     "PaymentMethodSchemaField",
     "PaymentMethodSchemaFieldType",
     "PaymentMethodSchemaId",
     "PaymentMethodSchemaRequest",
     "PaymentMethodSchemaResponse",
     "PaymentMethodType",
     "PaymentMethodUpdateRequest",
     "PaymentMethodUpdateRequest_BankAccount",
     "PaymentMethodUpdateRequest_Card",
     "PaymentMethodUpdateRequest_Check",
     "PaymentMethodUpdateRequest_Custom",
+    "PaymentMethodUpdateRequest_OffPlatform",
     "PaymentMethodsRequest",
     "PaymentMethodsResponse",
     "PaymentRailMarkup",
     "PaymentRailMarkupType",
     "PaymentRailRequest",
     "PaymentRailResponse",
     "PhoneNumber",
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.3.8/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.3.8/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.3.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/commons/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/commons/errors/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/commons/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/commons/types/address.py` & `mercoa-0.3.8/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.3.8/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.3.8/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.3.8/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.3.8/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.3.8/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.3.8/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/approval_policy/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/approval_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/counterparty/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/codat_company_creation_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/codat_company_creation_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/codat_company_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/codat_company_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/external_accounting_system_company_creation_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/external_accounting_system_company_creation_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/external_accounting_system/types/external_accounting_system_company_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/external_accounting_system/types/external_accounting_system_company_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/invoice/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/invoice/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/metadata/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/metadata/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/notification_policy/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/notification_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/payment_method/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/payment_method/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.forbidden import Forbidden
 from ....commons.errors.not_found import NotFound
 from ....commons.errors.unauthorized import Unauthorized
 from ....commons.errors.unimplemented import Unimplemented
 from ....entity_types.types.entity_id import EntityId
 from ....payment_method_types.errors.payment_method_error import PaymentMethodError
+from ....payment_method_types.types.payment_method_balance_response import PaymentMethodBalanceResponse
 from ....payment_method_types.types.payment_method_id import PaymentMethodId
 from ....payment_method_types.types.payment_method_request import PaymentMethodRequest
 from ....payment_method_types.types.payment_method_response import PaymentMethodResponse
 from ....payment_method_types.types.payment_method_type import PaymentMethodType
 from ....payment_method_types.types.payment_method_update_request import PaymentMethodUpdateRequest
 
 try:
@@ -320,14 +321,55 @@
                 raise Forbidden(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "NotFound":
                 raise NotFound(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unimplemented":
                 raise Unimplemented(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get_balance(self, entity_id: EntityId, payment_method_id: PaymentMethodId) -> PaymentMethodBalanceResponse:
+        """
+        Get the available balance of a payment method. Only bank accounts added with Plaid are supported.
+
+        Parameters:
+            - entity_id: EntityId.
+
+            - payment_method_id: PaymentMethodId.
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"entity/{entity_id}/paymentMethod/{payment_method_id}/balance",
+            ),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(PaymentMethodBalanceResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "PaymentMethodError":
+                raise PaymentMethodError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Forbidden":
+                raise Forbidden(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "NotFound":
+                raise NotFound(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unimplemented":
+                raise Unimplemented(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncPaymentMethodClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get_all(
         self,
@@ -606,14 +648,57 @@
         if "errorName" in _response_json:
             if _response_json["errorName"] == "PaymentMethodError":
                 raise PaymentMethodError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Forbidden":
+                raise Forbidden(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "NotFound":
+                raise NotFound(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unimplemented":
+                raise Unimplemented(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_balance(
+        self, entity_id: EntityId, payment_method_id: PaymentMethodId
+    ) -> PaymentMethodBalanceResponse:
+        """
+        Get the available balance of a payment method. Only bank accounts added with Plaid are supported.
+
+        Parameters:
+            - entity_id: EntityId.
+
+            - payment_method_id: PaymentMethodId.
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"entity/{entity_id}/paymentMethod/{payment_method_id}/balance",
+            ),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(PaymentMethodBalanceResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "PaymentMethodError":
+                raise PaymentMethodError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Forbidden":
                 raise Forbidden(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "NotFound":
                 raise NotFound(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unimplemented":
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/representative/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/user/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity/resources/user/resources/notifications/client.py` & `mercoa-0.3.8/src/mercoa/resources/entity/resources/user/resources/notifications/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/amount_trigger.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/amount_trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/approval_policy_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/approval_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/approval_policy_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/approval_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/approval_policy_update_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/approval_policy_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/approver_rule.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/approver_rule.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/business_profile_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/business_profile_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/business_type.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/counterparty_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/ein.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_add_payees_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_add_payees_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_add_payors_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_add_payors_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_hide_payees_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_hide_payees_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_hide_payors_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_hide_payors_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_metadata_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_metadata_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_status.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_update_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_user_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_user_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_user_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_user_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/entity_with_payment_method_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/entity_with_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/find_counterparties_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/find_counterparties_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/find_entity_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/find_entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/find_notification_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/find_notification_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/identifier_list.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/identifier_list.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/individual_profile_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/individual_profile_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/metadata_trigger.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/metadata_trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/notification_policy_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/notification_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/notification_policy_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/notification_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/notification_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/notification_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/notification_type.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/notification_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/profile_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/profile_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/representative_request.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/representative_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/responsibilities.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/responsibilities.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/tax_id.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_entity_options.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_entity_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/vendor_trigger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ...invoice_types.types.invoice_status import InvoiceStatus
+from .entity_id import EntityId
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class TokenGenerationInvoiceOptions(pydantic.BaseModel):
-    status: typing.List[InvoiceStatus]
-    mark_paid: typing.Optional[bool] = pydantic.Field(
-        alias="markPaid", description="If true, the user will be able to mark invoices as paid."
-    )
+class VendorTrigger(pydantic.BaseModel):
+    vendor_ids: typing.List[EntityId] = pydantic.Field(alias="vendorIds")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_options.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_pages_options.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_pages_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_style_options.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_style_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/trigger.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/user_notification_policy_response.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/user_notification_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/vendor_network.py` & `mercoa-0.3.8/src/mercoa/resources/entity_types/types/vendor_network.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/entity_types/types/vendor_trigger.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_rail_markup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .entity_id import EntityId
+from .payment_rail_markup_type import PaymentRailMarkupType
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class VendorTrigger(pydantic.BaseModel):
-    vendor_ids: typing.List[EntityId] = pydantic.Field(alias="vendorIds")
+class PaymentRailMarkup(pydantic.BaseModel):
+    type: PaymentRailMarkupType
+    amount: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice/client.py` & `mercoa-0.3.8/src/mercoa/resources/invoice/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice/resources/approval/client.py` & `mercoa-0.3.8/src/mercoa/resources/invoice/resources/approval/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice/resources/comment/client.py` & `mercoa-0.3.8/src/mercoa/resources/invoice/resources/comment/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice/resources/document/client.py` & `mercoa-0.3.8/src/mercoa/resources/invoice/resources/document/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/approval_request.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/approval_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/approval_slot.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/approval_slot.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/approver_action.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/approver_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/associated_approval_action.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/associated_approval_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/comment_request.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/comment_response.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/document_response.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/find_invoice_response.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/find_invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_failure_type.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_failure_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_fees_response.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_fees_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_request.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_response.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/invoice_types/types/invoice_status.py` & `mercoa-0.3.8/src/mercoa/resources/invoice_types/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/ocr/client.py` & `mercoa-0.3.8/src/mercoa/resources/ocr/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/ocr/types/cloud_mailin_attachment.py` & `mercoa-0.3.8/src/mercoa/resources/ocr/types/cloud_mailin_attachment.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/ocr/types/cloud_mailin_envelope.py` & `mercoa-0.3.8/src/mercoa/resources/ocr/types/cloud_mailin_envelope.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/ocr/types/cloud_mailin_request.py` & `mercoa-0.3.8/src/mercoa/resources/ocr/types/cloud_mailin_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.3.8/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization/client.py` & `mercoa-0.3.8/src/mercoa/resources/organization/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization/resources/notification_configuration/client.py` & `mercoa-0.3.8/src/mercoa/resources/organization/resources/notification_configuration/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/business_onboarding_options.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/business_onboarding_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/codat_provider_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/codat_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/color_scheme_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/color_scheme_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/color_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_log_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_provider_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_provider_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_sender_provider.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_sender_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/email_sender_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/external_accounting_system_provider_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/external_accounting_system_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/individual_onboarding_options.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/individual_onboarding_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/metadata_schema.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/metadata_schema.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/metadata_show_conditions.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/metadata_show_conditions.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/metadata_type.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/metadata_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/notification_configuration_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/notification_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/notification_configuration_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/notification_configuration_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/onboarding_option.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/onboarding_option.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/onboarding_options_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/onboarding_options_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/onboarding_options_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/onboarding_options_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/organization_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/organization_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/organization_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/organization_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_methods_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_methods_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_rail_markup.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_account_update_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .payment_rail_markup_type import PaymentRailMarkupType
+from .payment_method_base_request import PaymentMethodBaseRequest
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class PaymentRailMarkup(pydantic.BaseModel):
-    type: PaymentRailMarkupType
-    amount: float
+class BankAccountUpdateRequest(PaymentMethodBaseRequest):
+    account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_rail_request.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/organization_types/types/payment_rail_response.py` & `mercoa-0.3.8/src/mercoa/resources/organization_types/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,38 +12,42 @@
     CardType,
     CheckRequest,
     CheckResponse,
     CurrencyCode,
     CustomPaymentMethodRequest,
     CustomPaymentMethodResponse,
     CustomPaymentMethodUpdateRequest,
+    PaymentMethodBalanceResponse,
     PaymentMethodBaseRequest,
     PaymentMethodBaseResponse,
     PaymentMethodId,
     PaymentMethodRequest,
     PaymentMethodRequest_BankAccount,
     PaymentMethodRequest_Card,
     PaymentMethodRequest_Check,
     PaymentMethodRequest_Custom,
+    PaymentMethodRequest_OffPlatform,
     PaymentMethodResponse,
     PaymentMethodResponse_BankAccount,
     PaymentMethodResponse_Card,
     PaymentMethodResponse_Check,
     PaymentMethodResponse_Custom,
+    PaymentMethodResponse_OffPlatform,
     PaymentMethodSchemaField,
     PaymentMethodSchemaFieldType,
     PaymentMethodSchemaId,
     PaymentMethodSchemaRequest,
     PaymentMethodSchemaResponse,
     PaymentMethodType,
     PaymentMethodUpdateRequest,
     PaymentMethodUpdateRequest_BankAccount,
     PaymentMethodUpdateRequest_Card,
     PaymentMethodUpdateRequest_Check,
     PaymentMethodUpdateRequest_Custom,
+    PaymentMethodUpdateRequest_OffPlatform,
     PlaidLinkRequest,
 )
 from .errors import PaymentMethodError
 
 __all__ = [
     "BankAccountRequest",
     "BankAccountResponse",
@@ -56,34 +60,38 @@
     "CardType",
     "CheckRequest",
     "CheckResponse",
     "CurrencyCode",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
     "CustomPaymentMethodUpdateRequest",
+    "PaymentMethodBalanceResponse",
     "PaymentMethodBaseRequest",
     "PaymentMethodBaseResponse",
     "PaymentMethodError",
     "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodRequest_BankAccount",
     "PaymentMethodRequest_Card",
     "PaymentMethodRequest_Check",
     "PaymentMethodRequest_Custom",
+    "PaymentMethodRequest_OffPlatform",
     "PaymentMethodResponse",
     "PaymentMethodResponse_BankAccount",
     "PaymentMethodResponse_Card",
     "PaymentMethodResponse_Check",
     "PaymentMethodResponse_Custom",
+    "PaymentMethodResponse_OffPlatform",
     "PaymentMethodSchemaField",
     "PaymentMethodSchemaFieldType",
     "PaymentMethodSchemaId",
     "PaymentMethodSchemaRequest",
     "PaymentMethodSchemaResponse",
     "PaymentMethodType",
     "PaymentMethodUpdateRequest",
     "PaymentMethodUpdateRequest_BankAccount",
     "PaymentMethodUpdateRequest_Card",
     "PaymentMethodUpdateRequest_Check",
     "PaymentMethodUpdateRequest_Custom",
+    "PaymentMethodUpdateRequest_OffPlatform",
     "PlaidLinkRequest",
 ]
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/__init__.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,43 +11,47 @@
 from .card_type import CardType
 from .check_request import CheckRequest
 from .check_response import CheckResponse
 from .currency_code import CurrencyCode
 from .custom_payment_method_request import CustomPaymentMethodRequest
 from .custom_payment_method_response import CustomPaymentMethodResponse
 from .custom_payment_method_update_request import CustomPaymentMethodUpdateRequest
+from .payment_method_balance_response import PaymentMethodBalanceResponse
 from .payment_method_base_request import PaymentMethodBaseRequest
 from .payment_method_base_response import PaymentMethodBaseResponse
 from .payment_method_id import PaymentMethodId
 from .payment_method_request import (
     PaymentMethodRequest,
     PaymentMethodRequest_BankAccount,
     PaymentMethodRequest_Card,
     PaymentMethodRequest_Check,
     PaymentMethodRequest_Custom,
+    PaymentMethodRequest_OffPlatform,
 )
 from .payment_method_response import (
     PaymentMethodResponse,
     PaymentMethodResponse_BankAccount,
     PaymentMethodResponse_Card,
     PaymentMethodResponse_Check,
     PaymentMethodResponse_Custom,
+    PaymentMethodResponse_OffPlatform,
 )
 from .payment_method_schema_field import PaymentMethodSchemaField
 from .payment_method_schema_field_type import PaymentMethodSchemaFieldType
 from .payment_method_schema_id import PaymentMethodSchemaId
 from .payment_method_schema_request import PaymentMethodSchemaRequest
 from .payment_method_schema_response import PaymentMethodSchemaResponse
 from .payment_method_type import PaymentMethodType
 from .payment_method_update_request import (
     PaymentMethodUpdateRequest,
     PaymentMethodUpdateRequest_BankAccount,
     PaymentMethodUpdateRequest_Card,
     PaymentMethodUpdateRequest_Check,
     PaymentMethodUpdateRequest_Custom,
+    PaymentMethodUpdateRequest_OffPlatform,
 )
 from .plaid_link_request import PlaidLinkRequest
 
 __all__ = [
     "BankAccountRequest",
     "BankAccountResponse",
     "BankAccountUpdateRequest",
@@ -59,33 +63,37 @@
     "CardType",
     "CheckRequest",
     "CheckResponse",
     "CurrencyCode",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
     "CustomPaymentMethodUpdateRequest",
+    "PaymentMethodBalanceResponse",
     "PaymentMethodBaseRequest",
     "PaymentMethodBaseResponse",
     "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodRequest_BankAccount",
     "PaymentMethodRequest_Card",
     "PaymentMethodRequest_Check",
     "PaymentMethodRequest_Custom",
+    "PaymentMethodRequest_OffPlatform",
     "PaymentMethodResponse",
     "PaymentMethodResponse_BankAccount",
     "PaymentMethodResponse_Card",
     "PaymentMethodResponse_Check",
     "PaymentMethodResponse_Custom",
+    "PaymentMethodResponse_OffPlatform",
     "PaymentMethodSchemaField",
     "PaymentMethodSchemaFieldType",
     "PaymentMethodSchemaId",
     "PaymentMethodSchemaRequest",
     "PaymentMethodSchemaResponse",
     "PaymentMethodType",
     "PaymentMethodUpdateRequest",
     "PaymentMethodUpdateRequest_BankAccount",
     "PaymentMethodUpdateRequest_Card",
     "PaymentMethodUpdateRequest_Check",
     "PaymentMethodUpdateRequest_Custom",
+    "PaymentMethodUpdateRequest_OffPlatform",
     "PlaidLinkRequest",
 ]
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_account_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_account_response.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_account_update_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/plaid_link_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .payment_method_base_request import PaymentMethodBaseRequest
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class BankAccountUpdateRequest(PaymentMethodBaseRequest):
-    account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
+class PlaidLinkRequest(pydantic.BaseModel):
+    account_id: typing.Optional[str] = pydantic.Field(alias="accountId", description="Account ID from Plaid Link")
+    public_token: typing.Optional[str] = pydantic.Field(alias="publicToken", description="Public token from Plaid Link")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_status.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/bank_type.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/card_brand.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/card_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/card_response.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/card_type.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/check_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/check_response.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/currency_code.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_base_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_base_response.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import typing_extensions
 
 from .bank_account_request import BankAccountRequest
 from .card_request import CardRequest
 from .check_request import CheckRequest
 from .custom_payment_method_request import CustomPaymentMethodRequest
+from .payment_method_base_request import PaymentMethodBaseRequest
 
 
 class PaymentMethodRequest_BankAccount(BankAccountRequest):
     type: typing_extensions.Literal["bankAccount"]
 
     class Config:
         frozen = True
@@ -44,10 +45,23 @@
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
+class PaymentMethodRequest_OffPlatform(PaymentMethodBaseRequest):
+    type: typing_extensions.Literal["offPlatform"]
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+
+
 PaymentMethodRequest = typing.Union[
-    PaymentMethodRequest_BankAccount, PaymentMethodRequest_Card, PaymentMethodRequest_Check, PaymentMethodRequest_Custom
+    PaymentMethodRequest_BankAccount,
+    PaymentMethodRequest_Card,
+    PaymentMethodRequest_Check,
+    PaymentMethodRequest_Custom,
+    PaymentMethodRequest_OffPlatform,
 ]
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_response.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import typing_extensions
 
 from .bank_account_response import BankAccountResponse
 from .card_response import CardResponse
 from .check_response import CheckResponse
 from .custom_payment_method_response import CustomPaymentMethodResponse
+from .payment_method_base_response import PaymentMethodBaseResponse
 
 
 class PaymentMethodResponse_BankAccount(BankAccountResponse):
     type: typing_extensions.Literal["bankAccount"]
 
     class Config:
         frozen = True
@@ -44,13 +45,23 @@
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
+class PaymentMethodResponse_OffPlatform(PaymentMethodBaseResponse):
+    type: typing_extensions.Literal["offPlatform"]
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+
+
 PaymentMethodResponse = typing.Union[
     PaymentMethodResponse_BankAccount,
     PaymentMethodResponse_Card,
     PaymentMethodResponse_Check,
     PaymentMethodResponse_Custom,
+    PaymentMethodResponse_OffPlatform,
 ]
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_type.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,26 @@
     CUSTOM = "custom"
     CHECK = "check"
     BANK_ACCOUNT = "bankAccount"
     NA = "na"
     CARD = "card"
     BNPL = "bnpl"
     VIRTUAL_CARD = "virtualCard"
+    OFF_PLATFORM = "offPlatform"
 
     def visit(
         self,
         custom: typing.Callable[[], T_Result],
         check: typing.Callable[[], T_Result],
         bank_account: typing.Callable[[], T_Result],
         na: typing.Callable[[], T_Result],
         card: typing.Callable[[], T_Result],
         bnpl: typing.Callable[[], T_Result],
         virtual_card: typing.Callable[[], T_Result],
+        off_platform: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is PaymentMethodType.CUSTOM:
             return custom()
         if self is PaymentMethodType.CHECK:
             return check()
         if self is PaymentMethodType.BANK_ACCOUNT:
             return bank_account()
@@ -35,7 +37,9 @@
             return na()
         if self is PaymentMethodType.CARD:
             return card()
         if self is PaymentMethodType.BNPL:
             return bnpl()
         if self is PaymentMethodType.VIRTUAL_CARD:
             return virtual_card()
+        if self is PaymentMethodType.OFF_PLATFORM:
+            return off_platform()
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,13 +43,23 @@
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
+class PaymentMethodUpdateRequest_OffPlatform(PaymentMethodBaseRequest):
+    type: typing_extensions.Literal["offPlatform"]
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+
+
 PaymentMethodUpdateRequest = typing.Union[
     PaymentMethodUpdateRequest_Custom,
     PaymentMethodUpdateRequest_BankAccount,
     PaymentMethodUpdateRequest_Card,
     PaymentMethodUpdateRequest_Check,
+    PaymentMethodUpdateRequest_OffPlatform,
 ]
```

### Comparing `mercoa-0.3.7/src/mercoa/resources/payment_method_types/types/plaid_link_request.py` & `mercoa-0.3.8/src/mercoa/resources/payment_method_types/types/payment_method_balance_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
+from .currency_code import CurrencyCode
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class PlaidLinkRequest(pydantic.BaseModel):
-    account_id: typing.Optional[str] = pydantic.Field(alias="accountId", description="Account ID from Plaid Link")
-    public_token: typing.Optional[str] = pydantic.Field(alias="publicToken", description="Public token from Plaid Link")
+class PaymentMethodBalanceResponse(pydantic.BaseModel):
+    available_balance: float = pydantic.Field(alias="availableBalance")
+    currency: CurrencyCode
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.3.7/PKG-INFO` & `mercoa-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.3.7
+Version: 0.3.8
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

