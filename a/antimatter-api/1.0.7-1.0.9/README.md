# Comparing `tmp/antimatter_api-1.0.7.tar.gz` & `tmp/antimatter_api-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimatter_api-1.0.7.tar", last modified: Tue May 21 20:42:17 2024, max compression
+gzip compressed data, was "antimatter_api-1.0.9.tar", last modified: Tue May 21 23:44:45 2024, max compression
```

## Comparing `antimatter_api-1.0.7.tar` & `antimatter_api-1.0.9.tar`

### file list

```diff
@@ -1,331 +1,331 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:42:17.727872 antimatter_api-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      476 2024-05-21 20:42:17.727872 antimatter_api-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28466 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:42:17.599874 antimatter_api-1.0.7/antimatter_api/
--rw-r--r--   0 root         (0) root         (0)    13491 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:42:17.603874 antimatter_api-1.0.7/antimatter_api/api/
--rw-r--r--   0 root         (0) root         (0)      525 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31861 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api/account_management_api.py
--rw-r--r--   0 root         (0) root         (0)   199587 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api/authentication_api.py
--rw-r--r--   0 root         (0) root         (0)   146245 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api/capsules_api.py
--rw-r--r--   0 root         (0) root         (0)   202747 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api/contexts_api.py
--rw-r--r--   0 root         (0) root         (0)   107696 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api/encryption_api.py
--rw-r--r--   0 root         (0) root         (0)   162505 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api/general_api.py
--rw-r--r--   0 root         (0) root         (0)    79682 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api/internal_api.py
--rw-r--r--   0 root         (0) root         (0)   175135 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api/policy_api.py
--rw-r--r--   0 root         (0) root         (0)    25772 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api_client.py
--rw-r--r--   0 root         (0) root         (0)      652 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/api_response.py
--rw-r--r--   0 root         (0) root         (0)    15374 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5953 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:42:17.659873 antimatter_api-1.0.7/antimatter_api/models/
--rw-r--r--   0 root         (0) root         (0)    12470 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6818 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/access_log_entry.py
--rw-r--r--   0 root         (0) root         (0)     3307 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/access_log_entry_create_info.py
--rw-r--r--   0 root         (0) root         (0)     3147 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/access_log_entry_open_info.py
--rw-r--r--   0 root         (0) root         (0)     5338 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/access_log_entry_read_info.py
--rw-r--r--   0 root         (0) root         (0)     3206 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/access_log_results.py
--rw-r--r--   0 root         (0) root         (0)     3139 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/active_root_encryption_key_id.py
--rw-r--r--   0 root         (0) root         (0)     3096 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/add_capsule_log_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     4889 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/add_read_context.py
--rw-r--r--   0 root         (0) root         (0)     3269 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/add_write_context.py
--rw-r--r--   0 root         (0) root         (0)     3237 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/antimatter_delegated_aws_key_info.py
--rw-r--r--   0 root         (0) root         (0)     2888 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/api_key_domain_identity_provider_details.py
--rw-r--r--   0 root         (0) root         (0)     3372 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/available_delegated_root_encryption_key_provider.py
--rw-r--r--   0 root         (0) root         (0)     3196 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/available_root_encryption_key_providers.py
--rw-r--r--   0 root         (0) root         (0)     6733 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/available_root_encryption_key_providers_providers_inner.py
--rw-r--r--   0 root         (0) root         (0)     3264 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/available_service_account_root_encryption_key_provider.py
--rw-r--r--   0 root         (0) root         (0)     3526 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/aws_service_account_key_info.py
--rw-r--r--   0 root         (0) root         (0)     3216 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capability.py
--rw-r--r--   0 root         (0) root         (0)     5047 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capability_definition.py
--rw-r--r--   0 root         (0) root         (0)     3039 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capability_definition_list.py
--rw-r--r--   0 root         (0) root         (0)     2958 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capability_list.py
--rw-r--r--   0 root         (0) root         (0)     3322 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capability_rule.py
--rw-r--r--   0 root         (0) root         (0)     3707 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capability_rule_match_expressions_inner.py
--rw-r--r--   0 root         (0) root         (0)     4627 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capsule_create_response.py
--rw-r--r--   0 root         (0) root         (0)     4932 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capsule_info.py
--rw-r--r--   0 root         (0) root         (0)     3094 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capsule_list.py
--rw-r--r--   0 root         (0) root         (0)     2807 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capsule_open_request.py
--rw-r--r--   0 root         (0) root         (0)     4259 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capsule_open_response.py
--rw-r--r--   0 root         (0) root         (0)     3506 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capsule_open_response_read_context_configuration.py
--rw-r--r--   0 root         (0) root         (0)     3835 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/capsule_seal_request.py
--rw-r--r--   0 root         (0) root         (0)     3024 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/conflict_error.py
--rw-r--r--   0 root         (0) root         (0)     7376 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/create_peer_domain.py
--rw-r--r--   0 root         (0) root         (0)     3177 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_input.py
--rw-r--r--   0 root         (0) root         (0)     3254 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_input_records_inner.py
--rw-r--r--   0 root         (0) root         (0)     2922 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_input_records_inner_elements_inner.py
--rw-r--r--   0 root         (0) root         (0)     3614 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_response.py
--rw-r--r--   0 root         (0) root         (0)     3087 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_response_records_inner.py
--rw-r--r--   0 root         (0) root         (0)     2543 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/delete_tags.py
--rw-r--r--   0 root         (0) root         (0)     2892 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain.py
--rw-r--r--   0 root         (0) root         (0)     3033 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_add_read_context_rule200_response.py
--rw-r--r--   0 root         (0) root         (0)     2549 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_authenticate.py
--rw-r--r--   0 root         (0) root         (0)     2697 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_authenticate_response.py
--rw-r--r--   0 root         (0) root         (0)     2662 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_contact_issue_verify_request.py
--rw-r--r--   0 root         (0) root         (0)     4413 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_control_log_entry.py
--rw-r--r--   0 root         (0) root         (0)     3256 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_control_log_results.py
--rw-r--r--   0 root         (0) root         (0)     3024 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_fact_list.py
--rw-r--r--   0 root         (0) root         (0)     3008 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_hooks_list.py
--rw-r--r--   0 root         (0) root         (0)     3715 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_hooks_list_hooks_inner.py
--rw-r--r--   0 root         (0) root         (0)     3106 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_api_key_principal_params.py
--rw-r--r--   0 root         (0) root         (0)     3033 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_email_principal_params.py
--rw-r--r--   0 root         (0) root         (0)     3153 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_hosted_domain_principal_params.py
--rw-r--r--   0 root         (0) root         (0)     7429 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_principal_details.py
--rw-r--r--   0 root         (0) root         (0)     6301 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_details.py
--rw-r--r--   0 root         (0) root         (0)     5226 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_info.py
--rw-r--r--   0 root         (0) root         (0)     3259 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_list.py
--rw-r--r--   0 root         (0) root         (0)     3050 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_principal_list.py
--rw-r--r--   0 root         (0) root         (0)     3494 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_principal_params.py
--rw-r--r--   0 root         (0) root         (0)      844 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_principal_type.py
--rw-r--r--   0 root         (0) root         (0)      830 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_type.py
--rw-r--r--   0 root         (0) root         (0)     3359 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_insert_identity_provider_principal200_response.py
--rw-r--r--   0 root         (0) root         (0)     3026 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_insert_write_context_regex_rule200_response.py
--rw-r--r--   0 root         (0) root         (0)    14664 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_peer_config.py
--rw-r--r--   0 root         (0) root         (0)     2995 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_peer_list.py
--rw-r--r--   0 root         (0) root         (0)     3523 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_peer_list_peers_inner.py
--rw-r--r--   0 root         (0) root         (0)     3525 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_policy.py
--rw-r--r--   0 root         (0) root         (0)     7184 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_policy_rule.py
--rw-r--r--   0 root         (0) root         (0)     3966 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_private_info.py
--rw-r--r--   0 root         (0) root         (0)     3962 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_public_info.py
--rw-r--r--   0 root         (0) root         (0)     3092 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_resource_summary.py
--rw-r--r--   0 root         (0) root         (0)     3434 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_resource_summary_schema_inner.py
--rw-r--r--   0 root         (0) root         (0)     4066 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_settings.py
--rw-r--r--   0 root         (0) root         (0)     2927 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_settings_disaster_recovery.py
--rw-r--r--   0 root         (0) root         (0)     2962 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_settings_patch.py
--rw-r--r--   0 root         (0) root         (0)     3091 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_status.py
--rw-r--r--   0 root         (0) root         (0)     2953 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_status_notifications_inner.py
--rw-r--r--   0 root         (0) root         (0)     3094 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/domain_tag_info_results.py
--rw-r--r--   0 root         (0) root         (0)     2551 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/error.py
--rw-r--r--   0 root         (0) root         (0)     3886 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/fact.py
--rw-r--r--   0 root         (0) root         (0)     2847 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/fact_list.py
--rw-r--r--   0 root         (0) root         (0)     4310 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/fact_policy_rules_inner.py
--rw-r--r--   0 root         (0) root         (0)     4385 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/fact_policy_rules_inner_arguments_inner.py
--rw-r--r--   0 root         (0) root         (0)     5008 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/fact_type_definition.py
--rw-r--r--   0 root         (0) root         (0)     2658 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/forbidden_error.py
--rw-r--r--   0 root         (0) root         (0)     3959 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/gcp_service_account_key_info.py
--rw-r--r--   0 root         (0) root         (0)     3124 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/google_o_auth_domain_identity_provider_details.py
--rw-r--r--   0 root         (0) root         (0)     2583 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     2751 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/invalid_request_error.py
--rw-r--r--   0 root         (0) root         (0)     3275 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/json_patch_request_add.py
--rw-r--r--   0 root         (0) root         (0)     6099 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/json_patch_request_add_value.py
--rw-r--r--   0 root         (0) root         (0)     2878 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/json_patch_request_copy.py
--rw-r--r--   0 root         (0) root         (0)     2878 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/json_patch_request_move.py
--rw-r--r--   0 root         (0) root         (0)     2890 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/json_patch_request_remove.py
--rw-r--r--   0 root         (0) root         (0)     3315 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/json_patch_request_replace.py
--rw-r--r--   0 root         (0) root         (0)     6131 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/json_patch_request_replace_value.py
--rw-r--r--   0 root         (0) root         (0)     3277 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/json_patch_request_tst.py
--rw-r--r--   0 root         (0) root         (0)     6100 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/json_patch_request_tst_value.py
--rw-r--r--   0 root         (0) root         (0)     3064 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/key_infos.py
--rw-r--r--   0 root         (0) root         (0)     6802 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/key_infos_key_information.py
--rw-r--r--   0 root         (0) root         (0)     3508 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_access_log_entry.py
--rw-r--r--   0 root         (0) root         (0)     4654 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_access_log_entry_read_info.py
--rw-r--r--   0 root         (0) root         (0)     3240 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_capability_definition.py
--rw-r--r--   0 root         (0) root         (0)     2782 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_domain.py
--rw-r--r--   0 root         (0) root         (0)     4819 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_domain_policy_rule.py
--rw-r--r--   0 root         (0) root         (0)     3068 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_domain_response.py
--rw-r--r--   0 root         (0) root         (0)     2745 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_fact.py
--rw-r--r--   0 root         (0) root         (0)     3316 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_fact_type_definition.py
--rw-r--r--   0 root         (0) root         (0)     3193 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_fact_type_definition_arguments_inner.py
--rw-r--r--   0 root         (0) root         (0)     6250 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/new_read_context_config_rule.py
--rw-r--r--   0 root         (0) root         (0)     9116 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/patch_request_inner.py
--rw-r--r--   0 root         (0) root         (0)      759 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/policy_rule_operation.py
--rw-r--r--   0 root         (0) root         (0)      736 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/policy_rule_result.py
--rw-r--r--   0 root         (0) root         (0)     4118 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/principal_info.py
--rw-r--r--   0 root         (0) root         (0)     3506 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/principal_summary.py
--rw-r--r--   0 root         (0) root         (0)     7854 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/read_context_config_rule.py
--rw-r--r--   0 root         (0) root         (0)     7277 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/read_context_details.py
--rw-r--r--   0 root         (0) root         (0)     3058 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/read_context_list.py
--rw-r--r--   0 root         (0) root         (0)     2947 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/read_context_parameter.py
--rw-r--r--   0 root         (0) root         (0)     4997 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/read_context_required_hook.py
--rw-r--r--   0 root         (0) root         (0)     3803 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/read_context_rule_facts_inner.py
--rw-r--r--   0 root         (0) root         (0)     3326 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/read_context_rule_facts_inner_arguments_inner.py
--rw-r--r--   0 root         (0) root         (0)     4290 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/read_context_rule_match_expressions_inner.py
--rw-r--r--   0 root         (0) root         (0)     5759 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/read_context_short_details.py
--rw-r--r--   0 root         (0) root         (0)     2982 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/resource_exhausted_error.py
--rw-r--r--   0 root         (0) root         (0)     2974 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/resource_not_found_error.py
--rw-r--r--   0 root         (0) root         (0)     2600 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/root_encryption_key_id_response.py
--rw-r--r--   0 root         (0) root         (0)     3078 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/root_encryption_key_item.py
--rw-r--r--   0 root         (0) root         (0)     4271 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/root_encryption_key_test_response.py
--rw-r--r--   0 root         (0) root         (0)     2704 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/rotate_key_encryption_key_response.py
--rw-r--r--   0 root         (0) root         (0)     2561 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/starred_domain_list.py
--rw-r--r--   0 root         (0) root         (0)     4136 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     2550 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/tag_meta.py
--rw-r--r--   0 root         (0) root         (0)     3528 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/tag_set.py
--rw-r--r--   0 root         (0) root         (0)     3162 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/tag_set_span_tags_inner.py
--rw-r--r--   0 root         (0) root         (0)     3812 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/tag_summary.py
--rw-r--r--   0 root         (0) root         (0)     3050 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/tag_summary_elided_tags_inner.py
--rw-r--r--   0 root         (0) root         (0)     2898 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/tag_summary_unique_tags_inner.py
--rw-r--r--   0 root         (0) root         (0)      800 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/tag_type_field.py
--rw-r--r--   0 root         (0) root         (0)     2585 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/unauthorized_error.py
--rw-r--r--   0 root         (0) root         (0)     3066 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/upsert_span_tags_request.py
--rw-r--r--   0 root         (0) root         (0)     3141 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/verify_contact_response.py
--rw-r--r--   0 root         (0) root         (0)     4308 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/write_context_config_info.py
--rw-r--r--   0 root         (0) root         (0)     4716 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/write_context_config_info_required_hooks_inner.py
--rw-r--r--   0 root         (0) root         (0)     4987 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/write_context_details.py
--rw-r--r--   0 root         (0) root         (0)     3055 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/write_context_list.py
--rw-r--r--   0 root         (0) root         (0)     4388 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/write_context_regex_rule.py
--rw-r--r--   0 root         (0) root         (0)     3262 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/models/write_context_regex_tag.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/py.typed
--rw-r--r--   0 root         (0) root         (0)     9213 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/antimatter_api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:42:17.727872 antimatter_api-1.0.7/antimatter_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      476 2024-05-21 20:42:17.000000 antimatter_api-1.0.7/antimatter_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14126 2024-05-21 20:42:17.000000 antimatter_api-1.0.7/antimatter_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 20:42:17.000000 antimatter_api-1.0.7/antimatter_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-21 20:42:17.000000 antimatter_api-1.0.7/antimatter_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-21 20:42:17.000000 antimatter_api-1.0.7/antimatter_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1963 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-21 20:42:17.727872 antimatter_api-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1287 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:42:17.727872 antimatter_api-1.0.7/test/
--rw-r--r--   0 root         (0) root         (0)     4973 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_access_log_entry.py
--rw-r--r--   0 root         (0) root         (0)     1560 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_access_log_entry_create_info.py
--rw-r--r--   0 root         (0) root         (0)     1534 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_access_log_entry_open_info.py
--rw-r--r--   0 root         (0) root         (0)     8052 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_access_log_entry_read_info.py
--rw-r--r--   0 root         (0) root         (0)     9130 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_access_log_results.py
--rw-r--r--   0 root         (0) root         (0)     1129 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_account_management_api.py
--rw-r--r--   0 root         (0) root         (0)     1540 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_active_root_encryption_key_id.py
--rw-r--r--   0 root         (0) root         (0)     7506 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_add_capsule_log_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     2249 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_add_read_context.py
--rw-r--r--   0 root         (0) root         (0)     3354 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_add_write_context.py
--rw-r--r--   0 root         (0) root         (0)     1618 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_antimatter_delegated_aws_key_info.py
--rw-r--r--   0 root         (0) root         (0)     1622 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_api_key_domain_identity_provider_details.py
--rw-r--r--   0 root         (0) root         (0)     3574 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     2010 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_available_delegated_root_encryption_key_provider.py
--rw-r--r--   0 root         (0) root         (0)     1666 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_available_root_encryption_key_providers.py
--rw-r--r--   0 root         (0) root         (0)     2083 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_available_root_encryption_key_providers_providers_inner.py
--rw-r--r--   0 root         (0) root         (0)     2000 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_available_service_account_root_encryption_key_provider.py
--rw-r--r--   0 root         (0) root         (0)     1710 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_aws_service_account_key_info.py
--rw-r--r--   0 root         (0) root         (0)     1400 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capability.py
--rw-r--r--   0 root         (0) root         (0)     1839 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capability_definition.py
--rw-r--r--   0 root         (0) root         (0)     2394 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capability_definition_list.py
--rw-r--r--   0 root         (0) root         (0)     1757 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capability_list.py
--rw-r--r--   0 root         (0) root         (0)     1708 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capability_rule.py
--rw-r--r--   0 root         (0) root         (0)     1886 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capability_rule_match_expressions_inner.py
--rw-r--r--   0 root         (0) root         (0)     3992 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capsule_create_response.py
--rw-r--r--   0 root         (0) root         (0)     4666 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capsule_info.py
--rw-r--r--   0 root         (0) root         (0)     5497 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capsule_list.py
--rw-r--r--   0 root         (0) root         (0)     1520 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capsule_open_request.py
--rw-r--r--   0 root         (0) root         (0)     3214 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capsule_open_response.py
--rw-r--r--   0 root         (0) root         (0)     1849 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capsule_open_response_read_context_configuration.py
--rw-r--r--   0 root         (0) root         (0)     4632 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capsule_seal_request.py
--rw-r--r--   0 root         (0) root         (0)     1939 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_capsules_api.py
--rw-r--r--   0 root         (0) root         (0)     1519 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_conflict_error.py
--rw-r--r--   0 root         (0) root         (0)     3553 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_contexts_api.py
--rw-r--r--   0 root         (0) root         (0)     2183 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_create_peer_domain.py
--rw-r--r--   0 root         (0) root         (0)     2427 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_data_tagging_hook_input.py
--rw-r--r--   0 root         (0) root         (0)     2155 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_data_tagging_hook_input_records_inner.py
--rw-r--r--   0 root         (0) root         (0)     1879 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_data_tagging_hook_input_records_inner_elements_inner.py
--rw-r--r--   0 root         (0) root         (0)     5021 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_data_tagging_hook_response.py
--rw-r--r--   0 root         (0) root         (0)     4363 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_data_tagging_hook_response_records_inner.py
--rw-r--r--   0 root         (0) root         (0)     1357 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_delete_tags.py
--rw-r--r--   0 root         (0) root         (0)     1314 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain.py
--rw-r--r--   0 root         (0) root         (0)     1633 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_add_read_context_rule200_response.py
--rw-r--r--   0 root         (0) root         (0)     1437 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_authenticate.py
--rw-r--r--   0 root         (0) root         (0)     1637 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_authenticate_response.py
--rw-r--r--   0 root         (0) root         (0)     1620 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_contact_issue_verify_request.py
--rw-r--r--   0 root         (0) root         (0)     2215 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_control_log_entry.py
--rw-r--r--   0 root         (0) root         (0)     2747 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_control_log_results.py
--rw-r--r--   0 root         (0) root         (0)     2736 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_fact_list.py
--rw-r--r--   0 root         (0) root         (0)     1923 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_hooks_list.py
--rw-r--r--   0 root         (0) root         (0)     2130 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_hooks_list_hooks_inner.py
--rw-r--r--   0 root         (0) root         (0)     1718 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_api_key_principal_params.py
--rw-r--r--   0 root         (0) root         (0)     1726 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_email_principal_params.py
--rw-r--r--   0 root         (0) root         (0)     1841 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_hosted_domain_principal_params.py
--rw-r--r--   0 root         (0) root         (0)     1784 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_principal_details.py
--rw-r--r--   0 root         (0) root         (0)     1585 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_provider_details.py
--rw-r--r--   0 root         (0) root         (0)     2019 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_provider_info.py
--rw-r--r--   0 root         (0) root         (0)     2054 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_provider_list.py
--rw-r--r--   0 root         (0) root         (0)     2152 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_provider_principal_list.py
--rw-r--r--   0 root         (0) root         (0)     2100 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_provider_principal_params.py
--rw-r--r--   0 root         (0) root         (0)      842 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_provider_principal_type.py
--rw-r--r--   0 root         (0) root         (0)      778 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_identity_provider_type.py
--rw-r--r--   0 root         (0) root         (0)     1873 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_insert_identity_provider_principal200_response.py
--rw-r--r--   0 root         (0) root         (0)     1796 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_insert_write_context_regex_rule200_response.py
--rw-r--r--   0 root         (0) root         (0)     3665 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_peer_config.py
--rw-r--r--   0 root         (0) root         (0)     1836 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_peer_list.py
--rw-r--r--   0 root         (0) root         (0)     1624 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_peer_list_peers_inner.py
--rw-r--r--   0 root         (0) root         (0)     1405 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_policy.py
--rw-r--r--   0 root         (0) root         (0)     3223 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_policy_rule.py
--rw-r--r--   0 root         (0) root         (0)     2684 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_private_info.py
--rw-r--r--   0 root         (0) root         (0)     2672 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_public_info.py
--rw-r--r--   0 root         (0) root         (0)     2508 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_resource_summary.py
--rw-r--r--   0 root         (0) root         (0)     2134 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_resource_summary_schema_inner.py
--rw-r--r--   0 root         (0) root         (0)     1959 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_settings.py
--rw-r--r--   0 root         (0) root         (0)     1591 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_settings_disaster_recovery.py
--rw-r--r--   0 root         (0) root         (0)     1542 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_settings_patch.py
--rw-r--r--   0 root         (0) root         (0)     1599 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_status.py
--rw-r--r--   0 root         (0) root         (0)     1717 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_status_notifications_inner.py
--rw-r--r--   0 root         (0) root         (0)     1815 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_domain_tag_info_results.py
--rw-r--r--   0 root         (0) root         (0)     2529 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_encryption_api.py
--rw-r--r--   0 root         (0) root         (0)     1346 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_error.py
--rw-r--r--   0 root         (0) root         (0)     1538 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_fact.py
--rw-r--r--   0 root         (0) root         (0)     1879 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_fact_list.py
--rw-r--r--   0 root         (0) root         (0)     2285 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_fact_policy_rules_inner.py
--rw-r--r--   0 root         (0) root         (0)     1725 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_fact_policy_rules_inner_arguments_inner.py
--rw-r--r--   0 root         (0) root         (0)     2242 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_fact_type_definition.py
--rw-r--r--   0 root         (0) root         (0)     1393 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_forbidden_error.py
--rw-r--r--   0 root         (0) root         (0)     1858 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_gcp_service_account_key_info.py
--rw-r--r--   0 root         (0) root         (0)     2631 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_general_api.py
--rw-r--r--   0 root         (0) root         (0)     1720 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_google_o_auth_domain_identity_provider_details.py
--rw-r--r--   0 root         (0) root         (0)     1447 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     1558 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_internal_api.py
--rw-r--r--   0 root         (0) root         (0)     1510 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_invalid_request_error.py
--rw-r--r--   0 root         (0) root         (0)     1565 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_json_patch_request_add.py
--rw-r--r--   0 root         (0) root         (0)     1457 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_json_patch_request_add_value.py
--rw-r--r--   0 root         (0) root         (0)     1519 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_json_patch_request_copy.py
--rw-r--r--   0 root         (0) root         (0)     1519 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_json_patch_request_move.py
--rw-r--r--   0 root         (0) root         (0)     1547 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_json_patch_request_remove.py
--rw-r--r--   0 root         (0) root         (0)     1621 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_json_patch_request_replace.py
--rw-r--r--   0 root         (0) root         (0)     1505 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_json_patch_request_replace_value.py
--rw-r--r--   0 root         (0) root         (0)     1567 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_json_patch_request_tst.py
--rw-r--r--   0 root         (0) root         (0)     1457 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_json_patch_request_tst_value.py
--rw-r--r--   0 root         (0) root         (0)     1375 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_key_infos.py
--rw-r--r--   0 root         (0) root         (0)     2045 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_key_infos_key_information.py
--rw-r--r--   0 root         (0) root         (0)     6550 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_access_log_entry.py
--rw-r--r--   0 root         (0) root         (0)     7987 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_access_log_entry_read_info.py
--rw-r--r--   0 root         (0) root         (0)     1630 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_capability_definition.py
--rw-r--r--   0 root         (0) root         (0)     1388 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_domain.py
--rw-r--r--   0 root         (0) root         (0)     2912 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_domain_policy_rule.py
--rw-r--r--   0 root         (0) root         (0)     1508 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_domain_response.py
--rw-r--r--   0 root         (0) root         (0)     1401 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_fact.py
--rw-r--r--   0 root         (0) root         (0)     2033 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_fact_type_definition.py
--rw-r--r--   0 root         (0) root         (0)     1747 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_fact_type_definition_arguments_inner.py
--rw-r--r--   0 root         (0) root         (0)     2719 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_new_read_context_config_rule.py
--rw-r--r--   0 root         (0) root         (0)     1542 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_patch_request_inner.py
--rw-r--r--   0 root         (0) root         (0)     2981 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_policy_api.py
--rw-r--r--   0 root         (0) root         (0)      728 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_policy_rule_operation.py
--rw-r--r--   0 root         (0) root         (0)      707 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_policy_rule_result.py
--rw-r--r--   0 root         (0) root         (0)     1907 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_principal_info.py
--rw-r--r--   0 root         (0) root         (0)     1601 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_principal_summary.py
--rw-r--r--   0 root         (0) root         (0)     2930 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_read_context_config_rule.py
--rw-r--r--   0 root         (0) root         (0)     6344 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_read_context_details.py
--rw-r--r--   0 root         (0) root         (0)     3054 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_read_context_list.py
--rw-r--r--   0 root         (0) root         (0)     1499 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_read_context_parameter.py
--rw-r--r--   0 root         (0) root         (0)     1703 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_read_context_required_hook.py
--rw-r--r--   0 root         (0) root         (0)     1842 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_read_context_rule_facts_inner.py
--rw-r--r--   0 root         (0) root         (0)     1735 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_read_context_rule_facts_inner_arguments_inner.py
--rw-r--r--   0 root         (0) root         (0)     1906 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_read_context_rule_match_expressions_inner.py
--rw-r--r--   0 root         (0) root         (0)     2431 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_read_context_short_details.py
--rw-r--r--   0 root         (0) root         (0)     1628 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_resource_exhausted_error.py
--rw-r--r--   0 root         (0) root         (0)     1617 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_resource_not_found_error.py
--rw-r--r--   0 root         (0) root         (0)     1550 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_root_encryption_key_id_response.py
--rw-r--r--   0 root         (0) root         (0)     1683 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_root_encryption_key_item.py
--rw-r--r--   0 root         (0) root         (0)     2004 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_root_encryption_key_test_response.py
--rw-r--r--   0 root         (0) root         (0)     1594 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_rotate_key_encryption_key_response.py
--rw-r--r--   0 root         (0) root         (0)     1546 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_starred_domain_list.py
--rw-r--r--   0 root         (0) root         (0)     1607 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_tag.py
--rw-r--r--   0 root         (0) root         (0)     1355 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_tag_meta.py
--rw-r--r--   0 root         (0) root         (0)     3449 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_tag_set.py
--rw-r--r--   0 root         (0) root         (0)     2322 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_tag_set_span_tags_inner.py
--rw-r--r--   0 root         (0) root         (0)     3057 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_tag_summary.py
--rw-r--r--   0 root         (0) root         (0)     1686 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_tag_summary_elided_tags_inner.py
--rw-r--r--   0 root         (0) root         (0)     2224 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_tag_summary_unique_tags_inner.py
--rw-r--r--   0 root         (0) root         (0)      679 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_tag_type_field.py
--rw-r--r--   0 root         (0) root         (0)     1429 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_unauthorized_error.py
--rw-r--r--   0 root         (0) root         (0)     3777 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_upsert_span_tags_request.py
--rw-r--r--   0 root         (0) root         (0)     1620 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_verify_contact_response.py
--rw-r--r--   0 root         (0) root         (0)     2674 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_write_context_config_info.py
--rw-r--r--   0 root         (0) root         (0)     2126 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_write_context_config_info_required_hooks_inner.py
--rw-r--r--   0 root         (0) root         (0)     3648 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_write_context_details.py
--rw-r--r--   0 root         (0) root         (0)     4328 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_write_context_list.py
--rw-r--r--   0 root         (0) root         (0)     2735 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_write_context_regex_rule.py
--rw-r--r--   0 root         (0) root         (0)     1607 2020-04-16 12:00:00.000000 antimatter_api-1.0.7/test/test_write_context_regex_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 23:44:45.246813 antimatter_api-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      476 2024-05-21 23:44:45.246813 antimatter_api-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    28466 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 23:44:45.006812 antimatter_api-1.0.9/antimatter_api/
+-rw-r--r--   0 root         (0) root         (0)    13491 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 23:44:45.014812 antimatter_api-1.0.9/antimatter_api/api/
+-rw-r--r--   0 root         (0) root         (0)      525 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31861 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api/account_management_api.py
+-rw-r--r--   0 root         (0) root         (0)   199587 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api/authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)   146245 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api/capsules_api.py
+-rw-r--r--   0 root         (0) root         (0)   202747 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api/contexts_api.py
+-rw-r--r--   0 root         (0) root         (0)   107696 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api/encryption_api.py
+-rw-r--r--   0 root         (0) root         (0)   162505 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api/general_api.py
+-rw-r--r--   0 root         (0) root         (0)    79682 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api/internal_api.py
+-rw-r--r--   0 root         (0) root         (0)   175135 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api/policy_api.py
+-rw-r--r--   0 root         (0) root         (0)    25772 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/api_response.py
+-rw-r--r--   0 root         (0) root         (0)    15374 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 23:44:45.134812 antimatter_api-1.0.9/antimatter_api/models/
+-rw-r--r--   0 root         (0) root         (0)    12470 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6818 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/access_log_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/access_log_entry_create_info.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/access_log_entry_open_info.py
+-rw-r--r--   0 root         (0) root         (0)     5338 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/access_log_entry_read_info.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/access_log_results.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/active_root_encryption_key_id.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/add_capsule_log_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     4889 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/add_read_context.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/add_write_context.py
+-rw-r--r--   0 root         (0) root         (0)     3237 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/antimatter_delegated_aws_key_info.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/api_key_domain_identity_provider_details.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/available_delegated_root_encryption_key_provider.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/available_root_encryption_key_providers.py
+-rw-r--r--   0 root         (0) root         (0)     6733 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/available_root_encryption_key_providers_providers_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3264 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/available_service_account_root_encryption_key_provider.py
+-rw-r--r--   0 root         (0) root         (0)     3526 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/aws_service_account_key_info.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capability.py
+-rw-r--r--   0 root         (0) root         (0)     5047 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capability_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capability_definition_list.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capability_list.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capability_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capability_rule_match_expressions_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4627 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capsule_create_response.py
+-rw-r--r--   0 root         (0) root         (0)     4932 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capsule_info.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capsule_list.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capsule_open_request.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capsule_open_response.py
+-rw-r--r--   0 root         (0) root         (0)     3506 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capsule_open_response_read_context_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/capsule_seal_request.py
+-rw-r--r--   0 root         (0) root         (0)     3024 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/conflict_error.py
+-rw-r--r--   0 root         (0) root         (0)     7376 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/create_peer_domain.py
+-rw-r--r--   0 root         (0) root         (0)     3177 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_input.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_input_records_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_input_records_inner_elements_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_response.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_response_records_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/delete_tags.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_add_read_context_rule200_response.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_authenticate.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_authenticate_response.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_contact_issue_verify_request.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_control_log_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3256 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_control_log_results.py
+-rw-r--r--   0 root         (0) root         (0)     3024 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_fact_list.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_hooks_list.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_hooks_list_hooks_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_api_key_principal_params.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_email_principal_params.py
+-rw-r--r--   0 root         (0) root         (0)     3153 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_hosted_domain_principal_params.py
+-rw-r--r--   0 root         (0) root         (0)     7429 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_principal_details.py
+-rw-r--r--   0 root         (0) root         (0)     6301 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_details.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_info.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_list.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_principal_list.py
+-rw-r--r--   0 root         (0) root         (0)     3494 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_principal_params.py
+-rw-r--r--   0 root         (0) root         (0)      844 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_principal_type.py
+-rw-r--r--   0 root         (0) root         (0)      830 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_type.py
+-rw-r--r--   0 root         (0) root         (0)     3359 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_insert_identity_provider_principal200_response.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_insert_write_context_regex_rule200_response.py
+-rw-r--r--   0 root         (0) root         (0)    14664 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_peer_config.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_peer_list.py
+-rw-r--r--   0 root         (0) root         (0)     3523 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_peer_list_peers_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3525 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7184 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_policy_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_private_info.py
+-rw-r--r--   0 root         (0) root         (0)     3962 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_public_info.py
+-rw-r--r--   0 root         (0) root         (0)     3092 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_resource_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_resource_summary_schema_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4066 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_settings_disaster_recovery.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_settings_patch.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_status.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_status_notifications_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/domain_tag_info_results.py
+-rw-r--r--   0 root         (0) root         (0)     2551 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     3886 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/fact.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/fact_list.py
+-rw-r--r--   0 root         (0) root         (0)     4310 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/fact_policy_rules_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4385 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/fact_policy_rules_inner_arguments_inner.py
+-rw-r--r--   0 root         (0) root         (0)     5008 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/fact_type_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/forbidden_error.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/gcp_service_account_key_info.py
+-rw-r--r--   0 root         (0) root         (0)     3124 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/google_o_auth_domain_identity_provider_details.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/invalid_request_error.py
+-rw-r--r--   0 root         (0) root         (0)     3275 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/json_patch_request_add.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/json_patch_request_add_value.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/json_patch_request_copy.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/json_patch_request_move.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/json_patch_request_remove.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/json_patch_request_replace.py
+-rw-r--r--   0 root         (0) root         (0)     6131 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/json_patch_request_replace_value.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/json_patch_request_tst.py
+-rw-r--r--   0 root         (0) root         (0)     6100 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/json_patch_request_tst_value.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/key_infos.py
+-rw-r--r--   0 root         (0) root         (0)     6802 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/key_infos_key_information.py
+-rw-r--r--   0 root         (0) root         (0)     3508 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_access_log_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_access_log_entry_read_info.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_capability_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_domain.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_domain_policy_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3068 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_domain_response.py
+-rw-r--r--   0 root         (0) root         (0)     2745 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_fact.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_fact_type_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_fact_type_definition_arguments_inner.py
+-rw-r--r--   0 root         (0) root         (0)     6250 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/new_read_context_config_rule.py
+-rw-r--r--   0 root         (0) root         (0)     9116 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/patch_request_inner.py
+-rw-r--r--   0 root         (0) root         (0)      759 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/policy_rule_operation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/policy_rule_result.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/principal_info.py
+-rw-r--r--   0 root         (0) root         (0)     3506 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/principal_summary.py
+-rw-r--r--   0 root         (0) root         (0)     7854 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/read_context_config_rule.py
+-rw-r--r--   0 root         (0) root         (0)     7277 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/read_context_details.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/read_context_list.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/read_context_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/read_context_required_hook.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/read_context_rule_facts_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3326 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/read_context_rule_facts_inner_arguments_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/read_context_rule_match_expressions_inner.py
+-rw-r--r--   0 root         (0) root         (0)     5759 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/read_context_short_details.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/resource_exhausted_error.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/resource_not_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/root_encryption_key_id_response.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/root_encryption_key_item.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/root_encryption_key_test_response.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/rotate_key_encryption_key_response.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/starred_domain_list.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/tag_meta.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/tag_set.py
+-rw-r--r--   0 root         (0) root         (0)     3162 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/tag_set_span_tags_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3812 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/tag_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/tag_summary_elided_tags_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/tag_summary_unique_tags_inner.py
+-rw-r--r--   0 root         (0) root         (0)      800 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/tag_type_field.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/unauthorized_error.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/upsert_span_tags_request.py
+-rw-r--r--   0 root         (0) root         (0)     3141 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/verify_contact_response.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/write_context_config_info.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/write_context_config_info_required_hooks_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/write_context_details.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/write_context_list.py
+-rw-r--r--   0 root         (0) root         (0)     4388 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/write_context_regex_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/models/write_context_regex_tag.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9213 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/antimatter_api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 23:44:45.246813 antimatter_api-1.0.9/antimatter_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      476 2024-05-21 23:44:44.000000 antimatter_api-1.0.9/antimatter_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14126 2024-05-21 23:44:44.000000 antimatter_api-1.0.9/antimatter_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 23:44:44.000000 antimatter_api-1.0.9/antimatter_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-21 23:44:44.000000 antimatter_api-1.0.9/antimatter_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-21 23:44:44.000000 antimatter_api-1.0.9/antimatter_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1963 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-21 23:44:45.246813 antimatter_api-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1287 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 23:44:45.242813 antimatter_api-1.0.9/test/
+-rw-r--r--   0 root         (0) root         (0)     4973 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_access_log_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_access_log_entry_create_info.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_access_log_entry_open_info.py
+-rw-r--r--   0 root         (0) root         (0)     8052 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_access_log_entry_read_info.py
+-rw-r--r--   0 root         (0) root         (0)     9130 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_access_log_results.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_account_management_api.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_active_root_encryption_key_id.py
+-rw-r--r--   0 root         (0) root         (0)     7506 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_add_capsule_log_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_add_read_context.py
+-rw-r--r--   0 root         (0) root         (0)     3354 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_add_write_context.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_antimatter_delegated_aws_key_info.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_api_key_domain_identity_provider_details.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_available_delegated_root_encryption_key_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_available_root_encryption_key_providers.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_available_root_encryption_key_providers_providers_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_available_service_account_root_encryption_key_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_aws_service_account_key_info.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capability.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capability_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capability_definition_list.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capability_list.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capability_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capability_rule_match_expressions_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3992 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capsule_create_response.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capsule_info.py
+-rw-r--r--   0 root         (0) root         (0)     5497 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capsule_list.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capsule_open_request.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capsule_open_response.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capsule_open_response_read_context_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capsule_seal_request.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_capsules_api.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_conflict_error.py
+-rw-r--r--   0 root         (0) root         (0)     3553 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_contexts_api.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_create_peer_domain.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_data_tagging_hook_input.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_data_tagging_hook_input_records_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_data_tagging_hook_input_records_inner_elements_inner.py
+-rw-r--r--   0 root         (0) root         (0)     5021 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_data_tagging_hook_response.py
+-rw-r--r--   0 root         (0) root         (0)     4363 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_data_tagging_hook_response_records_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_delete_tags.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_add_read_context_rule200_response.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_authenticate.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_authenticate_response.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_contact_issue_verify_request.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_control_log_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_control_log_results.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_fact_list.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_hooks_list.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_hooks_list_hooks_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_api_key_principal_params.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_email_principal_params.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_hosted_domain_principal_params.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_principal_details.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_provider_details.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_provider_info.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_provider_list.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_provider_principal_list.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_provider_principal_params.py
+-rw-r--r--   0 root         (0) root         (0)      842 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_provider_principal_type.py
+-rw-r--r--   0 root         (0) root         (0)      778 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_identity_provider_type.py
+-rw-r--r--   0 root         (0) root         (0)     1873 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_insert_identity_provider_principal200_response.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_insert_write_context_regex_rule200_response.py
+-rw-r--r--   0 root         (0) root         (0)     3665 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_peer_config.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_peer_list.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_peer_list_peers_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_policy_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_private_info.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_public_info.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_resource_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_resource_summary_schema_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_settings_disaster_recovery.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_settings_patch.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_status.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_status_notifications_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_domain_tag_info_results.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_encryption_api.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_error.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_fact.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_fact_list.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_fact_policy_rules_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_fact_policy_rules_inner_arguments_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_fact_type_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_forbidden_error.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_gcp_service_account_key_info.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_general_api.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_google_o_auth_domain_identity_provider_details.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_internal_api.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_invalid_request_error.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_json_patch_request_add.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_json_patch_request_add_value.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_json_patch_request_copy.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_json_patch_request_move.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_json_patch_request_remove.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_json_patch_request_replace.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_json_patch_request_replace_value.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_json_patch_request_tst.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_json_patch_request_tst_value.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_key_infos.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_key_infos_key_information.py
+-rw-r--r--   0 root         (0) root         (0)     6550 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_access_log_entry.py
+-rw-r--r--   0 root         (0) root         (0)     7987 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_access_log_entry_read_info.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_capability_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_domain.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_domain_policy_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_domain_response.py
+-rw-r--r--   0 root         (0) root         (0)     1401 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_fact.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_fact_type_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_fact_type_definition_arguments_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_new_read_context_config_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_patch_request_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_policy_api.py
+-rw-r--r--   0 root         (0) root         (0)      728 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_policy_rule_operation.py
+-rw-r--r--   0 root         (0) root         (0)      707 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_policy_rule_result.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_principal_info.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_principal_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_read_context_config_rule.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_read_context_details.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_read_context_list.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_read_context_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_read_context_required_hook.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_read_context_rule_facts_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_read_context_rule_facts_inner_arguments_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_read_context_rule_match_expressions_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_read_context_short_details.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_resource_exhausted_error.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_resource_not_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_root_encryption_key_id_response.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_root_encryption_key_item.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_root_encryption_key_test_response.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_rotate_key_encryption_key_response.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_starred_domain_list.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_tag_meta.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_tag_set.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_tag_set_span_tags_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_tag_summary.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_tag_summary_elided_tags_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_tag_summary_unique_tags_inner.py
+-rw-r--r--   0 root         (0) root         (0)      679 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_tag_type_field.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_unauthorized_error.py
+-rw-r--r--   0 root         (0) root         (0)     3777 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_upsert_span_tags_request.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_verify_contact_response.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_write_context_config_info.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_write_context_config_info_required_hooks_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_write_context_details.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_write_context_list.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_write_context_regex_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2020-04-16 12:00:00.000000 antimatter_api-1.0.9/test/test_write_context_regex_tag.py
```

### Comparing `antimatter_api-1.0.7/README.md` & `antimatter_api-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # antimatter-api
 Interact with the Antimatter Cloud API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.7
