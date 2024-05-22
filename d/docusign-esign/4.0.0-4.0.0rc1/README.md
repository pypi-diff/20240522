# Comparing `tmp/docusign-esign-4.0.0.tar.gz` & `tmp/docusign-esign-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docusign-esign-4.0.0.tar", last modified: Wed May 22 11:46:35 2024, max compression
+gzip compressed data, was "dist/docusign-esign-4.0.0rc1.tar", last modified: Fri May  3 15:17:01 2024, max compression
```

## Comparing `docusign-esign-4.0.0.tar` & `docusign-esign-4.0.0rc1.tar`

### file list

```diff
@@ -1,625 +1,625 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/
--rw-r--r--   0 root         (0) root         (0)     1102 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5853 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5619 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/docusign_esign/
--rw-r--r--   0 root         (0) root         (0)    39088 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/docusign_esign/apis/
--rw-r--r--   0 root         (0) root         (0)     1058 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)   428943 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/accounts_api.py
--rw-r--r--   0 root         (0) root         (0)    36525 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    77219 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/billing_api.py
--rw-r--r--   0 root         (0) root         (0)   105694 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/bulk_envelopes_api.py
--rw-r--r--   0 root         (0) root         (0)    40007 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/bulk_process_data_api.py
--rw-r--r--   0 root         (0) root         (0)    24433 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/bulk_process_data_send_api.py
--rw-r--r--   0 root         (0) root         (0)    51067 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/cloud_storage_api.py
--rw-r--r--   0 root         (0) root         (0)   114632 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/connect_api.py
--rw-r--r--   0 root         (0) root         (0)    26196 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/custom_tabs_api.py
--rw-r--r--   0 root         (0) root         (0)     6118 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/data_feed_api.py
--rw-r--r--   0 root         (0) root         (0)    34477 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/diagnostics_api.py
--rw-r--r--   0 root         (0) root         (0)    23507 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/email_archive_api.py
--rw-r--r--   0 root         (0) root         (0)   840521 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/envelopes_api.py
--rw-r--r--   0 root         (0) root         (0)    29607 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/folders_api.py
--rw-r--r--   0 root         (0) root         (0)    53159 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/groups_api.py
--rw-r--r--   0 root         (0) root         (0)    47724 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/notary_api.py
--rw-r--r--   0 root         (0) root         (0)     6111 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/organizations_api.py
--rw-r--r--   0 root         (0) root         (0)    49102 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/power_forms_api.py
--rw-r--r--   0 root         (0) root         (0)    20853 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/signature_api.py
--rw-r--r--   0 root         (0) root         (0)    47054 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/signing_groups_api.py
--rw-r--r--   0 root         (0) root         (0)   301558 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/templates_api.py
--rw-r--r--   0 root         (0) root         (0)     5488 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/trust_service_providers_api.py
--rw-r--r--   0 root         (0) root         (0)   196161 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/users_api.py
--rw-r--r--   0 root         (0) root         (0)    67009 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/apis/workspaces_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/docusign_esign/client/
--rw-r--r--   0 root         (0) root         (0)      611 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35384 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/client/api_client.py
--rw-r--r--   0 root         (0) root         (0)     1799 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/client/api_exception.py
--rw-r--r--   0 root         (0) root         (0)    13506 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/client/api_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/docusign_esign/client/auth/
--rw-r--r--   0 root         (0) root         (0)      547 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/client/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14771 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/client/auth/oauth.py
--rw-r--r--   0 root         (0) root         (0)     8894 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/client/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/docusign_esign/models/
--rw-r--r--   0 root         (0) root         (0)    37584 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13277 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/access_code_format.py
--rw-r--r--   0 root         (0) root         (0)    11983 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_address.py
--rw-r--r--   0 root         (0) root         (0)    31800 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_billing_plan.py
--rw-r--r--   0 root         (0) root         (0)    17814 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_billing_plan_response.py
--rw-r--r--   0 root         (0) root         (0)     5281 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_identity_input_option.py
--rw-r--r--   0 root         (0) root         (0)     4061 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_identity_verification_response.py
--rw-r--r--   0 root         (0) root         (0)     4306 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_identity_verification_step.py
--rw-r--r--   0 root         (0) root         (0)    12168 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_identity_verification_workflow.py
--rw-r--r--   0 root         (0) root         (0)    39158 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_information.py
--rw-r--r--   0 root         (0) root         (0)     4625 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_minimum_password_length.py
--rw-r--r--   0 root         (0) root         (0)     5648 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_notification.py
--rw-r--r--   0 root         (0) root         (0)     4618 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_password_expire_password_days.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_password_lockout_duration_minutes.py
--rw-r--r--   0 root         (0) root         (0)     3705 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_password_lockout_duration_type.py
--rw-r--r--   0 root         (0) root         (0)     4634 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_password_minimum_password_age_days.py
--rw-r--r--   0 root         (0) root         (0)     4785 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_password_questions_required.py
--rw-r--r--   0 root         (0) root         (0)    25898 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_password_rules.py
--rw-r--r--   0 root         (0) root         (0)     3732 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_password_strength_type.py
--rw-r--r--   0 root         (0) root         (0)    10429 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_password_strength_type_option.py
--rw-r--r--   0 root         (0) root         (0)   113332 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_role_settings.py
--rw-r--r--   0 root         (0) root         (0)     3504 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_seals.py
--rw-r--r--   0 root         (0) root         (0)   939466 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_settings_information.py
--rw-r--r--   0 root         (0) root         (0)    11434 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_shared_access.py
--rw-r--r--   0 root         (0) root         (0)    32500 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_signature.py
--rw-r--r--   0 root         (0) root         (0)    19678 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_signature_definition.py
--rw-r--r--   0 root         (0) root         (0)    10210 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     6491 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_signature_provider_option.py
--rw-r--r--   0 root         (0) root         (0)     3902 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_signature_providers.py
--rw-r--r--   0 root         (0) root         (0)     3887 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_signatures_information.py
--rw-r--r--   0 root         (0) root         (0)    42099 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/account_ui_settings.py
--rw-r--r--   0 root         (0) root         (0)     5302 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/add_on.py
--rw-r--r--   0 root         (0) root         (0)     9933 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/address_information.py
--rw-r--r--   0 root         (0) root         (0)     7146 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/address_information_input.py
--rw-r--r--   0 root         (0) root         (0)     7769 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/address_information_v2.py
--rw-r--r--   0 root         (0) root         (0)     4417 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/admin_message.py
--rw-r--r--   0 root         (0) root         (0)    88051 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/agent.py
--rw-r--r--   0 root         (0) root         (0)     6358 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/api_request_log.py
--rw-r--r--   0 root         (0) root         (0)     3795 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/api_request_logs_result.py
--rw-r--r--   0 root         (0) root         (0)     4414 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/app_store_product.py
--rw-r--r--   0 root         (0) root         (0)     6308 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/app_store_receipt.py
--rw-r--r--   0 root         (0) root         (0)    91945 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/approve.py
--rw-r--r--   0 root         (0) root         (0)     5355 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/ask_an_admin.py
--rw-r--r--   0 root         (0) root         (0)     7885 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/attachment.py
--rw-r--r--   0 root         (0) root         (0)     6791 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/authentication_method.py
--rw-r--r--   0 root         (0) root         (0)    26660 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/authentication_status.py
--rw-r--r--   0 root         (0) root         (0)     5678 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/authorization_user.py
--rw-r--r--   0 root         (0) root         (0)     5791 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bcc_email_address.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bcc_email_archive.py
--rw-r--r--   0 root         (0) root         (0)     7856 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bcc_email_archive_history.py
--rw-r--r--   0 root         (0) root         (0)     9955 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bcc_email_archive_history_list.py
--rw-r--r--   0 root         (0) root         (0)     9578 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bcc_email_archive_list.py
--rw-r--r--   0 root         (0) root         (0)    16119 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_charge.py
--rw-r--r--   0 root         (0) root         (0)     3876 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_charge_response.py
--rw-r--r--   0 root         (0) root         (0)     5154 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_discount.py
--rw-r--r--   0 root         (0) root         (0)     6585 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_entity_information_response.py
--rw-r--r--   0 root         (0) root         (0)    10843 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_invoice.py
--rw-r--r--   0 root         (0) root         (0)     8481 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_invoice_item.py
--rw-r--r--   0 root         (0) root         (0)     5728 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_invoices_response.py
--rw-r--r--   0 root         (0) root         (0)     7242 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_invoices_summary.py
--rw-r--r--   0 root         (0) root         (0)     5019 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_payment.py
--rw-r--r--   0 root         (0) root         (0)     7040 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_payment_item.py
--rw-r--r--   0 root         (0) root         (0)     3957 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     3817 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     5740 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_payments_response.py
--rw-r--r--   0 root         (0) root         (0)    16632 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_plan.py
--rw-r--r--   0 root         (0) root         (0)    24833 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_plan_information.py
--rw-r--r--   0 root         (0) root         (0)     7645 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_plan_preview.py
--rw-r--r--   0 root         (0) root         (0)     4666 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_plan_response.py
--rw-r--r--   0 root         (0) root         (0)     9929 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_plan_update_response.py
--rw-r--r--   0 root         (0) root         (0)     3736 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_plans_response.py
--rw-r--r--   0 root         (0) root         (0)     5164 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/billing_price.py
--rw-r--r--   0 root         (0) root         (0)    17441 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brand.py
--rw-r--r--   0 root         (0) root         (0)     5965 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brand_email_content.py
--rw-r--r--   0 root         (0) root         (0)     5688 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brand_link.py
--rw-r--r--   0 root         (0) root         (0)     4811 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brand_logos.py
--rw-r--r--   0 root         (0) root         (0)     3580 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brand_request.py
--rw-r--r--   0 root         (0) root         (0)     5735 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brand_resource_urls.py
--rw-r--r--   0 root         (0) root         (0)    10377 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brand_resources.py
--rw-r--r--   0 root         (0) root         (0)     3880 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brand_resources_list.py
--rw-r--r--   0 root         (0) root         (0)     3563 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brands_request.py
--rw-r--r--   0 root         (0) root         (0)     5833 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/brands_response.py
--rw-r--r--   0 root         (0) root         (0)    11143 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_envelope.py
--rw-r--r--   0 root         (0) root         (0)    15435 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_envelope_status.py
--rw-r--r--   0 root         (0) root         (0)     9563 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_envelopes_response.py
--rw-r--r--   0 root         (0) root         (0)     4583 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_process_request.py
--rw-r--r--   0 root         (0) root         (0)     8228 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_process_response.py
--rw-r--r--   0 root         (0) root         (0)     4974 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_process_result.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_processing_list_summaries.py
--rw-r--r--   0 root         (0) root         (0)     6204 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_processing_list_summary.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_processing_lists.py
--rw-r--r--   0 root         (0) root         (0)    14950 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_recipient.py
--rw-r--r--   0 root         (0) root         (0)     4375 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_recipient_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     4258 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_recipient_tab_label.py
--rw-r--r--   0 root         (0) root         (0)     3919 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_recipients_request.py
--rw-r--r--   0 root         (0) root         (0)     9778 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_recipients_response.py
--rw-r--r--   0 root         (0) root         (0)     7157 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_recipients_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     3624 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_recipients_update_response.py
--rw-r--r--   0 root         (0) root         (0)     5253 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_action_request.py
--rw-r--r--   0 root         (0) root         (0)     4298 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_error.py
--rw-r--r--   0 root         (0) root         (0)     3614 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_request.py
--rw-r--r--   0 root         (0) root         (0)    17291 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_status.py
--rw-r--r--   0 root         (0) root         (0)    14262 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_summaries.py
--rw-r--r--   0 root         (0) root         (0)    10233 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_summary.py
--rw-r--r--   0 root         (0) root         (0)    13105 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_envelopes_info.py
--rw-r--r--   0 root         (0) root         (0)     6145 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_error_status.py
--rw-r--r--   0 root         (0) root         (0)     4544 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_request.py
--rw-r--r--   0 root         (0) root         (0)     9108 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_response.py
--rw-r--r--   0 root         (0) root         (0)     5573 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_send_test_response.py
--rw-r--r--   0 root         (0) root         (0)     8021 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_sending_copy.py
--rw-r--r--   0 root         (0) root         (0)     4323 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_sending_copy_custom_field.py
--rw-r--r--   0 root         (0) root         (0)    37255 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_sending_copy_recipient.py
--rw-r--r--   0 root         (0) root         (0)     4529 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_sending_copy_tab.py
--rw-r--r--   0 root         (0) root         (0)     4966 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_sending_list.py
--rw-r--r--   0 root         (0) root         (0)     3886 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_sending_list_summaries.py
--rw-r--r--   0 root         (0) root         (0)     6087 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulk_sending_list_summary.py
--rw-r--r--   0 root         (0) root         (0)     4375 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/bulksending_copy_doc_gen_form_field.py
--rw-r--r--   0 root         (0) root         (0)     6886 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/captive_recipient.py
--rw-r--r--   0 root         (0) root         (0)     4028 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/captive_recipient_information.py
--rw-r--r--   0 root         (0) root         (0)    94162 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/carbon_copy.py
--rw-r--r--   0 root         (0) root         (0)    94115 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/certified_delivery.py
--rw-r--r--   0 root         (0) root         (0)   105043 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     4196 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/chunked_upload_part.py
--rw-r--r--   0 root         (0) root         (0)     4395 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/chunked_upload_request.py
--rw-r--r--   0 root         (0) root         (0)    10714 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/chunked_upload_response.py
--rw-r--r--   0 root         (0) root         (0)     8154 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/cloud_storage_provider.py
--rw-r--r--   0 root         (0) root         (0)     3952 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/cloud_storage_providers.py
--rw-r--r--   0 root         (0) root         (0)    19343 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/comment.py
--rw-r--r--   0 root         (0) root         (0)     5953 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/comment_history_result.py
--rw-r--r--   0 root         (0) root         (0)     7164 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/comment_publish.py
--rw-r--r--   0 root         (0) root         (0)    93586 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/comment_thread.py
--rw-r--r--   0 root         (0) root         (0)     3781 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/comments_publish.py
--rw-r--r--   0 root         (0) root         (0)   110382 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/commission_county.py
--rw-r--r--   0 root         (0) root         (0)   112034 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/commission_expiration.py
--rw-r--r--   0 root         (0) root         (0)   110382 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/commission_number.py
--rw-r--r--   0 root         (0) root         (0)   109969 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/commission_state.py
--rw-r--r--   0 root         (0) root         (0)   106745 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/company.py
--rw-r--r--   0 root         (0) root         (0)     5556 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/complete_sign_hash_response.py
--rw-r--r--   0 root         (0) root         (0)     9079 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/complete_sign_request.py
--rw-r--r--   0 root         (0) root         (0)     9603 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/composite_template.py
--rw-r--r--   0 root         (0) root         (0)     6568 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/conditional_recipient_rule.py
--rw-r--r--   0 root         (0) root         (0)     5408 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/conditional_recipient_rule_condition.py
--rw-r--r--   0 root         (0) root         (0)     8761 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/conditional_recipient_rule_filter.py
--rw-r--r--   0 root         (0) root         (0)     4617 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_config_results.py
--rw-r--r--   0 root         (0) root         (0)    49382 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_custom_configuration.py
--rw-r--r--   0 root         (0) root         (0)     6888 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_debug_log.py
--rw-r--r--   0 root         (0) root         (0)     2881 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_delete_failure_result.py
--rw-r--r--   0 root         (0) root         (0)     5002 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_event_data.py
--rw-r--r--   0 root         (0) root         (0)     4450 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_failure_filter.py
--rw-r--r--   0 root         (0) root         (0)     7197 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_failure_result.py
--rw-r--r--   0 root         (0) root         (0)     3710 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_failure_results.py
--rw-r--r--   0 root         (0) root         (0)     4558 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_historical_envelope_republish.py
--rw-r--r--   0 root         (0) root         (0)    17883 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_log.py
--rw-r--r--   0 root         (0) root         (0)     6011 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_logs.py
--rw-r--r--   0 root         (0) root         (0)     6940 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_o_auth_config.py
--rw-r--r--   0 root         (0) root         (0)     8902 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_salesforce_field.py
--rw-r--r--   0 root         (0) root         (0)     9993 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_salesforce_object.py
--rw-r--r--   0 root         (0) root         (0)     5655 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_user_info.py
--rw-r--r--   0 root         (0) root         (0)     7148 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/connect_user_object.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/consent_details.py
--rw-r--r--   0 root         (0) root         (0)     4625 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/console_view_request.py
--rw-r--r--   0 root         (0) root         (0)    35223 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/consumer_disclosure.py
--rw-r--r--   0 root         (0) root         (0)    14823 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/contact.py
--rw-r--r--   0 root         (0) root         (0)     9343 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/contact_get_response.py
--rw-r--r--   0 root         (0) root         (0)     3653 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/contact_mod_request.py
--rw-r--r--   0 root         (0) root         (0)     4387 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/contact_phone_number.py
--rw-r--r--   0 root         (0) root         (0)     3618 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/contact_update_response.py
--rw-r--r--   0 root         (0) root         (0)     7296 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/correct_view_request.py
--rw-r--r--   0 root         (0) root         (0)     5647 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/country.py
--rw-r--r--   0 root         (0) root         (0)     5359 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/credential.py
--rw-r--r--   0 root         (0) root         (0)    10769 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/credit_card_information.py
--rw-r--r--   0 root         (0) root         (0)     3683 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/credit_card_types.py
--rw-r--r--   0 root         (0) root         (0)   118797 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/currency.py
--rw-r--r--   0 root         (0) root         (0)     7661 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/currency_feature_set_price.py
--rw-r--r--   0 root         (0) root         (0)    10088 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/currency_plan_price.py
--rw-r--r--   0 root         (0) root         (0)     8698 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/custom_field.py
--rw-r--r--   0 root         (0) root         (0)     7023 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/custom_field_v2.py
--rw-r--r--   0 root         (0) root         (0)     4791 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/custom_fields.py
--rw-r--r--   0 root         (0) root         (0)     4895 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/custom_fields_envelope.py
--rw-r--r--   0 root         (0) root         (0)     3785 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/custom_settings_information.py
--rw-r--r--   0 root         (0) root         (0)   120684 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/date.py
--rw-r--r--   0 root         (0) root         (0)    94370 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/date_signed.py
--rw-r--r--   0 root         (0) root         (0)     6112 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/date_stamp_properties.py
--rw-r--r--   0 root         (0) root         (0)    93947 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/decline.py
--rw-r--r--   0 root         (0) root         (0)     6268 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/delayed_routing.py
--rw-r--r--   0 root         (0) root         (0)     6568 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/delayed_routing_api_model.py
--rw-r--r--   0 root         (0) root         (0)     5724 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/delegation_info.py
--rw-r--r--   0 root         (0) root         (0)     6551 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/diagnostics_settings_information.py
--rw-r--r--   0 root         (0) root         (0)    13477 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/direct_debit_processor_information.py
--rw-r--r--   0 root         (0) root         (0)     7881 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_account.py
--rw-r--r--   0 root         (0) root         (0)     4296 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_custom_field.py
--rw-r--r--   0 root         (0) root         (0)    12940 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_document.py
--rw-r--r--   0 root         (0) root         (0)     9685 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_document_page.py
--rw-r--r--   0 root         (0) root         (0)    18516 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_envelope.py
--rw-r--r--   0 root         (0) root         (0)     2533 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_info.py
--rw-r--r--   0 root         (0) root         (0)     9243 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_page.py
--rw-r--r--   0 root         (0) root         (0)     2529 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_pdf.py
--rw-r--r--   0 root         (0) root         (0)    25341 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_recipient.py
--rw-r--r--   0 root         (0) root         (0)     2581 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/display_appliance_signer_attachment.py
--rw-r--r--   0 root         (0) root         (0)     5952 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/dob_information_input.py
--rw-r--r--   0 root         (0) root         (0)    10404 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field.py
--rw-r--r--   0 root         (0) root         (0)     5794 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_option.py
--rw-r--r--   0 root         (0) root         (0)     3849 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     4746 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_response.py
--rw-r--r--   0 root         (0) root         (0)     3926 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_row_value.py
--rw-r--r--   0 root         (0) root         (0)     4497 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_validation.py
--rw-r--r--   0 root         (0) root         (0)     6715 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_fields.py
--rw-r--r--   0 root         (0) root         (0)     5108 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/doc_gen_syntax_error.py
--rw-r--r--   0 root         (0) root         (0)    30429 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document.py
--rw-r--r--   0 root         (0) root         (0)     4623 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_fields_information.py
--rw-r--r--   0 root         (0) root         (0)    12081 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_html_collapsible_display_settings.py
--rw-r--r--   0 root         (0) root         (0)    12749 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_html_definition.py
--rw-r--r--   0 root         (0) root         (0)     5954 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_html_definition_original.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_html_definition_originals.py
--rw-r--r--   0 root         (0) root         (0)     3767 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_html_definitions.py
--rw-r--r--   0 root         (0) root         (0)     8339 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_html_display_anchor.py
--rw-r--r--   0 root         (0) root         (0)    13796 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_html_display_settings.py
--rw-r--r--   0 root         (0) root         (0)     4748 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_security_store.py
--rw-r--r--   0 root         (0) root         (0)     7423 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_template.py
--rw-r--r--   0 root         (0) root         (0)     3815 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_template_list.py
--rw-r--r--   0 root         (0) root         (0)     8591 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_update_info.py
--rw-r--r--   0 root         (0) root         (0)     7105 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_visibility.py
--rw-r--r--   0 root         (0) root         (0)     3857 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/document_visibility_list.py
--rw-r--r--   0 root         (0) root         (0)     4990 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/downgrad_request_billing_info_response.py
--rw-r--r--   0 root         (0) root         (0)     8633 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/downgrade_billing_plan_information.py
--rw-r--r--   0 root         (0) root         (0)    14854 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/downgrade_plan_update_response.py
--rw-r--r--   0 root         (0) root         (0)     6119 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/downgrade_request_information.py
--rw-r--r--   0 root         (0) root         (0)    83131 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/draw.py
--rw-r--r--   0 root         (0) root         (0)     7570 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/e_note_configuration.py
--rw-r--r--   0 root         (0) root         (0)    86073 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/editor.py
--rw-r--r--   0 root         (0) root         (0)   121153 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/email.py
--rw-r--r--   0 root         (0) root         (0)    95100 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/email_address.py
--rw-r--r--   0 root         (0) root         (0)     6088 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/email_settings.py
--rw-r--r--   0 root         (0) root         (0)    78819 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope.py
--rw-r--r--   0 root         (0) root         (0)     7504 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_attachment.py
--rw-r--r--   0 root         (0) root         (0)     3726 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_attachments_request.py
--rw-r--r--   0 root         (0) root         (0)     3741 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_attachments_result.py
--rw-r--r--   0 root         (0) root         (0)     3668 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_audit_event.py
--rw-r--r--   0 root         (0) root         (0)     3793 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_audit_event_response.py
--rw-r--r--   0 root         (0) root         (0)     4062 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_custom_metadata.py
--rw-r--r--   0 root         (0) root         (0)    98736 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_definition.py
--rw-r--r--   0 root         (0) root         (0)     5337 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_delay_rule.py
--rw-r--r--   0 root         (0) root         (0)     5441 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_delay_rule_api_model.py
--rw-r--r--   0 root         (0) root         (0)    31835 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_document.py
--rw-r--r--   0 root         (0) root         (0)     4753 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_documents_result.py
--rw-r--r--   0 root         (0) root         (0)     5050 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_event.py
--rw-r--r--   0 root         (0) root         (0)     9783 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_form_data.py
--rw-r--r--   0 root         (0) root         (0)     3420 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_form_data_prefill_form_data.py
--rw-r--r--   0 root         (0) root         (0)    92708 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_id.py
--rw-r--r--   0 root         (0) root         (0)     4787 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_ids_request.py
--rw-r--r--   0 root         (0) root         (0)     5573 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_metadata.py
--rw-r--r--   0 root         (0) root         (0)     5766 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    16022 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_publish_transaction.py
--rw-r--r--   0 root         (0) root         (0)     4509 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_publish_transaction_error_rollup.py
--rw-r--r--   0 root         (0) root         (0)     6656 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_purge_configuration.py
--rw-r--r--   0 root         (0) root         (0)    10287 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_summary.py
--rw-r--r--   0 root         (0) root         (0)   100293 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_template.py
--rw-r--r--   0 root         (0) root         (0)    13907 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_template_definition.py
--rw-r--r--   0 root         (0) root         (0)    59810 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_template_result.py
--rw-r--r--   0 root         (0) root         (0)    10527 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_template_results.py
--rw-r--r--   0 root         (0) root         (0)     7470 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_transaction_status.py
--rw-r--r--   0 root         (0) root         (0)    11767 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_transfer_rule.py
--rw-r--r--   0 root         (0) root         (0)    10079 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_transfer_rule_information.py
--rw-r--r--   0 root         (0) root         (0)    11938 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_transfer_rule_request.py
--rw-r--r--   0 root         (0) root         (0)    12023 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_update_summary.py
--rw-r--r--   0 root         (0) root         (0)     7089 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_view_document_settings.py
--rw-r--r--   0 root         (0) root         (0)     4089 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_view_envelope_custom_field_settings.py
--rw-r--r--   0 root         (0) root         (0)     6610 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_view_recipient_settings.py
--rw-r--r--   0 root         (0) root         (0)     5157 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_view_request.py
--rw-r--r--   0 root         (0) root         (0)    15021 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_view_settings.py
--rw-r--r--   0 root         (0) root         (0)     5584 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_view_tagger_settings.py
--rw-r--r--   0 root         (0) root         (0)     4044 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelope_view_template_settings.py
--rw-r--r--   0 root         (0) root         (0)    14217 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/envelopes_information.py
--rw-r--r--   0 root         (0) root         (0)     4344 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)    26563 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/event_notification.py
--rw-r--r--   0 root         (0) root         (0)     6541 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/event_result.py
--rw-r--r--   0 root         (0) root         (0)     6087 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/expirations.py
--rw-r--r--   0 root         (0) root         (0)     5475 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/external_claim.py
--rw-r--r--   0 root         (0) root         (0)     5427 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/external_doc_service_error_details.py
--rw-r--r--   0 root         (0) root         (0)    12835 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/external_document_sources.py
--rw-r--r--   0 root         (0) root         (0)     9541 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/external_file.py
--rw-r--r--   0 root         (0) root         (0)    11306 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/external_folder.py
--rw-r--r--   0 root         (0) root         (0)     7162 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/external_primary_account_recipient_auth_requirements.py
--rw-r--r--   0 root         (0) root         (0)     5671 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/favorite_templates_content_item.py
--rw-r--r--   0 root         (0) root         (0)     5740 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/favorite_templates_info.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/feature_available_metadata.py
--rw-r--r--   0 root         (0) root         (0)    10487 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/feature_set.py
--rw-r--r--   0 root         (0) root         (0)     4399 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/file_type.py
--rw-r--r--   0 root         (0) root         (0)     3629 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/file_type_list.py
--rw-r--r--   0 root         (0) root         (0)    11057 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/filter.py
--rw-r--r--   0 root         (0) root         (0)    94005 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/first_name.py
--rw-r--r--   0 root         (0) root         (0)    13945 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/folder.py
--rw-r--r--   0 root         (0) root         (0)    17939 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/folder_item.py
--rw-r--r--   0 root         (0) root         (0)     9136 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/folder_item_response.py
--rw-r--r--   0 root         (0) root         (0)    20880 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/folder_item_v2.py
--rw-r--r--   0 root         (0) root         (0)    10151 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/folder_items_response.py
--rw-r--r--   0 root         (0) root         (0)    11417 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/folder_shared_item.py
--rw-r--r--   0 root         (0) root         (0)     5233 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/folders_request.py
--rw-r--r--   0 root         (0) root         (0)    10003 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/folders_response.py
--rw-r--r--   0 root         (0) root         (0)    12851 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/forgotten_password_information.py
--rw-r--r--   0 root         (0) root         (0)     8611 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/form_data_item.py
--rw-r--r--   0 root         (0) root         (0)   133296 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/formula_tab.py
--rw-r--r--   0 root         (0) root         (0)    93640 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/full_name.py
--rw-r--r--   0 root         (0) root         (0)     5073 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/graphics_context.py
--rw-r--r--   0 root         (0) root         (0)    10448 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/group.py
--rw-r--r--   0 root         (0) root         (0)     5907 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/group_brands.py
--rw-r--r--   0 root         (0) root         (0)     9387 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/group_information.py
--rw-r--r--   0 root         (0) root         (0)     5099 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/id_check_configuration.py
--rw-r--r--   0 root         (0) root         (0)     7874 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/id_check_information_input.py
--rw-r--r--   0 root         (0) root         (0)     3587 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/id_check_security_step.py
--rw-r--r--   0 root         (0) root         (0)     4559 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/id_evidence_resource_token.py
--rw-r--r--   0 root         (0) root         (0)     3578 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/id_evidence_view_link.py
--rw-r--r--   0 root         (0) root         (0)   111517 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/in_person_signer.py
--rw-r--r--   0 root         (0) root         (0)    85322 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/initial_here.py
--rw-r--r--   0 root         (0) root         (0)     7832 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/inline_template.py
--rw-r--r--   0 root         (0) root         (0)     9676 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/integrated_connect_user_info_list.py
--rw-r--r--   0 root         (0) root         (0)    10338 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/integrated_user_info_list.py
--rw-r--r--   0 root         (0) root         (0)    90158 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/intermediary.py
--rw-r--r--   0 root         (0) root         (0)    11103 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/jurisdiction.py
--rw-r--r--   0 root         (0) root         (0)     6419 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/jurisdiction_summary.py
--rw-r--r--   0 root         (0) root         (0)    93640 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/last_name.py
--rw-r--r--   0 root         (0) root         (0)    10192 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/linked_external_primary_account.py
--rw-r--r--   0 root         (0) root         (0)   110330 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/list.py
--rw-r--r--   0 root         (0) root         (0)     9399 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/list_custom_field.py
--rw-r--r--   0 root         (0) root         (0)     7999 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/list_item.py
--rw-r--r--   0 root         (0) root         (0)    43378 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/locale_policy.py
--rw-r--r--   0 root         (0) root         (0)    14590 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/locale_policy_tab.py
--rw-r--r--   0 root         (0) root         (0)    10997 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/lock_information.py
--rw-r--r--   0 root         (0) root         (0)     7711 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/lock_request.py
--rw-r--r--   0 root         (0) root         (0)    12815 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/login_account.py
--rw-r--r--   0 root         (0) root         (0)     4970 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/login_information.py
--rw-r--r--   0 root         (0) root         (0)     6882 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/match_box.py
--rw-r--r--   0 root         (0) root         (0)     5266 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/member_group_shared_item.py
--rw-r--r--   0 root         (0) root         (0)     6800 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/member_shared_items.py
--rw-r--r--   0 root         (0) root         (0)    14847 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/merge_field.py
--rw-r--r--   0 root         (0) root         (0)     5319 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/mobile_notifier_configuration.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/mobile_notifier_configuration_information.py
--rw-r--r--   0 root         (0) root         (0)   123029 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/model_date.py
--rw-r--r--   0 root         (0) root         (0)     5082 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/money.py
--rw-r--r--   0 root         (0) root         (0)     5937 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/name_value.py
--rw-r--r--   0 root         (0) root         (0)    22204 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/new_account_definition.py
--rw-r--r--   0 root         (0) root         (0)     9520 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/new_account_summary.py
--rw-r--r--   0 root         (0) root         (0)    11493 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/new_user.py
--rw-r--r--   0 root         (0) root         (0)     3632 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/new_users_definition.py
--rw-r--r--   0 root         (0) root         (0)     3581 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/new_users_summary.py
--rw-r--r--   0 root         (0) root         (0)    79841 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notarize.py
--rw-r--r--   0 root         (0) root         (0)     5719 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary.py
--rw-r--r--   0 root         (0) root         (0)    76227 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_certificate.py
--rw-r--r--   0 root         (0) root         (0)     4749 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_contact_details.py
--rw-r--r--   0 root         (0) root         (0)    79330 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_host.py
--rw-r--r--   0 root         (0) root         (0)     8019 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_journal.py
--rw-r--r--   0 root         (0) root         (0)     5206 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_journal_credible_witness.py
--rw-r--r--   0 root         (0) root         (0)     9453 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_journal_list.py
--rw-r--r--   0 root         (0) root         (0)     6269 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_journal_meta_data.py
--rw-r--r--   0 root         (0) root         (0)     8712 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_jurisdiction.py
--rw-r--r--   0 root         (0) root         (0)     9723 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_jurisdiction_list.py
--rw-r--r--   0 root         (0) root         (0)   118673 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_recipient.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_result.py
--rw-r--r--   0 root         (0) root         (0)    82091 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notary_seal.py
--rw-r--r--   0 root         (0) root         (0)    93944 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/note.py
--rw-r--r--   0 root         (0) root         (0)     5691 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     6742 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notification_default_settings.py
--rw-r--r--   0 root         (0) root         (0)     5204 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/notification_defaults.py
--rw-r--r--   0 root         (0) root         (0)   126200 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/number.py
--rw-r--r--   0 root         (0) root         (0)   115339 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/numerical.py
--rw-r--r--   0 root         (0) root         (0)     7198 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/oauth_access.py
--rw-r--r--   0 root         (0) root         (0)     6939 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/ocr_request.py
--rw-r--r--   0 root         (0) root         (0)     8568 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/offline_attributes.py
--rw-r--r--   0 root         (0) root         (0)     8316 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/page.py
--rw-r--r--   0 root         (0) root         (0)     9016 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/page_images.py
--rw-r--r--   0 root         (0) root         (0)     4326 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/page_request.py
--rw-r--r--   0 root         (0) root         (0)     3588 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/page_size.py
--rw-r--r--   0 root         (0) root         (0)     3498 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/palette_item_settings.py
--rw-r--r--   0 root         (0) root         (0)     8224 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/palette_settings.py
--rw-r--r--   0 root         (0) root         (0)    83205 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/participant.py
--rw-r--r--   0 root         (0) root         (0)     4891 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/path_extended_element.py
--rw-r--r--   0 root         (0) root         (0)     6454 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/pay_pal_legacy_settings.py
--rw-r--r--   0 root         (0) root         (0)    19177 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/payment_details.py
--rw-r--r--   0 root         (0) root         (0)    16489 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/payment_gateway_account.py
--rw-r--r--   0 root         (0) root         (0)     6359 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/payment_gateway_account_setting.py
--rw-r--r--   0 root         (0) root         (0)     3991 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/payment_gateway_accounts_info.py
--rw-r--r--   0 root         (0) root         (0)     5800 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/payment_line_item.py
--rw-r--r--   0 root         (0) root         (0)     5443 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/payment_method_with_options.py
--rw-r--r--   0 root         (0) root         (0)     5457 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/payment_processor_information.py
--rw-r--r--   0 root         (0) root         (0)     3677 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/payment_signer_values.py
--rw-r--r--   0 root         (0) root         (0)     9011 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/permission_profile.py
--rw-r--r--   0 root         (0) root         (0)     4032 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/permission_profile_information.py
--rw-r--r--   0 root         (0) root         (0)   108317 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/phone_number.py
--rw-r--r--   0 root         (0) root         (0)     8214 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/plan_information.py
--rw-r--r--   0 root         (0) root         (0)     5079 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/poly_line.py
--rw-r--r--   0 root         (0) root         (0)    86376 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/poly_line_overlay.py
--rw-r--r--   0 root         (0) root         (0)    23001 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/power_form.py
--rw-r--r--   0 root         (0) root         (0)     4732 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/power_form_form_data_envelope.py
--rw-r--r--   0 root         (0) root         (0)     6103 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/power_form_form_data_recipient.py
--rw-r--r--   0 root         (0) root         (0)    16344 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/power_form_recipient.py
--rw-r--r--   0 root         (0) root         (0)     9722 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/power_form_senders_response.py
--rw-r--r--   0 root         (0) root         (0)     3735 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/power_forms_form_data_response.py
--rw-r--r--   0 root         (0) root         (0)     3641 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/power_forms_request.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/power_forms_response.py
--rw-r--r--   0 root         (0) root         (0)     5950 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/prefill_form_data.py
--rw-r--r--   0 root         (0) root         (0)    16899 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/prefill_tabs.py
--rw-r--r--   0 root         (0) root         (0)     4585 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/proof_service_resource_token.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/proof_service_view_link.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/property_metadata.py
--rw-r--r--   0 root         (0) root         (0)     4078 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/province.py
--rw-r--r--   0 root         (0) root         (0)     9758 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/provisioning_information.py
--rw-r--r--   0 root         (0) root         (0)    10890 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/purchased_envelopes_information.py
--rw-r--r--   0 root         (0) root         (0)    58880 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/radio.py
--rw-r--r--   0 root         (0) root         (0)    37201 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/radio_group.py
--rw-r--r--   0 root         (0) root         (0)     7408 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_additional_notification.py
--rw-r--r--   0 root         (0) root         (0)     7241 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_attachment.py
--rw-r--r--   0 root         (0) root         (0)     5924 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_domain.py
--rw-r--r--   0 root         (0) root         (0)    11289 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     5145 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_event.py
--rw-r--r--   0 root         (0) root         (0)     9053 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_form_data.py
--rw-r--r--   0 root         (0) root         (0)     5257 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_group.py
--rw-r--r--   0 root         (0) root         (0)     5387 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_identity_input_option.py
--rw-r--r--   0 root         (0) root         (0)     9459 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_identity_phone_number.py
--rw-r--r--   0 root         (0) root         (0)     6547 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_identity_verification.py
--rw-r--r--   0 root         (0) root         (0)     5729 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_names_response.py
--rw-r--r--   0 root         (0) root         (0)     7316 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_option.py
--rw-r--r--   0 root         (0) root         (0)    12853 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_phone_authentication.py
--rw-r--r--   0 root         (0) root         (0)     6487 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_phone_number.py
--rw-r--r--   0 root         (0) root         (0)    12762 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_preview_request.py
--rw-r--r--   0 root         (0) root         (0)     4654 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_proof_file.py
--rw-r--r--   0 root         (0) root         (0)     3578 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_routing.py
--rw-r--r--   0 root         (0) root         (0)     3857 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_rules.py
--rw-r--r--   0 root         (0) root         (0)     3416 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_saml_authentication.py
--rw-r--r--   0 root         (0) root         (0)     5577 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_signature_information.py
--rw-r--r--   0 root         (0) root         (0)     8406 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)    10732 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_signature_provider_options.py
--rw-r--r--   0 root         (0) root         (0)     5495 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_sms_authentication.py
--rw-r--r--   0 root         (0) root         (0)    11624 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_token_client_ur_ls.py
--rw-r--r--   0 root         (0) root         (0)     7184 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_update_response.py
--rw-r--r--   0 root         (0) root         (0)    22630 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipient_view_request.py
--rw-r--r--   0 root         (0) root         (0)    16176 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipients.py
--rw-r--r--   0 root         (0) root         (0)     3970 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/recipients_update_summary.py
--rw-r--r--   0 root         (0) root         (0)    20200 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/referral_information.py
--rw-r--r--   0 root         (0) root         (0)     6181 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/reminders.py
--rw-r--r--   0 root         (0) root         (0)    29193 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_csv_run_request.py
--rw-r--r--   0 root         (0) root         (0)     5869 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_field.py
--rw-r--r--   0 root         (0) root         (0)    31244 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_get.py
--rw-r--r--   0 root         (0) root         (0)     3630 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_list.py
--rw-r--r--   0 root         (0) root         (0)    15380 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_list_item.py
--rw-r--r--   0 root         (0) root         (0)    25655 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_run_request.py
--rw-r--r--   0 root         (0) root         (0)     9821 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_run_response.py
--rw-r--r--   0 root         (0) root         (0)     4609 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_run_response_row.py
--rw-r--r--   0 root         (0) root         (0)   137530 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_run_response_row_fields.py
--rw-r--r--   0 root         (0) root         (0)     3856 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_save_response.py
--rw-r--r--   0 root         (0) root         (0)     4530 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/report_in_product_sent_by_details.py
--rw-r--r--   0 root         (0) root         (0)     4470 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/reserved_domain_existence.py
--rw-r--r--   0 root         (0) root         (0)     3624 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/resource_information.py
--rw-r--r--   0 root         (0) root         (0)     4608 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/return_url_request.py
--rw-r--r--   0 root         (0) root         (0)     7282 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/revision.py
--rw-r--r--   0 root         (0) root         (0)     5227 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/saml_assertion_attribute.py
--rw-r--r--   0 root         (0) root         (0)     6812 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/scheduled_sending.py
--rw-r--r--   0 root         (0) root         (0)     6324 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/scheduled_sending_api_model.py
--rw-r--r--   0 root         (0) root         (0)     4083 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/seal.py
--rw-r--r--   0 root         (0) root         (0)     4406 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/seal_identifier.py
--rw-r--r--   0 root         (0) root         (0)    69442 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/seal_sign.py
--rw-r--r--   0 root         (0) root         (0)     5342 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/seat_discount.py
--rw-r--r--   0 root         (0) root         (0)     4132 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/sender.py
--rw-r--r--   0 root         (0) root         (0)    95465 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/sender_company.py
--rw-r--r--   0 root         (0) root         (0)    16135 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/sender_email_notifications.py
--rw-r--r--   0 root         (0) root         (0)    94370 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/sender_name.py
--rw-r--r--   0 root         (0) root         (0)     4474 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/server_template.py
--rw-r--r--   0 root         (0) root         (0)     8135 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/service_information.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/service_version.py
--rw-r--r--   0 root         (0) root         (0)     7302 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/settings_metadata.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/shared_item.py
--rw-r--r--   0 root         (0) root         (0)     9010 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/sign_hash_document.py
--rw-r--r--   0 root         (0) root         (0)     9273 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/sign_hash_session_info_response.py
--rw-r--r--   0 root         (0) root         (0)    87320 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/sign_here.py
--rw-r--r--   0 root         (0) root         (0)     6365 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/sign_session_info_request.py
--rw-r--r--   0 root         (0) root         (0)     5353 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signature_data_info.py
--rw-r--r--   0 root         (0) root         (0)     4975 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signature_group.py
--rw-r--r--   0 root         (0) root         (0)     4231 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signature_group_def.py
--rw-r--r--   0 root         (0) root         (0)     3990 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signature_properties.py
--rw-r--r--   0 root         (0) root         (0)     5057 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signature_provider_required_option.py
--rw-r--r--   0 root         (0) root         (0)     4179 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signature_type.py
--rw-r--r--   0 root         (0) root         (0)     5613 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signature_user.py
--rw-r--r--   0 root         (0) root         (0)     4947 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signature_user_def.py
--rw-r--r--   0 root         (0) root         (0)   112680 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signer.py
--rw-r--r--   0 root         (0) root         (0)    86619 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signer_attachment.py
--rw-r--r--   0 root         (0) root         (0)    20403 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signer_email_notifications.py
--rw-r--r--   0 root         (0) root         (0)    10819 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signing_group.py
--rw-r--r--   0 root         (0) root         (0)     3767 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signing_group_information.py
--rw-r--r--   0 root         (0) root         (0)     5206 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signing_group_user.py
--rw-r--r--   0 root         (0) root         (0)     3555 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/signing_group_users.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/smart_contract_information.py
--rw-r--r--   0 root         (0) root         (0)    90643 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/smart_section.py
--rw-r--r--   0 root         (0) root         (0)     5820 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/smart_section_anchor_position.py
--rw-r--r--   0 root         (0) root         (0)    12081 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/smart_section_collapsible_display_settings.py
--rw-r--r--   0 root         (0) root         (0)    13796 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/smart_section_display_settings.py
--rw-r--r--   0 root         (0) root         (0)     7013 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/social_account_information.py
--rw-r--r--   0 root         (0) root         (0)     3713 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/social_authentication.py
--rw-r--r--   0 root         (0) root         (0)   120295 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/ssn.py
--rw-r--r--   0 root         (0) root         (0)     5833 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/ssn4_information_input.py
--rw-r--r--   0 root         (0) root         (0)     4711 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/ssn9_information_input.py
--rw-r--r--   0 root         (0) root         (0)    17071 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/stamp.py
--rw-r--r--   0 root         (0) root         (0)     3615 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/supported_languages.py
--rw-r--r--   0 root         (0) root         (0)    49511 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/tab_account_settings.py
--rw-r--r--   0 root         (0) root         (0)    87759 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/tab_group.py
--rw-r--r--   0 root         (0) root         (0)    55118 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/tab_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3504 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/tab_metadata_list.py
--rw-r--r--   0 root         (0) root         (0)    47428 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/tabs.py
--rw-r--r--   0 root         (0) root         (0)     4895 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_custom_fields.py
--rw-r--r--   0 root         (0) root         (0)     3929 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_document_visibility_list.py
--rw-r--r--   0 root         (0) root         (0)     4827 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_documents_result.py
--rw-r--r--   0 root         (0) root         (0)     3642 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_information.py
--rw-r--r--   0 root         (0) root         (0)     5415 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_match.py
--rw-r--r--   0 root         (0) root         (0)     6702 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    17168 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_recipients.py
--rw-r--r--   0 root         (0) root         (0)    25189 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_role.py
--rw-r--r--   0 root         (0) root         (0)     9485 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_shared_item.py
--rw-r--r--   0 root         (0) root         (0)     9238 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_summary.py
--rw-r--r--   0 root         (0) root         (0)    48716 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_tabs.py
--rw-r--r--   0 root         (0) root         (0)    12023 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_update_summary.py
--rw-r--r--   0 root         (0) root         (0)     4382 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/template_view_request.py
--rw-r--r--   0 root         (0) root         (0)   125230 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/text.py
--rw-r--r--   0 root         (0) root         (0)     8572 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/text_custom_field.py
--rw-r--r--   0 root         (0) root         (0)     5661 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/time_stamp_field.py
--rw-r--r--   0 root         (0) root         (0)   105839 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/title.py
--rw-r--r--   0 root         (0) root         (0)     6912 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/tsp_health_check_request.py
--rw-r--r--   0 root         (0) root         (0)     7650 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/tsp_health_check_status_description.py
--rw-r--r--   0 root         (0) root         (0)     4742 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/update_transaction_request.py
--rw-r--r--   0 root         (0) root         (0)     3447 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/update_transaction_response.py
--rw-r--r--   0 root         (0) root         (0)     6505 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/usage_history.py
--rw-r--r--   0 root         (0) root         (0)     7057 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user.py
--rw-r--r--   0 root         (0) root         (0)    35237 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_account_management_granular_information.py
--rw-r--r--   0 root         (0) root         (0)    10505 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorization.py
--rw-r--r--   0 root         (0) root         (0)     6120 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorization_create_request.py
--rw-r--r--   0 root         (0) root         (0)     7181 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorization_create_request_with_id.py
--rw-r--r--   0 root         (0) root         (0)     5402 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorization_id_with_status.py
--rw-r--r--   0 root         (0) root         (0)     4471 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorization_update_request.py
--rw-r--r--   0 root         (0) root         (0)     5357 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorization_with_status.py
--rw-r--r--   0 root         (0) root         (0)     9481 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorizations.py
--rw-r--r--   0 root         (0) root         (0)     3804 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorizations_delete_request.py
--rw-r--r--   0 root         (0) root         (0)     3765 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorizations_delete_response.py
--rw-r--r--   0 root         (0) root         (0)     3849 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorizations_request.py
--rw-r--r--   0 root         (0) root         (0)     3705 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_authorizations_response.py
--rw-r--r--   0 root         (0) root         (0)    13254 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_info.py
--rw-r--r--   0 root         (0) root         (0)     3486 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_info_list.py
--rw-r--r--   0 root         (0) root         (0)     5966 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_info_response.py
--rw-r--r--   0 root         (0) root         (0)    43490 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_information.py
--rw-r--r--   0 root         (0) root         (0)     9346 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_information_list.py
--rw-r--r--   0 root         (0) root         (0)     6759 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_password_information.py
--rw-r--r--   0 root         (0) root         (0)     4517 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_password_rules.py
--rw-r--r--   0 root         (0) root         (0)    14770 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_profile.py
--rw-r--r--   0 root         (0) root         (0)   168247 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_settings_information.py
--rw-r--r--   0 root         (0) root         (0)     5192 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_shared_item.py
--rw-r--r--   0 root         (0) root         (0)    31028 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_signature.py
--rw-r--r--   0 root         (0) root         (0)    17594 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_signature_definition.py
--rw-r--r--   0 root         (0) root         (0)     3797 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_signatures_information.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/user_social_id_result.py
--rw-r--r--   0 root         (0) root         (0)     9127 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/users_response.py
--rw-r--r--   0 root         (0) root         (0)    93319 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/view.py
--rw-r--r--   0 root         (0) root         (0)     3436 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/view_url.py
--rw-r--r--   0 root         (0) root         (0)    10333 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/watermark.py
--rw-r--r--   0 root         (0) root         (0)   112714 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/witness.py
--rw-r--r--   0 root         (0) root         (0)     8038 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workflow.py
--rw-r--r--   0 root         (0) root         (0)    10414 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workflow_step.py
--rw-r--r--   0 root         (0) root         (0)    14793 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workspace.py
--rw-r--r--   0 root         (0) root         (0)    10272 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workspace_folder_contents.py
--rw-r--r--   0 root         (0) root         (0)    22565 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workspace_item.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workspace_item_list.py
--rw-r--r--   0 root         (0) root         (0)     7440 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workspace_list.py
--rw-r--r--   0 root         (0) root         (0)     3695 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workspace_settings.py
--rw-r--r--   0 root         (0) root         (0)    18913 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workspace_user.py
--rw-r--r--   0 root         (0) root         (0)    12341 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/workspace_user_authorization.py
--rw-r--r--   0 root         (0) root         (0)   121905 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/docusign_esign/models/zip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/docusign_esign.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5853 2024-05-22 11:46:34.000000 docusign-esign-4.0.0/docusign_esign.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28060 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/docusign_esign.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 11:46:34.000000 docusign-esign-4.0.0/docusign_esign.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      128 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/docusign_esign.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/docusign_esign.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 11:46:35.000000 docusign-esign-4.0.0/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/test/test_oauth.py
--rw-r--r--   0 root         (0) root         (0)    41312 2024-05-22 11:46:31.000000 docusign-esign-4.0.0/test/unit_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5856 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5619 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/docusign_esign/
+-rw-r--r--   0 root         (0) root         (0)    39088 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   428943 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/accounts_api.py
+-rw-r--r--   0 root         (0) root         (0)    36525 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)    77219 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/billing_api.py
+-rw-r--r--   0 root         (0) root         (0)   105694 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/bulk_envelopes_api.py
+-rw-r--r--   0 root         (0) root         (0)    40007 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/bulk_process_data_api.py
+-rw-r--r--   0 root         (0) root         (0)    24433 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/bulk_process_data_send_api.py
+-rw-r--r--   0 root         (0) root         (0)    51067 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/cloud_storage_api.py
+-rw-r--r--   0 root         (0) root         (0)   114632 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/connect_api.py
+-rw-r--r--   0 root         (0) root         (0)    26196 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/custom_tabs_api.py
+-rw-r--r--   0 root         (0) root         (0)     6118 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/data_feed_api.py
+-rw-r--r--   0 root         (0) root         (0)    34477 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/diagnostics_api.py
+-rw-r--r--   0 root         (0) root         (0)    23507 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/email_archive_api.py
+-rw-r--r--   0 root         (0) root         (0)   840521 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/envelopes_api.py
+-rw-r--r--   0 root         (0) root         (0)    29607 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/folders_api.py
+-rw-r--r--   0 root         (0) root         (0)    53159 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/groups_api.py
+-rw-r--r--   0 root         (0) root         (0)    47724 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/notary_api.py
+-rw-r--r--   0 root         (0) root         (0)     6111 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/organizations_api.py
+-rw-r--r--   0 root         (0) root         (0)    49102 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/power_forms_api.py
+-rw-r--r--   0 root         (0) root         (0)    20853 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/signature_api.py
+-rw-r--r--   0 root         (0) root         (0)    47054 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/signing_groups_api.py
+-rw-r--r--   0 root         (0) root         (0)   301558 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/templates_api.py
+-rw-r--r--   0 root         (0) root         (0)     5488 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/trust_service_providers_api.py
+-rw-r--r--   0 root         (0) root         (0)   196161 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/users_api.py
+-rw-r--r--   0 root         (0) root         (0)    67009 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/apis/workspaces_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/docusign_esign/client/
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35384 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/client/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/client/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)    13506 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/client/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/docusign_esign/client/auth/
+-rw-r--r--   0 root         (0) root         (0)      547 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/client/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14771 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/client/auth/oauth.py
+-rw-r--r--   0 root         (0) root         (0)     8903 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/client/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/docusign_esign/models/
+-rw-r--r--   0 root         (0) root         (0)    37584 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13277 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/access_code_format.py
+-rw-r--r--   0 root         (0) root         (0)    11983 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_address.py
+-rw-r--r--   0 root         (0) root         (0)    31800 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_billing_plan.py
+-rw-r--r--   0 root         (0) root         (0)    17814 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_billing_plan_response.py
+-rw-r--r--   0 root         (0) root         (0)     5281 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_identity_input_option.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_identity_verification_response.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_identity_verification_step.py
+-rw-r--r--   0 root         (0) root         (0)    12168 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_identity_verification_workflow.py
+-rw-r--r--   0 root         (0) root         (0)    39158 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_information.py
+-rw-r--r--   0 root         (0) root         (0)     4625 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_minimum_password_length.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_notification.py
+-rw-r--r--   0 root         (0) root         (0)     4618 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_password_expire_password_days.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_password_lockout_duration_minutes.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_password_lockout_duration_type.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_password_minimum_password_age_days.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_password_questions_required.py
+-rw-r--r--   0 root         (0) root         (0)    25898 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_password_rules.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_password_strength_type.py
+-rw-r--r--   0 root         (0) root         (0)    10429 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_password_strength_type_option.py
+-rw-r--r--   0 root         (0) root         (0)   113332 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_role_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_seals.py
+-rw-r--r--   0 root         (0) root         (0)   939466 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_settings_information.py
+-rw-r--r--   0 root         (0) root         (0)    11434 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_shared_access.py
+-rw-r--r--   0 root         (0) root         (0)    32500 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_signature.py
+-rw-r--r--   0 root         (0) root         (0)    19678 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_signature_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10210 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     6491 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_signature_provider_option.py
+-rw-r--r--   0 root         (0) root         (0)     3902 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_signature_providers.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_signatures_information.py
+-rw-r--r--   0 root         (0) root         (0)    42099 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/account_ui_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5302 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/add_on.py
+-rw-r--r--   0 root         (0) root         (0)     9933 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/address_information.py
+-rw-r--r--   0 root         (0) root         (0)     7146 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/address_information_input.py
+-rw-r--r--   0 root         (0) root         (0)     7769 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/address_information_v2.py
+-rw-r--r--   0 root         (0) root         (0)     4417 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/admin_message.py
+-rw-r--r--   0 root         (0) root         (0)    88051 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/agent.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/api_request_log.py
+-rw-r--r--   0 root         (0) root         (0)     3795 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/api_request_logs_result.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/app_store_product.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/app_store_receipt.py
+-rw-r--r--   0 root         (0) root         (0)    91945 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/approve.py
+-rw-r--r--   0 root         (0) root         (0)     5355 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/ask_an_admin.py
+-rw-r--r--   0 root         (0) root         (0)     7885 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/attachment.py
+-rw-r--r--   0 root         (0) root         (0)     6791 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)    26660 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/authentication_status.py
+-rw-r--r--   0 root         (0) root         (0)     5678 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/authorization_user.py
+-rw-r--r--   0 root         (0) root         (0)     5791 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_address.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_archive.py
+-rw-r--r--   0 root         (0) root         (0)     7856 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_archive_history.py
+-rw-r--r--   0 root         (0) root         (0)     9955 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_archive_history_list.py
+-rw-r--r--   0 root         (0) root         (0)     9578 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_archive_list.py
+-rw-r--r--   0 root         (0) root         (0)    16119 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_charge.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_charge_response.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_discount.py
+-rw-r--r--   0 root         (0) root         (0)     6585 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_entity_information_response.py
+-rw-r--r--   0 root         (0) root         (0)    10843 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     8481 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_invoice_item.py
+-rw-r--r--   0 root         (0) root         (0)     5728 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_invoices_response.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_invoices_summary.py
+-rw-r--r--   0 root         (0) root         (0)     5019 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_payment.py
+-rw-r--r--   0 root         (0) root         (0)     7040 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_payment_item.py
+-rw-r--r--   0 root         (0) root         (0)     3957 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_payments_response.py
+-rw-r--r--   0 root         (0) root         (0)    16632 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan.py
+-rw-r--r--   0 root         (0) root         (0)    24833 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan_information.py
+-rw-r--r--   0 root         (0) root         (0)     7645 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan_preview.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan_response.py
+-rw-r--r--   0 root         (0) root         (0)     9929 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan_update_response.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_plans_response.py
+-rw-r--r--   0 root         (0) root         (0)     5164 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/billing_price.py
+-rw-r--r--   0 root         (0) root         (0)    17441 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brand.py
+-rw-r--r--   0 root         (0) root         (0)     5965 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brand_email_content.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brand_link.py
+-rw-r--r--   0 root         (0) root         (0)     4811 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brand_logos.py
+-rw-r--r--   0 root         (0) root         (0)     3580 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brand_request.py
+-rw-r--r--   0 root         (0) root         (0)     5735 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brand_resource_urls.py
+-rw-r--r--   0 root         (0) root         (0)    10377 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brand_resources.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brand_resources_list.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brands_request.py
+-rw-r--r--   0 root         (0) root         (0)     5833 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/brands_response.py
+-rw-r--r--   0 root         (0) root         (0)    11143 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_envelope.py
+-rw-r--r--   0 root         (0) root         (0)    15435 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_envelope_status.py
+-rw-r--r--   0 root         (0) root         (0)     9563 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_envelopes_response.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_process_request.py
+-rw-r--r--   0 root         (0) root         (0)     8228 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_process_response.py
+-rw-r--r--   0 root         (0) root         (0)     4974 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_processing_list_summaries.py
+-rw-r--r--   0 root         (0) root         (0)     6204 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_processing_list_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_processing_lists.py
+-rw-r--r--   0 root         (0) root         (0)    14950 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     4375 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipient_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipient_tab_label.py
+-rw-r--r--   0 root         (0) root         (0)     3919 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipients_request.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipients_response.py
+-rw-r--r--   0 root         (0) root         (0)     7157 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipients_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipients_update_response.py
+-rw-r--r--   0 root         (0) root         (0)     5253 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_action_request.py
+-rw-r--r--   0 root         (0) root         (0)     4298 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_error.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_request.py
+-rw-r--r--   0 root         (0) root         (0)    17291 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_status.py
+-rw-r--r--   0 root         (0) root         (0)    14262 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_summaries.py
+-rw-r--r--   0 root         (0) root         (0)    10233 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_summary.py
+-rw-r--r--   0 root         (0) root         (0)    13105 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_envelopes_info.py
+-rw-r--r--   0 root         (0) root         (0)     6145 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_error_status.py
+-rw-r--r--   0 root         (0) root         (0)     4544 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_request.py
+-rw-r--r--   0 root         (0) root         (0)     9108 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_response.py
+-rw-r--r--   0 root         (0) root         (0)     5573 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_test_response.py
+-rw-r--r--   0 root         (0) root         (0)     8021 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_copy.py
+-rw-r--r--   0 root         (0) root         (0)     4323 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_copy_custom_field.py
+-rw-r--r--   0 root         (0) root         (0)    37255 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_copy_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     4529 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_copy_tab.py
+-rw-r--r--   0 root         (0) root         (0)     4966 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_list.py
+-rw-r--r--   0 root         (0) root         (0)     3886 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_list_summaries.py
+-rw-r--r--   0 root         (0) root         (0)     6087 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_list_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4375 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/bulksending_copy_doc_gen_form_field.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/captive_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     4028 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/captive_recipient_information.py
+-rw-r--r--   0 root         (0) root         (0)    94162 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/carbon_copy.py
+-rw-r--r--   0 root         (0) root         (0)    94115 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/certified_delivery.py
+-rw-r--r--   0 root         (0) root         (0)   105043 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     4196 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/chunked_upload_part.py
+-rw-r--r--   0 root         (0) root         (0)     4395 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/chunked_upload_request.py
+-rw-r--r--   0 root         (0) root         (0)    10714 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/chunked_upload_response.py
+-rw-r--r--   0 root         (0) root         (0)     8154 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/cloud_storage_provider.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/cloud_storage_providers.py
+-rw-r--r--   0 root         (0) root         (0)    19343 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/comment.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/comment_history_result.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/comment_publish.py
+-rw-r--r--   0 root         (0) root         (0)    93586 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/comment_thread.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/comments_publish.py
+-rw-r--r--   0 root         (0) root         (0)   110382 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/commission_county.py
+-rw-r--r--   0 root         (0) root         (0)   112034 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/commission_expiration.py
+-rw-r--r--   0 root         (0) root         (0)   110382 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/commission_number.py
+-rw-r--r--   0 root         (0) root         (0)   109969 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/commission_state.py
+-rw-r--r--   0 root         (0) root         (0)   106745 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/company.py
+-rw-r--r--   0 root         (0) root         (0)     5556 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/complete_sign_hash_response.py
+-rw-r--r--   0 root         (0) root         (0)     9079 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/complete_sign_request.py
+-rw-r--r--   0 root         (0) root         (0)     9603 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/composite_template.py
+-rw-r--r--   0 root         (0) root         (0)     6568 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/conditional_recipient_rule.py
+-rw-r--r--   0 root         (0) root         (0)     5408 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/conditional_recipient_rule_condition.py
+-rw-r--r--   0 root         (0) root         (0)     8761 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/conditional_recipient_rule_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4617 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_config_results.py
+-rw-r--r--   0 root         (0) root         (0)    49382 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_custom_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6888 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_debug_log.py
+-rw-r--r--   0 root         (0) root         (0)     2881 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_delete_failure_result.py
+-rw-r--r--   0 root         (0) root         (0)     5002 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_event_data.py
+-rw-r--r--   0 root         (0) root         (0)     4450 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_failure_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7197 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_failure_result.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_failure_results.py
+-rw-r--r--   0 root         (0) root         (0)     4558 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_historical_envelope_republish.py
+-rw-r--r--   0 root         (0) root         (0)    17883 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_log.py
+-rw-r--r--   0 root         (0) root         (0)     6011 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_logs.py
+-rw-r--r--   0 root         (0) root         (0)     6940 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_o_auth_config.py
+-rw-r--r--   0 root         (0) root         (0)     8902 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_salesforce_field.py
+-rw-r--r--   0 root         (0) root         (0)     9993 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_salesforce_object.py
+-rw-r--r--   0 root         (0) root         (0)     5655 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_user_info.py
+-rw-r--r--   0 root         (0) root         (0)     7148 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/connect_user_object.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/consent_details.py
+-rw-r--r--   0 root         (0) root         (0)     4625 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/console_view_request.py
+-rw-r--r--   0 root         (0) root         (0)    35223 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/consumer_disclosure.py
+-rw-r--r--   0 root         (0) root         (0)    14823 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/contact.py
+-rw-r--r--   0 root         (0) root         (0)     9343 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/contact_get_response.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/contact_mod_request.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/contact_phone_number.py
+-rw-r--r--   0 root         (0) root         (0)     3618 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/contact_update_response.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/correct_view_request.py
+-rw-r--r--   0 root         (0) root         (0)     5647 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/country.py
+-rw-r--r--   0 root         (0) root         (0)     5359 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/credential.py
+-rw-r--r--   0 root         (0) root         (0)    10769 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/credit_card_information.py
+-rw-r--r--   0 root         (0) root         (0)     3683 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/credit_card_types.py
+-rw-r--r--   0 root         (0) root         (0)   118797 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/currency.py
+-rw-r--r--   0 root         (0) root         (0)     7661 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/currency_feature_set_price.py
+-rw-r--r--   0 root         (0) root         (0)    10088 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/currency_plan_price.py
+-rw-r--r--   0 root         (0) root         (0)     8698 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/custom_field.py
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/custom_field_v2.py
+-rw-r--r--   0 root         (0) root         (0)     4791 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/custom_fields.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/custom_fields_envelope.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/custom_settings_information.py
+-rw-r--r--   0 root         (0) root         (0)   120684 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/date.py
+-rw-r--r--   0 root         (0) root         (0)    94370 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/date_signed.py
+-rw-r--r--   0 root         (0) root         (0)     6112 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/date_stamp_properties.py
+-rw-r--r--   0 root         (0) root         (0)    93947 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/decline.py
+-rw-r--r--   0 root         (0) root         (0)     6268 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/delayed_routing.py
+-rw-r--r--   0 root         (0) root         (0)     6568 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/delayed_routing_api_model.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/delegation_info.py
+-rw-r--r--   0 root         (0) root         (0)     6551 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/diagnostics_settings_information.py
+-rw-r--r--   0 root         (0) root         (0)    13477 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/direct_debit_processor_information.py
+-rw-r--r--   0 root         (0) root         (0)     7881 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_account.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_custom_field.py
+-rw-r--r--   0 root         (0) root         (0)    12940 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_document.py
+-rw-r--r--   0 root         (0) root         (0)     9685 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_document_page.py
+-rw-r--r--   0 root         (0) root         (0)    18516 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_envelope.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_info.py
+-rw-r--r--   0 root         (0) root         (0)     9243 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_page.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_pdf.py
+-rw-r--r--   0 root         (0) root         (0)    25341 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_signer_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/dob_information_input.py
+-rw-r--r--   0 root         (0) root         (0)    10404 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field.py
+-rw-r--r--   0 root         (0) root         (0)     5794 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_option.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     4746 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_response.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_row_value.py
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_validation.py
+-rw-r--r--   0 root         (0) root         (0)     6715 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_fields.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_syntax_error.py
+-rw-r--r--   0 root         (0) root         (0)    30429 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document.py
+-rw-r--r--   0 root         (0) root         (0)     4623 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_fields_information.py
+-rw-r--r--   0 root         (0) root         (0)    12081 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_html_collapsible_display_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12749 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_html_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_html_definition_original.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_html_definition_originals.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_html_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8339 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_html_display_anchor.py
+-rw-r--r--   0 root         (0) root         (0)    13796 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_html_display_settings.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_security_store.py
+-rw-r--r--   0 root         (0) root         (0)     7423 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_template.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_template_list.py
+-rw-r--r--   0 root         (0) root         (0)     8591 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_update_info.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_visibility.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/document_visibility_list.py
+-rw-r--r--   0 root         (0) root         (0)     4990 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/downgrad_request_billing_info_response.py
+-rw-r--r--   0 root         (0) root         (0)     8633 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/downgrade_billing_plan_information.py
+-rw-r--r--   0 root         (0) root         (0)    14854 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/downgrade_plan_update_response.py
+-rw-r--r--   0 root         (0) root         (0)     6119 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/downgrade_request_information.py
+-rw-r--r--   0 root         (0) root         (0)    83131 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/draw.py
+-rw-r--r--   0 root         (0) root         (0)     7570 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/e_note_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    86073 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/editor.py
+-rw-r--r--   0 root         (0) root         (0)   121153 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/email.py
+-rw-r--r--   0 root         (0) root         (0)    95100 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/email_address.py
+-rw-r--r--   0 root         (0) root         (0)     6088 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/email_settings.py
+-rw-r--r--   0 root         (0) root         (0)    78819 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_attachments_request.py
+-rw-r--r--   0 root         (0) root         (0)     3741 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_attachments_result.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_audit_event.py
+-rw-r--r--   0 root         (0) root         (0)     3793 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_audit_event_response.py
+-rw-r--r--   0 root         (0) root         (0)     4062 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_custom_metadata.py
+-rw-r--r--   0 root         (0) root         (0)    98736 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5337 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_delay_rule.py
+-rw-r--r--   0 root         (0) root         (0)     5441 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_delay_rule_api_model.py
+-rw-r--r--   0 root         (0) root         (0)    31835 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_document.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_documents_result.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_event.py
+-rw-r--r--   0 root         (0) root         (0)     9783 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_form_data.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_form_data_prefill_form_data.py
+-rw-r--r--   0 root         (0) root         (0)    92708 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_id.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_ids_request.py
+-rw-r--r--   0 root         (0) root         (0)     5573 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     5766 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    16022 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_publish_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     4509 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_publish_transaction_error_rollup.py
+-rw-r--r--   0 root         (0) root         (0)     6656 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_purge_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    10287 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_summary.py
+-rw-r--r--   0 root         (0) root         (0)   100293 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_template.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_template_definition.py
+-rw-r--r--   0 root         (0) root         (0)    59810 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_template_result.py
+-rw-r--r--   0 root         (0) root         (0)    10527 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_template_results.py
+-rw-r--r--   0 root         (0) root         (0)     7470 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_transaction_status.py
+-rw-r--r--   0 root         (0) root         (0)    11767 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_transfer_rule.py
+-rw-r--r--   0 root         (0) root         (0)    10079 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_transfer_rule_information.py
+-rw-r--r--   0 root         (0) root         (0)    11938 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_transfer_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)    12023 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_update_summary.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_document_settings.py
+-rw-r--r--   0 root         (0) root         (0)     4089 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_envelope_custom_field_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_recipient_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5157 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_request.py
+-rw-r--r--   0 root         (0) root         (0)    15021 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5584 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_tagger_settings.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_template_settings.py
+-rw-r--r--   0 root         (0) root         (0)    14217 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/envelopes_information.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)    26563 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/event_notification.py
+-rw-r--r--   0 root         (0) root         (0)     6541 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/event_result.py
+-rw-r--r--   0 root         (0) root         (0)     6087 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/expirations.py
+-rw-r--r--   0 root         (0) root         (0)     5475 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/external_claim.py
+-rw-r--r--   0 root         (0) root         (0)     5427 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/external_doc_service_error_details.py
+-rw-r--r--   0 root         (0) root         (0)    12835 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/external_document_sources.py
+-rw-r--r--   0 root         (0) root         (0)     9541 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/external_file.py
+-rw-r--r--   0 root         (0) root         (0)    11306 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/external_folder.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/external_primary_account_recipient_auth_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     5671 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/favorite_templates_content_item.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/favorite_templates_info.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/feature_available_metadata.py
+-rw-r--r--   0 root         (0) root         (0)    10487 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/feature_set.py
+-rw-r--r--   0 root         (0) root         (0)     4399 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/file_type.py
+-rw-r--r--   0 root         (0) root         (0)     3629 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/file_type_list.py
+-rw-r--r--   0 root         (0) root         (0)    11057 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/filter.py
+-rw-r--r--   0 root         (0) root         (0)    94005 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/first_name.py
+-rw-r--r--   0 root         (0) root         (0)    13945 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/folder.py
+-rw-r--r--   0 root         (0) root         (0)    17939 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/folder_item.py
+-rw-r--r--   0 root         (0) root         (0)     9136 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/folder_item_response.py
+-rw-r--r--   0 root         (0) root         (0)    20880 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/folder_item_v2.py
+-rw-r--r--   0 root         (0) root         (0)    10151 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/folder_items_response.py
+-rw-r--r--   0 root         (0) root         (0)    11417 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/folder_shared_item.py
+-rw-r--r--   0 root         (0) root         (0)     5233 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/folders_request.py
+-rw-r--r--   0 root         (0) root         (0)    10003 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/folders_response.py
+-rw-r--r--   0 root         (0) root         (0)    12851 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/forgotten_password_information.py
+-rw-r--r--   0 root         (0) root         (0)     8611 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/form_data_item.py
+-rw-r--r--   0 root         (0) root         (0)   133296 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/formula_tab.py
+-rw-r--r--   0 root         (0) root         (0)    93640 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/full_name.py
+-rw-r--r--   0 root         (0) root         (0)     5073 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/graphics_context.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     5907 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/group_brands.py
+-rw-r--r--   0 root         (0) root         (0)     9387 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/group_information.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/id_check_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7874 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/id_check_information_input.py
+-rw-r--r--   0 root         (0) root         (0)     3587 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/id_check_security_step.py
+-rw-r--r--   0 root         (0) root         (0)     4559 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/id_evidence_resource_token.py
+-rw-r--r--   0 root         (0) root         (0)     3578 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/id_evidence_view_link.py
+-rw-r--r--   0 root         (0) root         (0)   111517 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/in_person_signer.py
+-rw-r--r--   0 root         (0) root         (0)    85322 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/initial_here.py
+-rw-r--r--   0 root         (0) root         (0)     7832 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/inline_template.py
+-rw-r--r--   0 root         (0) root         (0)     9676 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/integrated_connect_user_info_list.py
+-rw-r--r--   0 root         (0) root         (0)    10338 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/integrated_user_info_list.py
+-rw-r--r--   0 root         (0) root         (0)    90158 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/intermediary.py
+-rw-r--r--   0 root         (0) root         (0)    11103 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/jurisdiction.py
+-rw-r--r--   0 root         (0) root         (0)     6419 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/jurisdiction_summary.py
+-rw-r--r--   0 root         (0) root         (0)    93640 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/last_name.py
+-rw-r--r--   0 root         (0) root         (0)    10192 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/linked_external_primary_account.py
+-rw-r--r--   0 root         (0) root         (0)   110330 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/list.py
+-rw-r--r--   0 root         (0) root         (0)     9399 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/list_custom_field.py
+-rw-r--r--   0 root         (0) root         (0)     7999 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/list_item.py
+-rw-r--r--   0 root         (0) root         (0)    43378 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/locale_policy.py
+-rw-r--r--   0 root         (0) root         (0)    14590 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/locale_policy_tab.py
+-rw-r--r--   0 root         (0) root         (0)    10997 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/lock_information.py
+-rw-r--r--   0 root         (0) root         (0)     7711 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/lock_request.py
+-rw-r--r--   0 root         (0) root         (0)    12815 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/login_account.py
+-rw-r--r--   0 root         (0) root         (0)     4970 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/login_information.py
+-rw-r--r--   0 root         (0) root         (0)     6882 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/match_box.py
+-rw-r--r--   0 root         (0) root         (0)     5266 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/member_group_shared_item.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/member_shared_items.py
+-rw-r--r--   0 root         (0) root         (0)    14847 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/merge_field.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/mobile_notifier_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/mobile_notifier_configuration_information.py
+-rw-r--r--   0 root         (0) root         (0)   123029 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/model_date.py
+-rw-r--r--   0 root         (0) root         (0)     5082 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/money.py
+-rw-r--r--   0 root         (0) root         (0)     5937 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/name_value.py
+-rw-r--r--   0 root         (0) root         (0)    22204 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/new_account_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9520 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/new_account_summary.py
+-rw-r--r--   0 root         (0) root         (0)    11493 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/new_user.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/new_users_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3581 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/new_users_summary.py
+-rw-r--r--   0 root         (0) root         (0)    79841 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notarize.py
+-rw-r--r--   0 root         (0) root         (0)     5719 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary.py
+-rw-r--r--   0 root         (0) root         (0)    76227 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     4749 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_contact_details.py
+-rw-r--r--   0 root         (0) root         (0)    79330 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_host.py
+-rw-r--r--   0 root         (0) root         (0)     8019 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_journal.py
+-rw-r--r--   0 root         (0) root         (0)     5206 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_journal_credible_witness.py
+-rw-r--r--   0 root         (0) root         (0)     9453 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_journal_list.py
+-rw-r--r--   0 root         (0) root         (0)     6269 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_journal_meta_data.py
+-rw-r--r--   0 root         (0) root         (0)     8712 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_jurisdiction.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_jurisdiction_list.py
+-rw-r--r--   0 root         (0) root         (0)   118673 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_result.py
+-rw-r--r--   0 root         (0) root         (0)    82091 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notary_seal.py
+-rw-r--r--   0 root         (0) root         (0)    93944 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/note.py
+-rw-r--r--   0 root         (0) root         (0)     5691 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notification_default_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5204 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/notification_defaults.py
+-rw-r--r--   0 root         (0) root         (0)   126200 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/number.py
+-rw-r--r--   0 root         (0) root         (0)   115339 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/numerical.py
+-rw-r--r--   0 root         (0) root         (0)     7198 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/oauth_access.py
+-rw-r--r--   0 root         (0) root         (0)     6939 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/ocr_request.py
+-rw-r--r--   0 root         (0) root         (0)     8568 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/offline_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     8316 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/page.py
+-rw-r--r--   0 root         (0) root         (0)     9016 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/page_images.py
+-rw-r--r--   0 root         (0) root         (0)     4326 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/page_request.py
+-rw-r--r--   0 root         (0) root         (0)     3588 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/page_size.py
+-rw-r--r--   0 root         (0) root         (0)     3498 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/palette_item_settings.py
+-rw-r--r--   0 root         (0) root         (0)     8224 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/palette_settings.py
+-rw-r--r--   0 root         (0) root         (0)    83205 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/participant.py
+-rw-r--r--   0 root         (0) root         (0)     4891 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/path_extended_element.py
+-rw-r--r--   0 root         (0) root         (0)     6454 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/pay_pal_legacy_settings.py
+-rw-r--r--   0 root         (0) root         (0)    19177 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/payment_details.py
+-rw-r--r--   0 root         (0) root         (0)    16489 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/payment_gateway_account.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/payment_gateway_account_setting.py
+-rw-r--r--   0 root         (0) root         (0)     3991 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/payment_gateway_accounts_info.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/payment_line_item.py
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/payment_method_with_options.py
+-rw-r--r--   0 root         (0) root         (0)     5457 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/payment_processor_information.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/payment_signer_values.py
+-rw-r--r--   0 root         (0) root         (0)     9011 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/permission_profile.py
+-rw-r--r--   0 root         (0) root         (0)     4032 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/permission_profile_information.py
+-rw-r--r--   0 root         (0) root         (0)   108317 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/phone_number.py
+-rw-r--r--   0 root         (0) root         (0)     8214 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/plan_information.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/poly_line.py
+-rw-r--r--   0 root         (0) root         (0)    86376 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/poly_line_overlay.py
+-rw-r--r--   0 root         (0) root         (0)    23001 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/power_form.py
+-rw-r--r--   0 root         (0) root         (0)     4732 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/power_form_form_data_envelope.py
+-rw-r--r--   0 root         (0) root         (0)     6103 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/power_form_form_data_recipient.py
+-rw-r--r--   0 root         (0) root         (0)    16344 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/power_form_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     9722 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/power_form_senders_response.py
+-rw-r--r--   0 root         (0) root         (0)     3735 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/power_forms_form_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/power_forms_request.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/power_forms_response.py
+-rw-r--r--   0 root         (0) root         (0)     5950 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/prefill_form_data.py
+-rw-r--r--   0 root         (0) root         (0)    16899 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/prefill_tabs.py
+-rw-r--r--   0 root         (0) root         (0)     4585 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/proof_service_resource_token.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/proof_service_view_link.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/property_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     4078 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/province.py
+-rw-r--r--   0 root         (0) root         (0)     9758 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/provisioning_information.py
+-rw-r--r--   0 root         (0) root         (0)    10890 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/purchased_envelopes_information.py
+-rw-r--r--   0 root         (0) root         (0)    58880 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/radio.py
+-rw-r--r--   0 root         (0) root         (0)    37201 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/radio_group.py
+-rw-r--r--   0 root         (0) root         (0)     7408 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_additional_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7241 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     5924 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_domain.py
+-rw-r--r--   0 root         (0) root         (0)    11289 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     5145 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_event.py
+-rw-r--r--   0 root         (0) root         (0)     9053 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_form_data.py
+-rw-r--r--   0 root         (0) root         (0)     5257 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_group.py
+-rw-r--r--   0 root         (0) root         (0)     5387 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_identity_input_option.py
+-rw-r--r--   0 root         (0) root         (0)     9459 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_identity_phone_number.py
+-rw-r--r--   0 root         (0) root         (0)     6547 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_identity_verification.py
+-rw-r--r--   0 root         (0) root         (0)     5729 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_names_response.py
+-rw-r--r--   0 root         (0) root         (0)     7316 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_option.py
+-rw-r--r--   0 root         (0) root         (0)    12853 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_phone_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_phone_number.py
+-rw-r--r--   0 root         (0) root         (0)    12762 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_preview_request.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_proof_file.py
+-rw-r--r--   0 root         (0) root         (0)     3578 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_routing.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_rules.py
+-rw-r--r--   0 root         (0) root         (0)     3416 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_saml_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     5577 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_signature_information.py
+-rw-r--r--   0 root         (0) root         (0)     8406 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)    10732 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_signature_provider_options.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_sms_authentication.py
+-rw-r--r--   0 root         (0) root         (0)    11624 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_token_client_ur_ls.py
+-rw-r--r--   0 root         (0) root         (0)     7184 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_update_response.py
+-rw-r--r--   0 root         (0) root         (0)    22630 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipient_view_request.py
+-rw-r--r--   0 root         (0) root         (0)    16176 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipients.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/recipients_update_summary.py
+-rw-r--r--   0 root         (0) root         (0)    20200 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/referral_information.py
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/reminders.py
+-rw-r--r--   0 root         (0) root         (0)    29193 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_csv_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     5869 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_field.py
+-rw-r--r--   0 root         (0) root         (0)    31244 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_get.py
+-rw-r--r--   0 root         (0) root         (0)     3630 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_list.py
+-rw-r--r--   0 root         (0) root         (0)    15380 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_list_item.py
+-rw-r--r--   0 root         (0) root         (0)    25655 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     9821 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_run_response.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_run_response_row.py
+-rw-r--r--   0 root         (0) root         (0)   137530 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_run_response_row_fields.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_save_response.py
+-rw-r--r--   0 root         (0) root         (0)     4530 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_sent_by_details.py
+-rw-r--r--   0 root         (0) root         (0)     4470 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/reserved_domain_existence.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/resource_information.py
+-rw-r--r--   0 root         (0) root         (0)     4608 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/return_url_request.py
+-rw-r--r--   0 root         (0) root         (0)     7282 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/revision.py
+-rw-r--r--   0 root         (0) root         (0)     5227 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/saml_assertion_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     6812 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/scheduled_sending.py
+-rw-r--r--   0 root         (0) root         (0)     6324 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/scheduled_sending_api_model.py
+-rw-r--r--   0 root         (0) root         (0)     4083 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/seal.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/seal_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    69442 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/seal_sign.py
+-rw-r--r--   0 root         (0) root         (0)     5342 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/seat_discount.py
+-rw-r--r--   0 root         (0) root         (0)     4132 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/sender.py
+-rw-r--r--   0 root         (0) root         (0)    95465 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/sender_company.py
+-rw-r--r--   0 root         (0) root         (0)    16135 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/sender_email_notifications.py
+-rw-r--r--   0 root         (0) root         (0)    94370 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/sender_name.py
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/server_template.py
+-rw-r--r--   0 root         (0) root         (0)     8135 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/service_information.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/service_version.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/settings_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/shared_item.py
+-rw-r--r--   0 root         (0) root         (0)     9010 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/sign_hash_document.py
+-rw-r--r--   0 root         (0) root         (0)     9273 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/sign_hash_session_info_response.py
+-rw-r--r--   0 root         (0) root         (0)    87320 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/sign_here.py
+-rw-r--r--   0 root         (0) root         (0)     6365 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/sign_session_info_request.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signature_data_info.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signature_group.py
+-rw-r--r--   0 root         (0) root         (0)     4231 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signature_group_def.py
+-rw-r--r--   0 root         (0) root         (0)     3990 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signature_properties.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signature_provider_required_option.py
+-rw-r--r--   0 root         (0) root         (0)     4179 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signature_type.py
+-rw-r--r--   0 root         (0) root         (0)     5613 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signature_user.py
+-rw-r--r--   0 root         (0) root         (0)     4947 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signature_user_def.py
+-rw-r--r--   0 root         (0) root         (0)   112680 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signer.py
+-rw-r--r--   0 root         (0) root         (0)    86619 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signer_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    20403 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signer_email_notifications.py
+-rw-r--r--   0 root         (0) root         (0)    10819 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signing_group.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signing_group_information.py
+-rw-r--r--   0 root         (0) root         (0)     5206 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signing_group_user.py
+-rw-r--r--   0 root         (0) root         (0)     3555 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/signing_group_users.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/smart_contract_information.py
+-rw-r--r--   0 root         (0) root         (0)    90643 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/smart_section.py
+-rw-r--r--   0 root         (0) root         (0)     5820 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/smart_section_anchor_position.py
+-rw-r--r--   0 root         (0) root         (0)    12081 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/smart_section_collapsible_display_settings.py
+-rw-r--r--   0 root         (0) root         (0)    13796 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/smart_section_display_settings.py
+-rw-r--r--   0 root         (0) root         (0)     7013 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/social_account_information.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/social_authentication.py
+-rw-r--r--   0 root         (0) root         (0)   120295 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/ssn.py
+-rw-r--r--   0 root         (0) root         (0)     5833 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/ssn4_information_input.py
+-rw-r--r--   0 root         (0) root         (0)     4711 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/ssn9_information_input.py
+-rw-r--r--   0 root         (0) root         (0)    17071 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/stamp.py
+-rw-r--r--   0 root         (0) root         (0)     3615 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/supported_languages.py
+-rw-r--r--   0 root         (0) root         (0)    49511 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/tab_account_settings.py
+-rw-r--r--   0 root         (0) root         (0)    87759 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/tab_group.py
+-rw-r--r--   0 root         (0) root         (0)    55118 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/tab_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/tab_metadata_list.py
+-rw-r--r--   0 root         (0) root         (0)    47428 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/tabs.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_custom_fields.py
+-rw-r--r--   0 root         (0) root         (0)     3929 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_document_visibility_list.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_documents_result.py
+-rw-r--r--   0 root         (0) root         (0)     3642 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_information.py
+-rw-r--r--   0 root         (0) root         (0)     5415 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_match.py
+-rw-r--r--   0 root         (0) root         (0)     6702 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    17168 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_recipients.py
+-rw-r--r--   0 root         (0) root         (0)    25189 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_role.py
+-rw-r--r--   0 root         (0) root         (0)     9485 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_shared_item.py
+-rw-r--r--   0 root         (0) root         (0)     9238 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_summary.py
+-rw-r--r--   0 root         (0) root         (0)    48716 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_tabs.py
+-rw-r--r--   0 root         (0) root         (0)    12023 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_update_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4382 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/template_view_request.py
+-rw-r--r--   0 root         (0) root         (0)   125230 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/text.py
+-rw-r--r--   0 root         (0) root         (0)     8572 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/text_custom_field.py
+-rw-r--r--   0 root         (0) root         (0)     5661 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/time_stamp_field.py
+-rw-r--r--   0 root         (0) root         (0)   105839 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/title.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/tsp_health_check_request.py
+-rw-r--r--   0 root         (0) root         (0)     7650 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/tsp_health_check_status_description.py
+-rw-r--r--   0 root         (0) root         (0)     4742 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/update_transaction_request.py
+-rw-r--r--   0 root         (0) root         (0)     3447 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/update_transaction_response.py
+-rw-r--r--   0 root         (0) root         (0)     6505 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/usage_history.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user.py
+-rw-r--r--   0 root         (0) root         (0)    35237 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_account_management_granular_information.py
+-rw-r--r--   0 root         (0) root         (0)    10505 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     6120 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_create_request.py
+-rw-r--r--   0 root         (0) root         (0)     7181 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_create_request_with_id.py
+-rw-r--r--   0 root         (0) root         (0)     5402 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_id_with_status.py
+-rw-r--r--   0 root         (0) root         (0)     4471 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_update_request.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_with_status.py
+-rw-r--r--   0 root         (0) root         (0)     9481 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations_delete_request.py
+-rw-r--r--   0 root         (0) root         (0)     3765 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations_delete_response.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations_request.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations_response.py
+-rw-r--r--   0 root         (0) root         (0)    13254 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_info.py
+-rw-r--r--   0 root         (0) root         (0)     3486 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_info_list.py
+-rw-r--r--   0 root         (0) root         (0)     5966 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_info_response.py
+-rw-r--r--   0 root         (0) root         (0)    43490 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_information.py
+-rw-r--r--   0 root         (0) root         (0)     9346 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_information_list.py
+-rw-r--r--   0 root         (0) root         (0)     6759 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_password_information.py
+-rw-r--r--   0 root         (0) root         (0)     4517 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_password_rules.py
+-rw-r--r--   0 root         (0) root         (0)    14770 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_profile.py
+-rw-r--r--   0 root         (0) root         (0)   168247 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_settings_information.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_shared_item.py
+-rw-r--r--   0 root         (0) root         (0)    31028 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_signature.py
+-rw-r--r--   0 root         (0) root         (0)    17594 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_signature_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3797 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_signatures_information.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/user_social_id_result.py
+-rw-r--r--   0 root         (0) root         (0)     9127 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/users_response.py
+-rw-r--r--   0 root         (0) root         (0)    93319 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/view.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/view_url.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/watermark.py
+-rw-r--r--   0 root         (0) root         (0)   112714 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/witness.py
+-rw-r--r--   0 root         (0) root         (0)     8038 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workflow.py
+-rw-r--r--   0 root         (0) root         (0)    10414 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workflow_step.py
+-rw-r--r--   0 root         (0) root         (0)    14793 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workspace.py
+-rw-r--r--   0 root         (0) root         (0)    10272 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workspace_folder_contents.py
+-rw-r--r--   0 root         (0) root         (0)    22565 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workspace_item.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workspace_item_list.py
+-rw-r--r--   0 root         (0) root         (0)     7440 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workspace_list.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workspace_settings.py
+-rw-r--r--   0 root         (0) root         (0)    18913 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workspace_user.py
+-rw-r--r--   0 root         (0) root         (0)    12341 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/workspace_user_authorization.py
+-rw-r--r--   0 root         (0) root         (0)   121905 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/docusign_esign/models/zip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/docusign_esign.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5856 2024-05-03 15:17:00.000000 docusign-esign-4.0.0rc1/docusign_esign.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    28060 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/docusign_esign.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 15:17:00.000000 docusign-esign-4.0.0rc1/docusign_esign.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/docusign_esign.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/docusign_esign.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:01.000000 docusign-esign-4.0.0rc1/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/test/test_oauth.py
+-rw-r--r--   0 root         (0) root         (0)    41312 2024-05-03 15:16:57.000000 docusign-esign-4.0.0rc1/test/unit_tests.py
```

### Comparing `docusign-esign-4.0.0/LICENSE` & `docusign-esign-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/PKG-INFO` & `docusign-esign-4.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docusign-esign
-Version: 4.0.0
+Version: 4.0.0rc1
 Summary: DocuSign REST API
 Home-page: 
 Author-email: devcenter@docusign.com
 Keywords: Swagger,DocuSign REST API
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docusign-esign-4.0.0/README.md` & `docusign-esign-4.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/__init__.py` & `docusign-esign-4.0.0rc1/docusign_esign/__init__.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/__init__.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/accounts_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/accounts_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/authentication_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/authentication_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/billing_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/billing_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/bulk_envelopes_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/bulk_envelopes_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/bulk_process_data_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/bulk_process_data_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/bulk_process_data_send_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/bulk_process_data_send_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/cloud_storage_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/cloud_storage_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/connect_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/connect_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/custom_tabs_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/custom_tabs_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/data_feed_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/data_feed_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/diagnostics_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/diagnostics_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/email_archive_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/email_archive_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/envelopes_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/envelopes_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/folders_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/folders_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/groups_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/groups_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/notary_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/notary_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/organizations_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/organizations_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/power_forms_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/power_forms_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/signature_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/signature_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/signing_groups_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/signing_groups_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/templates_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/templates_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/trust_service_providers_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/trust_service_providers_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/users_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/users_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/apis/workspaces_api.py` & `docusign-esign-4.0.0rc1/docusign_esign/apis/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/client/__init__.py` & `docusign-esign-4.0.0rc1/docusign_esign/client/__init__.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/client/api_client.py` & `docusign-esign-4.0.0rc1/docusign_esign/client/api_client.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/client/api_exception.py` & `docusign-esign-4.0.0rc1/docusign_esign/client/api_exception.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/client/api_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/client/api_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/client/auth/__init__.py` & `docusign-esign-4.0.0rc1/docusign_esign/client/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/client/auth/oauth.py` & `docusign-esign-4.0.0rc1/docusign_esign/client/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/client/configuration.py` & `docusign-esign-4.0.0rc1/docusign_esign/client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,17 @@
 
         # Disable client side validation
         self.client_side_validation = True
 
         python_version = platform.python_version()
 
         if six.PY3:
-            self.user_agent = "Swagger-Codegen/v2.1/4.0.0/python3/" + f"{python_version}"
+            self.user_agent = "Swagger-Codegen/v2.1/4.0.0rc1/python3/" + f"{python_version}"
         else:
-            self.user_agent = "Swagger-Codegen/v2.1/4.0.0/python2/" + f"{python_version}"
+            self.user_agent = "Swagger-Codegen/v2.1/4.0.0rc1/python2/" + f"{python_version}"
 
 
     @classmethod
     def set_default(cls, default):
         cls._default = default
 
     @property
@@ -273,9 +273,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v2.1\n"\
-               "SDK Package Version: 4.0.0".\
+               "SDK Package Version: 4.0.0rc1".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `docusign-esign-4.0.0/docusign_esign/models/__init__.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/__init__.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/access_code_format.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/access_code_format.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_address.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_address.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_billing_plan.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_billing_plan.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_billing_plan_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_billing_plan_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_identity_input_option.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_identity_input_option.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_identity_verification_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_identity_verification_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_identity_verification_step.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_identity_verification_step.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_identity_verification_workflow.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_identity_verification_workflow.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_minimum_password_length.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_minimum_password_length.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_notification.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_notification.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_password_expire_password_days.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_password_expire_password_days.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_password_lockout_duration_minutes.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_password_lockout_duration_minutes.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_password_lockout_duration_type.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_password_lockout_duration_type.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_password_minimum_password_age_days.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_password_minimum_password_age_days.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_password_questions_required.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_password_questions_required.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_password_rules.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_password_rules.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_password_strength_type.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_password_strength_type.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_password_strength_type_option.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_password_strength_type_option.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_role_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_role_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_seals.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_seals.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_settings_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_settings_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_shared_access.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_shared_access.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_signature.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_signature.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_signature_definition.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_signature_definition.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_signature_provider.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_signature_provider.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_signature_provider_option.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_signature_provider_option.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_signature_providers.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_signature_providers.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_signatures_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_signatures_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/account_ui_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/account_ui_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/add_on.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/add_on.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/address_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/address_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/address_information_input.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/address_information_input.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/address_information_v2.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/address_information_v2.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/admin_message.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/admin_message.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/agent.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/agent.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/api_request_log.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/api_request_log.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/api_request_logs_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/api_request_logs_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/app_store_product.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/app_store_product.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/app_store_receipt.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/app_store_receipt.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/approve.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/approve.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/ask_an_admin.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/ask_an_admin.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/attachment.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/attachment.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/authentication_method.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/authentication_method.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/authentication_status.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/authentication_status.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/authorization_user.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/authorization_user.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bcc_email_address.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_address.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bcc_email_archive.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_archive.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bcc_email_archive_history.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_archive_history.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bcc_email_archive_history_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_archive_history_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bcc_email_archive_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bcc_email_archive_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_charge.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_charge.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_charge_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_charge_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_discount.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_discount.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_entity_information_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_entity_information_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_invoice.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_invoice.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_invoice_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_invoice_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_invoices_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_invoices_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_invoices_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_invoices_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_payment.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_payment.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_payment_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_payment_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_payment_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_payment_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_payment_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_payment_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_payments_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_payments_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_plan.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_plan_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_plan_preview.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan_preview.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_plan_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_plan_update_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_plan_update_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_plans_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_plans_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/billing_price.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/billing_price.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brand.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brand.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brand_email_content.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brand_email_content.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brand_link.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brand_link.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brand_logos.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brand_logos.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brand_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brand_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brand_resource_urls.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brand_resource_urls.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brand_resources.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brand_resources.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brand_resources_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brand_resources_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brands_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brands_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/brands_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/brands_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_envelope.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_envelope.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_envelope_status.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_envelope_status.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_envelopes_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_envelopes_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_process_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_process_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_process_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_process_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_process_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_process_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_processing_list_summaries.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_processing_list_summaries.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_processing_list_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_processing_list_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_processing_lists.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_processing_lists.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_recipient.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipient.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_recipient_signature_provider.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipient_signature_provider.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_recipient_tab_label.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipient_tab_label.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_recipients_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipients_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_recipients_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipients_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_recipients_summary_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipients_summary_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_recipients_update_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_recipients_update_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_action_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_action_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_error.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_error.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_status.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_status.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_summaries.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_summaries.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_batch_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_batch_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_envelopes_info.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_envelopes_info.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_error_status.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_error_status.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_send_test_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_send_test_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_sending_copy.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_copy.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_sending_copy_custom_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_copy_custom_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_sending_copy_recipient.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_copy_recipient.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_sending_copy_tab.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_copy_tab.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_sending_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_sending_list_summaries.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_list_summaries.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulk_sending_list_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulk_sending_list_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/bulksending_copy_doc_gen_form_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/bulksending_copy_doc_gen_form_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/captive_recipient.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/captive_recipient.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/captive_recipient_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/captive_recipient_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/carbon_copy.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/carbon_copy.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/certified_delivery.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/certified_delivery.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/checkbox.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/checkbox.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/chunked_upload_part.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/chunked_upload_part.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/chunked_upload_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/chunked_upload_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/chunked_upload_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/chunked_upload_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/cloud_storage_provider.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/cloud_storage_provider.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/cloud_storage_providers.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/cloud_storage_providers.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/comment.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/comment.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/comment_history_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/comment_history_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/comment_publish.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/comment_publish.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/comment_thread.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/comment_thread.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/comments_publish.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/comments_publish.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/commission_county.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/commission_county.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/commission_expiration.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/commission_expiration.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/commission_number.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/commission_number.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/commission_state.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/commission_state.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/company.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/company.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/complete_sign_hash_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/complete_sign_hash_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/complete_sign_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/complete_sign_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/composite_template.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/composite_template.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/conditional_recipient_rule.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/conditional_recipient_rule.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/conditional_recipient_rule_condition.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/conditional_recipient_rule_condition.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/conditional_recipient_rule_filter.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/conditional_recipient_rule_filter.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_config_results.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_config_results.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_custom_configuration.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_custom_configuration.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_debug_log.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_debug_log.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_delete_failure_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_delete_failure_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_event_data.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_event_data.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_failure_filter.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_failure_filter.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_failure_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_failure_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_failure_results.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_failure_results.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_historical_envelope_republish.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_historical_envelope_republish.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_log.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_log.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_logs.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_logs.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_o_auth_config.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_o_auth_config.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_salesforce_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_salesforce_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_salesforce_object.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_salesforce_object.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_user_info.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_user_info.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/connect_user_object.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/connect_user_object.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/consent_details.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/consent_details.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/console_view_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/console_view_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/consumer_disclosure.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/consumer_disclosure.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/contact.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/contact.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/contact_get_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/contact_get_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/contact_mod_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/contact_mod_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/contact_phone_number.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/contact_phone_number.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/contact_update_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/contact_update_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/correct_view_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/correct_view_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/country.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/country.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/credential.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/credential.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/credit_card_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/credit_card_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/credit_card_types.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/credit_card_types.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/currency.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/currency.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/currency_feature_set_price.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/currency_feature_set_price.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/currency_plan_price.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/currency_plan_price.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/custom_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/custom_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/custom_field_v2.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/custom_field_v2.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/custom_fields.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/custom_fields.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/custom_fields_envelope.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/custom_fields_envelope.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/custom_settings_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/custom_settings_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/date.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/date.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/date_signed.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/date_signed.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/date_stamp_properties.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/date_stamp_properties.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/decline.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/decline.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/delayed_routing.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/delayed_routing.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/delayed_routing_api_model.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/delayed_routing_api_model.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/delegation_info.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/delegation_info.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/diagnostics_settings_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/diagnostics_settings_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/direct_debit_processor_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/direct_debit_processor_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_account.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_account.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_custom_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_custom_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_document.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_document.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_document_page.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_document_page.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_envelope.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_envelope.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_info.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_info.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_page.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_page.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_pdf.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_pdf.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_recipient.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_recipient.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/display_appliance_signer_attachment.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/display_appliance_signer_attachment.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/dob_information_input.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/dob_information_input.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_option.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_option.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_row_value.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_row_value.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_field_validation.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_field_validation.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/doc_gen_form_fields.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_form_fields.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/doc_gen_syntax_error.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/doc_gen_syntax_error.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_fields_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_fields_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_html_collapsible_display_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_html_collapsible_display_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_html_definition.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_html_definition.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_html_definition_original.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_html_definition_original.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_html_definition_originals.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_html_definition_originals.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_html_definitions.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_html_definitions.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_html_display_anchor.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_html_display_anchor.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_html_display_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_html_display_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_security_store.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_security_store.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_template.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_template.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_template_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_template_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_update_info.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_update_info.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_visibility.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_visibility.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/document_visibility_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/document_visibility_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/downgrad_request_billing_info_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/downgrad_request_billing_info_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/downgrade_billing_plan_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/downgrade_billing_plan_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/downgrade_plan_update_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/downgrade_plan_update_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/downgrade_request_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/downgrade_request_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/draw.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/draw.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/e_note_configuration.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/e_note_configuration.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/editor.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/editor.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/email.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/email.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/email_address.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/email_address.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/email_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/email_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_attachment.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_attachment.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_attachments_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_attachments_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_attachments_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_attachments_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_audit_event.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_audit_event.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_audit_event_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_audit_event_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_custom_metadata.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_definition.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_definition.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_delay_rule.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_delay_rule.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_delay_rule_api_model.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_delay_rule_api_model.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_document.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_document.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_documents_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_documents_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_event.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_event.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_form_data.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_form_data.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_form_data_prefill_form_data.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_form_data_prefill_form_data.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_id.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_id.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_ids_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_ids_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_metadata.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_metadata.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_notification_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_notification_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_publish_transaction.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_publish_transaction.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_publish_transaction_error_rollup.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_publish_transaction_error_rollup.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_purge_configuration.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_purge_configuration.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_template.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_template.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_template_definition.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_template_definition.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_template_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_template_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_template_results.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_template_results.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_transaction_status.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_transaction_status.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_transfer_rule.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_transfer_rule.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_transfer_rule_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_transfer_rule_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_transfer_rule_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_transfer_rule_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_update_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_update_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_view_document_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_document_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_view_envelope_custom_field_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_envelope_custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_view_recipient_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_recipient_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_view_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_view_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_view_tagger_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_tagger_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelope_view_template_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelope_view_template_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/envelopes_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/envelopes_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/error_details.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/error_details.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/event_notification.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/event_notification.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/event_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/event_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/expirations.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/expirations.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/external_claim.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/external_claim.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/external_doc_service_error_details.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/external_doc_service_error_details.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/external_document_sources.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/external_document_sources.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/external_file.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/external_file.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/external_folder.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/external_folder.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/external_primary_account_recipient_auth_requirements.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/external_primary_account_recipient_auth_requirements.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/favorite_templates_content_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/favorite_templates_content_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/favorite_templates_info.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/favorite_templates_info.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/feature_available_metadata.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/feature_available_metadata.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/feature_set.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/feature_set.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/file_type.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/file_type.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/file_type_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/file_type_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/filter.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/filter.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/first_name.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/first_name.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/folder.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/folder.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/folder_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/folder_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/folder_item_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/folder_item_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/folder_item_v2.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/folder_item_v2.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/folder_items_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/folder_items_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/folder_shared_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/folder_shared_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/folders_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/folders_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/folders_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/folders_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/forgotten_password_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/forgotten_password_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/form_data_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/form_data_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/formula_tab.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/formula_tab.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/full_name.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/full_name.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/graphics_context.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/graphics_context.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/group.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/group.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/group_brands.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/group_brands.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/group_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/group_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/id_check_configuration.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/id_check_configuration.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/id_check_information_input.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/id_check_information_input.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/id_check_security_step.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/id_check_security_step.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/id_evidence_resource_token.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/id_evidence_resource_token.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/id_evidence_view_link.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/id_evidence_view_link.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/in_person_signer.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/in_person_signer.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/initial_here.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/initial_here.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/inline_template.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/inline_template.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/integrated_connect_user_info_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/integrated_connect_user_info_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/integrated_user_info_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/integrated_user_info_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/intermediary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/intermediary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/jurisdiction.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/jurisdiction_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/jurisdiction_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/last_name.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/last_name.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/linked_external_primary_account.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/linked_external_primary_account.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/list_custom_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/list_custom_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/list_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/list_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/locale_policy.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/locale_policy.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/locale_policy_tab.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/locale_policy_tab.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/lock_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/lock_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/lock_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/lock_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/login_account.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/login_account.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/login_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/login_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/match_box.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/match_box.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/member_group_shared_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/member_group_shared_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/member_shared_items.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/member_shared_items.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/merge_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/merge_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/mobile_notifier_configuration.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/mobile_notifier_configuration.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/mobile_notifier_configuration_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/mobile_notifier_configuration_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/model_date.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/model_date.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/money.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/money.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/name_value.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/name_value.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/new_account_definition.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/new_account_definition.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/new_account_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/new_account_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/new_user.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/new_user.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/new_users_definition.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/new_users_definition.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/new_users_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/new_users_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notarize.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notarize.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_certificate.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_certificate.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_contact_details.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_contact_details.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_host.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_host.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_journal.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_journal.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_journal_credible_witness.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_journal_credible_witness.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_journal_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_journal_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_journal_meta_data.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_journal_meta_data.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_jurisdiction.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_jurisdiction.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_jurisdiction_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_jurisdiction_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_recipient.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_recipient.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notary_seal.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notary_seal.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/note.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/note.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notification.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notification.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notification_default_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notification_default_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/notification_defaults.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/notification_defaults.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/number.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/number.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/numerical.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/numerical.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/oauth_access.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/oauth_access.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/ocr_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/ocr_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/offline_attributes.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/offline_attributes.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/page.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/page.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/page_images.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/page_images.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/page_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/page_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/page_size.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/page_size.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/palette_item_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/palette_item_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/palette_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/palette_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/participant.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/participant.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/path_extended_element.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/path_extended_element.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/pay_pal_legacy_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/pay_pal_legacy_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/payment_details.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/payment_details.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/payment_gateway_account.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/payment_gateway_account.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/payment_gateway_account_setting.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/payment_gateway_account_setting.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/payment_gateway_accounts_info.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/payment_gateway_accounts_info.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/payment_line_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/payment_line_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/payment_method_with_options.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/payment_method_with_options.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/payment_processor_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/payment_processor_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/payment_signer_values.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/payment_signer_values.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/permission_profile.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/permission_profile.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/permission_profile_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/permission_profile_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/phone_number.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/phone_number.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/plan_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/plan_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/poly_line.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/poly_line.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/poly_line_overlay.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/poly_line_overlay.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/power_form.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/power_form.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/power_form_form_data_envelope.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/power_form_form_data_envelope.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/power_form_form_data_recipient.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/power_form_form_data_recipient.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/power_form_recipient.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/power_form_recipient.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/power_form_senders_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/power_form_senders_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/power_forms_form_data_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/power_forms_form_data_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/power_forms_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/power_forms_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/power_forms_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/power_forms_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/prefill_form_data.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/prefill_form_data.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/prefill_tabs.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/prefill_tabs.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/proof_service_resource_token.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/proof_service_resource_token.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/proof_service_view_link.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/proof_service_view_link.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/property_metadata.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/property_metadata.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/province.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/province.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/provisioning_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/provisioning_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/purchased_envelopes_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/purchased_envelopes_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/radio.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/radio.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/radio_group.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/radio_group.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_additional_notification.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_additional_notification.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_attachment.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_attachment.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_domain.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_domain.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_email_notification.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_email_notification.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_event.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_event.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_form_data.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_form_data.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_group.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_group.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_identity_input_option.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_identity_input_option.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_identity_phone_number.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_identity_phone_number.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_identity_verification.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_identity_verification.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_names_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_names_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_option.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_option.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_phone_authentication.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_phone_authentication.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_phone_number.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_phone_number.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_preview_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_preview_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_proof_file.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_proof_file.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_routing.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_routing.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_rules.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_rules.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_saml_authentication.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_saml_authentication.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_signature_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_signature_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_signature_provider.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_signature_provider.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_signature_provider_options.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_signature_provider_options.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_sms_authentication.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_sms_authentication.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_token_client_ur_ls.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_token_client_ur_ls.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_update_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_update_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipient_view_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipient_view_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipients.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipients.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/recipients_update_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/recipients_update_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/referral_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/referral_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/reminders.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/reminders.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_csv_run_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_csv_run_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_get.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_get.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_list_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_list_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_run_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_run_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_run_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_run_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_run_response_row.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_run_response_row.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_run_response_row_fields.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_run_response_row_fields.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_save_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_save_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/report_in_product_sent_by_details.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/report_in_product_sent_by_details.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/reserved_domain_existence.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/reserved_domain_existence.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/resource_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/resource_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/return_url_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/return_url_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/revision.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/revision.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/saml_assertion_attribute.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/saml_assertion_attribute.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/scheduled_sending.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/scheduled_sending.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/scheduled_sending_api_model.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/scheduled_sending_api_model.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/seal.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/seal.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/seal_identifier.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/seal_identifier.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/seal_sign.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/seal_sign.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/seat_discount.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/seat_discount.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/sender.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/sender.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/sender_company.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/sender_company.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/sender_email_notifications.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/sender_email_notifications.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/sender_name.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/sender_name.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/server_template.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/server_template.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/service_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/service_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/service_version.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/service_version.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/settings_metadata.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/settings_metadata.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/shared_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/shared_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/sign_hash_document.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/sign_hash_document.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/sign_hash_session_info_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/sign_hash_session_info_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/sign_here.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/sign_here.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/sign_session_info_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/sign_session_info_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signature_data_info.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signature_data_info.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signature_group.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signature_group.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signature_group_def.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signature_group_def.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signature_properties.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signature_properties.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signature_provider_required_option.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signature_provider_required_option.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signature_type.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signature_type.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signature_user.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signature_user.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signature_user_def.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signature_user_def.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signer.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signer.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signer_attachment.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signer_attachment.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signer_email_notifications.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signer_email_notifications.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signing_group.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signing_group.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signing_group_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signing_group_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signing_group_user.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signing_group_user.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/signing_group_users.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/signing_group_users.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/smart_contract_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/smart_contract_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/smart_section.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/smart_section.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/smart_section_anchor_position.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/smart_section_anchor_position.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/smart_section_collapsible_display_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/smart_section_collapsible_display_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/smart_section_display_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/smart_section_display_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/social_account_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/social_account_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/social_authentication.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/social_authentication.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/ssn.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/ssn.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/ssn4_information_input.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/ssn4_information_input.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/ssn9_information_input.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/ssn9_information_input.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/stamp.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/stamp.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/supported_languages.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/supported_languages.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/tab_account_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/tab_account_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/tab_group.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/tab_group.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/tab_metadata.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/tab_metadata.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/tab_metadata_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/tab_metadata_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/tabs.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/tabs.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_custom_fields.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_custom_fields.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_document_visibility_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_document_visibility_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_documents_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_documents_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_match.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_match.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_notification_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_notification_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_recipients.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_recipients.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_role.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_role.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_shared_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_shared_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_tabs.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_tabs.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_update_summary.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_update_summary.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/template_view_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/template_view_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/text.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/text.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/text_custom_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/text_custom_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/time_stamp_field.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/time_stamp_field.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/title.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/title.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/tsp_health_check_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/tsp_health_check_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/tsp_health_check_status_description.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/tsp_health_check_status_description.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/update_transaction_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/update_transaction_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/update_transaction_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/update_transaction_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/usage_history.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/usage_history.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_account_management_granular_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_account_management_granular_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorization.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorization_create_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_create_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorization_create_request_with_id.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_create_request_with_id.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorization_id_with_status.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_id_with_status.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorization_update_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_update_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorization_with_status.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorization_with_status.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorizations.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorizations_delete_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations_delete_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorizations_delete_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations_delete_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorizations_request.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations_request.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_authorizations_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_authorizations_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_info.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_info.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_info_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_info_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_info_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_info_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_information_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_information_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_password_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_password_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_password_rules.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_password_rules.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_profile.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_profile.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_settings_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_settings_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_shared_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_shared_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_signature.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_signature.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_signature_definition.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_signature_definition.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_signatures_information.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_signatures_information.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/user_social_id_result.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/user_social_id_result.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/users_response.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/users_response.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/view.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/view.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/view_url.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/view_url.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/watermark.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/watermark.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/witness.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/witness.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workflow.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workflow.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workflow_step.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workflow_step.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workspace.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workspace.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workspace_folder_contents.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workspace_folder_contents.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workspace_item.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workspace_item.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workspace_item_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workspace_item_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workspace_list.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workspace_list.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workspace_settings.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workspace_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workspace_user.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workspace_user.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/workspace_user_authorization.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/workspace_user_authorization.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign/models/zip.py` & `docusign-esign-4.0.0rc1/docusign_esign/models/zip.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/docusign_esign.egg-info/PKG-INFO` & `docusign-esign-4.0.0rc1/docusign_esign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docusign-esign
-Version: 4.0.0
+Version: 4.0.0rc1
 Summary: DocuSign REST API
 Home-page: 
 Author-email: devcenter@docusign.com
 Keywords: Swagger,DocuSign REST API
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docusign-esign-4.0.0/docusign_esign.egg-info/SOURCES.txt` & `docusign-esign-4.0.0rc1/docusign_esign.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/setup.py` & `docusign-esign-4.0.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages, Command, os  # noqa: H301	
 
 NAME = "docusign-esign"
-VERSION = "4.0.0"
+VERSION = "4.0.0rc1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `docusign-esign-4.0.0/test/test_oauth.py` & `docusign-esign-4.0.0rc1/test/test_oauth.py`

 * *Files identical despite different names*

### Comparing `docusign-esign-4.0.0/test/unit_tests.py` & `docusign-esign-4.0.0rc1/test/unit_tests.py`

 * *Files identical despite different names*