-- Package version: 1.0.7
+- API version: 1.0.9
+- Package version: 1.0.9
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `antimatter_api-1.0.7/antimatter_api/__init__.py` & `antimatter_api-1.0.9/antimatter_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.7"
+__version__ = "1.0.9"
 
 # import apis into sdk package
 from antimatter_api.api.account_management_api import AccountManagementApi
 from antimatter_api.api.authentication_api import AuthenticationApi
 from antimatter_api.api.capsules_api import CapsulesApi
 from antimatter_api.api.contexts_api import ContextsApi
 from antimatter_api.api.encryption_api import EncryptionApi
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api/__init__.py` & `antimatter_api-1.0.9/antimatter_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `antimatter_api-1.0.7/antimatter_api/api/account_management_api.py` & `antimatter_api-1.0.9/antimatter_api/api/account_management_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api/authentication_api.py` & `antimatter_api-1.0.9/antimatter_api/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api/capsules_api.py` & `antimatter_api-1.0.9/antimatter_api/api/capsules_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api/contexts_api.py` & `antimatter_api-1.0.9/antimatter_api/api/contexts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api/encryption_api.py` & `antimatter_api-1.0.9/antimatter_api/api/encryption_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api/general_api.py` & `antimatter_api-1.0.9/antimatter_api/api/general_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api/internal_api.py` & `antimatter_api-1.0.9/antimatter_api/api/internal_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api/policy_api.py` & `antimatter_api-1.0.9/antimatter_api/api/policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api_client.py` & `antimatter_api-1.0.9/antimatter_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.7/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.9/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `antimatter_api-1.0.7/antimatter_api/api_response.py` & `antimatter_api-1.0.9/antimatter_api/api_response.py`

 * *Files identical despite different names*

### Comparing `antimatter_api-1.0.7/antimatter_api/configuration.py` & `antimatter_api-1.0.9/antimatter_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -391,16 +391,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.7\n"\
-               "SDK Package Version: 1.0.7".\
+               "Version of the API: 1.0.9\n"\
+               "SDK Package Version: 1.0.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `antimatter_api-1.0.7/antimatter_api/exceptions.py` & `antimatter_api-1.0.9/antimatter_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/__init__.py` & `antimatter_api-1.0.9/antimatter_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/access_log_entry.py` & `antimatter_api-1.0.9/antimatter_api/models/access_log_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/access_log_entry_create_info.py` & `antimatter_api-1.0.9/antimatter_api/models/access_log_entry_create_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/access_log_entry_open_info.py` & `antimatter_api-1.0.9/antimatter_api/models/access_log_entry_open_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/access_log_entry_read_info.py` & `antimatter_api-1.0.9/antimatter_api/models/access_log_entry_read_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/access_log_results.py` & `antimatter_api-1.0.9/antimatter_api/models/access_log_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/active_root_encryption_key_id.py` & `antimatter_api-1.0.9/antimatter_api/models/active_root_encryption_key_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/add_capsule_log_entry_request.py` & `antimatter_api-1.0.9/antimatter_api/models/add_capsule_log_entry_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/add_read_context.py` & `antimatter_api-1.0.9/antimatter_api/models/add_read_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/add_write_context.py` & `antimatter_api-1.0.9/antimatter_api/models/add_write_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/antimatter_delegated_aws_key_info.py` & `antimatter_api-1.0.9/antimatter_api/models/antimatter_delegated_aws_key_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/api_key_domain_identity_provider_details.py` & `antimatter_api-1.0.9/antimatter_api/models/api_key_domain_identity_provider_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/available_delegated_root_encryption_key_provider.py` & `antimatter_api-1.0.9/antimatter_api/models/available_delegated_root_encryption_key_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/available_root_encryption_key_providers.py` & `antimatter_api-1.0.9/antimatter_api/models/available_root_encryption_key_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/available_root_encryption_key_providers_providers_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/available_root_encryption_key_providers_providers_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/available_service_account_root_encryption_key_provider.py` & `antimatter_api-1.0.9/antimatter_api/models/available_service_account_root_encryption_key_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/aws_service_account_key_info.py` & `antimatter_api-1.0.9/antimatter_api/models/aws_service_account_key_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capability.py` & `antimatter_api-1.0.9/antimatter_api/models/capability.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capability_definition.py` & `antimatter_api-1.0.9/antimatter_api/models/capability_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capability_definition_list.py` & `antimatter_api-1.0.9/antimatter_api/models/capability_definition_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capability_list.py` & `antimatter_api-1.0.9/antimatter_api/models/capability_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capability_rule.py` & `antimatter_api-1.0.9/antimatter_api/models/capability_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capability_rule_match_expressions_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/capability_rule_match_expressions_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capsule_create_response.py` & `antimatter_api-1.0.9/antimatter_api/models/capsule_create_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capsule_info.py` & `antimatter_api-1.0.9/antimatter_api/models/capsule_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capsule_list.py` & `antimatter_api-1.0.9/antimatter_api/models/capsule_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capsule_open_request.py` & `antimatter_api-1.0.9/antimatter_api/models/capsule_open_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capsule_open_response.py` & `antimatter_api-1.0.9/antimatter_api/models/capsule_open_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capsule_open_response_read_context_configuration.py` & `antimatter_api-1.0.9/antimatter_api/models/capsule_open_response_read_context_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/capsule_seal_request.py` & `antimatter_api-1.0.9/antimatter_api/models/capsule_seal_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/conflict_error.py` & `antimatter_api-1.0.9/antimatter_api/models/conflict_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/create_peer_domain.py` & `antimatter_api-1.0.9/antimatter_api/models/create_peer_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_input.py` & `antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_input_records_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_input_records_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_input_records_inner_elements_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_input_records_inner_elements_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_response.py` & `antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/data_tagging_hook_response_records_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/data_tagging_hook_response_records_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/delete_tags.py` & `antimatter_api-1.0.9/antimatter_api/models/delete_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain.py` & `antimatter_api-1.0.9/antimatter_api/models/domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_add_read_context_rule200_response.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_add_read_context_rule200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_authenticate.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_authenticate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_authenticate_response.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_authenticate_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_contact_issue_verify_request.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_contact_issue_verify_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_control_log_entry.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_control_log_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_control_log_results.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_control_log_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_fact_list.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_fact_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_hooks_list.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_hooks_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_hooks_list_hooks_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_hooks_list_hooks_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_api_key_principal_params.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_api_key_principal_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_email_principal_params.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_email_principal_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_hosted_domain_principal_params.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_hosted_domain_principal_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_principal_details.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_principal_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_details.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_info.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_list.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_principal_list.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_principal_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_principal_params.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_principal_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_principal_type.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_principal_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_identity_provider_type.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_identity_provider_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_insert_identity_provider_principal200_response.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_insert_identity_provider_principal200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_insert_write_context_regex_rule200_response.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_insert_write_context_regex_rule200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_peer_config.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_peer_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_peer_list.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_peer_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_peer_list_peers_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_peer_list_peers_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_policy.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_policy_rule.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_policy_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_private_info.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_private_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_public_info.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_public_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_resource_summary.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_resource_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_resource_summary_schema_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_resource_summary_schema_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_settings.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_settings_disaster_recovery.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_settings_disaster_recovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_settings_patch.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_settings_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_status.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_status_notifications_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_status_notifications_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/domain_tag_info_results.py` & `antimatter_api-1.0.9/antimatter_api/models/domain_tag_info_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/error.py` & `antimatter_api-1.0.9/antimatter_api/models/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/fact.py` & `antimatter_api-1.0.9/antimatter_api/models/fact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/fact_list.py` & `antimatter_api-1.0.9/antimatter_api/models/fact_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/fact_policy_rules_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/fact_policy_rules_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/fact_policy_rules_inner_arguments_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/fact_policy_rules_inner_arguments_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/fact_type_definition.py` & `antimatter_api-1.0.9/antimatter_api/models/fact_type_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/forbidden_error.py` & `antimatter_api-1.0.9/antimatter_api/models/forbidden_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/gcp_service_account_key_info.py` & `antimatter_api-1.0.9/antimatter_api/models/gcp_service_account_key_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/google_o_auth_domain_identity_provider_details.py` & `antimatter_api-1.0.9/antimatter_api/models/google_o_auth_domain_identity_provider_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/hook_invocation.py` & `antimatter_api-1.0.9/antimatter_api/models/hook_invocation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/invalid_request_error.py` & `antimatter_api-1.0.9/antimatter_api/models/invalid_request_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/json_patch_request_add.py` & `antimatter_api-1.0.9/antimatter_api/models/json_patch_request_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/json_patch_request_add_value.py` & `antimatter_api-1.0.9/antimatter_api/models/json_patch_request_add_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/json_patch_request_copy.py` & `antimatter_api-1.0.9/antimatter_api/models/json_patch_request_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/json_patch_request_move.py` & `antimatter_api-1.0.9/antimatter_api/models/json_patch_request_move.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/json_patch_request_remove.py` & `antimatter_api-1.0.9/antimatter_api/models/json_patch_request_remove.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/json_patch_request_replace.py` & `antimatter_api-1.0.9/antimatter_api/models/json_patch_request_replace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/json_patch_request_replace_value.py` & `antimatter_api-1.0.9/antimatter_api/models/json_patch_request_replace_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/json_patch_request_tst.py` & `antimatter_api-1.0.9/antimatter_api/models/json_patch_request_tst.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/json_patch_request_tst_value.py` & `antimatter_api-1.0.9/antimatter_api/models/json_patch_request_tst_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/key_infos.py` & `antimatter_api-1.0.9/antimatter_api/models/key_infos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/key_infos_key_information.py` & `antimatter_api-1.0.9/antimatter_api/models/key_infos_key_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_access_log_entry.py` & `antimatter_api-1.0.9/antimatter_api/models/new_access_log_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_access_log_entry_read_info.py` & `antimatter_api-1.0.9/antimatter_api/models/new_access_log_entry_read_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_capability_definition.py` & `antimatter_api-1.0.9/antimatter_api/models/new_capability_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_domain.py` & `antimatter_api-1.0.9/antimatter_api/models/new_domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_domain_policy_rule.py` & `antimatter_api-1.0.9/antimatter_api/models/new_domain_policy_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_domain_response.py` & `antimatter_api-1.0.9/antimatter_api/models/new_domain_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_fact.py` & `antimatter_api-1.0.9/antimatter_api/models/new_fact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_fact_type_definition.py` & `antimatter_api-1.0.9/antimatter_api/models/new_fact_type_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_fact_type_definition_arguments_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/new_fact_type_definition_arguments_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/new_read_context_config_rule.py` & `antimatter_api-1.0.9/antimatter_api/models/new_read_context_config_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/patch_request_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/patch_request_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/policy_rule_operation.py` & `antimatter_api-1.0.9/antimatter_api/models/policy_rule_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/policy_rule_result.py` & `antimatter_api-1.0.9/antimatter_api/models/policy_rule_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/principal_info.py` & `antimatter_api-1.0.9/antimatter_api/models/principal_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/principal_summary.py` & `antimatter_api-1.0.9/antimatter_api/models/principal_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/read_context_config_rule.py` & `antimatter_api-1.0.9/antimatter_api/models/read_context_config_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/read_context_details.py` & `antimatter_api-1.0.9/antimatter_api/models/read_context_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/read_context_list.py` & `antimatter_api-1.0.9/antimatter_api/models/read_context_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/read_context_parameter.py` & `antimatter_api-1.0.9/antimatter_api/models/read_context_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/read_context_required_hook.py` & `antimatter_api-1.0.9/antimatter_api/models/read_context_required_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/read_context_rule_facts_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/read_context_rule_facts_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/read_context_rule_facts_inner_arguments_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/read_context_rule_facts_inner_arguments_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/read_context_rule_match_expressions_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/read_context_rule_match_expressions_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/read_context_short_details.py` & `antimatter_api-1.0.9/antimatter_api/models/read_context_short_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/resource_exhausted_error.py` & `antimatter_api-1.0.9/antimatter_api/models/resource_exhausted_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/resource_not_found_error.py` & `antimatter_api-1.0.9/antimatter_api/models/resource_not_found_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/root_encryption_key_id_response.py` & `antimatter_api-1.0.9/antimatter_api/models/root_encryption_key_id_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/root_encryption_key_item.py` & `antimatter_api-1.0.9/antimatter_api/models/root_encryption_key_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/root_encryption_key_test_response.py` & `antimatter_api-1.0.9/antimatter_api/models/root_encryption_key_test_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/rotate_key_encryption_key_response.py` & `antimatter_api-1.0.9/antimatter_api/models/rotate_key_encryption_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/starred_domain_list.py` & `antimatter_api-1.0.9/antimatter_api/models/starred_domain_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/tag.py` & `antimatter_api-1.0.9/antimatter_api/models/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/tag_meta.py` & `antimatter_api-1.0.9/antimatter_api/models/tag_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/tag_set.py` & `antimatter_api-1.0.9/antimatter_api/models/tag_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/tag_set_span_tags_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/tag_set_span_tags_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/tag_summary.py` & `antimatter_api-1.0.9/antimatter_api/models/tag_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/tag_summary_elided_tags_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/tag_summary_elided_tags_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/tag_summary_unique_tags_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/tag_summary_unique_tags_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/tag_type_field.py` & `antimatter_api-1.0.9/antimatter_api/models/tag_type_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/unauthorized_error.py` & `antimatter_api-1.0.9/antimatter_api/models/unauthorized_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/upsert_span_tags_request.py` & `antimatter_api-1.0.9/antimatter_api/models/upsert_span_tags_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/verify_contact_response.py` & `antimatter_api-1.0.9/antimatter_api/models/verify_contact_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/write_context_config_info.py` & `antimatter_api-1.0.9/antimatter_api/models/write_context_config_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/write_context_config_info_required_hooks_inner.py` & `antimatter_api-1.0.9/antimatter_api/models/write_context_config_info_required_hooks_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/write_context_details.py` & `antimatter_api-1.0.9/antimatter_api/models/write_context_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/write_context_list.py` & `antimatter_api-1.0.9/antimatter_api/models/write_context_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/write_context_regex_rule.py` & `antimatter_api-1.0.9/antimatter_api/models/write_context_regex_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/models/write_context_regex_tag.py` & `antimatter_api-1.0.9/antimatter_api/models/write_context_regex_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api/rest.py` & `antimatter_api-1.0.9/antimatter_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/antimatter_api.egg-info/SOURCES.txt` & `antimatter_api-1.0.9/antimatter_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antimatter_api-1.0.7/pyproject.toml` & `antimatter_api-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antimatter_api"
-version = "1.0.7"
+version = "1.0.9"
 description = "Antimatter Public API"
 authors = ["OpenAPI Generator Community <support@antimatter.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Antimatter Public API"]
 include = ["antimatter_api/py.typed"]
```

### Comparing `antimatter_api-1.0.7/setup.py` & `antimatter_api-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "antimatter-api"
-VERSION = "1.0.7"
+VERSION = "1.0.9"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `antimatter_api-1.0.7/test/test_access_log_entry.py` & `antimatter_api-1.0.9/test/test_access_log_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_access_log_entry_create_info.py` & `antimatter_api-1.0.9/test/test_access_log_entry_create_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_access_log_entry_open_info.py` & `antimatter_api-1.0.9/test/test_access_log_entry_open_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_access_log_entry_read_info.py` & `antimatter_api-1.0.9/test/test_access_log_entry_read_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_access_log_results.py` & `antimatter_api-1.0.9/test/test_access_log_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_account_management_api.py` & `antimatter_api-1.0.9/test/test_account_management_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_active_root_encryption_key_id.py` & `antimatter_api-1.0.9/test/test_active_root_encryption_key_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_add_capsule_log_entry_request.py` & `antimatter_api-1.0.9/test/test_add_capsule_log_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_add_read_context.py` & `antimatter_api-1.0.9/test/test_add_read_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_add_write_context.py` & `antimatter_api-1.0.9/test/test_add_write_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_antimatter_delegated_aws_key_info.py` & `antimatter_api-1.0.9/test/test_antimatter_delegated_aws_key_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_api_key_domain_identity_provider_details.py` & `antimatter_api-1.0.9/test/test_api_key_domain_identity_provider_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_authentication_api.py` & `antimatter_api-1.0.9/test/test_authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_available_delegated_root_encryption_key_provider.py` & `antimatter_api-1.0.9/test/test_available_delegated_root_encryption_key_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_available_root_encryption_key_providers.py` & `antimatter_api-1.0.9/test/test_available_root_encryption_key_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_available_root_encryption_key_providers_providers_inner.py` & `antimatter_api-1.0.9/test/test_available_root_encryption_key_providers_providers_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_available_service_account_root_encryption_key_provider.py` & `antimatter_api-1.0.9/test/test_available_service_account_root_encryption_key_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_aws_service_account_key_info.py` & `antimatter_api-1.0.9/test/test_aws_service_account_key_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capability.py` & `antimatter_api-1.0.9/test/test_capability.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capability_definition.py` & `antimatter_api-1.0.9/test/test_capability_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capability_definition_list.py` & `antimatter_api-1.0.9/test/test_capability_definition_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capability_list.py` & `antimatter_api-1.0.9/test/test_capability_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capability_rule.py` & `antimatter_api-1.0.9/test/test_capability_rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capability_rule_match_expressions_inner.py` & `antimatter_api-1.0.9/test/test_capability_rule_match_expressions_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capsule_create_response.py` & `antimatter_api-1.0.9/test/test_capsule_create_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capsule_info.py` & `antimatter_api-1.0.9/test/test_capsule_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capsule_list.py` & `antimatter_api-1.0.9/test/test_capsule_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capsule_open_request.py` & `antimatter_api-1.0.9/test/test_capsule_open_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capsule_open_response.py` & `antimatter_api-1.0.9/test/test_capsule_open_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capsule_open_response_read_context_configuration.py` & `antimatter_api-1.0.9/test/test_capsule_open_response_read_context_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capsule_seal_request.py` & `antimatter_api-1.0.9/test/test_capsule_seal_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_capsules_api.py` & `antimatter_api-1.0.9/test/test_capsules_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_conflict_error.py` & `antimatter_api-1.0.9/test/test_conflict_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_contexts_api.py` & `antimatter_api-1.0.9/test/test_contexts_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_create_peer_domain.py` & `antimatter_api-1.0.9/test/test_create_peer_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_data_tagging_hook_input.py` & `antimatter_api-1.0.9/test/test_data_tagging_hook_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_data_tagging_hook_input_records_inner.py` & `antimatter_api-1.0.9/test/test_data_tagging_hook_input_records_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_data_tagging_hook_input_records_inner_elements_inner.py` & `antimatter_api-1.0.9/test/test_data_tagging_hook_input_records_inner_elements_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_data_tagging_hook_response.py` & `antimatter_api-1.0.9/test/test_data_tagging_hook_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_data_tagging_hook_response_records_inner.py` & `antimatter_api-1.0.9/test/test_data_tagging_hook_response_records_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_delete_tags.py` & `antimatter_api-1.0.9/test/test_delete_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain.py` & `antimatter_api-1.0.9/test/test_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_add_read_context_rule200_response.py` & `antimatter_api-1.0.9/test/test_domain_add_read_context_rule200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_authenticate.py` & `antimatter_api-1.0.9/test/test_domain_authenticate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_authenticate_response.py` & `antimatter_api-1.0.9/test/test_domain_authenticate_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_contact_issue_verify_request.py` & `antimatter_api-1.0.9/test/test_domain_contact_issue_verify_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_control_log_entry.py` & `antimatter_api-1.0.9/test/test_domain_control_log_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_control_log_results.py` & `antimatter_api-1.0.9/test/test_domain_control_log_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_fact_list.py` & `antimatter_api-1.0.9/test/test_domain_fact_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_hooks_list.py` & `antimatter_api-1.0.9/test/test_domain_hooks_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_hooks_list_hooks_inner.py` & `antimatter_api-1.0.9/test/test_domain_hooks_list_hooks_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_api_key_principal_params.py` & `antimatter_api-1.0.9/test/test_domain_identity_api_key_principal_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_email_principal_params.py` & `antimatter_api-1.0.9/test/test_domain_identity_email_principal_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_hosted_domain_principal_params.py` & `antimatter_api-1.0.9/test/test_domain_identity_hosted_domain_principal_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_principal_details.py` & `antimatter_api-1.0.9/test/test_domain_identity_principal_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_provider_details.py` & `antimatter_api-1.0.9/test/test_domain_identity_provider_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_provider_info.py` & `antimatter_api-1.0.9/test/test_domain_identity_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_provider_list.py` & `antimatter_api-1.0.9/test/test_domain_identity_provider_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_provider_principal_list.py` & `antimatter_api-1.0.9/test/test_domain_identity_provider_principal_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_provider_principal_params.py` & `antimatter_api-1.0.9/test/test_domain_identity_provider_principal_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_provider_principal_type.py` & `antimatter_api-1.0.9/test/test_domain_identity_provider_principal_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_identity_provider_type.py` & `antimatter_api-1.0.9/test/test_domain_identity_provider_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_insert_identity_provider_principal200_response.py` & `antimatter_api-1.0.9/test/test_domain_insert_identity_provider_principal200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_insert_write_context_regex_rule200_response.py` & `antimatter_api-1.0.9/test/test_domain_insert_write_context_regex_rule200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_peer_config.py` & `antimatter_api-1.0.9/test/test_domain_peer_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_peer_list.py` & `antimatter_api-1.0.9/test/test_domain_peer_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_peer_list_peers_inner.py` & `antimatter_api-1.0.9/test/test_domain_peer_list_peers_inner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_policy.py` & `antimatter_api-1.0.9/test/test_domain_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_policy_rule.py` & `antimatter_api-1.0.9/test/test_domain_policy_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_private_info.py` & `antimatter_api-1.0.9/test/test_domain_private_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_public_info.py` & `antimatter_api-1.0.9/test/test_domain_public_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_resource_summary.py` & `antimatter_api-1.0.9/test/test_domain_resource_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_resource_summary_schema_inner.py` & `antimatter_api-1.0.9/test/test_domain_resource_summary_schema_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_settings.py` & `antimatter_api-1.0.9/test/test_domain_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_settings_disaster_recovery.py` & `antimatter_api-1.0.9/test/test_domain_settings_disaster_recovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_settings_patch.py` & `antimatter_api-1.0.9/test/test_domain_settings_patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_status.py` & `antimatter_api-1.0.9/test/test_domain_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_status_notifications_inner.py` & `antimatter_api-1.0.9/test/test_domain_status_notifications_inner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_domain_tag_info_results.py` & `antimatter_api-1.0.9/test/test_domain_tag_info_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_encryption_api.py` & `antimatter_api-1.0.9/test/test_encryption_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_error.py` & `antimatter_api-1.0.9/test/test_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_fact.py` & `antimatter_api-1.0.9/test/test_fact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_fact_list.py` & `antimatter_api-1.0.9/test/test_fact_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_fact_policy_rules_inner.py` & `antimatter_api-1.0.9/test/test_fact_policy_rules_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_fact_policy_rules_inner_arguments_inner.py` & `antimatter_api-1.0.9/test/test_fact_policy_rules_inner_arguments_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_fact_type_definition.py` & `antimatter_api-1.0.9/test/test_fact_type_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_forbidden_error.py` & `antimatter_api-1.0.9/test/test_forbidden_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_gcp_service_account_key_info.py` & `antimatter_api-1.0.9/test/test_gcp_service_account_key_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_general_api.py` & `antimatter_api-1.0.9/test/test_general_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_google_o_auth_domain_identity_provider_details.py` & `antimatter_api-1.0.9/test/test_google_o_auth_domain_identity_provider_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_hook_invocation.py` & `antimatter_api-1.0.9/test/test_hook_invocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_internal_api.py` & `antimatter_api-1.0.9/test/test_internal_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_invalid_request_error.py` & `antimatter_api-1.0.9/test/test_invalid_request_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_json_patch_request_add.py` & `antimatter_api-1.0.9/test/test_json_patch_request_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_json_patch_request_add_value.py` & `antimatter_api-1.0.9/test/test_json_patch_request_add_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_json_patch_request_copy.py` & `antimatter_api-1.0.9/test/test_json_patch_request_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_json_patch_request_move.py` & `antimatter_api-1.0.9/test/test_json_patch_request_move.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_json_patch_request_remove.py` & `antimatter_api-1.0.9/test/test_json_patch_request_remove.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_json_patch_request_replace.py` & `antimatter_api-1.0.9/test/test_json_patch_request_replace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_json_patch_request_replace_value.py` & `antimatter_api-1.0.9/test/test_json_patch_request_replace_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_json_patch_request_tst.py` & `antimatter_api-1.0.9/test/test_json_patch_request_tst.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_json_patch_request_tst_value.py` & `antimatter_api-1.0.9/test/test_json_patch_request_tst_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_key_infos.py` & `antimatter_api-1.0.9/test/test_key_infos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_key_infos_key_information.py` & `antimatter_api-1.0.9/test/test_key_infos_key_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_access_log_entry.py` & `antimatter_api-1.0.9/test/test_new_access_log_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_access_log_entry_read_info.py` & `antimatter_api-1.0.9/test/test_new_access_log_entry_read_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_capability_definition.py` & `antimatter_api-1.0.9/test/test_new_capability_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_domain.py` & `antimatter_api-1.0.9/test/test_new_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_domain_policy_rule.py` & `antimatter_api-1.0.9/test/test_new_domain_policy_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_domain_response.py` & `antimatter_api-1.0.9/test/test_new_domain_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_fact.py` & `antimatter_api-1.0.9/test/test_new_fact.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_fact_type_definition.py` & `antimatter_api-1.0.9/test/test_new_fact_type_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_fact_type_definition_arguments_inner.py` & `antimatter_api-1.0.9/test/test_new_fact_type_definition_arguments_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_new_read_context_config_rule.py` & `antimatter_api-1.0.9/test/test_new_read_context_config_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_patch_request_inner.py` & `antimatter_api-1.0.9/test/test_patch_request_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_policy_api.py` & `antimatter_api-1.0.9/test/test_policy_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_policy_rule_operation.py` & `antimatter_api-1.0.9/test/test_policy_rule_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_policy_rule_result.py` & `antimatter_api-1.0.9/test/test_policy_rule_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_principal_info.py` & `antimatter_api-1.0.9/test/test_principal_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_principal_summary.py` & `antimatter_api-1.0.9/test/test_principal_summary.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_read_context_config_rule.py` & `antimatter_api-1.0.9/test/test_read_context_config_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_read_context_details.py` & `antimatter_api-1.0.9/test/test_read_context_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_read_context_list.py` & `antimatter_api-1.0.9/test/test_read_context_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_read_context_parameter.py` & `antimatter_api-1.0.9/test/test_read_context_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_read_context_required_hook.py` & `antimatter_api-1.0.9/test/test_read_context_required_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_read_context_rule_facts_inner.py` & `antimatter_api-1.0.9/test/test_read_context_rule_facts_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_read_context_rule_facts_inner_arguments_inner.py` & `antimatter_api-1.0.9/test/test_read_context_rule_facts_inner_arguments_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_read_context_rule_match_expressions_inner.py` & `antimatter_api-1.0.9/test/test_read_context_rule_match_expressions_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_read_context_short_details.py` & `antimatter_api-1.0.9/test/test_read_context_short_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_resource_exhausted_error.py` & `antimatter_api-1.0.9/test/test_resource_exhausted_error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_resource_not_found_error.py` & `antimatter_api-1.0.9/test/test_resource_not_found_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_root_encryption_key_id_response.py` & `antimatter_api-1.0.9/test/test_root_encryption_key_id_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_root_encryption_key_item.py` & `antimatter_api-1.0.9/test/test_root_encryption_key_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_root_encryption_key_test_response.py` & `antimatter_api-1.0.9/test/test_root_encryption_key_test_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_rotate_key_encryption_key_response.py` & `antimatter_api-1.0.9/test/test_rotate_key_encryption_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_starred_domain_list.py` & `antimatter_api-1.0.9/test/test_starred_domain_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_tag.py` & `antimatter_api-1.0.9/test/test_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_tag_meta.py` & `antimatter_api-1.0.9/test/test_tag_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_tag_set.py` & `antimatter_api-1.0.9/test/test_tag_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_tag_set_span_tags_inner.py` & `antimatter_api-1.0.9/test/test_tag_set_span_tags_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_tag_summary.py` & `antimatter_api-1.0.9/test/test_tag_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_tag_summary_elided_tags_inner.py` & `antimatter_api-1.0.9/test/test_tag_summary_elided_tags_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_tag_summary_unique_tags_inner.py` & `antimatter_api-1.0.9/test/test_tag_summary_unique_tags_inner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_tag_type_field.py` & `antimatter_api-1.0.9/test/test_tag_type_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_unauthorized_error.py` & `antimatter_api-1.0.9/test/test_unauthorized_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_upsert_span_tags_request.py` & `antimatter_api-1.0.9/test/test_upsert_span_tags_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_verify_contact_response.py` & `antimatter_api-1.0.9/test/test_verify_contact_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_write_context_config_info.py` & `antimatter_api-1.0.9/test/test_write_context_config_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_write_context_config_info_required_hooks_inner.py` & `antimatter_api-1.0.9/test/test_write_context_config_info_required_hooks_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_write_context_details.py` & `antimatter_api-1.0.9/test/test_write_context_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_write_context_list.py` & `antimatter_api-1.0.9/test/test_write_context_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_write_context_regex_rule.py` & `antimatter_api-1.0.9/test/test_write_context_regex_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `antimatter_api-1.0.7/test/test_write_context_regex_tag.py` & `antimatter_api-1.0.9/test/test_write_context_regex_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.0.7
+    The version of the OpenAPI document: 1.0.9
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

