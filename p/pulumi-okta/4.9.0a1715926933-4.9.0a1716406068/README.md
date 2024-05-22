# Comparing `tmp/pulumi_okta-4.9.0a1715926933.tar.gz` & `tmp/pulumi_okta-4.9.0a1716406068.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.9.0a1715926933.tar", last modified: Fri May 17 06:33:07 2024, max compression
+gzip compressed data, was "pulumi_okta-4.9.0a1716406068.tar", last modified: Wed May 22 19:32:15 2024, max compression
```

## Comparing `pulumi_okta-4.9.0a1715926933.tar` & `pulumi_okta-4.9.0a1716406068.tar`

### file list

```diff
@@ -1,206 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.175207 pulumi_okta-4.9.0a1715926933/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-17 06:33:07.171207 pulumi_okta-4.9.0a1715926933/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.151207 pulumi_okta-4.9.0a1715926933/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20463 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.155207 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/access_policy_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    63791 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    36995 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    40308 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18000 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    32266 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)   146700 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    16081 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/oauth_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   137735 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    72763 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    59398 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    66043 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    91374 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23559 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    51344 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.159207 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23481 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    47855 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    47497 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    20026 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    23943 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    47422 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24328 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    12900 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.159207 pulumi_okta-4.9.0a1715926933/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    17334 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    18426 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.159207 pulumi_okta-4.9.0a1715926933/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.159207 pulumi_okta-4.9.0a1715926933/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/group/get_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    20849 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    47772 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.163207 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (127)    87393 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    83406 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    15030 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    72932 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.163207 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50207 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/customized_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/email_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/email_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/get_default_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/get_log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/get_org_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18617 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/index/preview_signin_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.167207 pulumi_okta-4.9.0a1715926933/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.167207 pulumi_okta-4.9.0a1715926933/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26287 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    36750 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    37142 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.171207 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22720 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_android.py
--rw-r--r--   0 runner    (1001) docker     (127)    48216 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_chromeos.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_ios.py
--rw-r--r--   0 runner    (1001) docker     (127)    56471 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_macos.py
--rw-r--r--   0 runner    (1001) docker     (127)    71871 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    69208 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    79597 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (127)    49623 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    69718 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    65321 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    71399 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    34771 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.171207 pulumi_okta-4.9.0a1715926933/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13898 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21186 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.171207 pulumi_okta-4.9.0a1715926933/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.171207 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    97718 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22897 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    52236 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:33:07.171207 pulumi_okta-4.9.0a1715926933/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-17 06:33:07.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-05-17 06:33:07.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:33:07.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 06:33:07.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 06:33:07.000000 pulumi_okta-4.9.0a1715926933/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-17 06:33:00.000000 pulumi_okta-4.9.0a1715926933/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:33:07.175207 pulumi_okta-4.9.0a1715926933/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.844307 pulumi_okta-4.9.0a1716406068/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-22 19:32:15.844307 pulumi_okta-4.9.0a1716406068/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.820307 pulumi_okta-4.9.0a1716406068/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (127)    21451 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70310 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.828307 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/access_policy_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63791 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36995 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40308 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18000 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32373 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146700 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16081 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/oauth_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137735 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72763 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59398 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66043 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91374 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23559 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51344 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.828307 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23481 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47855 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47497 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20026 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23943 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47422 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24328 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31125 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12900 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.832307 pulumi_okta-4.9.0a1716406068/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/customized_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17334 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15162 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18426 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.832307 pulumi_okta-4.9.0a1716406068/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_default_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_org_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.832307 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20849 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47772 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.832307 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87393 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83406 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15030 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72932 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.836307 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/link_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/log_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.836307 pulumi_okta-4.9.0a1716406068/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26287 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36750 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80451 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22720 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48216 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_chromeos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56471 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71871 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69208 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79597 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49623 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69718 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65321 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71399 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34771 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_rule_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/preview_signin_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13898 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21186 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97718 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22897 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52236 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:32:15.844307 pulumi_okta-4.9.0a1716406068/setup.cfg
```

### Comparing `pulumi_okta-4.9.0a1715926933/PKG-INFO` & `pulumi_okta-4.9.0a1716406068/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1715926933
+Version: 4.9.0a1716406068
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1715926933/README.md` & `pulumi_okta-4.9.0a1716406068/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/__init__.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,21 @@
 from .auth_server_claim_default import *
 from .auth_server_default import *
 from .authenticator import *
 from .behaviour import *
 from .brand import *
 from .captcha import *
 from .captcha_org_wide_settings import *
+from .customized_signin_page import *
 from .domain import *
 from .domain_certificate import *
 from .domain_verification import *
 from .email_customization import *
+from .email_domain import *
+from .email_domain_verification import *
 from .email_sender import *
 from .email_sender_verification import *
 from .event_hook import *
 from .event_hook_verification import *
 from .factor_totp import *
 from .get_app_group_assignments import *
 from .get_app_signon_policy import *
@@ -38,36 +41,42 @@
 from .get_auth_server_claim import *
 from .get_auth_server_claims import *
 from .get_authenticator import *
 from .get_behaviour import *
 from .get_behaviours import *
 from .get_brand import *
 from .get_brands import *
+from .get_default_signin_page import *
+from .get_domain import *
 from .get_email_customization import *
 from .get_email_customizations import *
 from .get_groups import *
+from .get_log_stream import *
 from .get_network_zone import *
+from .get_org_metadata import *
 from .get_role_subscription import *
 from .get_template import *
 from .get_templates import *
 from .get_theme import *
 from .get_themes import *
 from .get_trusted_origins import *
 from .get_user_security_questions import *
 from .group_memberships import *
 from .group_schema_property import *
 from .link_definition import *
 from .link_value import *
+from .log_stream import *
 from .org_configuration import *
 from .org_support import *
 from .policy_mfa_default import *
 from .policy_password_default import *
 from .policy_profile_enrollment import *
 from .policy_profile_enrollment_apps import *
 from .policy_rule_profile_enrollment import *
+from .preview_signin_page import *
 from .provider import *
 from .rate_limiting import *
 from .resource_set import *
 from .role_subscription import *
 from .security_notification_emails import *
 from .template_sms import *
 from .theme import *
@@ -90,16 +99,14 @@
     config = __config
     import pulumi_okta.factor as __factor
     factor = __factor
     import pulumi_okta.group as __group
     group = __group
     import pulumi_okta.idp as __idp
     idp = __idp
-    import pulumi_okta.index as __index
-    index = __index
     import pulumi_okta.inline as __inline
     inline = __inline
     import pulumi_okta.network as __network
     network = __network
     import pulumi_okta.policy as __policy
     policy = __policy
     import pulumi_okta.profile as __profile
@@ -111,67 +118,26 @@
 else:
     app = _utilities.lazy_import('pulumi_okta.app')
     auth = _utilities.lazy_import('pulumi_okta.auth')
     config = _utilities.lazy_import('pulumi_okta.config')
     factor = _utilities.lazy_import('pulumi_okta.factor')
     group = _utilities.lazy_import('pulumi_okta.group')
     idp = _utilities.lazy_import('pulumi_okta.idp')
-    index = _utilities.lazy_import('pulumi_okta.index')
     inline = _utilities.lazy_import('pulumi_okta.inline')
     network = _utilities.lazy_import('pulumi_okta.network')
     policy = _utilities.lazy_import('pulumi_okta.policy')
     profile = _utilities.lazy_import('pulumi_okta.profile')
     trustedorigin = _utilities.lazy_import('pulumi_okta.trustedorigin')
     user = _utilities.lazy_import('pulumi_okta.user')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "okta",
-  "mod": "Index/customizedSigninPage",
-  "fqn": "pulumi_okta.index",
-  "classes": {
-   "okta:Index/customizedSigninPage:CustomizedSigninPage": "CustomizedSigninPage"
-  }
- },
- {
-  "pkg": "okta",
-  "mod": "Index/emailDomain",
-  "fqn": "pulumi_okta.index",
-  "classes": {
-   "okta:Index/emailDomain:EmailDomain": "EmailDomain"
-  }
- },
- {
-  "pkg": "okta",
-  "mod": "Index/emailDomainVerification",
-  "fqn": "pulumi_okta.index",
-  "classes": {
-   "okta:Index/emailDomainVerification:EmailDomainVerification": "EmailDomainVerification"
-  }
- },
- {
-  "pkg": "okta",
-  "mod": "Index/logStream",
-  "fqn": "pulumi_okta.index",
-  "classes": {
-   "okta:Index/logStream:LogStream": "LogStream"
-  }
- },
- {
-  "pkg": "okta",
-  "mod": "Index/previewSigninPage",
-  "fqn": "pulumi_okta.index",
-  "classes": {
-   "okta:Index/previewSigninPage:PreviewSigninPage": "PreviewSigninPage"
-  }
- },
- {
-  "pkg": "okta",
   "mod": "app/accessPolicyAssignment",
   "fqn": "pulumi_okta.app",
   "classes": {
    "okta:app/accessPolicyAssignment:AccessPolicyAssignment": "AccessPolicyAssignment"
   }
  },
  {
@@ -532,14 +498,22 @@
   "fqn": "pulumi_okta",
   "classes": {
    "okta:index/captchaOrgWideSettings:CaptchaOrgWideSettings": "CaptchaOrgWideSettings"
   }
  },
  {
   "pkg": "okta",
+  "mod": "index/customizedSigninPage",
+  "fqn": "pulumi_okta",
+  "classes": {
+   "okta:index/customizedSigninPage:CustomizedSigninPage": "CustomizedSigninPage"
+  }
+ },
+ {
+  "pkg": "okta",
   "mod": "index/domain",
   "fqn": "pulumi_okta",
   "classes": {
    "okta:index/domain:Domain": "Domain"
   }
  },
  {
@@ -564,14 +538,30 @@
   "fqn": "pulumi_okta",
   "classes": {
    "okta:index/emailCustomization:EmailCustomization": "EmailCustomization"
   }
  },
  {
   "pkg": "okta",
+  "mod": "index/emailDomain",
+  "fqn": "pulumi_okta",
+  "classes": {
+   "okta:index/emailDomain:EmailDomain": "EmailDomain"
+  }
+ },
+ {
+  "pkg": "okta",
+  "mod": "index/emailDomainVerification",
+  "fqn": "pulumi_okta",
+  "classes": {
+   "okta:index/emailDomainVerification:EmailDomainVerification": "EmailDomainVerification"
+  }
+ },
+ {
+  "pkg": "okta",
   "mod": "index/emailSender",
   "fqn": "pulumi_okta",
   "classes": {
    "okta:index/emailSender:EmailSender": "EmailSender"
   }
  },
  {
@@ -636,14 +626,22 @@
   "fqn": "pulumi_okta",
   "classes": {
    "okta:index/linkValue:LinkValue": "LinkValue"
   }
  },
  {
   "pkg": "okta",
+  "mod": "index/logStream",
+  "fqn": "pulumi_okta",
+  "classes": {
+   "okta:index/logStream:LogStream": "LogStream"
+  }
+ },
+ {
+  "pkg": "okta",
   "mod": "index/orgConfiguration",
   "fqn": "pulumi_okta",
   "classes": {
    "okta:index/orgConfiguration:OrgConfiguration": "OrgConfiguration"
   }
  },
  {
@@ -692,14 +690,22 @@
   "fqn": "pulumi_okta",
   "classes": {
    "okta:index/policyRuleProfileEnrollment:PolicyRuleProfileEnrollment": "PolicyRuleProfileEnrollment"
   }
  },
  {
   "pkg": "okta",
+  "mod": "index/previewSigninPage",
+  "fqn": "pulumi_okta",
+  "classes": {
+   "okta:index/previewSigninPage:PreviewSigninPage": "PreviewSigninPage"
+  }
+ },
+ {
+  "pkg": "okta",
   "mod": "index/rateLimiting",
   "fqn": "pulumi_okta",
   "classes": {
    "okta:index/rateLimiting:RateLimiting": "RateLimiting"
   }
  },
  {
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/_inputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/_inputs.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,678 +3,470 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
 __all__ = [
-    'AppGroupAssignmentsGroupArgs',
-    'AppSignonPolicyRulePlatformIncludeArgs',
-    'AppUserSchemaPropertyArrayOneOfArgs',
-    'AppUserSchemaPropertyOneOfArgs',
-    'DomainDnsRecordArgs',
-    'EmailSenderDnsRecordArgs',
-    'EventHookHeaderArgs',
-    'GroupSchemaPropertyArrayOneOfArgs',
-    'GroupSchemaPropertyMasterOverridePriorityArgs',
-    'GroupSchemaPropertyOneOfArgs',
-    'PolicyRuleProfileEnrollmentProfileAttributeArgs',
-    'TemplateSmsTranslationArgs',
-    'UserSchemaPropertyArrayOneOfArgs',
-    'UserSchemaPropertyMasterOverridePriorityArgs',
-    'UserSchemaPropertyOneOfArgs',
+    'OAuthGroupsClaimArgs',
+    'OAuthJwkArgs',
+    'SamlAttributeStatementArgs',
+    'SamlKeyArgs',
 ]
 
 @pulumi.input_type
-class AppGroupAssignmentsGroupArgs:
+class OAuthGroupsClaimArgs:
     def __init__(__self__, *,
-                 id: pulumi.Input[str],
-                 profile: pulumi.Input[str],
-                 priority: Optional[pulumi.Input[int]] = None):
+                 name: pulumi.Input[str],
+                 type: pulumi.Input[str],
+                 value: pulumi.Input[str],
+                 filter_type: Optional[pulumi.Input[str]] = None,
+                 issuer_mode: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] id: ID of the group to assign.
-        :param pulumi.Input[str] profile: JSON document containing [application profile](https://developer.okta.com/docs/reference/api/apps/#profile-object)
-        :param pulumi.Input[int] priority: Priority of group assignment
+        :param pulumi.Input[str] name: Name of the claim that will be used in the token.
+        :param pulumi.Input[str] type: Groups claim type. Valid values: `"FILTER"`, `"EXPRESSION"`.
+        :param pulumi.Input[str] value: Value of the claim. Can be an Okta Expression Language statement that evaluates at the time the token is minted.
+        :param pulumi.Input[str] filter_type: Groups claim filter. Can only be set if type is `"FILTER"`. Valid values: `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`, `"REGEX"`.
+        :param pulumi.Input[str] issuer_mode: Issuer Mode is inherited from the Issuer Mode on the OAuth app itself.
         """
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "profile", profile)
-        if priority is not None:
-            pulumi.set(__self__, "priority", priority)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "type", type)
+        pulumi.set(__self__, "value", value)
+        if filter_type is not None:
+            pulumi.set(__self__, "filter_type", filter_type)
+        if issuer_mode is not None:
+            pulumi.set(__self__, "issuer_mode", issuer_mode)
 
     @property
     @pulumi.getter
-    def id(self) -> pulumi.Input[str]:
+    def name(self) -> pulumi.Input[str]:
         """
-        ID of the group to assign.
+        Name of the claim that will be used in the token.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "name")
 
-    @id.setter
-    def id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "id", value)
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def profile(self) -> pulumi.Input[str]:
+    def type(self) -> pulumi.Input[str]:
         """
-        JSON document containing [application profile](https://developer.okta.com/docs/reference/api/apps/#profile-object)
+        Groups claim type. Valid values: `"FILTER"`, `"EXPRESSION"`.
         """
-        return pulumi.get(self, "profile")
+        return pulumi.get(self, "type")
 
-    @profile.setter
-    def profile(self, value: pulumi.Input[str]):
-        pulumi.set(self, "profile", value)
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
-    def priority(self) -> Optional[pulumi.Input[int]]:
-        """
-        Priority of group assignment
-        """
-        return pulumi.get(self, "priority")
-
-    @priority.setter
-    def priority(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "priority", value)
-
-
-@pulumi.input_type
-class AppSignonPolicyRulePlatformIncludeArgs:
-    def __init__(__self__, *,
-                 os_expression: Optional[pulumi.Input[str]] = None,
-                 os_type: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] os_expression: Only available and required when using `os_type = "OTHER"`
-        :param pulumi.Input[str] os_type: One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`, `"CHROMEOS"`
-        :param pulumi.Input[str] type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
-        """
-        if os_expression is not None:
-            pulumi.set(__self__, "os_expression", os_expression)
-        if os_type is not None:
-            pulumi.set(__self__, "os_type", os_type)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="osExpression")
-    def os_expression(self) -> Optional[pulumi.Input[str]]:
+    def value(self) -> pulumi.Input[str]:
         """
-        Only available and required when using `os_type = "OTHER"`
+        Value of the claim. Can be an Okta Expression Language statement that evaluates at the time the token is minted.
         """
-        return pulumi.get(self, "os_expression")
+        return pulumi.get(self, "value")
 
-    @os_expression.setter
-    def os_expression(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "os_expression", value)
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
 
     @property
-    @pulumi.getter(name="osType")
-    def os_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="filterType")
+    def filter_type(self) -> Optional[pulumi.Input[str]]:
         """
-        One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`, `"CHROMEOS"`
+        Groups claim filter. Can only be set if type is `"FILTER"`. Valid values: `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`, `"REGEX"`.
         """
-        return pulumi.get(self, "os_type")
+        return pulumi.get(self, "filter_type")
 
-    @os_type.setter
-    def os_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "os_type", value)
+    @filter_type.setter
+    def filter_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "filter_type", value)
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="issuerMode")
+    def issuer_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
+        Issuer Mode is inherited from the Issuer Mode on the OAuth app itself.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "issuer_mode")
 
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    @issuer_mode.setter
+    def issuer_mode(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "issuer_mode", value)
 
 
 @pulumi.input_type
-class AppUserSchemaPropertyArrayOneOfArgs:
+class OAuthJwkArgs:
     def __init__(__self__, *,
-                 const: pulumi.Input[str],
-                 title: pulumi.Input[str]):
+                 kid: pulumi.Input[str],
+                 kty: pulumi.Input[str],
+                 e: Optional[pulumi.Input[str]] = None,
+                 n: Optional[pulumi.Input[str]] = None,
+                 x: Optional[pulumi.Input[str]] = None,
+                 y: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] const: value mapping to member of `array_enum`.
-        :param pulumi.Input[str] title: display name for the enum value.
+        :param pulumi.Input[str] kid: Key ID
+        :param pulumi.Input[str] kty: Key type
+        :param pulumi.Input[str] e: RSA Exponent
+        :param pulumi.Input[str] n: RSA Modulus
+        :param pulumi.Input[str] x: X coordinate of the elliptic curve point
+        :param pulumi.Input[str] y: Y coordinate of the elliptic curve point
         """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
+        pulumi.set(__self__, "kid", kid)
+        pulumi.set(__self__, "kty", kty)
+        if e is not None:
+            pulumi.set(__self__, "e", e)
+        if n is not None:
+            pulumi.set(__self__, "n", n)
+        if x is not None:
+            pulumi.set(__self__, "x", x)
+        if y is not None:
+            pulumi.set(__self__, "y", y)
 
     @property
     @pulumi.getter
-    def const(self) -> pulumi.Input[str]:
+    def kid(self) -> pulumi.Input[str]:
         """
-        value mapping to member of `array_enum`.
+        Key ID
         """
-        return pulumi.get(self, "const")
+        return pulumi.get(self, "kid")
 
-    @const.setter
-    def const(self, value: pulumi.Input[str]):
-        pulumi.set(self, "const", value)
+    @kid.setter
+    def kid(self, value: pulumi.Input[str]):
+        pulumi.set(self, "kid", value)
 
     @property
     @pulumi.getter
-    def title(self) -> pulumi.Input[str]:
+    def kty(self) -> pulumi.Input[str]:
         """
-        display name for the enum value.
+        Key type
         """
-        return pulumi.get(self, "title")
-
-    @title.setter
-    def title(self, value: pulumi.Input[str]):
-        pulumi.set(self, "title", value)
+        return pulumi.get(self, "kty")
 
-
-@pulumi.input_type
-class AppUserSchemaPropertyOneOfArgs:
-    def __init__(__self__, *,
-                 const: pulumi.Input[str],
-                 title: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] const: value mapping to member of `enum`.
-        :param pulumi.Input[str] title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
-
-    @property
-    @pulumi.getter
-    def const(self) -> pulumi.Input[str]:
-        """
-        value mapping to member of `enum`.
-        """
-        return pulumi.get(self, "const")
-
-    @const.setter
-    def const(self, value: pulumi.Input[str]):
-        pulumi.set(self, "const", value)
+    @kty.setter
+    def kty(self, value: pulumi.Input[str]):
+        pulumi.set(self, "kty", value)
 
     @property
     @pulumi.getter
-    def title(self) -> pulumi.Input[str]:
+    def e(self) -> Optional[pulumi.Input[str]]:
         """
-        display name for the enum value.
+        RSA Exponent
         """
-        return pulumi.get(self, "title")
-
-    @title.setter
-    def title(self, value: pulumi.Input[str]):
-        pulumi.set(self, "title", value)
+        return pulumi.get(self, "e")
 
-
-@pulumi.input_type
-class DomainDnsRecordArgs:
-    def __init__(__self__, *,
-                 expiration: Optional[pulumi.Input[str]] = None,
-                 fqdn: Optional[pulumi.Input[str]] = None,
-                 record_type: Optional[pulumi.Input[str]] = None,
-                 values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[str] expiration: TXT record expiration.
-        :param pulumi.Input[str] fqdn: DNS record name.
-        :param pulumi.Input[str] record_type: Record type can be TXT or CNAME.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] values: DNS verification value
-        """
-        if expiration is not None:
-            pulumi.set(__self__, "expiration", expiration)
-        if fqdn is not None:
-            pulumi.set(__self__, "fqdn", fqdn)
-        if record_type is not None:
-            pulumi.set(__self__, "record_type", record_type)
-        if values is not None:
-            pulumi.set(__self__, "values", values)
+    @e.setter
+    def e(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "e", value)
 
     @property
     @pulumi.getter
-    def expiration(self) -> Optional[pulumi.Input[str]]:
+    def n(self) -> Optional[pulumi.Input[str]]:
         """
-        TXT record expiration.
+        RSA Modulus
         """
-        return pulumi.get(self, "expiration")
+        return pulumi.get(self, "n")
 
-    @expiration.setter
-    def expiration(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "expiration", value)
+    @n.setter
+    def n(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "n", value)
 
     @property
     @pulumi.getter
-    def fqdn(self) -> Optional[pulumi.Input[str]]:
+    def x(self) -> Optional[pulumi.Input[str]]:
         """
-        DNS record name.
+        X coordinate of the elliptic curve point
         """
-        return pulumi.get(self, "fqdn")
+        return pulumi.get(self, "x")
 
-    @fqdn.setter
-    def fqdn(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "fqdn", value)
-
-    @property
-    @pulumi.getter(name="recordType")
-    def record_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        Record type can be TXT or CNAME.
-        """
-        return pulumi.get(self, "record_type")
-
-    @record_type.setter
-    def record_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "record_type", value)
+    @x.setter
+    def x(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "x", value)
 
     @property
     @pulumi.getter
-    def values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def y(self) -> Optional[pulumi.Input[str]]:
         """
-        DNS verification value
+        Y coordinate of the elliptic curve point
         """
-        return pulumi.get(self, "values")
+        return pulumi.get(self, "y")
 
-    @values.setter
-    def values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "values", value)
+    @y.setter
+    def y(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "y", value)
 
 
 @pulumi.input_type
-class EmailSenderDnsRecordArgs:
+class SamlAttributeStatementArgs:
     def __init__(__self__, *,
-                 fqdn: Optional[pulumi.Input[str]] = None,
-                 record_type: Optional[pulumi.Input[str]] = None,
-                 value: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] fqdn: DNS record name.
-        :param pulumi.Input[str] record_type: Record type can be TXT or CNAME.
-        :param pulumi.Input[str] value: DNS verification value
-        """
-        if fqdn is not None:
-            pulumi.set(__self__, "fqdn", fqdn)
-        if record_type is not None:
-            pulumi.set(__self__, "record_type", record_type)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
-
-    @property
-    @pulumi.getter
-    def fqdn(self) -> Optional[pulumi.Input[str]]:
-        """
-        DNS record name.
-        """
-        return pulumi.get(self, "fqdn")
-
-    @fqdn.setter
-    def fqdn(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "fqdn", value)
-
-    @property
-    @pulumi.getter(name="recordType")
-    def record_type(self) -> Optional[pulumi.Input[str]]:
+                 name: pulumi.Input[str],
+                 filter_type: Optional[pulumi.Input[str]] = None,
+                 filter_value: Optional[pulumi.Input[str]] = None,
+                 namespace: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
+                 values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Record type can be TXT or CNAME.
+        :param pulumi.Input[str] name: The name of the attribute statement.
+        :param pulumi.Input[str] filter_type: Type of group attribute filter. Valid values are: `"STARTS_WITH"`, `"EQUALS"`, `"CONTAINS"`, or `"REGEX"`
+        :param pulumi.Input[str] filter_value: Filter value to use.
+        :param pulumi.Input[str] namespace: The attribute namespace. It can be set to `"urn:oasis:names:tc:SAML:2.0:attrname-format:unspecified"`, `"urn:oasis:names:tc:SAML:2.0:attrname-format:uri"`, or `"urn:oasis:names:tc:SAML:2.0:attrname-format:basic"`.
+        :param pulumi.Input[str] type: The type of attribute statement value. Valid values are: `"EXPRESSION"` or `"GROUP"`. Default is `"EXPRESSION"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] values: Array of values to use.
         """
-        return pulumi.get(self, "record_type")
-
-    @record_type.setter
-    def record_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "record_type", value)
+        pulumi.set(__self__, "name", name)
+        if filter_type is not None:
+            pulumi.set(__self__, "filter_type", filter_type)
+        if filter_value is not None:
+            pulumi.set(__self__, "filter_value", filter_value)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+        if values is not None:
+            pulumi.set(__self__, "values", values)
 
     @property
     @pulumi.getter
-    def value(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> pulumi.Input[str]:
         """
-        DNS verification value
+        The name of the attribute statement.
         """
-        return pulumi.get(self, "value")
-
-    @value.setter
-    def value(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "value", value)
-
-
-@pulumi.input_type
-class EventHookHeaderArgs:
-    def __init__(__self__, *,
-                 key: Optional[pulumi.Input[str]] = None,
-                 value: Optional[pulumi.Input[str]] = None):
-        if key is not None:
-            pulumi.set(__self__, "key", key)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
-
-    @property
-    @pulumi.getter
-    def key(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "key")
-
-    @key.setter
-    def key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key", value)
-
-    @property
-    @pulumi.getter
-    def value(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "value")
-
-    @value.setter
-    def value(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "value", value)
-
+        return pulumi.get(self, "name")
 
-@pulumi.input_type
-class GroupSchemaPropertyArrayOneOfArgs:
-    def __init__(__self__, *,
-                 const: pulumi.Input[str],
-                 title: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] const: value mapping to member of `enum`.
-        :param pulumi.Input[str] title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def const(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="filterType")
+    def filter_type(self) -> Optional[pulumi.Input[str]]:
         """
-        value mapping to member of `enum`.
+        Type of group attribute filter. Valid values are: `"STARTS_WITH"`, `"EQUALS"`, `"CONTAINS"`, or `"REGEX"`
         """
-        return pulumi.get(self, "const")
+        return pulumi.get(self, "filter_type")
 
-    @const.setter
-    def const(self, value: pulumi.Input[str]):
-        pulumi.set(self, "const", value)
+    @filter_type.setter
+    def filter_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "filter_type", value)
 
     @property
-    @pulumi.getter
-    def title(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="filterValue")
+    def filter_value(self) -> Optional[pulumi.Input[str]]:
         """
-        display name for the enum value.
+        Filter value to use.
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "filter_value")
 
-    @title.setter
-    def title(self, value: pulumi.Input[str]):
-        pulumi.set(self, "title", value)
-
-
-@pulumi.input_type
-class GroupSchemaPropertyMasterOverridePriorityArgs:
-    def __init__(__self__, *,
-                 value: pulumi.Input[str],
-                 type: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] value: ID of profile source.
-        :param pulumi.Input[str] type: Type of profile source.
-        """
-        pulumi.set(__self__, "value", value)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
+    @filter_value.setter
+    def filter_value(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "filter_value", value)
 
     @property
     @pulumi.getter
-    def value(self) -> pulumi.Input[str]:
+    def namespace(self) -> Optional[pulumi.Input[str]]:
         """
-        ID of profile source.
+        The attribute namespace. It can be set to `"urn:oasis:names:tc:SAML:2.0:attrname-format:unspecified"`, `"urn:oasis:names:tc:SAML:2.0:attrname-format:uri"`, or `"urn:oasis:names:tc:SAML:2.0:attrname-format:basic"`.
         """
-        return pulumi.get(self, "value")
+        return pulumi.get(self, "namespace")
 
-    @value.setter
-    def value(self, value: pulumi.Input[str]):
-        pulumi.set(self, "value", value)
+    @namespace.setter
+    def namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Type of profile source.
+        The type of attribute statement value. Valid values are: `"EXPRESSION"` or `"GROUP"`. Default is `"EXPRESSION"`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
-
-@pulumi.input_type
-class GroupSchemaPropertyOneOfArgs:
-    def __init__(__self__, *,
-                 const: pulumi.Input[str],
-                 title: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] const: value mapping to member of `enum`.
-        :param pulumi.Input[str] title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
-
     @property
     @pulumi.getter
-    def const(self) -> pulumi.Input[str]:
-        """
-        value mapping to member of `enum`.
-        """
-        return pulumi.get(self, "const")
-
-    @const.setter
-    def const(self, value: pulumi.Input[str]):
-        pulumi.set(self, "const", value)
-
-    @property
-    @pulumi.getter
-    def title(self) -> pulumi.Input[str]:
+    def values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        display name for the enum value.
+        Array of values to use.
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "values")
 
-    @title.setter
-    def title(self, value: pulumi.Input[str]):
-        pulumi.set(self, "title", value)
+    @values.setter
+    def values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "values", value)
 
 
 @pulumi.input_type
-class PolicyRuleProfileEnrollmentProfileAttributeArgs:
+class SamlKeyArgs:
     def __init__(__self__, *,
-                 label: pulumi.Input[str],
-                 name: pulumi.Input[str],
-                 required: Optional[pulumi.Input[bool]] = None):
+                 created: Optional[pulumi.Input[str]] = None,
+                 e: Optional[pulumi.Input[str]] = None,
+                 expires_at: Optional[pulumi.Input[str]] = None,
+                 kid: Optional[pulumi.Input[str]] = None,
+                 kty: Optional[pulumi.Input[str]] = None,
+                 last_updated: Optional[pulumi.Input[str]] = None,
+                 n: Optional[pulumi.Input[str]] = None,
+                 use: Optional[pulumi.Input[str]] = None,
+                 x5cs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 x5t_s256: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] label: A display-friendly label for this property
-        :param pulumi.Input[str] name: The name of a User Profile property
-        :param pulumi.Input[bool] required: Indicates if this property is required for enrollment. Default is `false`.
+        :param pulumi.Input[str] created: Date created.
+        :param pulumi.Input[str] e: RSA exponent.
+        :param pulumi.Input[str] expires_at: Date the key expires.
+        :param pulumi.Input[str] kid: Key ID.
+        :param pulumi.Input[str] kty: Identifies the cryptographic algorithm family used with the key.
+        :param pulumi.Input[str] last_updated: Date the key was last updated.
+        :param pulumi.Input[str] n: RSA modulus.
+        :param pulumi.Input[str] use: Intended use of the public key.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] x5cs: X.509 certificate chain.
+        :param pulumi.Input[str] x5t_s256: X.509 certificate SHA-256 thumbprint.
         """
-        pulumi.set(__self__, "label", label)
-        pulumi.set(__self__, "name", name)
-        if required is not None:
-            pulumi.set(__self__, "required", required)
+        if created is not None:
+            pulumi.set(__self__, "created", created)
+        if e is not None:
+            pulumi.set(__self__, "e", e)
+        if expires_at is not None:
+            pulumi.set(__self__, "expires_at", expires_at)
+        if kid is not None:
+            pulumi.set(__self__, "kid", kid)
+        if kty is not None:
+            pulumi.set(__self__, "kty", kty)
+        if last_updated is not None:
+            pulumi.set(__self__, "last_updated", last_updated)
+        if n is not None:
+            pulumi.set(__self__, "n", n)
+        if use is not None:
+            pulumi.set(__self__, "use", use)
+        if x5cs is not None:
+            pulumi.set(__self__, "x5cs", x5cs)
+        if x5t_s256 is not None:
+            pulumi.set(__self__, "x5t_s256", x5t_s256)
 
     @property
     @pulumi.getter
-    def label(self) -> pulumi.Input[str]:
+    def created(self) -> Optional[pulumi.Input[str]]:
         """
-        A display-friendly label for this property
+        Date created.
         """
-        return pulumi.get(self, "label")
+        return pulumi.get(self, "created")
 
-    @label.setter
-    def label(self, value: pulumi.Input[str]):
-        pulumi.set(self, "label", value)
+    @created.setter
+    def created(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "created", value)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
+    def e(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of a User Profile property
+        RSA exponent.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "e")
 
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+    @e.setter
+    def e(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "e", value)
 
     @property
-    @pulumi.getter
-    def required(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="expiresAt")
+    def expires_at(self) -> Optional[pulumi.Input[str]]:
         """
-        Indicates if this property is required for enrollment. Default is `false`.
+        Date the key expires.
         """
-        return pulumi.get(self, "required")
-
-    @required.setter
-    def required(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "required", value)
+        return pulumi.get(self, "expires_at")
 
-
-@pulumi.input_type
-class TemplateSmsTranslationArgs:
-    def __init__(__self__, *,
-                 language: pulumi.Input[str],
-                 template: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] language: The language to map the template to.
-        :param pulumi.Input[str] template: The SMS message.
-        """
-        pulumi.set(__self__, "language", language)
-        pulumi.set(__self__, "template", template)
+    @expires_at.setter
+    def expires_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "expires_at", value)
 
     @property
     @pulumi.getter
-    def language(self) -> pulumi.Input[str]:
+    def kid(self) -> Optional[pulumi.Input[str]]:
         """
-        The language to map the template to.
+        Key ID.
         """
-        return pulumi.get(self, "language")
+        return pulumi.get(self, "kid")
 
-    @language.setter
-    def language(self, value: pulumi.Input[str]):
-        pulumi.set(self, "language", value)
+    @kid.setter
+    def kid(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "kid", value)
 
     @property
     @pulumi.getter
-    def template(self) -> pulumi.Input[str]:
+    def kty(self) -> Optional[pulumi.Input[str]]:
         """
-        The SMS message.
+        Identifies the cryptographic algorithm family used with the key.
         """
-        return pulumi.get(self, "template")
-
-    @template.setter
-    def template(self, value: pulumi.Input[str]):
-        pulumi.set(self, "template", value)
+        return pulumi.get(self, "kty")
 
-
-@pulumi.input_type
-class UserSchemaPropertyArrayOneOfArgs:
-    def __init__(__self__, *,
-                 const: pulumi.Input[str],
-                 title: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] const: value mapping to member of `enum`.
-        :param pulumi.Input[str] title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
+    @kty.setter
+    def kty(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "kty", value)
 
     @property
-    @pulumi.getter
-    def const(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="lastUpdated")
+    def last_updated(self) -> Optional[pulumi.Input[str]]:
         """
-        value mapping to member of `enum`.
+        Date the key was last updated.
         """
-        return pulumi.get(self, "const")
+        return pulumi.get(self, "last_updated")
 
-    @const.setter
-    def const(self, value: pulumi.Input[str]):
-        pulumi.set(self, "const", value)
+    @last_updated.setter
+    def last_updated(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "last_updated", value)
 
     @property
     @pulumi.getter
-    def title(self) -> pulumi.Input[str]:
+    def n(self) -> Optional[pulumi.Input[str]]:
         """
-        display name for the enum value.
+        RSA modulus.
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "n")
 
-    @title.setter
-    def title(self, value: pulumi.Input[str]):
-        pulumi.set(self, "title", value)
-
-
-@pulumi.input_type
-class UserSchemaPropertyMasterOverridePriorityArgs:
-    def __init__(__self__, *,
-                 value: pulumi.Input[str],
-                 type: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] value: ID of profile source.
-        :param pulumi.Input[str] type: Type of profile source.
-        """
-        pulumi.set(__self__, "value", value)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter
-    def value(self) -> pulumi.Input[str]:
-        """
-        ID of profile source.
-        """
-        return pulumi.get(self, "value")
-
-    @value.setter
-    def value(self, value: pulumi.Input[str]):
-        pulumi.set(self, "value", value)
+    @n.setter
+    def n(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "n", value)
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    def use(self) -> Optional[pulumi.Input[str]]:
         """
-        Type of profile source.
+        Intended use of the public key.
         """
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+        return pulumi.get(self, "use")
 
-
-@pulumi.input_type
-class UserSchemaPropertyOneOfArgs:
-    def __init__(__self__, *,
-                 const: pulumi.Input[str],
-                 title: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] const: value mapping to member of `enum`.
-        :param pulumi.Input[str] title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
+    @use.setter
+    def use(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "use", value)
 
     @property
     @pulumi.getter
-    def const(self) -> pulumi.Input[str]:
+    def x5cs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        value mapping to member of `enum`.
+        X.509 certificate chain.
         """
-        return pulumi.get(self, "const")
+        return pulumi.get(self, "x5cs")
 
-    @const.setter
-    def const(self, value: pulumi.Input[str]):
-        pulumi.set(self, "const", value)
+    @x5cs.setter
+    def x5cs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "x5cs", value)
 
     @property
-    @pulumi.getter
-    def title(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="x5tS256")
+    def x5t_s256(self) -> Optional[pulumi.Input[str]]:
         """
-        display name for the enum value.
+        X.509 certificate SHA-256 thumbprint.
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "x5t_s256")
 
-    @title.setter
-    def title(self, value: pulumi.Input[str]):
-        pulumi.set(self, "title", value)
+    @x5t_s256.setter
+    def x5t_s256(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "x5t_s256", value)
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/_utilities.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/__init__.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/_inputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,467 +6,409 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'OAuthGroupsClaimArgs',
-    'OAuthJwkArgs',
-    'SamlAttributeStatementArgs',
-    'SamlKeyArgs',
+    'RuleIdpDiscoveryAppExcludeArgs',
+    'RuleIdpDiscoveryAppIncludeArgs',
+    'RuleIdpDiscoveryPlatformIncludeArgs',
+    'RuleIdpDiscoveryUserIdentifierPatternArgs',
+    'RuleMfaAppExcludeArgs',
+    'RuleMfaAppIncludeArgs',
+    'RuleSignonFactorSequenceArgs',
+    'RuleSignonFactorSequenceSecondaryCriteriaArgs',
 ]
 
 @pulumi.input_type
-class OAuthGroupsClaimArgs:
+class RuleIdpDiscoveryAppExcludeArgs:
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
                  type: pulumi.Input[str],
-                 value: pulumi.Input[str],
-                 filter_type: Optional[pulumi.Input[str]] = None,
-                 issuer_mode: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: Name of the claim that will be used in the token.
-        :param pulumi.Input[str] type: Groups claim type. Valid values: `"FILTER"`, `"EXPRESSION"`.
-        :param pulumi.Input[str] value: Value of the claim. Can be an Okta Expression Language statement that evaluates at the time the token is minted.
-        :param pulumi.Input[str] filter_type: Groups claim filter. Can only be set if type is `"FILTER"`. Valid values: `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`, `"REGEX"`.
-        :param pulumi.Input[str] issuer_mode: Issuer Mode is inherited from the Issuer Mode on the OAuth app itself.
+                 id: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
         """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "type", type)
-        pulumi.set(__self__, "value", value)
-        if filter_type is not None:
-            pulumi.set(__self__, "filter_type", filter_type)
-        if issuer_mode is not None:
-            pulumi.set(__self__, "issuer_mode", issuer_mode)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
+        :param pulumi.Input[str] id: ID of the Rule.
+        :param pulumi.Input[str] name: Policy rule name.
         """
-        Name of the claim that will be used in the token.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+        pulumi.set(__self__, "type", type)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Groups claim type. Valid values: `"FILTER"`, `"EXPRESSION"`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
-    def value(self) -> pulumi.Input[str]:
+    def id(self) -> Optional[pulumi.Input[str]]:
         """
-        Value of the claim. Can be an Okta Expression Language statement that evaluates at the time the token is minted.
+        ID of the Rule.
         """
-        return pulumi.get(self, "value")
+        return pulumi.get(self, "id")
 
-    @value.setter
-    def value(self, value: pulumi.Input[str]):
-        pulumi.set(self, "value", value)
+    @id.setter
+    def id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "id", value)
 
     @property
-    @pulumi.getter(name="filterType")
-    def filter_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        Groups claim filter. Can only be set if type is `"FILTER"`. Valid values: `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`, `"REGEX"`.
-        """
-        return pulumi.get(self, "filter_type")
-
-    @filter_type.setter
-    def filter_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "filter_type", value)
-
-    @property
-    @pulumi.getter(name="issuerMode")
-    def issuer_mode(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Issuer Mode is inherited from the Issuer Mode on the OAuth app itself.
+        Policy rule name.
         """
-        return pulumi.get(self, "issuer_mode")
+        return pulumi.get(self, "name")
 
-    @issuer_mode.setter
-    def issuer_mode(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "issuer_mode", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class OAuthJwkArgs:
+class RuleIdpDiscoveryAppIncludeArgs:
     def __init__(__self__, *,
-                 kid: pulumi.Input[str],
-                 kty: pulumi.Input[str],
-                 e: Optional[pulumi.Input[str]] = None,
-                 n: Optional[pulumi.Input[str]] = None,
-                 x: Optional[pulumi.Input[str]] = None,
-                 y: Optional[pulumi.Input[str]] = None):
+                 type: pulumi.Input[str],
+                 id: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] kid: Key ID
-        :param pulumi.Input[str] kty: Key type
-        :param pulumi.Input[str] e: RSA Exponent
-        :param pulumi.Input[str] n: RSA Modulus
-        :param pulumi.Input[str] x: X coordinate of the elliptic curve point
-        :param pulumi.Input[str] y: Y coordinate of the elliptic curve point
+        :param pulumi.Input[str] type: One of: `"APP"`, `"APP_TYPE"`
+        :param pulumi.Input[str] id: Use if `type` is `"APP"` to indicate the application id to include.
+        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         """
-        pulumi.set(__self__, "kid", kid)
-        pulumi.set(__self__, "kty", kty)
-        if e is not None:
-            pulumi.set(__self__, "e", e)
-        if n is not None:
-            pulumi.set(__self__, "n", n)
-        if x is not None:
-            pulumi.set(__self__, "x", x)
-        if y is not None:
-            pulumi.set(__self__, "y", y)
+        pulumi.set(__self__, "type", type)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def kid(self) -> pulumi.Input[str]:
+    def type(self) -> pulumi.Input[str]:
         """
-        Key ID
+        One of: `"APP"`, `"APP_TYPE"`
         """
-        return pulumi.get(self, "kid")
+        return pulumi.get(self, "type")
 
-    @kid.setter
-    def kid(self, value: pulumi.Input[str]):
-        pulumi.set(self, "kid", value)
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
-    def kty(self) -> pulumi.Input[str]:
+    def id(self) -> Optional[pulumi.Input[str]]:
         """
-        Key type
+        Use if `type` is `"APP"` to indicate the application id to include.
         """
-        return pulumi.get(self, "kty")
+        return pulumi.get(self, "id")
 
-    @kty.setter
-    def kty(self, value: pulumi.Input[str]):
-        pulumi.set(self, "kty", value)
+    @id.setter
+    def id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
-    def e(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        RSA Exponent
+        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         """
-        return pulumi.get(self, "e")
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
-    @e.setter
-    def e(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "e", value)
+
+@pulumi.input_type
+class RuleIdpDiscoveryPlatformIncludeArgs:
+    def __init__(__self__, *,
+                 os_expression: Optional[pulumi.Input[str]] = None,
+                 os_type: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] os_expression: Only available when using `os_type = "OTHER"`
+        :param pulumi.Input[str] os_type: One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`
+        :param pulumi.Input[str] type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
+        """
+        if os_expression is not None:
+            pulumi.set(__self__, "os_expression", os_expression)
+        if os_type is not None:
+            pulumi.set(__self__, "os_type", os_type)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
 
     @property
-    @pulumi.getter
-    def n(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="osExpression")
+    def os_expression(self) -> Optional[pulumi.Input[str]]:
         """
-        RSA Modulus
+        Only available when using `os_type = "OTHER"`
         """
-        return pulumi.get(self, "n")
+        return pulumi.get(self, "os_expression")
 
-    @n.setter
-    def n(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "n", value)
+    @os_expression.setter
+    def os_expression(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "os_expression", value)
 
     @property
-    @pulumi.getter
-    def x(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="osType")
+    def os_type(self) -> Optional[pulumi.Input[str]]:
         """
-        X coordinate of the elliptic curve point
+        One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`
         """
-        return pulumi.get(self, "x")
+        return pulumi.get(self, "os_type")
 
-    @x.setter
-    def x(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "x", value)
+    @os_type.setter
+    def os_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "os_type", value)
 
     @property
     @pulumi.getter
-    def y(self) -> Optional[pulumi.Input[str]]:
+    def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Y coordinate of the elliptic curve point
+        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
         """
-        return pulumi.get(self, "y")
+        return pulumi.get(self, "type")
 
-    @y.setter
-    def y(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "y", value)
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
-class SamlAttributeStatementArgs:
+class RuleIdpDiscoveryUserIdentifierPatternArgs:
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 filter_type: Optional[pulumi.Input[str]] = None,
-                 filter_value: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[str] name: The name of the attribute statement.
-        :param pulumi.Input[str] filter_type: Type of group attribute filter. Valid values are: `"STARTS_WITH"`, `"EQUALS"`, `"CONTAINS"`, or `"REGEX"`
-        :param pulumi.Input[str] filter_value: Filter value to use.
-        :param pulumi.Input[str] namespace: The attribute namespace. It can be set to `"urn:oasis:names:tc:SAML:2.0:attrname-format:unspecified"`, `"urn:oasis:names:tc:SAML:2.0:attrname-format:uri"`, or `"urn:oasis:names:tc:SAML:2.0:attrname-format:basic"`.
-        :param pulumi.Input[str] type: The type of attribute statement value. Valid values are: `"EXPRESSION"` or `"GROUP"`. Default is `"EXPRESSION"`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] values: Array of values to use.
-        """
-        pulumi.set(__self__, "name", name)
-        if filter_type is not None:
-            pulumi.set(__self__, "filter_type", filter_type)
-        if filter_value is not None:
-            pulumi.set(__self__, "filter_value", filter_value)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-        if values is not None:
-            pulumi.set(__self__, "values", values)
+                 match_type: Optional[pulumi.Input[str]] = None,
+                 value: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] match_type: The kind of pattern. For regex, use `"EXPRESSION"`. For simple string matches, use one of the following: `"SUFFIX"`, `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`
+        :param pulumi.Input[str] value: The regex or simple match string to match against.
+        """
+        if match_type is not None:
+            pulumi.set(__self__, "match_type", match_type)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="matchType")
+    def match_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the attribute statement.
+        The kind of pattern. For regex, use `"EXPRESSION"`. For simple string matches, use one of the following: `"SUFFIX"`, `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "match_type")
 
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+    @match_type.setter
+    def match_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "match_type", value)
 
     @property
-    @pulumi.getter(name="filterType")
-    def filter_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def value(self) -> Optional[pulumi.Input[str]]:
         """
-        Type of group attribute filter. Valid values are: `"STARTS_WITH"`, `"EQUALS"`, `"CONTAINS"`, or `"REGEX"`
+        The regex or simple match string to match against.
         """
-        return pulumi.get(self, "filter_type")
+        return pulumi.get(self, "value")
 
-    @filter_type.setter
-    def filter_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "filter_type", value)
+    @value.setter
+    def value(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "value", value)
 
-    @property
-    @pulumi.getter(name="filterValue")
-    def filter_value(self) -> Optional[pulumi.Input[str]]:
+
+@pulumi.input_type
+class RuleMfaAppExcludeArgs:
+    def __init__(__self__, *,
+                 type: pulumi.Input[str],
+                 id: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
         """
-        Filter value to use.
+        :param pulumi.Input[str] id: ID of the Rule.
+        :param pulumi.Input[str] name: Policy Rule Name.
         """
-        return pulumi.get(self, "filter_value")
-
-    @filter_value.setter
-    def filter_value(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "filter_value", value)
+        pulumi.set(__self__, "type", type)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        The attribute namespace. It can be set to `"urn:oasis:names:tc:SAML:2.0:attrname-format:unspecified"`, `"urn:oasis:names:tc:SAML:2.0:attrname-format:uri"`, or `"urn:oasis:names:tc:SAML:2.0:attrname-format:basic"`.
-        """
-        return pulumi.get(self, "namespace")
+    def type(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "type")
 
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    def id(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of attribute statement value. Valid values are: `"EXPRESSION"` or `"GROUP"`. Default is `"EXPRESSION"`.
+        ID of the Rule.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "id")
 
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    @id.setter
+    def id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
-    def values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Array of values to use.
+        Policy Rule Name.
         """
-        return pulumi.get(self, "values")
+        return pulumi.get(self, "name")
 
-    @values.setter
-    def values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "values", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class SamlKeyArgs:
+class RuleMfaAppIncludeArgs:
     def __init__(__self__, *,
-                 created: Optional[pulumi.Input[str]] = None,
-                 e: Optional[pulumi.Input[str]] = None,
-                 expires_at: Optional[pulumi.Input[str]] = None,
-                 kid: Optional[pulumi.Input[str]] = None,
-                 kty: Optional[pulumi.Input[str]] = None,
-                 last_updated: Optional[pulumi.Input[str]] = None,
-                 n: Optional[pulumi.Input[str]] = None,
-                 use: Optional[pulumi.Input[str]] = None,
-                 x5cs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 x5t_s256: Optional[pulumi.Input[str]] = None):
+                 type: pulumi.Input[str],
+                 id: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] created: Date created.
-        :param pulumi.Input[str] e: RSA exponent.
-        :param pulumi.Input[str] expires_at: Date the key expires.
-        :param pulumi.Input[str] kid: Key ID.
-        :param pulumi.Input[str] kty: Identifies the cryptographic algorithm family used with the key.
-        :param pulumi.Input[str] last_updated: Date the key was last updated.
-        :param pulumi.Input[str] n: RSA modulus.
-        :param pulumi.Input[str] use: Intended use of the public key.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] x5cs: X.509 certificate chain.
-        :param pulumi.Input[str] x5t_s256: X.509 certificate SHA-256 thumbprint.
+        :param pulumi.Input[str] type: One of: `"APP"`, `"APP_TYPE"`
+        :param pulumi.Input[str] id: Use if `type` is `"APP"` to indicate the application id to include.
+        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         """
-        if created is not None:
-            pulumi.set(__self__, "created", created)
-        if e is not None:
-            pulumi.set(__self__, "e", e)
-        if expires_at is not None:
-            pulumi.set(__self__, "expires_at", expires_at)
-        if kid is not None:
-            pulumi.set(__self__, "kid", kid)
-        if kty is not None:
-            pulumi.set(__self__, "kty", kty)
-        if last_updated is not None:
-            pulumi.set(__self__, "last_updated", last_updated)
-        if n is not None:
-            pulumi.set(__self__, "n", n)
-        if use is not None:
-            pulumi.set(__self__, "use", use)
-        if x5cs is not None:
-            pulumi.set(__self__, "x5cs", x5cs)
-        if x5t_s256 is not None:
-            pulumi.set(__self__, "x5t_s256", x5t_s256)
+        pulumi.set(__self__, "type", type)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def created(self) -> Optional[pulumi.Input[str]]:
+    def type(self) -> pulumi.Input[str]:
         """
-        Date created.
+        One of: `"APP"`, `"APP_TYPE"`
         """
-        return pulumi.get(self, "created")
+        return pulumi.get(self, "type")
 
-    @created.setter
-    def created(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "created", value)
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
-    def e(self) -> Optional[pulumi.Input[str]]:
+    def id(self) -> Optional[pulumi.Input[str]]:
         """
-        RSA exponent.
+        Use if `type` is `"APP"` to indicate the application id to include.
         """
-        return pulumi.get(self, "e")
+        return pulumi.get(self, "id")
 
-    @e.setter
-    def e(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "e", value)
+    @id.setter
+    def id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "id", value)
 
     @property
-    @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Date the key expires.
+        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         """
-        return pulumi.get(self, "expires_at")
+        return pulumi.get(self, "name")
 
-    @expires_at.setter
-    def expires_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "expires_at", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
-    @property
-    @pulumi.getter
-    def kid(self) -> Optional[pulumi.Input[str]]:
+
+@pulumi.input_type
+class RuleSignonFactorSequenceArgs:
+    def __init__(__self__, *,
+                 primary_criteria_factor_type: pulumi.Input[str],
+                 primary_criteria_provider: pulumi.Input[str],
+                 secondary_criterias: Optional[pulumi.Input[Sequence[pulumi.Input['RuleSignonFactorSequenceSecondaryCriteriaArgs']]]] = None):
         """
-        Key ID.
+        :param pulumi.Input[str] primary_criteria_factor_type: Primary factor type of the auth section.
+        :param pulumi.Input[str] primary_criteria_provider: Primary provider of the auth section.
+        :param pulumi.Input[Sequence[pulumi.Input['RuleSignonFactorSequenceSecondaryCriteriaArgs']]] secondary_criterias: Additional authentication steps.
         """
-        return pulumi.get(self, "kid")
-
-    @kid.setter
-    def kid(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "kid", value)
+        pulumi.set(__self__, "primary_criteria_factor_type", primary_criteria_factor_type)
+        pulumi.set(__self__, "primary_criteria_provider", primary_criteria_provider)
+        if secondary_criterias is not None:
+            pulumi.set(__self__, "secondary_criterias", secondary_criterias)
 
     @property
-    @pulumi.getter
-    def kty(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="primaryCriteriaFactorType")
+    def primary_criteria_factor_type(self) -> pulumi.Input[str]:
         """
-        Identifies the cryptographic algorithm family used with the key.
+        Primary factor type of the auth section.
         """
-        return pulumi.get(self, "kty")
+        return pulumi.get(self, "primary_criteria_factor_type")
 
-    @kty.setter
-    def kty(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "kty", value)
+    @primary_criteria_factor_type.setter
+    def primary_criteria_factor_type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "primary_criteria_factor_type", value)
 
     @property
-    @pulumi.getter(name="lastUpdated")
-    def last_updated(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="primaryCriteriaProvider")
+    def primary_criteria_provider(self) -> pulumi.Input[str]:
         """
-        Date the key was last updated.
+        Primary provider of the auth section.
         """
-        return pulumi.get(self, "last_updated")
+        return pulumi.get(self, "primary_criteria_provider")
 
-    @last_updated.setter
-    def last_updated(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "last_updated", value)
+    @primary_criteria_provider.setter
+    def primary_criteria_provider(self, value: pulumi.Input[str]):
+        pulumi.set(self, "primary_criteria_provider", value)
 
     @property
-    @pulumi.getter
-    def n(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="secondaryCriterias")
+    def secondary_criterias(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleSignonFactorSequenceSecondaryCriteriaArgs']]]]:
         """
-        RSA modulus.
+        Additional authentication steps.
         """
-        return pulumi.get(self, "n")
+        return pulumi.get(self, "secondary_criterias")
 
-    @n.setter
-    def n(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "n", value)
+    @secondary_criterias.setter
+    def secondary_criterias(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleSignonFactorSequenceSecondaryCriteriaArgs']]]]):
+        pulumi.set(self, "secondary_criterias", value)
 
-    @property
-    @pulumi.getter
-    def use(self) -> Optional[pulumi.Input[str]]:
+
+@pulumi.input_type
+class RuleSignonFactorSequenceSecondaryCriteriaArgs:
+    def __init__(__self__, *,
+                 factor_type: pulumi.Input[str],
+                 provider: pulumi.Input[str]):
         """
-        Intended use of the public key.
+        :param pulumi.Input[str] factor_type: Type of a Factor
+        :param pulumi.Input[str] provider: Factor provider
         """
-        return pulumi.get(self, "use")
-
-    @use.setter
-    def use(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "use", value)
+        pulumi.set(__self__, "factor_type", factor_type)
+        pulumi.set(__self__, "provider", provider)
 
     @property
-    @pulumi.getter
-    def x5cs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="factorType")
+    def factor_type(self) -> pulumi.Input[str]:
         """
-        X.509 certificate chain.
+        Type of a Factor
         """
-        return pulumi.get(self, "x5cs")
+        return pulumi.get(self, "factor_type")
 
-    @x5cs.setter
-    def x5cs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "x5cs", value)
+    @factor_type.setter
+    def factor_type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "factor_type", value)
 
     @property
-    @pulumi.getter(name="x5tS256")
-    def x5t_s256(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def provider(self) -> pulumi.Input[str]:
         """
-        X.509 certificate SHA-256 thumbprint.
+        Factor provider
         """
-        return pulumi.get(self, "x5t_s256")
+        return pulumi.get(self, "provider")
 
-    @x5t_s256.setter
-    def x5t_s256(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "x5t_s256", value)
+    @provider.setter
+    def provider(self, value: pulumi.Input[str]):
+        pulumi.set(self, "provider", value)
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/access_policy_assignment.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/access_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/get_app.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_oauth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_saml.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,15 @@
         return pulumi.get(self, "features")
 
     @property
     @pulumi.getter
     def groups(self) -> Sequence[str]:
         """
         List of groups IDs assigned to the application.
+        - `DEPRECATED`: Please replace all usage of this field with the data source `AppGroupAssignments`.
         """
         warnings.warn("""The `groups` field is now deprecated for the data source `app.Saml`, please replace all uses of this with: `AppGroupAssignments`""", DeprecationWarning)
         pulumi.log.warn("""groups is deprecated: The `groups` field is now deprecated for the data source `app.Saml`, please replace all uses of this with: `AppGroupAssignments`""")
 
         return pulumi.get(self, "groups")
 
     @property
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/oauth_role_assignment.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/oauth_role_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/outputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/saml.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/swa.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/three_field.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app/user.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_oauth_api_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_signon_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth_server_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/authenticator.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/behaviour.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/brand.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/brand.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
                  locale: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  remove_powered_by_okta: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Brand resource.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
         :param pulumi.Input[str] brand_id: (Read-only) Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
+               - `DEPRECATED`: Please stop using this field as it has become noop.
         :param pulumi.Input[str] custom_privacy_policy_url: Custom privacy policy URL
         :param pulumi.Input[str] default_app_app_instance_id: Default app app instance id
         :param pulumi.Input[str] default_app_app_link_name: Default app app link name
         :param pulumi.Input[str] default_app_classic_application_uri: Default app classic application uri
         :param pulumi.Input[str] locale: The language specified as an IETF BCP 47 language tag
         :param pulumi.Input[str] name: Name of the brand
         :param pulumi.Input[bool] remove_powered_by_okta: Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
@@ -70,14 +71,15 @@
         pulumi.set(self, "agree_to_custom_privacy_policy", value)
 
     @property
     @pulumi.getter(name="brandId")
     def brand_id(self) -> Optional[pulumi.Input[str]]:
         """
         (Read-only) Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
+        - `DEPRECATED`: Please stop using this field as it has become noop.
         """
         warnings.warn("""Okta has fully support brand creation, this attribute is a no op and will be removed""", DeprecationWarning)
         pulumi.log.warn("""brand_id is deprecated: Okta has fully support brand creation, this attribute is a no op and will be removed""")
 
         return pulumi.get(self, "brand_id")
 
     @brand_id.setter
@@ -184,14 +186,15 @@
                  locale: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  remove_powered_by_okta: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Brand resources.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
         :param pulumi.Input[str] brand_id: (Read-only) Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
+               - `DEPRECATED`: Please stop using this field as it has become noop.
         :param pulumi.Input[str] custom_privacy_policy_url: Custom privacy policy URL
         :param pulumi.Input[str] default_app_app_instance_id: Default app app instance id
         :param pulumi.Input[str] default_app_app_link_name: Default app app link name
         :param pulumi.Input[str] default_app_classic_application_uri: Default app classic application uri
         :param pulumi.Input[str] email_domain_id: (Read-only) Email Domain ID tied to this brand
         :param pulumi.Input[bool] is_default: (Read-only) Is this the default brand
         :param pulumi.Input[str] links: (Read-only) Link relations for this object - JSON HAL - Discoverable resources related to the brand
@@ -240,14 +243,15 @@
         pulumi.set(self, "agree_to_custom_privacy_policy", value)
 
     @property
     @pulumi.getter(name="brandId")
     def brand_id(self) -> Optional[pulumi.Input[str]]:
         """
         (Read-only) Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
+        - `DEPRECATED`: Please stop using this field as it has become noop.
         """
         warnings.warn("""Okta has fully support brand creation, this attribute is a no op and will be removed""", DeprecationWarning)
         pulumi.log.warn("""brand_id is deprecated: Okta has fully support brand creation, this attribute is a no op and will be removed""")
 
         return pulumi.get(self, "brand_id")
 
     @brand_id.setter
@@ -402,14 +406,15 @@
         $ pulumi import okta:index/brand:Brand example &#60;brand id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
         :param pulumi.Input[str] brand_id: (Read-only) Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
+               - `DEPRECATED`: Please stop using this field as it has become noop.
         :param pulumi.Input[str] custom_privacy_policy_url: Custom privacy policy URL
         :param pulumi.Input[str] default_app_app_instance_id: Default app app instance id
         :param pulumi.Input[str] default_app_app_link_name: Default app app link name
         :param pulumi.Input[str] default_app_classic_application_uri: Default app classic application uri
         :param pulumi.Input[str] locale: The language specified as an IETF BCP 47 language tag
         :param pulumi.Input[str] name: Name of the brand
         :param pulumi.Input[bool] remove_powered_by_okta: Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
@@ -504,14 +509,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
         :param pulumi.Input[str] brand_id: (Read-only) Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
+               - `DEPRECATED`: Please stop using this field as it has become noop.
         :param pulumi.Input[str] custom_privacy_policy_url: Custom privacy policy URL
         :param pulumi.Input[str] default_app_app_instance_id: Default app app instance id
         :param pulumi.Input[str] default_app_app_link_name: Default app app link name
         :param pulumi.Input[str] default_app_classic_application_uri: Default app classic application uri
         :param pulumi.Input[str] email_domain_id: (Read-only) Email Domain ID tied to this brand
         :param pulumi.Input[bool] is_default: (Read-only) Is this the default brand
         :param pulumi.Input[str] links: (Read-only) Link relations for this object - JSON HAL - Discoverable resources related to the brand
@@ -546,14 +552,15 @@
         return pulumi.get(self, "agree_to_custom_privacy_policy")
 
     @property
     @pulumi.getter(name="brandId")
     def brand_id(self) -> pulumi.Output[str]:
         """
         (Read-only) Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
+        - `DEPRECATED`: Please stop using this field as it has become noop.
         """
         warnings.warn("""Okta has fully support brand creation, this attribute is a no op and will be removed""", DeprecationWarning)
         pulumi.log.warn("""brand_id is deprecated: Okta has fully support brand creation, this attribute is a no op and will be removed""")
 
         return pulumi.get(self, "brand_id")
 
     @property
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/captcha.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/config/__init__.pyi` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/config/vars.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/domain.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/domain_verification.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/email_customization.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/email_sender.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_sender.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  from_address: Optional[pulumi.Input[str]] = None,
                  from_name: Optional[pulumi.Input[str]] = None,
                  subdomain: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        > **DEPRECATED** use `Index.EmailDomain` instead.
+        > **DEPRECATED** use `EmailDomain` instead.
 
         This resource allows you to create and configure a custom email sender.
 
         ## Example Usage
 
         ```python
         import pulumi
@@ -197,15 +197,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: EmailSenderArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        > **DEPRECATED** use `Index.EmailDomain` instead.
+        > **DEPRECATED** use `EmailDomain` instead.
 
         This resource allows you to create and configure a custom email sender.
 
         ## Example Usage
 
         ```python
         import pulumi
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_sender_verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  sender_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        > **DEPRECATED** use `Index.EmailDomainVerification` instead.
+        > **DEPRECATED** use `EmailDomainVerification` instead.
 
         Verifies the email sender. The resource won't be created if the email sender could not be verified.
 
         ## Example Usage
 
         ```python
         import pulumi
@@ -94,15 +94,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: EmailSenderVerificationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        > **DEPRECATED** use `Index.EmailDomainVerification` instead.
+        > **DEPRECATED** use `EmailDomainVerification` instead.
 
         Verifies the email sender. The resource won't be created if the email sender could not be verified.
 
         ## Example Usage
 
         ```python
         import pulumi
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/event_hook.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/event_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/factor/factor.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/factor_totp.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_user_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_auth_server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_auth_server_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_behaviours.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_brand.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_brands.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_brands.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_groups.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_template.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_templates.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_theme.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_themes.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_trusted_origins.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_user_security_questions.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_everyone_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/group/get_group.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/group/get_rule.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/group/group.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/group/role.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/group/rule.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/group_memberships.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/saml.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/idp/social.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/_inputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/_inputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,31 +3,228 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
 __all__ = [
+    'AppGroupAssignmentsGroupArgs',
+    'AppSignonPolicyRulePlatformIncludeArgs',
+    'AppUserSchemaPropertyArrayOneOfArgs',
+    'AppUserSchemaPropertyOneOfArgs',
     'CustomizedSigninPageContentSecurityPolicySettingArgs',
     'CustomizedSigninPageWidgetCustomizationsArgs',
+    'DomainDnsRecordArgs',
     'EmailDomainDnsValidationRecordArgs',
+    'EmailSenderDnsRecordArgs',
+    'EventHookHeaderArgs',
+    'GroupSchemaPropertyArrayOneOfArgs',
+    'GroupSchemaPropertyMasterOverridePriorityArgs',
+    'GroupSchemaPropertyOneOfArgs',
     'LogStreamSettingsArgs',
+    'PolicyRuleProfileEnrollmentProfileAttributeArgs',
     'PreviewSigninPageContentSecurityPolicySettingArgs',
     'PreviewSigninPageWidgetCustomizationsArgs',
+    'TemplateSmsTranslationArgs',
+    'UserSchemaPropertyArrayOneOfArgs',
+    'UserSchemaPropertyMasterOverridePriorityArgs',
+    'UserSchemaPropertyOneOfArgs',
     'GetDefaultSigninPageContentSecurityPolicySettingArgs',
     'GetDefaultSigninPageWidgetCustomizationsArgs',
     'GetLogStreamSettingsArgs',
     'GetOrgMetadataDomainsArgs',
     'GetOrgMetadataSettingsArgs',
 ]
 
 @pulumi.input_type
+class AppGroupAssignmentsGroupArgs:
+    def __init__(__self__, *,
+                 id: pulumi.Input[str],
+                 profile: pulumi.Input[str],
+                 priority: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[str] id: ID of the group to assign.
+        :param pulumi.Input[str] profile: JSON document containing [application profile](https://developer.okta.com/docs/reference/api/apps/#profile-object)
+        :param pulumi.Input[int] priority: Priority of group assignment
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "profile", profile)
+        if priority is not None:
+            pulumi.set(__self__, "priority", priority)
+
+    @property
+    @pulumi.getter
+    def id(self) -> pulumi.Input[str]:
+        """
+        ID of the group to assign.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def profile(self) -> pulumi.Input[str]:
+        """
+        JSON document containing [application profile](https://developer.okta.com/docs/reference/api/apps/#profile-object)
+        """
+        return pulumi.get(self, "profile")
+
+    @profile.setter
+    def profile(self, value: pulumi.Input[str]):
+        pulumi.set(self, "profile", value)
+
+    @property
+    @pulumi.getter
+    def priority(self) -> Optional[pulumi.Input[int]]:
+        """
+        Priority of group assignment
+        """
+        return pulumi.get(self, "priority")
+
+    @priority.setter
+    def priority(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "priority", value)
+
+
+@pulumi.input_type
+class AppSignonPolicyRulePlatformIncludeArgs:
+    def __init__(__self__, *,
+                 os_expression: Optional[pulumi.Input[str]] = None,
+                 os_type: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] os_expression: Only available and required when using `os_type = "OTHER"`
+        :param pulumi.Input[str] os_type: One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`, `"CHROMEOS"`
+        :param pulumi.Input[str] type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
+        """
+        if os_expression is not None:
+            pulumi.set(__self__, "os_expression", os_expression)
+        if os_type is not None:
+            pulumi.set(__self__, "os_type", os_type)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter(name="osExpression")
+    def os_expression(self) -> Optional[pulumi.Input[str]]:
+        """
+        Only available and required when using `os_type = "OTHER"`
+        """
+        return pulumi.get(self, "os_expression")
+
+    @os_expression.setter
+    def os_expression(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "os_expression", value)
+
+    @property
+    @pulumi.getter(name="osType")
+    def os_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`, `"CHROMEOS"`
+        """
+        return pulumi.get(self, "os_type")
+
+    @os_type.setter
+    def os_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "os_type", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
+
+@pulumi.input_type
+class AppUserSchemaPropertyArrayOneOfArgs:
+    def __init__(__self__, *,
+                 const: pulumi.Input[str],
+                 title: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] const: value mapping to member of `array_enum`.
+        :param pulumi.Input[str] title: display name for the enum value.
+        """
+        pulumi.set(__self__, "const", const)
+        pulumi.set(__self__, "title", title)
+
+    @property
+    @pulumi.getter
+    def const(self) -> pulumi.Input[str]:
+        """
+        value mapping to member of `array_enum`.
+        """
+        return pulumi.get(self, "const")
+
+    @const.setter
+    def const(self, value: pulumi.Input[str]):
+        pulumi.set(self, "const", value)
+
+    @property
+    @pulumi.getter
+    def title(self) -> pulumi.Input[str]:
+        """
+        display name for the enum value.
+        """
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: pulumi.Input[str]):
+        pulumi.set(self, "title", value)
+
+
+@pulumi.input_type
+class AppUserSchemaPropertyOneOfArgs:
+    def __init__(__self__, *,
+                 const: pulumi.Input[str],
+                 title: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] const: value mapping to member of `enum`.
+        :param pulumi.Input[str] title: display name for the enum value.
+        """
+        pulumi.set(__self__, "const", const)
+        pulumi.set(__self__, "title", title)
+
+    @property
+    @pulumi.getter
+    def const(self) -> pulumi.Input[str]:
+        """
+        value mapping to member of `enum`.
+        """
+        return pulumi.get(self, "const")
+
+    @const.setter
+    def const(self, value: pulumi.Input[str]):
+        pulumi.set(self, "const", value)
+
+    @property
+    @pulumi.getter
+    def title(self) -> pulumi.Input[str]:
+        """
+        display name for the enum value.
+        """
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: pulumi.Input[str]):
+        pulumi.set(self, "title", value)
+
+
+@pulumi.input_type
 class CustomizedSigninPageContentSecurityPolicySettingArgs:
     def __init__(__self__, *,
                  mode: Optional[pulumi.Input[str]] = None,
                  report_uri: Optional[pulumi.Input[str]] = None,
                  src_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] mode: enforced or report_only
@@ -323,14 +520,85 @@
 
     @username_label.setter
     def username_label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username_label", value)
 
 
 @pulumi.input_type
+class DomainDnsRecordArgs:
+    def __init__(__self__, *,
+                 expiration: Optional[pulumi.Input[str]] = None,
+                 fqdn: Optional[pulumi.Input[str]] = None,
+                 record_type: Optional[pulumi.Input[str]] = None,
+                 values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] expiration: TXT record expiration.
+        :param pulumi.Input[str] fqdn: DNS record name.
+        :param pulumi.Input[str] record_type: Record type can be TXT or CNAME.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] values: DNS verification value
+        """
+        if expiration is not None:
+            pulumi.set(__self__, "expiration", expiration)
+        if fqdn is not None:
+            pulumi.set(__self__, "fqdn", fqdn)
+        if record_type is not None:
+            pulumi.set(__self__, "record_type", record_type)
+        if values is not None:
+            pulumi.set(__self__, "values", values)
+
+    @property
+    @pulumi.getter
+    def expiration(self) -> Optional[pulumi.Input[str]]:
+        """
+        TXT record expiration.
+        """
+        return pulumi.get(self, "expiration")
+
+    @expiration.setter
+    def expiration(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "expiration", value)
+
+    @property
+    @pulumi.getter
+    def fqdn(self) -> Optional[pulumi.Input[str]]:
+        """
+        DNS record name.
+        """
+        return pulumi.get(self, "fqdn")
+
+    @fqdn.setter
+    def fqdn(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "fqdn", value)
+
+    @property
+    @pulumi.getter(name="recordType")
+    def record_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Record type can be TXT or CNAME.
+        """
+        return pulumi.get(self, "record_type")
+
+    @record_type.setter
+    def record_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "record_type", value)
+
+    @property
+    @pulumi.getter
+    def values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        DNS verification value
+        """
+        return pulumi.get(self, "values")
+
+    @values.setter
+    def values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "values", value)
+
+
+@pulumi.input_type
 class EmailDomainDnsValidationRecordArgs:
     def __init__(__self__, *,
                  expiration: Optional[pulumi.Input[str]] = None,
                  fqdn: Optional[pulumi.Input[str]] = None,
                  record_type: Optional[pulumi.Input[str]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
@@ -402,14 +670,210 @@
 
     @value.setter
     def value(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value", value)
 
 
 @pulumi.input_type
+class EmailSenderDnsRecordArgs:
+    def __init__(__self__, *,
+                 fqdn: Optional[pulumi.Input[str]] = None,
+                 record_type: Optional[pulumi.Input[str]] = None,
+                 value: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] fqdn: DNS record name.
+        :param pulumi.Input[str] record_type: Record type can be TXT or CNAME.
+        :param pulumi.Input[str] value: DNS verification value
+        """
+        if fqdn is not None:
+            pulumi.set(__self__, "fqdn", fqdn)
+        if record_type is not None:
+            pulumi.set(__self__, "record_type", record_type)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def fqdn(self) -> Optional[pulumi.Input[str]]:
+        """
+        DNS record name.
+        """
+        return pulumi.get(self, "fqdn")
+
+    @fqdn.setter
+    def fqdn(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "fqdn", value)
+
+    @property
+    @pulumi.getter(name="recordType")
+    def record_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Record type can be TXT or CNAME.
+        """
+        return pulumi.get(self, "record_type")
+
+    @record_type.setter
+    def record_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "record_type", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[pulumi.Input[str]]:
+        """
+        DNS verification value
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
+class EventHookHeaderArgs:
+    def __init__(__self__, *,
+                 key: Optional[pulumi.Input[str]] = None,
+                 value: Optional[pulumi.Input[str]] = None):
+        if key is not None:
+            pulumi.set(__self__, "key", key)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
+class GroupSchemaPropertyArrayOneOfArgs:
+    def __init__(__self__, *,
+                 const: pulumi.Input[str],
+                 title: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] const: value mapping to member of `enum`.
+        :param pulumi.Input[str] title: display name for the enum value.
+        """
+        pulumi.set(__self__, "const", const)
+        pulumi.set(__self__, "title", title)
+
+    @property
+    @pulumi.getter
+    def const(self) -> pulumi.Input[str]:
+        """
+        value mapping to member of `enum`.
+        """
+        return pulumi.get(self, "const")
+
+    @const.setter
+    def const(self, value: pulumi.Input[str]):
+        pulumi.set(self, "const", value)
+
+    @property
+    @pulumi.getter
+    def title(self) -> pulumi.Input[str]:
+        """
+        display name for the enum value.
+        """
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: pulumi.Input[str]):
+        pulumi.set(self, "title", value)
+
+
+@pulumi.input_type
+class GroupSchemaPropertyMasterOverridePriorityArgs:
+    def __init__(__self__, *,
+                 value: pulumi.Input[str],
+                 type: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] value: ID of profile source.
+        :param pulumi.Input[str] type: Type of profile source.
+        """
+        pulumi.set(__self__, "value", value)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        """
+        ID of profile source.
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Type of profile source.
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
+
+@pulumi.input_type
+class GroupSchemaPropertyOneOfArgs:
+    def __init__(__self__, *,
+                 const: pulumi.Input[str],
+                 title: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] const: value mapping to member of `enum`.
+        :param pulumi.Input[str] title: display name for the enum value.
+        """
+        pulumi.set(__self__, "const", const)
+        pulumi.set(__self__, "title", title)
+
+    @property
+    @pulumi.getter
+    def const(self) -> pulumi.Input[str]:
+        """
+        value mapping to member of `enum`.
+        """
+        return pulumi.get(self, "const")
+
+    @const.setter
+    def const(self, value: pulumi.Input[str]):
+        pulumi.set(self, "const", value)
+
+    @property
+    @pulumi.getter
+    def title(self) -> pulumi.Input[str]:
+        """
+        display name for the enum value.
+        """
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: pulumi.Input[str]):
+        pulumi.set(self, "title", value)
+
+
+@pulumi.input_type
 class LogStreamSettingsArgs:
     def __init__(__self__, *,
                  account_id: Optional[pulumi.Input[str]] = None,
                  edition: Optional[pulumi.Input[str]] = None,
                  event_source_name: Optional[pulumi.Input[str]] = None,
                  host: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
@@ -505,14 +969,67 @@
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
 
 @pulumi.input_type
+class PolicyRuleProfileEnrollmentProfileAttributeArgs:
+    def __init__(__self__, *,
+                 label: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 required: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[str] label: A display-friendly label for this property
+        :param pulumi.Input[str] name: The name of a User Profile property
+        :param pulumi.Input[bool] required: Indicates if this property is required for enrollment. Default is `false`.
+        """
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "name", name)
+        if required is not None:
+            pulumi.set(__self__, "required", required)
+
+    @property
+    @pulumi.getter
+    def label(self) -> pulumi.Input[str]:
+        """
+        A display-friendly label for this property
+        """
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: pulumi.Input[str]):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        The name of a User Profile property
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def required(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Indicates if this property is required for enrollment. Default is `false`.
+        """
+        return pulumi.get(self, "required")
+
+    @required.setter
+    def required(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "required", value)
+
+
+@pulumi.input_type
 class PreviewSigninPageContentSecurityPolicySettingArgs:
     def __init__(__self__, *,
                  mode: Optional[pulumi.Input[str]] = None,
                  report_uri: Optional[pulumi.Input[str]] = None,
                  src_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] mode: enforced or report_only
@@ -808,14 +1325,163 @@
 
     @username_label.setter
     def username_label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username_label", value)
 
 
 @pulumi.input_type
+class TemplateSmsTranslationArgs:
+    def __init__(__self__, *,
+                 language: pulumi.Input[str],
+                 template: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] language: The language to map the template to.
+        :param pulumi.Input[str] template: The SMS message.
+        """
+        pulumi.set(__self__, "language", language)
+        pulumi.set(__self__, "template", template)
+
+    @property
+    @pulumi.getter
+    def language(self) -> pulumi.Input[str]:
+        """
+        The language to map the template to.
+        """
+        return pulumi.get(self, "language")
+
+    @language.setter
+    def language(self, value: pulumi.Input[str]):
+        pulumi.set(self, "language", value)
+
+    @property
+    @pulumi.getter
+    def template(self) -> pulumi.Input[str]:
+        """
+        The SMS message.
+        """
+        return pulumi.get(self, "template")
+
+    @template.setter
+    def template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "template", value)
+
+
+@pulumi.input_type
+class UserSchemaPropertyArrayOneOfArgs:
+    def __init__(__self__, *,
+                 const: pulumi.Input[str],
+                 title: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] const: value mapping to member of `enum`.
+        :param pulumi.Input[str] title: display name for the enum value.
+        """
+        pulumi.set(__self__, "const", const)
+        pulumi.set(__self__, "title", title)
+
+    @property
+    @pulumi.getter
+    def const(self) -> pulumi.Input[str]:
+        """
+        value mapping to member of `enum`.
+        """
+        return pulumi.get(self, "const")
+
+    @const.setter
+    def const(self, value: pulumi.Input[str]):
+        pulumi.set(self, "const", value)
+
+    @property
+    @pulumi.getter
+    def title(self) -> pulumi.Input[str]:
+        """
+        display name for the enum value.
+        """
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: pulumi.Input[str]):
+        pulumi.set(self, "title", value)
+
+
+@pulumi.input_type
+class UserSchemaPropertyMasterOverridePriorityArgs:
+    def __init__(__self__, *,
+                 value: pulumi.Input[str],
+                 type: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] value: ID of profile source.
+        :param pulumi.Input[str] type: Type of profile source.
+        """
+        pulumi.set(__self__, "value", value)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        """
+        ID of profile source.
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Type of profile source.
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
+
+@pulumi.input_type
+class UserSchemaPropertyOneOfArgs:
+    def __init__(__self__, *,
+                 const: pulumi.Input[str],
+                 title: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] const: value mapping to member of `enum`.
+        :param pulumi.Input[str] title: display name for the enum value.
+        """
+        pulumi.set(__self__, "const", const)
+        pulumi.set(__self__, "title", title)
+
+    @property
+    @pulumi.getter
+    def const(self) -> pulumi.Input[str]:
+        """
+        value mapping to member of `enum`.
+        """
+        return pulumi.get(self, "const")
+
+    @const.setter
+    def const(self, value: pulumi.Input[str]):
+        pulumi.set(self, "const", value)
+
+    @property
+    @pulumi.getter
+    def title(self) -> pulumi.Input[str]:
+        """
+        display name for the enum value.
+        """
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: pulumi.Input[str]):
+        pulumi.set(self, "title", value)
+
+
+@pulumi.input_type
 class GetDefaultSigninPageContentSecurityPolicySettingArgs:
     def __init__(__self__, *,
                  mode: str,
                  report_uri: str,
                  src_lists: Sequence[str]):
         """
         :param str mode: enforced or report_only
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/customized_signin_page.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/customized_signin_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = ['CustomizedSigninPageArgs', 'CustomizedSigninPage']
 
 @pulumi.input_type
 class CustomizedSigninPageArgs:
@@ -203,15 +203,15 @@
                  __props__=None):
         """
         Manage the customized signin page of a brand
 
         ## Import
 
         ```sh
-        $ pulumi import okta:Index/customizedSigninPage:CustomizedSigninPage example &#60;customized_signin_page_id&#62;
+        $ pulumi import okta:index/customizedSigninPage:CustomizedSigninPage example &#60;customized_signin_page_id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] brand_id: brand id of the preview signin page
         :param pulumi.Input[str] page_content: page content of the preview signin page
         :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported
@@ -229,15 +229,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage the customized signin page of a brand
 
         ## Import
 
         ```sh
-        $ pulumi import okta:Index/customizedSigninPage:CustomizedSigninPage example &#60;customized_signin_page_id&#62;
+        $ pulumi import okta:index/customizedSigninPage:CustomizedSigninPage example &#60;customized_signin_page_id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param CustomizedSigninPageArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -273,15 +273,15 @@
                 raise TypeError("Missing required property 'page_content'")
             __props__.__dict__["page_content"] = page_content
             __props__.__dict__["widget_customizations"] = widget_customizations
             if widget_version is None and not opts.urn:
                 raise TypeError("Missing required property 'widget_version'")
             __props__.__dict__["widget_version"] = widget_version
         super(CustomizedSigninPage, __self__).__init__(
-            'okta:Index/customizedSigninPage:CustomizedSigninPage',
+            'okta:index/customizedSigninPage:CustomizedSigninPage',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/email_domain.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = ['EmailDomainArgs', 'EmailDomain']
 
 @pulumi.input_type
 class EmailDomainArgs:
@@ -200,27 +200,27 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.index.EmailDomain("example",
+        example = okta.EmailDomain("example",
             brand_id="abc123",
             domain="example.com",
             display_name="test",
             user_name="paul_atreides")
         ```
 
         ## Import
 
         Custom email domain can be imported via the Okta ID.
 
         ```sh
-        $ pulumi import okta:Index/emailDomain:EmailDomain example &#60;domain id&#62;
+        $ pulumi import okta:index/emailDomain:EmailDomain example &#60;domain id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] brand_id: Brand id of the email domain.
         :param pulumi.Input[str] display_name: Display name of the email domain.
         :param pulumi.Input[str] domain: Mail domain to send from.
@@ -237,27 +237,27 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.index.EmailDomain("example",
+        example = okta.EmailDomain("example",
             brand_id="abc123",
             domain="example.com",
             display_name="test",
             user_name="paul_atreides")
         ```
 
         ## Import
 
         Custom email domain can be imported via the Okta ID.
 
         ```sh
-        $ pulumi import okta:Index/emailDomain:EmailDomain example &#60;domain id&#62;
+        $ pulumi import okta:index/emailDomain:EmailDomain example &#60;domain id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param EmailDomainArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -295,15 +295,15 @@
             __props__.__dict__["domain"] = domain
             if user_name is None and not opts.urn:
                 raise TypeError("Missing required property 'user_name'")
             __props__.__dict__["user_name"] = user_name
             __props__.__dict__["dns_validation_records"] = None
             __props__.__dict__["validation_status"] = None
         super(EmailDomain, __self__).__init__(
-            'okta:Index/emailDomain:EmailDomain',
+            'okta:index/emailDomain:EmailDomain',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/email_domain_verification.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_domain_verification.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
 __all__ = ['EmailDomainVerificationArgs', 'EmailDomainVerification']
 
 @pulumi.input_type
 class EmailDomainVerificationArgs:
     def __init__(__self__, *,
                  email_domain_id: pulumi.Input[str]):
@@ -70,20 +70,20 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.index.EmailDomain("example",
+        example = okta.EmailDomain("example",
             brand_id="abc123",
             domain="example.com",
             display_name="test",
             user_name="paul_atreides")
-        example_email_domain_verification = okta.index.EmailDomainVerification("example", email_domain_id=valid["id"])
+        example_email_domain_verification = okta.EmailDomainVerification("example", email_domain_id=valid["id"])
         ```
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
@@ -101,20 +101,20 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.index.EmailDomain("example",
+        example = okta.EmailDomain("example",
             brand_id="abc123",
             domain="example.com",
             display_name="test",
             user_name="paul_atreides")
-        example_email_domain_verification = okta.index.EmailDomainVerification("example", email_domain_id=valid["id"])
+        example_email_domain_verification = okta.EmailDomainVerification("example", email_domain_id=valid["id"])
         ```
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
@@ -142,15 +142,15 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EmailDomainVerificationArgs.__new__(EmailDomainVerificationArgs)
 
             if email_domain_id is None and not opts.urn:
                 raise TypeError("Missing required property 'email_domain_id'")
             __props__.__dict__["email_domain_id"] = email_domain_id
         super(EmailDomainVerification, __self__).__init__(
-            'okta:Index/emailDomainVerification:EmailDomainVerification',
+            'okta:index/emailDomainVerification:EmailDomainVerification',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/get_default_signin_page.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_default_signin_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = [
     'GetDefaultSigninPageResult',
     'AwaitableGetDefaultSigninPageResult',
     'get_default_signin_page',
@@ -111,15 +111,15 @@
     :param str brand_id: brand id of the preview signin page
     """
     __args__ = dict()
     __args__['brandId'] = brand_id
     __args__['contentSecurityPolicySetting'] = content_security_policy_setting
     __args__['widgetCustomizations'] = widget_customizations
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('okta:Index/getDefaultSigninPage:getDefaultSigninPage', __args__, opts=opts, typ=GetDefaultSigninPageResult).value
+    __ret__ = pulumi.runtime.invoke('okta:index/getDefaultSigninPage:getDefaultSigninPage', __args__, opts=opts, typ=GetDefaultSigninPageResult).value
 
     return AwaitableGetDefaultSigninPageResult(
         brand_id=pulumi.get(__ret__, 'brand_id'),
         content_security_policy_setting=pulumi.get(__ret__, 'content_security_policy_setting'),
         id=pulumi.get(__ret__, 'id'),
         page_content=pulumi.get(__ret__, 'page_content'),
         widget_customizations=pulumi.get(__ret__, 'widget_customizations'),
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 
 __all__ = [
     'GetDomainResult',
     'AwaitableGetDomainResult',
     'get_domain',
     'get_domain_output',
@@ -125,25 +125,25 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.Domain("example", name="www.example.com")
-    by_name = okta.Index.get_domain(domain_id_or_name="www.example.com")
-    by_id = okta.Index.get_domain_output(domain_id_or_name=example.id)
+    by_name = okta.get_domain(domain_id_or_name="www.example.com")
+    by_id = okta.get_domain_output(domain_id_or_name=example.id)
     ```
 
 
     :param str domain_id_or_name: The Okta ID of the domain or the domain name itself.
     """
     __args__ = dict()
     __args__['domainIdOrName'] = domain_id_or_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('okta:Index/getDomain:getDomain', __args__, opts=opts, typ=GetDomainResult).value
+    __ret__ = pulumi.runtime.invoke('okta:index/getDomain:getDomain', __args__, opts=opts, typ=GetDomainResult).value
 
     return AwaitableGetDomainResult(
         certificate_source_type=pulumi.get(__ret__, 'certificate_source_type'),
         dns_records=pulumi.get(__ret__, 'dns_records'),
         domain=pulumi.get(__ret__, 'domain'),
         domain_id_or_name=pulumi.get(__ret__, 'domain_id_or_name'),
         id=pulumi.get(__ret__, 'id'),
@@ -163,15 +163,15 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.Domain("example", name="www.example.com")
-    by_name = okta.Index.get_domain(domain_id_or_name="www.example.com")
-    by_id = okta.Index.get_domain_output(domain_id_or_name=example.id)
+    by_name = okta.get_domain(domain_id_or_name="www.example.com")
+    by_id = okta.get_domain_output(domain_id_or_name=example.id)
     ```
 
 
     :param str domain_id_or_name: The Okta ID of the domain or the domain name itself.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/get_log_stream.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_log_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = [
     'GetLogStreamResult',
     'AwaitableGetLogStreamResult',
     'get_log_stream',
@@ -103,28 +103,28 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    example = okta.Index.get_log_stream(name="Example Stream")
+    example = okta.get_log_stream(name="Example Stream")
     ```
 
 
     :param str id: ID of the log stream to retrieve, conflicts with `name`.
     :param str name: Name of the log stream to retrieve, conflicts with `id`.
     :param pulumi.InputType['GetLogStreamSettingsArgs'] settings: Provider specific configuration.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     __args__['settings'] = settings
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('okta:Index/getLogStream:getLogStream', __args__, opts=opts, typ=GetLogStreamResult).value
+    __ret__ = pulumi.runtime.invoke('okta:index/getLogStream:getLogStream', __args__, opts=opts, typ=GetLogStreamResult).value
 
     return AwaitableGetLogStreamResult(
         id=pulumi.get(__ret__, 'id'),
         name=pulumi.get(__ret__, 'name'),
         settings=pulumi.get(__ret__, 'settings'),
         status=pulumi.get(__ret__, 'status'),
         type=pulumi.get(__ret__, 'type'))
@@ -140,15 +140,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    example = okta.Index.get_log_stream(name="Example Stream")
+    example = okta.get_log_stream(name="Example Stream")
     ```
 
 
     :param str id: ID of the log stream to retrieve, conflicts with `name`.
     :param str name: Name of the log stream to retrieve, conflicts with `id`.
     :param pulumi.InputType['GetLogStreamSettingsArgs'] settings: Provider specific configuration.
     """
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/get_org_metadata.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_org_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = [
     'GetOrgMetadataResult',
     'AwaitableGetOrgMetadataResult',
     'get_org_metadata',
@@ -92,26 +92,26 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.Index.get_org_metadata()
+    test = okta.get_org_metadata()
     ```
 
 
     :param pulumi.InputType['GetOrgMetadataDomainsArgs'] domains: The URIs for the org's configured domains.
     :param pulumi.InputType['GetOrgMetadataSettingsArgs'] settings: The wellknown org settings (safe for public consumption).
     """
     __args__ = dict()
     __args__['domains'] = domains
     __args__['settings'] = settings
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('okta:Index/getOrgMetadata:getOrgMetadata', __args__, opts=opts, typ=GetOrgMetadataResult).value
+    __ret__ = pulumi.runtime.invoke('okta:index/getOrgMetadata:getOrgMetadata', __args__, opts=opts, typ=GetOrgMetadataResult).value
 
     return AwaitableGetOrgMetadataResult(
         domains=pulumi.get(__ret__, 'domains'),
         id=pulumi.get(__ret__, 'id'),
         pipeline=pulumi.get(__ret__, 'pipeline'),
         settings=pulumi.get(__ret__, 'settings'))
 
@@ -127,15 +127,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.Index.get_org_metadata()
+    test = okta.get_org_metadata()
     ```
 
 
     :param pulumi.InputType['GetOrgMetadataDomainsArgs'] domains: The URIs for the org's configured domains.
     :param pulumi.InputType['GetOrgMetadataSettingsArgs'] settings: The wellknown org settings (safe for public consumption).
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/log_stream.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/log_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = ['LogStreamArgs', 'LogStream']
 
 @pulumi.input_type
 class LogStreamArgs:
@@ -174,15 +174,15 @@
         ## Example Usage
 
         ## Import
 
         Okta Log Stream can be imported via the Okta ID.
 
         ```sh
-        $ pulumi import okta:Index/logStream:LogStream example &#60;strema id&#62;
+        $ pulumi import okta:index/logStream:LogStream example &#60;strema id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: Name of the Log Stream Resource.
         :param pulumi.Input[pulumi.InputType['LogStreamSettingsArgs']] settings: Stream provider specific configuration.
         :param pulumi.Input[str] status: Log Stream Status - can either be ACTIVE or INACTIVE only. Default is ACTIVE.
@@ -202,15 +202,15 @@
         ## Example Usage
 
         ## Import
 
         Okta Log Stream can be imported via the Okta ID.
 
         ```sh
-        $ pulumi import okta:Index/logStream:LogStream example &#60;strema id&#62;
+        $ pulumi import okta:index/logStream:LogStream example &#60;strema id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param LogStreamArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -240,15 +240,15 @@
             __props__.__dict__["name"] = name
             __props__.__dict__["settings"] = settings
             __props__.__dict__["status"] = status
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
         super(LogStream, __self__).__init__(
-            'okta:Index/logStream:LogStream',
+            'okta:index/logStream:LogStream',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/index/preview_signin_page.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/preview_signin_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = ['PreviewSigninPageArgs', 'PreviewSigninPage']
 
 @pulumi.input_type
 class PreviewSigninPageArgs:
@@ -261,15 +261,15 @@
                 raise TypeError("Missing required property 'page_content'")
             __props__.__dict__["page_content"] = page_content
             __props__.__dict__["widget_customizations"] = widget_customizations
             if widget_version is None and not opts.urn:
                 raise TypeError("Missing required property 'widget_version'")
             __props__.__dict__["widget_version"] = widget_version
         super(PreviewSigninPage, __self__).__init__(
-            'okta:Index/previewSigninPage:PreviewSigninPage',
+            'okta:index/previewSigninPage:PreviewSigninPage',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/inline/hook.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/link_definition.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/link_value.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/network/zone.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/network/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/org_configuration.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/org_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/org_support.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/outputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_mfa.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,1222 +3,652 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
-
-__all__ = [
-    'AppGroupAssignmentsGroup',
-    'AppSignonPolicyRulePlatformInclude',
-    'AppUserSchemaPropertyArrayOneOf',
-    'AppUserSchemaPropertyOneOf',
-    'DomainDnsRecord',
-    'EmailSenderDnsRecord',
-    'EventHookHeader',
-    'GroupSchemaPropertyArrayOneOf',
-    'GroupSchemaPropertyMasterOverridePriority',
-    'GroupSchemaPropertyOneOf',
-    'PolicyRuleProfileEnrollmentProfileAttribute',
-    'TemplateSmsTranslation',
-    'UserSchemaPropertyArrayOneOf',
-    'UserSchemaPropertyMasterOverridePriority',
-    'UserSchemaPropertyOneOf',
-    'GetAuthServerClaimsClaimResult',
-    'GetBehavioursBehaviorResult',
-    'GetBrandsBrandResult',
-    'GetEmailCustomizationsEmailCustomizationResult',
-    'GetGroupsGroupResult',
-    'GetTemplatesEmailTemplateResult',
-    'GetThemesThemeResult',
-    'GetTrustedOriginsTrustedOriginResult',
-    'GetUserSecurityQuestionsQuestionResult',
-]
-
-@pulumi.output_type
-class AppGroupAssignmentsGroup(dict):
-    def __init__(__self__, *,
-                 id: str,
-                 profile: str,
-                 priority: Optional[int] = None):
-        """
-        :param str id: ID of the group to assign.
-        :param str profile: JSON document containing [application profile](https://developer.okta.com/docs/reference/api/apps/#profile-object)
-        :param int priority: Priority of group assignment
-        """
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "profile", profile)
+from .. import _utilities
+from . import outputs
+from ._inputs import *
+
+__all__ = ['RuleMfaArgs', 'RuleMfa']
+
+@pulumi.input_type
+class RuleMfaArgs:
+    def __init__(__self__, *,
+                 app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]] = None,
+                 app_includes: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]] = None,
+                 enroll: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_connection: Optional[pulumi.Input[str]] = None,
+                 network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 policy_id: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        The set of arguments for constructing a RuleMfa resource.
+        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
+        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
+        :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
+        :param pulumi.Input[str] name: Policy Rule Name.
+        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
+        :param pulumi.Input[str] policy_id: Policy ID.
+        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
+        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
+        """
+        if app_excludes is not None:
+            pulumi.set(__self__, "app_excludes", app_excludes)
+        if app_includes is not None:
+            pulumi.set(__self__, "app_includes", app_includes)
+        if enroll is not None:
+            pulumi.set(__self__, "enroll", enroll)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if network_connection is not None:
+            pulumi.set(__self__, "network_connection", network_connection)
+        if network_excludes is not None:
+            pulumi.set(__self__, "network_excludes", network_excludes)
+        if network_includes is not None:
+            pulumi.set(__self__, "network_includes", network_includes)
+        if policy_id is not None:
+            pulumi.set(__self__, "policy_id", policy_id)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+        if users_excludeds is not None:
+            pulumi.set(__self__, "users_excludeds", users_excludeds)
 
     @property
-    @pulumi.getter
-    def id(self) -> str:
-        """
-        ID of the group to assign.
-        """
-        return pulumi.get(self, "id")
-
-    @property
-    @pulumi.getter
-    def profile(self) -> str:
-        """
-        JSON document containing [application profile](https://developer.okta.com/docs/reference/api/apps/#profile-object)
-        """
-        return pulumi.get(self, "profile")
-
-    @property
-    @pulumi.getter
-    def priority(self) -> Optional[int]:
-        """
-        Priority of group assignment
-        """
-        return pulumi.get(self, "priority")
-
-
-@pulumi.output_type
-class AppSignonPolicyRulePlatformInclude(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "osExpression":
-            suggest = "os_expression"
-        elif key == "osType":
-            suggest = "os_type"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in AppSignonPolicyRulePlatformInclude. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        AppSignonPolicyRulePlatformInclude.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        AppSignonPolicyRulePlatformInclude.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 os_expression: Optional[str] = None,
-                 os_type: Optional[str] = None,
-                 type: Optional[str] = None):
-        """
-        :param str os_expression: Only available and required when using `os_type = "OTHER"`
-        :param str os_type: One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`, `"CHROMEOS"`
-        :param str type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
-        """
-        if os_expression is not None:
-            pulumi.set(__self__, "os_expression", os_expression)
-        if os_type is not None:
-            pulumi.set(__self__, "os_type", os_type)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="osExpression")
-    def os_expression(self) -> Optional[str]:
-        """
-        Only available and required when using `os_type = "OTHER"`
-        """
-        return pulumi.get(self, "os_expression")
-
-    @property
-    @pulumi.getter(name="osType")
-    def os_type(self) -> Optional[str]:
-        """
-        One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`, `"CHROMEOS"`
-        """
-        return pulumi.get(self, "os_type")
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        """
-        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
-        """
-        return pulumi.get(self, "type")
-
-
-@pulumi.output_type
-class AppUserSchemaPropertyArrayOneOf(dict):
-    def __init__(__self__, *,
-                 const: str,
-                 title: str):
-        """
-        :param str const: value mapping to member of `array_enum`.
-        :param str title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
-
-    @property
-    @pulumi.getter
-    def const(self) -> str:
-        """
-        value mapping to member of `array_enum`.
-        """
-        return pulumi.get(self, "const")
-
-    @property
-    @pulumi.getter
-    def title(self) -> str:
-        """
-        display name for the enum value.
-        """
-        return pulumi.get(self, "title")
-
-
-@pulumi.output_type
-class AppUserSchemaPropertyOneOf(dict):
-    def __init__(__self__, *,
-                 const: str,
-                 title: str):
-        """
-        :param str const: value mapping to member of `enum`.
-        :param str title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
-
-    @property
-    @pulumi.getter
-    def const(self) -> str:
-        """
-        value mapping to member of `enum`.
-        """
-        return pulumi.get(self, "const")
-
-    @property
-    @pulumi.getter
-    def title(self) -> str:
-        """
-        display name for the enum value.
-        """
-        return pulumi.get(self, "title")
-
-
-@pulumi.output_type
-class DomainDnsRecord(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "recordType":
-            suggest = "record_type"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in DomainDnsRecord. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        DomainDnsRecord.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        DomainDnsRecord.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 expiration: Optional[str] = None,
-                 fqdn: Optional[str] = None,
-                 record_type: Optional[str] = None,
-                 values: Optional[Sequence[str]] = None):
-        """
-        :param str expiration: TXT record expiration.
-        :param str fqdn: DNS record name.
-        :param str record_type: Record type can be TXT or CNAME.
-        :param Sequence[str] values: DNS verification value
-        """
-        if expiration is not None:
-            pulumi.set(__self__, "expiration", expiration)
-        if fqdn is not None:
-            pulumi.set(__self__, "fqdn", fqdn)
-        if record_type is not None:
-            pulumi.set(__self__, "record_type", record_type)
-        if values is not None:
-            pulumi.set(__self__, "values", values)
-
-    @property
-    @pulumi.getter
-    def expiration(self) -> Optional[str]:
+    @pulumi.getter(name="appExcludes")
+    def app_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]:
         """
-        TXT record expiration.
+        Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+        - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+        is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+        of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         """
-        return pulumi.get(self, "expiration")
+        return pulumi.get(self, "app_excludes")
 
-    @property
-    @pulumi.getter
-    def fqdn(self) -> Optional[str]:
-        """
-        DNS record name.
-        """
-        return pulumi.get(self, "fqdn")
+    @app_excludes.setter
+    def app_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]):
+        pulumi.set(self, "app_excludes", value)
 
     @property
-    @pulumi.getter(name="recordType")
-    def record_type(self) -> Optional[str]:
+    @pulumi.getter(name="appIncludes")
+    def app_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]]:
         """
-        Record type can be TXT or CNAME.
+        Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         """
-        return pulumi.get(self, "record_type")
+        return pulumi.get(self, "app_includes")
 
-    @property
-    @pulumi.getter
-    def values(self) -> Optional[Sequence[str]]:
-        """
-        DNS verification value
-        """
-        return pulumi.get(self, "values")
-
-
-@pulumi.output_type
-class EmailSenderDnsRecord(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "recordType":
-            suggest = "record_type"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in EmailSenderDnsRecord. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        EmailSenderDnsRecord.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        EmailSenderDnsRecord.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 fqdn: Optional[str] = None,
-                 record_type: Optional[str] = None,
-                 value: Optional[str] = None):
-        """
-        :param str fqdn: DNS record name.
-        :param str record_type: Record type can be TXT or CNAME.
-        :param str value: DNS verification value
-        """
-        if fqdn is not None:
-            pulumi.set(__self__, "fqdn", fqdn)
-        if record_type is not None:
-            pulumi.set(__self__, "record_type", record_type)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
+    @app_includes.setter
+    def app_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]]):
+        pulumi.set(self, "app_includes", value)
 
     @property
     @pulumi.getter
-    def fqdn(self) -> Optional[str]:
+    def enroll(self) -> Optional[pulumi.Input[str]]:
         """
-        DNS record name.
+        When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
         """
-        return pulumi.get(self, "fqdn")
+        return pulumi.get(self, "enroll")
 
-    @property
-    @pulumi.getter(name="recordType")
-    def record_type(self) -> Optional[str]:
-        """
-        Record type can be TXT or CNAME.
-        """
-        return pulumi.get(self, "record_type")
+    @enroll.setter
+    def enroll(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "enroll", value)
 
     @property
     @pulumi.getter
-    def value(self) -> Optional[str]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        DNS verification value
-        """
-        return pulumi.get(self, "value")
-
-
-@pulumi.output_type
-class EventHookHeader(dict):
-    def __init__(__self__, *,
-                 key: Optional[str] = None,
-                 value: Optional[str] = None):
-        if key is not None:
-            pulumi.set(__self__, "key", key)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
-
-    @property
-    @pulumi.getter
-    def key(self) -> Optional[str]:
-        return pulumi.get(self, "key")
-
-    @property
-    @pulumi.getter
-    def value(self) -> Optional[str]:
-        return pulumi.get(self, "value")
-
-
-@pulumi.output_type
-class GroupSchemaPropertyArrayOneOf(dict):
-    def __init__(__self__, *,
-                 const: str,
-                 title: str):
-        """
-        :param str const: value mapping to member of `enum`.
-        :param str title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
-
-    @property
-    @pulumi.getter
-    def const(self) -> str:
-        """
-        value mapping to member of `enum`.
-        """
-        return pulumi.get(self, "const")
-
-    @property
-    @pulumi.getter
-    def title(self) -> str:
-        """
-        display name for the enum value.
-        """
-        return pulumi.get(self, "title")
-
-
-@pulumi.output_type
-class GroupSchemaPropertyMasterOverridePriority(dict):
-    def __init__(__self__, *,
-                 value: str,
-                 type: Optional[str] = None):
-        """
-        :param str value: ID of profile source.
-        :param str type: Type of profile source.
-        """
-        pulumi.set(__self__, "value", value)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter
-    def value(self) -> str:
-        """
-        ID of profile source.
-        """
-        return pulumi.get(self, "value")
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        """
-        Type of profile source.
-        """
-        return pulumi.get(self, "type")
-
-
-@pulumi.output_type
-class GroupSchemaPropertyOneOf(dict):
-    def __init__(__self__, *,
-                 const: str,
-                 title: str):
-        """
-        :param str const: value mapping to member of `enum`.
-        :param str title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
-
-    @property
-    @pulumi.getter
-    def const(self) -> str:
-        """
-        value mapping to member of `enum`.
-        """
-        return pulumi.get(self, "const")
-
-    @property
-    @pulumi.getter
-    def title(self) -> str:
-        """
-        display name for the enum value.
-        """
-        return pulumi.get(self, "title")
-
-
-@pulumi.output_type
-class PolicyRuleProfileEnrollmentProfileAttribute(dict):
-    def __init__(__self__, *,
-                 label: str,
-                 name: str,
-                 required: Optional[bool] = None):
-        """
-        :param str label: A display-friendly label for this property
-        :param str name: The name of a User Profile property
-        :param bool required: Indicates if this property is required for enrollment. Default is `false`.
-        """
-        pulumi.set(__self__, "label", label)
-        pulumi.set(__self__, "name", name)
-        if required is not None:
-            pulumi.set(__self__, "required", required)
-
-    @property
-    @pulumi.getter
-    def label(self) -> str:
-        """
-        A display-friendly label for this property
-        """
-        return pulumi.get(self, "label")
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        The name of a User Profile property
+        Policy Rule Name.
         """
         return pulumi.get(self, "name")
 
-    @property
-    @pulumi.getter
-    def required(self) -> Optional[bool]:
-        """
-        Indicates if this property is required for enrollment. Default is `false`.
-        """
-        return pulumi.get(self, "required")
-
-
-@pulumi.output_type
-class TemplateSmsTranslation(dict):
-    def __init__(__self__, *,
-                 language: str,
-                 template: str):
-        """
-        :param str language: The language to map the template to.
-        :param str template: The SMS message.
-        """
-        pulumi.set(__self__, "language", language)
-        pulumi.set(__self__, "template", template)
-
-    @property
-    @pulumi.getter
-    def language(self) -> str:
-        """
-        The language to map the template to.
-        """
-        return pulumi.get(self, "language")
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def template(self) -> str:
+    @pulumi.getter(name="networkConnection")
+    def network_connection(self) -> Optional[pulumi.Input[str]]:
         """
-        The SMS message.
+        Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         """
-        return pulumi.get(self, "template")
-
+        return pulumi.get(self, "network_connection")
 
-@pulumi.output_type
-class UserSchemaPropertyArrayOneOf(dict):
-    def __init__(__self__, *,
-                 const: str,
-                 title: str):
-        """
-        :param str const: value mapping to member of `enum`.
-        :param str title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
+    @network_connection.setter
+    def network_connection(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network_connection", value)
 
     @property
-    @pulumi.getter
-    def const(self) -> str:
+    @pulumi.getter(name="networkExcludes")
+    def network_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        value mapping to member of `enum`.
+        The network zones to exclude. Conflicts with `network_includes`.
         """
-        return pulumi.get(self, "const")
+        return pulumi.get(self, "network_excludes")
 
-    @property
-    @pulumi.getter
-    def title(self) -> str:
-        """
-        display name for the enum value.
-        """
-        return pulumi.get(self, "title")
-
-
-@pulumi.output_type
-class UserSchemaPropertyMasterOverridePriority(dict):
-    def __init__(__self__, *,
-                 value: str,
-                 type: Optional[str] = None):
-        """
-        :param str value: ID of profile source.
-        :param str type: Type of profile source.
-        """
-        pulumi.set(__self__, "value", value)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter
-    def value(self) -> str:
-        """
-        ID of profile source.
-        """
-        return pulumi.get(self, "value")
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        """
-        Type of profile source.
-        """
-        return pulumi.get(self, "type")
-
-
-@pulumi.output_type
-class UserSchemaPropertyOneOf(dict):
-    def __init__(__self__, *,
-                 const: str,
-                 title: str):
-        """
-        :param str const: value mapping to member of `enum`.
-        :param str title: display name for the enum value.
-        """
-        pulumi.set(__self__, "const", const)
-        pulumi.set(__self__, "title", title)
-
-    @property
-    @pulumi.getter
-    def const(self) -> str:
-        """
-        value mapping to member of `enum`.
-        """
-        return pulumi.get(self, "const")
+    @network_excludes.setter
+    def network_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "network_excludes", value)
 
     @property
-    @pulumi.getter
-    def title(self) -> str:
+    @pulumi.getter(name="networkIncludes")
+    def network_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        display name for the enum value.
+        The network zones to include. Conflicts with `network_excludes`.
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "network_includes")
 
-
-@pulumi.output_type
-class GetAuthServerClaimsClaimResult(dict):
-    def __init__(__self__, *,
-                 always_include_in_token: bool,
-                 claim_type: str,
-                 id: str,
-                 name: str,
-                 scopes: Sequence[str],
-                 status: str,
-                 value: str,
-                 value_type: str):
-        """
-        :param bool always_include_in_token: Specifies whether to include Claims in the token.
-        :param str claim_type: Specifies whether the Claim is for an access token (`"RESOURCE"`) or ID token (`"IDENTITY"`).
-        :param str id: ID of the claim.
-        :param str name: Name of the claim.
-        :param Sequence[str] scopes: Specifies the scopes for this Claim.
-        :param str status: Status of the claim.
-        :param str value: Value of the claim
-        :param str value_type: Specifies whether the Claim is an Okta EL expression (`"EXPRESSION"`), a set of groups (`"GROUPS"`), or a system claim (`"SYSTEM"`)
-        """
-        pulumi.set(__self__, "always_include_in_token", always_include_in_token)
-        pulumi.set(__self__, "claim_type", claim_type)
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "scopes", scopes)
-        pulumi.set(__self__, "status", status)
-        pulumi.set(__self__, "value", value)
-        pulumi.set(__self__, "value_type", value_type)
-
-    @property
-    @pulumi.getter(name="alwaysIncludeInToken")
-    def always_include_in_token(self) -> bool:
-        """
-        Specifies whether to include Claims in the token.
-        """
-        return pulumi.get(self, "always_include_in_token")
+    @network_includes.setter
+    def network_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "network_includes", value)
 
     @property
-    @pulumi.getter(name="claimType")
-    def claim_type(self) -> str:
+    @pulumi.getter(name="policyId")
+    def policy_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Specifies whether the Claim is for an access token (`"RESOURCE"`) or ID token (`"IDENTITY"`).
+        Policy ID.
         """
-        return pulumi.get(self, "claim_type")
+        return pulumi.get(self, "policy_id")
 
-    @property
-    @pulumi.getter
-    def id(self) -> str:
-        """
-        ID of the claim.
-        """
-        return pulumi.get(self, "id")
+    @policy_id.setter
+    def policy_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "policy_id", value)
 
     @property
     @pulumi.getter
-    def name(self) -> str:
+    def priority(self) -> Optional[pulumi.Input[int]]:
         """
-        Name of the claim.
+        Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "priority")
 
-    @property
-    @pulumi.getter
-    def scopes(self) -> Sequence[str]:
-        """
-        Specifies the scopes for this Claim.
-        """
-        return pulumi.get(self, "scopes")
+    @priority.setter
+    def priority(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "priority", value)
 
     @property
     @pulumi.getter
-    def status(self) -> str:
+    def status(self) -> Optional[pulumi.Input[str]]:
         """
-        Status of the claim.
+        Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         """
         return pulumi.get(self, "status")
 
-    @property
-    @pulumi.getter
-    def value(self) -> str:
-        """
-        Value of the claim
-        """
-        return pulumi.get(self, "value")
-
-    @property
-    @pulumi.getter(name="valueType")
-    def value_type(self) -> str:
-        """
-        Specifies whether the Claim is an Okta EL expression (`"EXPRESSION"`), a set of groups (`"GROUPS"`), or a system claim (`"SYSTEM"`)
-        """
-        return pulumi.get(self, "value_type")
-
-
-@pulumi.output_type
-class GetBehavioursBehaviorResult(dict):
-    def __init__(__self__, *,
-                 id: str,
-                 name: str,
-                 settings: Mapping[str, str],
-                 status: str,
-                 type: str):
-        """
-        :param str id: Behavior ID.
-        :param str name: Behavior name.
-        :param Mapping[str, str] settings: Map of behavior settings.
-        :param str status: Behavior status.
-        :param str type: Behavior type.
-        """
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "settings", settings)
-        pulumi.set(__self__, "status", status)
-        pulumi.set(__self__, "type", type)
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
+
+    @property
+    @pulumi.getter(name="usersExcludeds")
+    def users_excludeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Set of User IDs to Exclude
+        """
+        return pulumi.get(self, "users_excludeds")
+
+    @users_excludeds.setter
+    def users_excludeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "users_excludeds", value)
+
+
+@pulumi.input_type
+class _RuleMfaState:
+    def __init__(__self__, *,
+                 app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]] = None,
+                 app_includes: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]] = None,
+                 enroll: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_connection: Optional[pulumi.Input[str]] = None,
+                 network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 policy_id: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        Input properties used for looking up and filtering RuleMfa resources.
+        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
+        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
+        :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
+        :param pulumi.Input[str] name: Policy Rule Name.
+        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
+        :param pulumi.Input[str] policy_id: Policy ID.
+        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
+        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
+        """
+        if app_excludes is not None:
+            pulumi.set(__self__, "app_excludes", app_excludes)
+        if app_includes is not None:
+            pulumi.set(__self__, "app_includes", app_includes)
+        if enroll is not None:
+            pulumi.set(__self__, "enroll", enroll)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if network_connection is not None:
+            pulumi.set(__self__, "network_connection", network_connection)
+        if network_excludes is not None:
+            pulumi.set(__self__, "network_excludes", network_excludes)
+        if network_includes is not None:
+            pulumi.set(__self__, "network_includes", network_includes)
+        if policy_id is not None:
+            pulumi.set(__self__, "policy_id", policy_id)
+        if priority is not None:
+            pulumi.set(__self__, "priority", priority)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+        if users_excludeds is not None:
+            pulumi.set(__self__, "users_excludeds", users_excludeds)
 
     @property
-    @pulumi.getter
-    def id(self) -> str:
+    @pulumi.getter(name="appExcludes")
+    def app_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]:
         """
-        Behavior ID.
+        Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+        - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+        is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+        of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "app_excludes")
 
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Behavior name.
-        """
-        return pulumi.get(self, "name")
+    @app_excludes.setter
+    def app_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]):
+        pulumi.set(self, "app_excludes", value)
 
     @property
-    @pulumi.getter
-    def settings(self) -> Mapping[str, str]:
+    @pulumi.getter(name="appIncludes")
+    def app_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]]:
         """
-        Map of behavior settings.
+        Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         """
-        return pulumi.get(self, "settings")
+        return pulumi.get(self, "app_includes")
 
-    @property
-    @pulumi.getter
-    def status(self) -> str:
-        """
-        Behavior status.
-        """
-        return pulumi.get(self, "status")
+    @app_includes.setter
+    def app_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]]):
+        pulumi.set(self, "app_includes", value)
 
     @property
     @pulumi.getter
-    def type(self) -> str:
+    def enroll(self) -> Optional[pulumi.Input[str]]:
         """
-        Behavior type.
+        When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
         """
-        return pulumi.get(self, "type")
-
+        return pulumi.get(self, "enroll")
 
-@pulumi.output_type
-class GetBrandsBrandResult(dict):
-    def __init__(__self__, *,
-                 custom_privacy_policy_url: str,
-                 id: str,
-                 links: str,
-                 name: str,
-                 remove_powered_by_okta: bool):
-        """
-        :param str custom_privacy_policy_url: Custom privacy policy URL
-        :param str id: The ID of the Brand
-        :param str links: Link relations for this object - JSON HAL - Discoverable resources related to the brand
-        :param str name: Brand name
-        :param bool remove_powered_by_okta: Removes "Powered by Okta" from the Okta-hosted sign-in page and "© 2021 Okta, Inc." from the Okta End-User Dashboard
-        """
-        pulumi.set(__self__, "custom_privacy_policy_url", custom_privacy_policy_url)
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "links", links)
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "remove_powered_by_okta", remove_powered_by_okta)
-
-    @property
-    @pulumi.getter(name="customPrivacyPolicyUrl")
-    def custom_privacy_policy_url(self) -> str:
-        """
-        Custom privacy policy URL
-        """
-        return pulumi.get(self, "custom_privacy_policy_url")
+    @enroll.setter
+    def enroll(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "enroll", value)
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the Brand
-        """
-        return pulumi.get(self, "id")
-
-    @property
-    @pulumi.getter
-    def links(self) -> str:
-        """
-        Link relations for this object - JSON HAL - Discoverable resources related to the brand
-        """
-        return pulumi.get(self, "links")
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Brand name
+        Policy Rule Name.
         """
         return pulumi.get(self, "name")
 
-    @property
-    @pulumi.getter(name="removePoweredByOkta")
-    def remove_powered_by_okta(self) -> bool:
-        """
-        Removes "Powered by Okta" from the Okta-hosted sign-in page and "© 2021 Okta, Inc." from the Okta End-User Dashboard
-        """
-        return pulumi.get(self, "remove_powered_by_okta")
-
-
-@pulumi.output_type
-class GetEmailCustomizationsEmailCustomizationResult(dict):
-    def __init__(__self__, *,
-                 body: str,
-                 id: str,
-                 is_default: bool,
-                 language: str,
-                 links: str,
-                 subject: str):
-        """
-        :param str body: The body of the customization
-        :param str id: The ID of the customization
-        :param bool is_default: Whether the customization is the default
-        :param str language: The language supported by the customization
-        :param str links: Link relations for this object - JSON HAL - Discoverable resources related to the email template
-        :param str subject: The subject of the customization
-        """
-        pulumi.set(__self__, "body", body)
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "is_default", is_default)
-        pulumi.set(__self__, "language", language)
-        pulumi.set(__self__, "links", links)
-        pulumi.set(__self__, "subject", subject)
-
-    @property
-    @pulumi.getter
-    def body(self) -> str:
-        """
-        The body of the customization
-        """
-        return pulumi.get(self, "body")
-
-    @property
-    @pulumi.getter
-    def id(self) -> str:
-        """
-        The ID of the customization
-        """
-        return pulumi.get(self, "id")
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="isDefault")
-    def is_default(self) -> bool:
+    @pulumi.getter(name="networkConnection")
+    def network_connection(self) -> Optional[pulumi.Input[str]]:
         """
-        Whether the customization is the default
+        Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         """
-        return pulumi.get(self, "is_default")
+        return pulumi.get(self, "network_connection")
 
-    @property
-    @pulumi.getter
-    def language(self) -> str:
-        """
-        The language supported by the customization
-        """
-        return pulumi.get(self, "language")
+    @network_connection.setter
+    def network_connection(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network_connection", value)
 
     @property
-    @pulumi.getter
-    def links(self) -> str:
+    @pulumi.getter(name="networkExcludes")
+    def network_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Link relations for this object - JSON HAL - Discoverable resources related to the email template
+        The network zones to exclude. Conflicts with `network_includes`.
         """
-        return pulumi.get(self, "links")
+        return pulumi.get(self, "network_excludes")
 
-    @property
-    @pulumi.getter
-    def subject(self) -> str:
-        """
-        The subject of the customization
-        """
-        return pulumi.get(self, "subject")
-
-
-@pulumi.output_type
-class GetGroupsGroupResult(dict):
-    def __init__(__self__, *,
-                 custom_profile_attributes: str,
-                 description: str,
-                 id: str,
-                 name: str,
-                 type: str):
-        """
-        :param str custom_profile_attributes: raw JSON containing all custom profile attributes. Likely only useful on groups of type `APP_GROUP`.
-        :param str description: Group description.
-        :param str id: Group ID.
-        :param str name: Group name.
-        :param str type: type of the group to retrieve. Can only be one of `OKTA_GROUP` (Native Okta Groups), `APP_GROUP`
-               (Imported App Groups), or `BUILT_IN` (Okta System Groups).
-        """
-        pulumi.set(__self__, "custom_profile_attributes", custom_profile_attributes)
-        pulumi.set(__self__, "description", description)
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "type", type)
+    @network_excludes.setter
+    def network_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "network_excludes", value)
 
     @property
-    @pulumi.getter(name="customProfileAttributes")
-    def custom_profile_attributes(self) -> str:
+    @pulumi.getter(name="networkIncludes")
+    def network_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        raw JSON containing all custom profile attributes. Likely only useful on groups of type `APP_GROUP`.
+        The network zones to include. Conflicts with `network_excludes`.
         """
-        return pulumi.get(self, "custom_profile_attributes")
+        return pulumi.get(self, "network_includes")
 
-    @property
-    @pulumi.getter
-    def description(self) -> str:
-        """
-        Group description.
-        """
-        return pulumi.get(self, "description")
+    @network_includes.setter
+    def network_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "network_includes", value)
 
     @property
-    @pulumi.getter
-    def id(self) -> str:
+    @pulumi.getter(name="policyId")
+    def policy_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Group ID.
+        Policy ID.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "policy_id")
 
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Group name.
-        """
-        return pulumi.get(self, "name")
+    @policy_id.setter
+    def policy_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "policy_id", value)
 
     @property
     @pulumi.getter
-    def type(self) -> str:
+    def priority(self) -> Optional[pulumi.Input[int]]:
         """
-        type of the group to retrieve. Can only be one of `OKTA_GROUP` (Native Okta Groups), `APP_GROUP`
-        (Imported App Groups), or `BUILT_IN` (Okta System Groups).
+        Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         """
-        return pulumi.get(self, "type")
-
+        return pulumi.get(self, "priority")
 
-@pulumi.output_type
-class GetTemplatesEmailTemplateResult(dict):
-    def __init__(__self__, *,
-                 links: str,
-                 name: str):
-        """
-        :param str links: Link relations for this object - JSON HAL - Discoverable resources related to the email template
-        :param str name: The name of the email template
-        """
-        pulumi.set(__self__, "links", links)
-        pulumi.set(__self__, "name", name)
+    @priority.setter
+    def priority(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "priority", value)
 
     @property
     @pulumi.getter
-    def links(self) -> str:
-        """
-        Link relations for this object - JSON HAL - Discoverable resources related to the email template
+    def status(self) -> Optional[pulumi.Input[str]]:
         """
-        return pulumi.get(self, "links")
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
+        Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         """
-        The name of the email template
-        """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "status")
 
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
+
+    @property
+    @pulumi.getter(name="usersExcludeds")
+    def users_excludeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Set of User IDs to Exclude
+        """
+        return pulumi.get(self, "users_excludeds")
+
+    @users_excludeds.setter
+    def users_excludeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "users_excludeds", value)
+
+
+class RuleMfa(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]]] = None,
+                 app_includes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]]] = None,
+                 enroll: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_connection: Optional[pulumi.Input[str]] = None,
+                 network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 policy_id: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 __props__=None):
+        """
+        This resource allows you to create and configure an MFA Policy Rule.
+
+        ## Import
+
+        A Policy Rule can be imported via the Policy and Rule ID.
+
+        ```sh
+        $ pulumi import okta:policy/ruleMfa:RuleMfa example &#60;policy id&#62;/&#60;rule id&#62;
+        ```
+
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
+        :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
+        :param pulumi.Input[str] name: Policy Rule Name.
+        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
+        :param pulumi.Input[str] policy_id: Policy ID.
+        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
+        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: Optional[RuleMfaArgs] = None,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        This resource allows you to create and configure an MFA Policy Rule.
+
+        ## Import
+
+        A Policy Rule can be imported via the Policy and Rule ID.
+
+        ```sh
+        $ pulumi import okta:policy/ruleMfa:RuleMfa example &#60;policy id&#62;/&#60;rule id&#62;
+        ```
+
+        :param str resource_name: The name of the resource.
+        :param RuleMfaArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(RuleMfaArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]]] = None,
+                 app_includes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]]] = None,
+                 enroll: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_connection: Optional[pulumi.Input[str]] = None,
+                 network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 policy_id: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = RuleMfaArgs.__new__(RuleMfaArgs)
+
+            __props__.__dict__["app_excludes"] = app_excludes
+            __props__.__dict__["app_includes"] = app_includes
+            __props__.__dict__["enroll"] = enroll
+            __props__.__dict__["name"] = name
+            __props__.__dict__["network_connection"] = network_connection
+            __props__.__dict__["network_excludes"] = network_excludes
+            __props__.__dict__["network_includes"] = network_includes
+            __props__.__dict__["policy_id"] = policy_id
+            __props__.__dict__["priority"] = priority
+            __props__.__dict__["status"] = status
+            __props__.__dict__["users_excludeds"] = users_excludeds
+        super(RuleMfa, __self__).__init__(
+            'okta:policy/ruleMfa:RuleMfa',
+            resource_name,
+            __props__,
+            opts)
 
-@pulumi.output_type
-class GetThemesThemeResult(dict):
-    def __init__(__self__, *,
-                 background_image_url: str,
-                 email_template_touch_point_variant: str,
-                 end_user_dashboard_touch_point_variant: str,
-                 error_page_touch_point_variant: str,
-                 favicon_url: str,
-                 id: str,
-                 links: str,
-                 logo_url: str,
-                 primary_color_contrast_hex: str,
-                 primary_color_hex: str,
-                 secondary_color_contrast_hex: str,
-                 secondary_color_hex: str,
-                 sign_in_page_touch_point_variant: str):
-        """
-        :param str background_image_url: Background image URL
-        :param str email_template_touch_point_variant: Variant for email templates (`OKTA_DEFAULT`, `FULL_THEME`)
-        :param str end_user_dashboard_touch_point_variant: Variant for the Okta End-User Dashboard (`OKTA_DEFAULT`, `WHITE_LOGO_BACKGROUND`, `FULL_THEME`, `LOGO_ON_FULL_WHITE_BACKGROUND`)
-        :param str error_page_touch_point_variant: Variant for the error page (`OKTA_DEFAULT`, `BACKGROUND_SECONDARY_COLOR`, `BACKGROUND_IMAGE`)
-        :param str favicon_url: Favicon URL
-        :param str id: The ID of the theme
-        :param str links: Link relations for this object - JSON HAL - Discoverable resources related to the email template
-        :param str logo_url: Logo URL
-        :param str primary_color_contrast_hex: Primary color contrast hex code
-        :param str primary_color_hex: Primary color hex code
-        :param str secondary_color_contrast_hex: Secondary color contrast hex code
-        :param str secondary_color_hex: Secondary color hex code
-        :param str sign_in_page_touch_point_variant: Variant for the Okta Sign-In Page (`OKTA_DEFAULT`, `BACKGROUND_SECONDARY_COLOR`, `BACKGROUND_IMAGE`)
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]]] = None,
+            app_includes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]]] = None,
+            enroll: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            network_connection: Optional[pulumi.Input[str]] = None,
+            network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            policy_id: Optional[pulumi.Input[str]] = None,
+            priority: Optional[pulumi.Input[int]] = None,
+            status: Optional[pulumi.Input[str]] = None,
+            users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'RuleMfa':
         """
-        pulumi.set(__self__, "background_image_url", background_image_url)
-        pulumi.set(__self__, "email_template_touch_point_variant", email_template_touch_point_variant)
-        pulumi.set(__self__, "end_user_dashboard_touch_point_variant", end_user_dashboard_touch_point_variant)
-        pulumi.set(__self__, "error_page_touch_point_variant", error_page_touch_point_variant)
-        pulumi.set(__self__, "favicon_url", favicon_url)
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "links", links)
-        pulumi.set(__self__, "logo_url", logo_url)
-        pulumi.set(__self__, "primary_color_contrast_hex", primary_color_contrast_hex)
-        pulumi.set(__self__, "primary_color_hex", primary_color_hex)
-        pulumi.set(__self__, "secondary_color_contrast_hex", secondary_color_contrast_hex)
-        pulumi.set(__self__, "secondary_color_hex", secondary_color_hex)
-        pulumi.set(__self__, "sign_in_page_touch_point_variant", sign_in_page_touch_point_variant)
+        Get an existing RuleMfa resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
 
-    @property
-    @pulumi.getter(name="backgroundImageUrl")
-    def background_image_url(self) -> str:
-        """
-        Background image URL
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
+        :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
+        :param pulumi.Input[str] name: Policy Rule Name.
+        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
+        :param pulumi.Input[str] policy_id: Policy ID.
+        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
+        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
         """
-        return pulumi.get(self, "background_image_url")
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-    @property
-    @pulumi.getter(name="emailTemplateTouchPointVariant")
-    def email_template_touch_point_variant(self) -> str:
-        """
-        Variant for email templates (`OKTA_DEFAULT`, `FULL_THEME`)
-        """
-        return pulumi.get(self, "email_template_touch_point_variant")
+        __props__ = _RuleMfaState.__new__(_RuleMfaState)
 
-    @property
-    @pulumi.getter(name="endUserDashboardTouchPointVariant")
-    def end_user_dashboard_touch_point_variant(self) -> str:
-        """
-        Variant for the Okta End-User Dashboard (`OKTA_DEFAULT`, `WHITE_LOGO_BACKGROUND`, `FULL_THEME`, `LOGO_ON_FULL_WHITE_BACKGROUND`)
-        """
-        return pulumi.get(self, "end_user_dashboard_touch_point_variant")
+        __props__.__dict__["app_excludes"] = app_excludes
+        __props__.__dict__["app_includes"] = app_includes
+        __props__.__dict__["enroll"] = enroll
+        __props__.__dict__["name"] = name
+        __props__.__dict__["network_connection"] = network_connection
+        __props__.__dict__["network_excludes"] = network_excludes
+        __props__.__dict__["network_includes"] = network_includes
+        __props__.__dict__["policy_id"] = policy_id
+        __props__.__dict__["priority"] = priority
+        __props__.__dict__["status"] = status
+        __props__.__dict__["users_excludeds"] = users_excludeds
+        return RuleMfa(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="errorPageTouchPointVariant")
-    def error_page_touch_point_variant(self) -> str:
+    @pulumi.getter(name="appExcludes")
+    def app_excludes(self) -> pulumi.Output[Optional[Sequence['outputs.RuleMfaAppExclude']]]:
         """
-        Variant for the error page (`OKTA_DEFAULT`, `BACKGROUND_SECONDARY_COLOR`, `BACKGROUND_IMAGE`)
+        Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+        - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+        is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+        of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         """
-        return pulumi.get(self, "error_page_touch_point_variant")
+        return pulumi.get(self, "app_excludes")
 
     @property
-    @pulumi.getter(name="faviconUrl")
-    def favicon_url(self) -> str:
+    @pulumi.getter(name="appIncludes")
+    def app_includes(self) -> pulumi.Output[Optional[Sequence['outputs.RuleMfaAppInclude']]]:
         """
-        Favicon URL
+        Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         """
-        return pulumi.get(self, "favicon_url")
+        return pulumi.get(self, "app_includes")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def enroll(self) -> pulumi.Output[Optional[str]]:
         """
-        The ID of the theme
+        When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "enroll")
 
     @property
     @pulumi.getter
-    def links(self) -> str:
-        """
-        Link relations for this object - JSON HAL - Discoverable resources related to the email template
-        """
-        return pulumi.get(self, "links")
-
-    @property
-    @pulumi.getter(name="logoUrl")
-    def logo_url(self) -> str:
-        """
-        Logo URL
-        """
-        return pulumi.get(self, "logo_url")
-
-    @property
-    @pulumi.getter(name="primaryColorContrastHex")
-    def primary_color_contrast_hex(self) -> str:
-        """
-        Primary color contrast hex code
-        """
-        return pulumi.get(self, "primary_color_contrast_hex")
-
-    @property
-    @pulumi.getter(name="primaryColorHex")
-    def primary_color_hex(self) -> str:
-        """
-        Primary color hex code
-        """
-        return pulumi.get(self, "primary_color_hex")
-
-    @property
-    @pulumi.getter(name="secondaryColorContrastHex")
-    def secondary_color_contrast_hex(self) -> str:
-        """
-        Secondary color contrast hex code
-        """
-        return pulumi.get(self, "secondary_color_contrast_hex")
-
-    @property
-    @pulumi.getter(name="secondaryColorHex")
-    def secondary_color_hex(self) -> str:
+    def name(self) -> pulumi.Output[str]:
         """
-        Secondary color hex code
+        Policy Rule Name.
         """
-        return pulumi.get(self, "secondary_color_hex")
-
-    @property
-    @pulumi.getter(name="signInPageTouchPointVariant")
-    def sign_in_page_touch_point_variant(self) -> str:
-        """
-        Variant for the Okta Sign-In Page (`OKTA_DEFAULT`, `BACKGROUND_SECONDARY_COLOR`, `BACKGROUND_IMAGE`)
-        """
-        return pulumi.get(self, "sign_in_page_touch_point_variant")
-
-
-@pulumi.output_type
-class GetTrustedOriginsTrustedOriginResult(dict):
-    def __init__(__self__, *,
-                 active: bool,
-                 id: str,
-                 name: str,
-                 origin: str,
-                 scopes: Sequence[str]):
-        """
-        :param bool active: Whether the Trusted Origin is active or not - can only be issued post-creation
-        :param str id: The ID of the Trusted Origin.
-        :param str name: Unique name for this trusted origin.
-        :param str origin: Unique origin URL for this trusted origin.
-        :param Sequence[str] scopes: Scopes of the Trusted Origin
-        """
-        pulumi.set(__self__, "active", active)
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "origin", origin)
-        pulumi.set(__self__, "scopes", scopes)
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def active(self) -> bool:
+    @pulumi.getter(name="networkConnection")
+    def network_connection(self) -> pulumi.Output[Optional[str]]:
         """
-        Whether the Trusted Origin is active or not - can only be issued post-creation
+        Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         """
-        return pulumi.get(self, "active")
+        return pulumi.get(self, "network_connection")
 
     @property
-    @pulumi.getter
-    def id(self) -> str:
+    @pulumi.getter(name="networkExcludes")
+    def network_excludes(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        The ID of the Trusted Origin.
+        The network zones to exclude. Conflicts with `network_includes`.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "network_excludes")
 
     @property
-    @pulumi.getter
-    def name(self) -> str:
+    @pulumi.getter(name="networkIncludes")
+    def network_includes(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        Unique name for this trusted origin.
+        The network zones to include. Conflicts with `network_excludes`.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "network_includes")
 
     @property
-    @pulumi.getter
-    def origin(self) -> str:
+    @pulumi.getter(name="policyId")
+    def policy_id(self) -> pulumi.Output[Optional[str]]:
         """
-        Unique origin URL for this trusted origin.
+        Policy ID.
         """
-        return pulumi.get(self, "origin")
+        return pulumi.get(self, "policy_id")
 
     @property
     @pulumi.getter
-    def scopes(self) -> Sequence[str]:
-        """
-        Scopes of the Trusted Origin
+    def priority(self) -> pulumi.Output[Optional[int]]:
         """
-        return pulumi.get(self, "scopes")
-
-
-@pulumi.output_type
-class GetUserSecurityQuestionsQuestionResult(dict):
-    def __init__(__self__, *,
-                 key: str,
-                 text: str):
+        Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         """
-        :param str key: Security question unique key.
-        :param str text: Display text for security question.
-        """
-        pulumi.set(__self__, "key", key)
-        pulumi.set(__self__, "text", text)
+        return pulumi.get(self, "priority")
 
     @property
     @pulumi.getter
-    def key(self) -> str:
+    def status(self) -> pulumi.Output[Optional[str]]:
         """
-        Security question unique key.
+        Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "status")
 
     @property
-    @pulumi.getter
-    def text(self) -> str:
+    @pulumi.getter(name="usersExcludeds")
+    def users_excludeds(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        Display text for security question.
+        Set of User IDs to Exclude
         """
-        return pulumi.get(self, "text")
-
+        return pulumi.get(self, "users_excludeds")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/signon.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,410 +5,375 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = [
-    'RuleIdpDiscoveryAppExcludeArgs',
-    'RuleIdpDiscoveryAppIncludeArgs',
-    'RuleIdpDiscoveryPlatformIncludeArgs',
-    'RuleIdpDiscoveryUserIdentifierPatternArgs',
-    'RuleMfaAppExcludeArgs',
-    'RuleMfaAppIncludeArgs',
-    'RuleSignonFactorSequenceArgs',
-    'RuleSignonFactorSequenceSecondaryCriteriaArgs',
-]
+__all__ = ['SignonArgs', 'Signon']
 
 @pulumi.input_type
-class RuleIdpDiscoveryAppExcludeArgs:
+class SignonArgs:
     def __init__(__self__, *,
-                 type: pulumi.Input[str],
-                 id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] id: ID of the Rule.
-        :param pulumi.Input[str] name: Policy rule name.
-        """
-        pulumi.set(__self__, "type", type)
-        if id is not None:
-            pulumi.set(__self__, "id", id)
+                 description: Optional[pulumi.Input[str]] = None,
+                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a Signon resource.
+        :param pulumi.Input[str] description: Policy Description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
+        :param pulumi.Input[str] name: Policy Name.
+        :param pulumi.Input[int] priority: Priority of the policy.
+        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if groups_includeds is not None:
+            pulumi.set(__self__, "groups_includeds", groups_includeds)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if priority is not None:
+            pulumi.set(__self__, "priority", priority)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "type")
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        Policy Description.
+        """
+        return pulumi.get(self, "description")
 
-    @type.setter
-    def type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "type", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="groupsIncludeds")
+    def groups_includeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        ID of the Rule.
+        List of Group IDs to Include.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "groups_includeds")
 
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
+    @groups_includeds.setter
+    def groups_includeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "groups_includeds", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy rule name.
+        Policy Name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
-
-@pulumi.input_type
-class RuleIdpDiscoveryAppIncludeArgs:
-    def __init__(__self__, *,
-                 type: pulumi.Input[str],
-                 id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] type: One of: `"APP"`, `"APP_TYPE"`
-        :param pulumi.Input[str] id: Use if `type` is `"APP"` to indicate the application id to include.
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
-        """
-        pulumi.set(__self__, "type", type)
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Input[str]:
+    def priority(self) -> Optional[pulumi.Input[int]]:
         """
-        One of: `"APP"`, `"APP_TYPE"`
+        Priority of the policy.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "priority")
 
-    @type.setter
-    def type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "type", value)
+    @priority.setter
+    def priority(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "priority", value)
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
+    def status(self) -> Optional[pulumi.Input[str]]:
         """
-        Use if `type` is `"APP"` to indicate the application id to include.
+        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "status")
 
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
-
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
 
 
 @pulumi.input_type
-class RuleIdpDiscoveryPlatformIncludeArgs:
+class _SignonState:
     def __init__(__self__, *,
-                 os_expression: Optional[pulumi.Input[str]] = None,
-                 os_type: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] os_expression: Only available when using `os_type = "OTHER"`
-        :param pulumi.Input[str] os_type: One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`
-        :param pulumi.Input[str] type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
-        """
-        if os_expression is not None:
-            pulumi.set(__self__, "os_expression", os_expression)
-        if os_type is not None:
-            pulumi.set(__self__, "os_type", os_type)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
+                 description: Optional[pulumi.Input[str]] = None,
+                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering Signon resources.
+        :param pulumi.Input[str] description: Policy Description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
+        :param pulumi.Input[str] name: Policy Name.
+        :param pulumi.Input[int] priority: Priority of the policy.
+        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if groups_includeds is not None:
+            pulumi.set(__self__, "groups_includeds", groups_includeds)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if priority is not None:
+            pulumi.set(__self__, "priority", priority)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
 
     @property
-    @pulumi.getter(name="osExpression")
-    def os_expression(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Only available when using `os_type = "OTHER"`
+        Policy Description.
         """
-        return pulumi.get(self, "os_expression")
+        return pulumi.get(self, "description")
 
-    @os_expression.setter
-    def os_expression(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "os_expression", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="osType")
-    def os_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="groupsIncludeds")
+    def groups_includeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`
+        List of Group IDs to Include.
         """
-        return pulumi.get(self, "os_type")
+        return pulumi.get(self, "groups_includeds")
 
-    @os_type.setter
-    def os_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "os_type", value)
+    @groups_includeds.setter
+    def groups_includeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "groups_includeds", value)
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
+        Policy Name.
         """
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
-
+        return pulumi.get(self, "name")
 
-@pulumi.input_type
-class RuleIdpDiscoveryUserIdentifierPatternArgs:
-    def __init__(__self__, *,
-                 match_type: Optional[pulumi.Input[str]] = None,
-                 value: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] match_type: The kind of pattern. For regex, use `"EXPRESSION"`. For simple string matches, use one of the following: `"SUFFIX"`, `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`
-        :param pulumi.Input[str] value: The regex or simple match string to match against.
-        """
-        if match_type is not None:
-            pulumi.set(__self__, "match_type", match_type)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="matchType")
-    def match_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def priority(self) -> Optional[pulumi.Input[int]]:
         """
-        The kind of pattern. For regex, use `"EXPRESSION"`. For simple string matches, use one of the following: `"SUFFIX"`, `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`
+        Priority of the policy.
         """
-        return pulumi.get(self, "match_type")
+        return pulumi.get(self, "priority")
 
-    @match_type.setter
-    def match_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "match_type", value)
+    @priority.setter
+    def priority(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "priority", value)
 
     @property
     @pulumi.getter
-    def value(self) -> Optional[pulumi.Input[str]]:
+    def status(self) -> Optional[pulumi.Input[str]]:
         """
-        The regex or simple match string to match against.
+        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
         """
-        return pulumi.get(self, "value")
+        return pulumi.get(self, "status")
 
-    @value.setter
-    def value(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "value", value)
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
 
 
-@pulumi.input_type
-class RuleMfaAppExcludeArgs:
-    def __init__(__self__, *,
-                 type: pulumi.Input[str],
-                 id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] id: ID of the Rule.
-        :param pulumi.Input[str] name: Policy Rule Name.
-        """
-        pulumi.set(__self__, "type", type)
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+class Signon(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        """
+        Creates a Sign On Policy.
 
-    @property
-    @pulumi.getter
-    def type(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "type")
+        This resource allows you to create and configure a Sign On Policy.
 
-    @type.setter
-    def type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "type", value)
+        ## Example Usage
 
-    @property
-    @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
-        """
-        ID of the Rule.
-        """
-        return pulumi.get(self, "id")
+        ```python
+        import pulumi
+        import pulumi_okta as okta
 
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
+        example = okta.policy.Signon("example",
+            name="example",
+            status="ACTIVE",
+            description="Example",
+            groups_includeds=[everyone["id"]])
+        ```
 
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+        ## Import
+
+        A Sign On Policy can be imported via the Okta ID.
+
+        ```sh
+        $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
+        ```
+
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] description: Policy Description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
+        :param pulumi.Input[str] name: Policy Name.
+        :param pulumi.Input[int] priority: Priority of the policy.
+        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
         """
-        Policy Rule Name.
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: Optional[SignonArgs] = None,
+                 opts: Optional[pulumi.ResourceOptions] = None):
         """
-        return pulumi.get(self, "name")
+        Creates a Sign On Policy.
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+        This resource allows you to create and configure a Sign On Policy.
 
+        ## Example Usage
 
-@pulumi.input_type
-class RuleMfaAppIncludeArgs:
-    def __init__(__self__, *,
-                 type: pulumi.Input[str],
-                 id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] type: One of: `"APP"`, `"APP_TYPE"`
-        :param pulumi.Input[str] id: Use if `type` is `"APP"` to indicate the application id to include.
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
-        """
-        pulumi.set(__self__, "type", type)
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+        ```python
+        import pulumi
+        import pulumi_okta as okta
 
-    @property
-    @pulumi.getter
-    def type(self) -> pulumi.Input[str]:
-        """
-        One of: `"APP"`, `"APP_TYPE"`
-        """
-        return pulumi.get(self, "type")
+        example = okta.policy.Signon("example",
+            name="example",
+            status="ACTIVE",
+            description="Example",
+            groups_includeds=[everyone["id"]])
+        ```
 
-    @type.setter
-    def type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "type", value)
+        ## Import
 
-    @property
-    @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
-        """
-        Use if `type` is `"APP"` to indicate the application id to include.
-        """
-        return pulumi.get(self, "id")
+        A Sign On Policy can be imported via the Okta ID.
 
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
+        ```sh
+        $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
+        ```
 
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+        :param str resource_name: The name of the resource.
+        :param SignonArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
-        """
-        return pulumi.get(self, "name")
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(SignonArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = SignonArgs.__new__(SignonArgs)
 
+            __props__.__dict__["description"] = description
+            __props__.__dict__["groups_includeds"] = groups_includeds
+            __props__.__dict__["name"] = name
+            __props__.__dict__["priority"] = priority
+            __props__.__dict__["status"] = status
+        super(Signon, __self__).__init__(
+            'okta:policy/signon:Signon',
+            resource_name,
+            __props__,
+            opts)
 
-@pulumi.input_type
-class RuleSignonFactorSequenceArgs:
-    def __init__(__self__, *,
-                 primary_criteria_factor_type: pulumi.Input[str],
-                 primary_criteria_provider: pulumi.Input[str],
-                 secondary_criterias: Optional[pulumi.Input[Sequence[pulumi.Input['RuleSignonFactorSequenceSecondaryCriteriaArgs']]]] = None):
-        """
-        :param pulumi.Input[str] primary_criteria_factor_type: Primary factor type of the auth section.
-        :param pulumi.Input[str] primary_criteria_provider: Primary provider of the auth section.
-        :param pulumi.Input[Sequence[pulumi.Input['RuleSignonFactorSequenceSecondaryCriteriaArgs']]] secondary_criterias: Additional authentication steps.
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            description: Optional[pulumi.Input[str]] = None,
+            groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            priority: Optional[pulumi.Input[int]] = None,
+            status: Optional[pulumi.Input[str]] = None) -> 'Signon':
         """
-        pulumi.set(__self__, "primary_criteria_factor_type", primary_criteria_factor_type)
-        pulumi.set(__self__, "primary_criteria_provider", primary_criteria_provider)
-        if secondary_criterias is not None:
-            pulumi.set(__self__, "secondary_criterias", secondary_criterias)
+        Get an existing Signon resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
 
-    @property
-    @pulumi.getter(name="primaryCriteriaFactorType")
-    def primary_criteria_factor_type(self) -> pulumi.Input[str]:
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] description: Policy Description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
+        :param pulumi.Input[str] name: Policy Name.
+        :param pulumi.Input[int] priority: Priority of the policy.
+        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
         """
-        Primary factor type of the auth section.
-        """
-        return pulumi.get(self, "primary_criteria_factor_type")
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = _SignonState.__new__(_SignonState)
 
-    @primary_criteria_factor_type.setter
-    def primary_criteria_factor_type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "primary_criteria_factor_type", value)
+        __props__.__dict__["description"] = description
+        __props__.__dict__["groups_includeds"] = groups_includeds
+        __props__.__dict__["name"] = name
+        __props__.__dict__["priority"] = priority
+        __props__.__dict__["status"] = status
+        return Signon(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="primaryCriteriaProvider")
-    def primary_criteria_provider(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
         """
-        Primary provider of the auth section.
+        Policy Description.
         """
-        return pulumi.get(self, "primary_criteria_provider")
-
-    @primary_criteria_provider.setter
-    def primary_criteria_provider(self, value: pulumi.Input[str]):
-        pulumi.set(self, "primary_criteria_provider", value)
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="secondaryCriterias")
-    def secondary_criterias(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleSignonFactorSequenceSecondaryCriteriaArgs']]]]:
+    @pulumi.getter(name="groupsIncludeds")
+    def groups_includeds(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        Additional authentication steps.
+        List of Group IDs to Include.
         """
-        return pulumi.get(self, "secondary_criterias")
-
-    @secondary_criterias.setter
-    def secondary_criterias(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleSignonFactorSequenceSecondaryCriteriaArgs']]]]):
-        pulumi.set(self, "secondary_criterias", value)
-
+        return pulumi.get(self, "groups_includeds")
 
-@pulumi.input_type
-class RuleSignonFactorSequenceSecondaryCriteriaArgs:
-    def __init__(__self__, *,
-                 factor_type: pulumi.Input[str],
-                 provider: pulumi.Input[str]):
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
         """
-        :param pulumi.Input[str] factor_type: Type of a Factor
-        :param pulumi.Input[str] provider: Factor provider
+        Policy Name.
         """
-        pulumi.set(__self__, "factor_type", factor_type)
-        pulumi.set(__self__, "provider", provider)
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="factorType")
-    def factor_type(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def priority(self) -> pulumi.Output[Optional[int]]:
         """
-        Type of a Factor
+        Priority of the policy.
         """
-        return pulumi.get(self, "factor_type")
-
-    @factor_type.setter
-    def factor_type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "factor_type", value)
+        return pulumi.get(self, "priority")
 
     @property
     @pulumi.getter
-    def provider(self) -> pulumi.Input[str]:
+    def status(self) -> pulumi.Output[Optional[str]]:
         """
-        Factor provider
+        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
         """
-        return pulumi.get(self, "provider")
-
-    @provider.setter
-    def provider(self, value: pulumi.Input[str]):
-        pulumi.set(self, "provider", value)
-
+        return pulumi.get(self, "status")
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_android.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_android.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_chromeos.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_chromeos.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_ios.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_ios.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_macos.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_macos.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/device_assurance_windows.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_windows.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/get_default_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/get_policy.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,14 +93,22 @@
         type="PASSWORD")
     ```
 
 
     :param str name: Name of policy to retrieve.
     :param str type: Type of policy to retrieve. See https://developer.okta.com/docs/reference/api/policy/#policy-object for valid values. Currently:
            - All:
+           - `OKTA_SIGN_ON`
+           - `PASSWORD`
+           - `MFA_ENROLL`
+           - `OAUTH_AUTHORIZATION_POLICY`
+           - `IDP_DISCOVERY`
+           - OIE Only:
+           - `ACCESS_POLICY`
+           - `PROFILE_ENROLLMENT`
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:policy/getPolicy:getPolicy', __args__, opts=opts, typ=GetPolicyResult).value
 
@@ -128,9 +136,17 @@
         type="PASSWORD")
     ```
 
 
     :param str name: Name of policy to retrieve.
     :param str type: Type of policy to retrieve. See https://developer.okta.com/docs/reference/api/policy/#policy-object for valid values. Currently:
            - All:
+           - `OKTA_SIGN_ON`
+           - `PASSWORD`
+           - `MFA_ENROLL`
+           - `OAUTH_AUTHORIZATION_POLICY`
+           - `IDP_DISCOVERY`
+           - OIE Only:
+           - `ACCESS_POLICY`
+           - `PROFILE_ENROLLMENT`
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/password.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_password.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,161 +4,153 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
-from ._inputs import *
 
-__all__ = ['RuleMfaArgs', 'RuleMfa']
+__all__ = ['RulePasswordArgs', 'RulePassword']
 
 @pulumi.input_type
-class RuleMfaArgs:
+class RulePasswordArgs:
     def __init__(__self__, *,
-                 app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]] = None,
-                 app_includes: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]] = None,
-                 enroll: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_connection: Optional[pulumi.Input[str]] = None,
                  network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 password_change: Optional[pulumi.Input[str]] = None,
+                 password_reset: Optional[pulumi.Input[str]] = None,
+                 password_unlock: Optional[pulumi.Input[str]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a RuleMfa resource.
-        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
-               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
-               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
-               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
-        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
-        :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        :param pulumi.Input[str] name: Policy Rule Name.
-        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
+        The set of arguments for constructing a RulePassword resource.
+        :param pulumi.Input[str] name: Policy Rule Name. Type `"string"`
+        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`. Type `"string"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`. Type `"list(string)"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`. Type `"list(string)"`
+        :param pulumi.Input[str] password_change: Allow or deny a user to change their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        :param pulumi.Input[str] password_reset: Allow or deny a user to reset their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        :param pulumi.Input[str] password_unlock: Allow or deny a user to unlock: `"ALLOW"` or `"DENY"`. By default, it is `"DENY"`, Type `"string"`
         :param pulumi.Input[str] policy_id: Policy ID.
-        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
-        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
-        """
-        if app_excludes is not None:
-            pulumi.set(__self__, "app_excludes", app_excludes)
-        if app_includes is not None:
-            pulumi.set(__self__, "app_includes", app_includes)
-        if enroll is not None:
-            pulumi.set(__self__, "enroll", enroll)
+        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there. Type `"number"`
+        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`. Type `"string"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: The users to exclude. Type `"set(string)"`
+        """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if network_connection is not None:
             pulumi.set(__self__, "network_connection", network_connection)
         if network_excludes is not None:
             pulumi.set(__self__, "network_excludes", network_excludes)
         if network_includes is not None:
             pulumi.set(__self__, "network_includes", network_includes)
+        if password_change is not None:
+            pulumi.set(__self__, "password_change", password_change)
+        if password_reset is not None:
+            pulumi.set(__self__, "password_reset", password_reset)
+        if password_unlock is not None:
+            pulumi.set(__self__, "password_unlock", password_unlock)
         if policy_id is not None:
             pulumi.set(__self__, "policy_id", policy_id)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if users_excludeds is not None:
             pulumi.set(__self__, "users_excludeds", users_excludeds)
 
     @property
-    @pulumi.getter(name="appExcludes")
-    def app_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]:
-        """
-        Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
-        - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
-        is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
-        of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
-        """
-        return pulumi.get(self, "app_excludes")
-
-    @app_excludes.setter
-    def app_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]):
-        pulumi.set(self, "app_excludes", value)
-
-    @property
-    @pulumi.getter(name="appIncludes")
-    def app_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]]:
-        """
-        Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
-        """
-        return pulumi.get(self, "app_includes")
-
-    @app_includes.setter
-    def app_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]]):
-        pulumi.set(self, "app_includes", value)
-
-    @property
-    @pulumi.getter
-    def enroll(self) -> Optional[pulumi.Input[str]]:
-        """
-        When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        """
-        return pulumi.get(self, "enroll")
-
-    @enroll.setter
-    def enroll(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "enroll", value)
-
-    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy Rule Name.
+        Policy Rule Name. Type `"string"`
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="networkConnection")
     def network_connection(self) -> Optional[pulumi.Input[str]]:
         """
-        Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
+        Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`. Type `"string"`
         """
         return pulumi.get(self, "network_connection")
 
     @network_connection.setter
     def network_connection(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_connection", value)
 
     @property
     @pulumi.getter(name="networkExcludes")
     def network_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The network zones to exclude. Conflicts with `network_includes`.
+        The network zones to exclude. Conflicts with `network_includes`. Type `"list(string)"`
         """
         return pulumi.get(self, "network_excludes")
 
     @network_excludes.setter
     def network_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "network_excludes", value)
 
     @property
     @pulumi.getter(name="networkIncludes")
     def network_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The network zones to include. Conflicts with `network_excludes`.
+        The network zones to include. Conflicts with `network_excludes`. Type `"list(string)"`
         """
         return pulumi.get(self, "network_includes")
 
     @network_includes.setter
     def network_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "network_includes", value)
 
     @property
+    @pulumi.getter(name="passwordChange")
+    def password_change(self) -> Optional[pulumi.Input[str]]:
+        """
+        Allow or deny a user to change their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        """
+        return pulumi.get(self, "password_change")
+
+    @password_change.setter
+    def password_change(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password_change", value)
+
+    @property
+    @pulumi.getter(name="passwordReset")
+    def password_reset(self) -> Optional[pulumi.Input[str]]:
+        """
+        Allow or deny a user to reset their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        """
+        return pulumi.get(self, "password_reset")
+
+    @password_reset.setter
+    def password_reset(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password_reset", value)
+
+    @property
+    @pulumi.getter(name="passwordUnlock")
+    def password_unlock(self) -> Optional[pulumi.Input[str]]:
+        """
+        Allow or deny a user to unlock: `"ALLOW"` or `"DENY"`. By default, it is `"DENY"`, Type `"string"`
+        """
+        return pulumi.get(self, "password_unlock")
+
+    @password_unlock.setter
+    def password_unlock(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password_unlock", value)
+
+    @property
     @pulumi.getter(name="policyId")
     def policy_id(self) -> Optional[pulumi.Input[str]]:
         """
         Policy ID.
         """
         return pulumi.get(self, "policy_id")
 
@@ -166,189 +158,183 @@
     def policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy_id", value)
 
     @property
     @pulumi.getter
     def priority(self) -> Optional[pulumi.Input[int]]:
         """
-        Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
+        Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there. Type `"number"`
         """
         return pulumi.get(self, "priority")
 
     @priority.setter
     def priority(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "priority", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
+        Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`. Type `"string"`
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
     @property
     @pulumi.getter(name="usersExcludeds")
     def users_excludeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Set of User IDs to Exclude
+        The users to exclude. Type `"set(string)"`
         """
         return pulumi.get(self, "users_excludeds")
 
     @users_excludeds.setter
     def users_excludeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "users_excludeds", value)
 
 
 @pulumi.input_type
-class _RuleMfaState:
+class _RulePasswordState:
     def __init__(__self__, *,
-                 app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]] = None,
-                 app_includes: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]] = None,
-                 enroll: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_connection: Optional[pulumi.Input[str]] = None,
                  network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 password_change: Optional[pulumi.Input[str]] = None,
+                 password_reset: Optional[pulumi.Input[str]] = None,
+                 password_unlock: Optional[pulumi.Input[str]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering RuleMfa resources.
-        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
-               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
-               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
-               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
-        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
-        :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        :param pulumi.Input[str] name: Policy Rule Name.
-        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
+        Input properties used for looking up and filtering RulePassword resources.
+        :param pulumi.Input[str] name: Policy Rule Name. Type `"string"`
+        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`. Type `"string"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`. Type `"list(string)"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`. Type `"list(string)"`
+        :param pulumi.Input[str] password_change: Allow or deny a user to change their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        :param pulumi.Input[str] password_reset: Allow or deny a user to reset their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        :param pulumi.Input[str] password_unlock: Allow or deny a user to unlock: `"ALLOW"` or `"DENY"`. By default, it is `"DENY"`, Type `"string"`
         :param pulumi.Input[str] policy_id: Policy ID.
-        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
-        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
-        """
-        if app_excludes is not None:
-            pulumi.set(__self__, "app_excludes", app_excludes)
-        if app_includes is not None:
-            pulumi.set(__self__, "app_includes", app_includes)
-        if enroll is not None:
-            pulumi.set(__self__, "enroll", enroll)
+        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there. Type `"number"`
+        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`. Type `"string"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: The users to exclude. Type `"set(string)"`
+        """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if network_connection is not None:
             pulumi.set(__self__, "network_connection", network_connection)
         if network_excludes is not None:
             pulumi.set(__self__, "network_excludes", network_excludes)
         if network_includes is not None:
             pulumi.set(__self__, "network_includes", network_includes)
+        if password_change is not None:
+            pulumi.set(__self__, "password_change", password_change)
+        if password_reset is not None:
+            pulumi.set(__self__, "password_reset", password_reset)
+        if password_unlock is not None:
+            pulumi.set(__self__, "password_unlock", password_unlock)
         if policy_id is not None:
             pulumi.set(__self__, "policy_id", policy_id)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if users_excludeds is not None:
             pulumi.set(__self__, "users_excludeds", users_excludeds)
 
     @property
-    @pulumi.getter(name="appExcludes")
-    def app_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]:
-        """
-        Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
-        - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
-        is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
-        of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
-        """
-        return pulumi.get(self, "app_excludes")
-
-    @app_excludes.setter
-    def app_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]):
-        pulumi.set(self, "app_excludes", value)
-
-    @property
-    @pulumi.getter(name="appIncludes")
-    def app_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]]:
-        """
-        Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
-        """
-        return pulumi.get(self, "app_includes")
-
-    @app_includes.setter
-    def app_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]]]):
-        pulumi.set(self, "app_includes", value)
-
-    @property
-    @pulumi.getter
-    def enroll(self) -> Optional[pulumi.Input[str]]:
-        """
-        When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        """
-        return pulumi.get(self, "enroll")
-
-    @enroll.setter
-    def enroll(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "enroll", value)
-
-    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy Rule Name.
+        Policy Rule Name. Type `"string"`
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="networkConnection")
     def network_connection(self) -> Optional[pulumi.Input[str]]:
         """
-        Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
+        Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`. Type `"string"`
         """
         return pulumi.get(self, "network_connection")
 
     @network_connection.setter
     def network_connection(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_connection", value)
 
     @property
     @pulumi.getter(name="networkExcludes")
     def network_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The network zones to exclude. Conflicts with `network_includes`.
+        The network zones to exclude. Conflicts with `network_includes`. Type `"list(string)"`
         """
         return pulumi.get(self, "network_excludes")
 
     @network_excludes.setter
     def network_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "network_excludes", value)
 
     @property
     @pulumi.getter(name="networkIncludes")
     def network_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The network zones to include. Conflicts with `network_excludes`.
+        The network zones to include. Conflicts with `network_excludes`. Type `"list(string)"`
         """
         return pulumi.get(self, "network_includes")
 
     @network_includes.setter
     def network_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "network_includes", value)
 
     @property
+    @pulumi.getter(name="passwordChange")
+    def password_change(self) -> Optional[pulumi.Input[str]]:
+        """
+        Allow or deny a user to change their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        """
+        return pulumi.get(self, "password_change")
+
+    @password_change.setter
+    def password_change(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password_change", value)
+
+    @property
+    @pulumi.getter(name="passwordReset")
+    def password_reset(self) -> Optional[pulumi.Input[str]]:
+        """
+        Allow or deny a user to reset their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        """
+        return pulumi.get(self, "password_reset")
+
+    @password_reset.setter
+    def password_reset(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password_reset", value)
+
+    @property
+    @pulumi.getter(name="passwordUnlock")
+    def password_unlock(self) -> Optional[pulumi.Input[str]]:
+        """
+        Allow or deny a user to unlock: `"ALLOW"` or `"DENY"`. By default, it is `"DENY"`, Type `"string"`
+        """
+        return pulumi.get(self, "password_unlock")
+
+    @password_unlock.setter
+    def password_unlock(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password_unlock", value)
+
+    @property
     @pulumi.getter(name="policyId")
     def policy_id(self) -> Optional[pulumi.Input[str]]:
         """
         Policy ID.
         """
         return pulumi.get(self, "policy_id")
 
@@ -356,299 +342,294 @@
     def policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy_id", value)
 
     @property
     @pulumi.getter
     def priority(self) -> Optional[pulumi.Input[int]]:
         """
-        Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
+        Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there. Type `"number"`
         """
         return pulumi.get(self, "priority")
 
     @priority.setter
     def priority(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "priority", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
+        Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`. Type `"string"`
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
     @property
     @pulumi.getter(name="usersExcludeds")
     def users_excludeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Set of User IDs to Exclude
+        The users to exclude. Type `"set(string)"`
         """
         return pulumi.get(self, "users_excludeds")
 
     @users_excludeds.setter
     def users_excludeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "users_excludeds", value)
 
 
-class RuleMfa(pulumi.CustomResource):
+class RulePassword(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]]] = None,
-                 app_includes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]]] = None,
-                 enroll: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_connection: Optional[pulumi.Input[str]] = None,
                  network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 password_change: Optional[pulumi.Input[str]] = None,
+                 password_reset: Optional[pulumi.Input[str]] = None,
+                 password_unlock: Optional[pulumi.Input[str]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        This resource allows you to create and configure an MFA Policy Rule.
+        Creates a Password Policy Rule.
+
+        This resource allows you to create and configure a Password Policy Rule.
 
         ## Import
 
         A Policy Rule can be imported via the Policy and Rule ID.
 
         ```sh
-        $ pulumi import okta:policy/ruleMfa:RuleMfa example &#60;policy id&#62;/&#60;rule id&#62;
+        $ pulumi import okta:policy/rulePassword:RulePassword example &#60;policy id&#62;/&#60;rule id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
-               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
-               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
-               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
-        :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        :param pulumi.Input[str] name: Policy Rule Name.
-        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
+        :param pulumi.Input[str] name: Policy Rule Name. Type `"string"`
+        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`. Type `"string"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`. Type `"list(string)"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`. Type `"list(string)"`
+        :param pulumi.Input[str] password_change: Allow or deny a user to change their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        :param pulumi.Input[str] password_reset: Allow or deny a user to reset their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        :param pulumi.Input[str] password_unlock: Allow or deny a user to unlock: `"ALLOW"` or `"DENY"`. By default, it is `"DENY"`, Type `"string"`
         :param pulumi.Input[str] policy_id: Policy ID.
-        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
-        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
+        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there. Type `"number"`
+        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`. Type `"string"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: The users to exclude. Type `"set(string)"`
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[RuleMfaArgs] = None,
+                 args: Optional[RulePasswordArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        This resource allows you to create and configure an MFA Policy Rule.
+        Creates a Password Policy Rule.
+
+        This resource allows you to create and configure a Password Policy Rule.
 
         ## Import
 
         A Policy Rule can be imported via the Policy and Rule ID.
 
         ```sh
-        $ pulumi import okta:policy/ruleMfa:RuleMfa example &#60;policy id&#62;/&#60;rule id&#62;
+        $ pulumi import okta:policy/rulePassword:RulePassword example &#60;policy id&#62;/&#60;rule id&#62;
         ```
 
         :param str resource_name: The name of the resource.
-        :param RuleMfaArgs args: The arguments to use to populate this resource's properties.
+        :param RulePasswordArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(RuleMfaArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(RulePasswordArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]]] = None,
-                 app_includes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]]] = None,
-                 enroll: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_connection: Optional[pulumi.Input[str]] = None,
                  network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 password_change: Optional[pulumi.Input[str]] = None,
+                 password_reset: Optional[pulumi.Input[str]] = None,
+                 password_unlock: Optional[pulumi.Input[str]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = RuleMfaArgs.__new__(RuleMfaArgs)
+            __props__ = RulePasswordArgs.__new__(RulePasswordArgs)
 
-            __props__.__dict__["app_excludes"] = app_excludes
-            __props__.__dict__["app_includes"] = app_includes
-            __props__.__dict__["enroll"] = enroll
             __props__.__dict__["name"] = name
             __props__.__dict__["network_connection"] = network_connection
             __props__.__dict__["network_excludes"] = network_excludes
             __props__.__dict__["network_includes"] = network_includes
+            __props__.__dict__["password_change"] = password_change
+            __props__.__dict__["password_reset"] = password_reset
+            __props__.__dict__["password_unlock"] = password_unlock
             __props__.__dict__["policy_id"] = policy_id
             __props__.__dict__["priority"] = priority
             __props__.__dict__["status"] = status
             __props__.__dict__["users_excludeds"] = users_excludeds
-        super(RuleMfa, __self__).__init__(
-            'okta:policy/ruleMfa:RuleMfa',
+        super(RulePassword, __self__).__init__(
+            'okta:policy/rulePassword:RulePassword',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            app_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]]] = None,
-            app_includes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]]] = None,
-            enroll: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             network_connection: Optional[pulumi.Input[str]] = None,
             network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            password_change: Optional[pulumi.Input[str]] = None,
+            password_reset: Optional[pulumi.Input[str]] = None,
+            password_unlock: Optional[pulumi.Input[str]] = None,
             policy_id: Optional[pulumi.Input[str]] = None,
             priority: Optional[pulumi.Input[int]] = None,
             status: Optional[pulumi.Input[str]] = None,
-            users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'RuleMfa':
+            users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'RulePassword':
         """
-        Get an existing RuleMfa resource's state with the given name, id, and optional extra
+        Get an existing RulePassword resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
-               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
-               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
-               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
-        :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        :param pulumi.Input[str] name: Policy Rule Name.
-        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
+        :param pulumi.Input[str] name: Policy Rule Name. Type `"string"`
+        :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`. Type `"string"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`. Type `"list(string)"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`. Type `"list(string)"`
+        :param pulumi.Input[str] password_change: Allow or deny a user to change their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        :param pulumi.Input[str] password_reset: Allow or deny a user to reset their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        :param pulumi.Input[str] password_unlock: Allow or deny a user to unlock: `"ALLOW"` or `"DENY"`. By default, it is `"DENY"`, Type `"string"`
         :param pulumi.Input[str] policy_id: Policy ID.
-        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
-        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
+        :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there. Type `"number"`
+        :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`. Type `"string"`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: The users to exclude. Type `"set(string)"`
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _RuleMfaState.__new__(_RuleMfaState)
+        __props__ = _RulePasswordState.__new__(_RulePasswordState)
 
-        __props__.__dict__["app_excludes"] = app_excludes
-        __props__.__dict__["app_includes"] = app_includes
-        __props__.__dict__["enroll"] = enroll
         __props__.__dict__["name"] = name
         __props__.__dict__["network_connection"] = network_connection
         __props__.__dict__["network_excludes"] = network_excludes
         __props__.__dict__["network_includes"] = network_includes
+        __props__.__dict__["password_change"] = password_change
+        __props__.__dict__["password_reset"] = password_reset
+        __props__.__dict__["password_unlock"] = password_unlock
         __props__.__dict__["policy_id"] = policy_id
         __props__.__dict__["priority"] = priority
         __props__.__dict__["status"] = status
         __props__.__dict__["users_excludeds"] = users_excludeds
-        return RuleMfa(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="appExcludes")
-    def app_excludes(self) -> pulumi.Output[Optional[Sequence['outputs.RuleMfaAppExclude']]]:
-        """
-        Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
-        - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
-        is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
-        of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
-        """
-        return pulumi.get(self, "app_excludes")
-
-    @property
-    @pulumi.getter(name="appIncludes")
-    def app_includes(self) -> pulumi.Output[Optional[Sequence['outputs.RuleMfaAppInclude']]]:
-        """
-        Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
-        """
-        return pulumi.get(self, "app_includes")
-
-    @property
-    @pulumi.getter
-    def enroll(self) -> pulumi.Output[Optional[str]]:
-        """
-        When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        """
-        return pulumi.get(self, "enroll")
+        return RulePassword(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Policy Rule Name.
+        Policy Rule Name. Type `"string"`
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="networkConnection")
     def network_connection(self) -> pulumi.Output[Optional[str]]:
         """
-        Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
+        Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`. Type `"string"`
         """
         return pulumi.get(self, "network_connection")
 
     @property
     @pulumi.getter(name="networkExcludes")
     def network_excludes(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        The network zones to exclude. Conflicts with `network_includes`.
+        The network zones to exclude. Conflicts with `network_includes`. Type `"list(string)"`
         """
         return pulumi.get(self, "network_excludes")
 
     @property
     @pulumi.getter(name="networkIncludes")
     def network_includes(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        The network zones to include. Conflicts with `network_excludes`.
+        The network zones to include. Conflicts with `network_excludes`. Type `"list(string)"`
         """
         return pulumi.get(self, "network_includes")
 
     @property
+    @pulumi.getter(name="passwordChange")
+    def password_change(self) -> pulumi.Output[Optional[str]]:
+        """
+        Allow or deny a user to change their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        """
+        return pulumi.get(self, "password_change")
+
+    @property
+    @pulumi.getter(name="passwordReset")
+    def password_reset(self) -> pulumi.Output[Optional[str]]:
+        """
+        Allow or deny a user to reset their password: `"ALLOW"` or `"DENY"`. By default, it is `"ALLOW"`. Type `"string"`
+        """
+        return pulumi.get(self, "password_reset")
+
+    @property
+    @pulumi.getter(name="passwordUnlock")
+    def password_unlock(self) -> pulumi.Output[Optional[str]]:
+        """
+        Allow or deny a user to unlock: `"ALLOW"` or `"DENY"`. By default, it is `"DENY"`, Type `"string"`
+        """
+        return pulumi.get(self, "password_unlock")
+
+    @property
     @pulumi.getter(name="policyId")
     def policy_id(self) -> pulumi.Output[Optional[str]]:
         """
         Policy ID.
         """
         return pulumi.get(self, "policy_id")
 
     @property
     @pulumi.getter
     def priority(self) -> pulumi.Output[Optional[int]]:
         """
-        Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
+        Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there. Type `"number"`
         """
         return pulumi.get(self, "priority")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[Optional[str]]:
         """
-        Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
+        Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`. Type `"string"`
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter(name="usersExcludeds")
     def users_excludeds(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        Set of User IDs to Exclude
+        The users to exclude. Type `"set(string)"`
         """
         return pulumi.get(self, "users_excludeds")
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy/signon.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_admin_roles.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,377 +3,298 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
-__all__ = ['SignonArgs', 'Signon']
+__all__ = ['UserAdminRolesArgs', 'UserAdminRoles']
 
 @pulumi.input_type
-class SignonArgs:
+class UserAdminRolesArgs:
     def __init__(__self__, *,
-                 description: Optional[pulumi.Input[str]] = None,
-                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 priority: Optional[pulumi.Input[int]] = None,
-                 status: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a Signon resource.
-        :param pulumi.Input[str] description: Policy Description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
-        :param pulumi.Input[str] name: Policy Name.
-        :param pulumi.Input[int] priority: Priority of the policy.
-        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
-        """
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if groups_includeds is not None:
-            pulumi.set(__self__, "groups_includeds", groups_includeds)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if priority is not None:
-            pulumi.set(__self__, "priority", priority)
-        if status is not None:
-            pulumi.set(__self__, "status", status)
-
-    @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        """
-        Policy Description.
-        """
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
-
-    @property
-    @pulumi.getter(name="groupsIncludeds")
-    def groups_includeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+                 admin_roles: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 user_id: pulumi.Input[str],
+                 disable_notifications: Optional[pulumi.Input[bool]] = None):
         """
-        List of Group IDs to Include.
+        The set of arguments for constructing a UserAdminRoles resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] admin_roles: The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
+        :param pulumi.Input[str] user_id: Okta user ID.
+        :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
+               administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         """
-        return pulumi.get(self, "groups_includeds")
-
-    @groups_includeds.setter
-    def groups_includeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "groups_includeds", value)
+        pulumi.set(__self__, "admin_roles", admin_roles)
+        pulumi.set(__self__, "user_id", user_id)
+        if disable_notifications is not None:
+            pulumi.set(__self__, "disable_notifications", disable_notifications)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="adminRoles")
+    def admin_roles(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        Policy Name.
+        The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "admin_roles")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @admin_roles.setter
+    def admin_roles(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "admin_roles", value)
 
     @property
-    @pulumi.getter
-    def priority(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Input[str]:
         """
-        Priority of the policy.
+        Okta user ID.
         """
-        return pulumi.get(self, "priority")
+        return pulumi.get(self, "user_id")
 
-    @priority.setter
-    def priority(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "priority", value)
+    @user_id.setter
+    def user_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "user_id", value)
 
     @property
-    @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="disableNotifications")
+    def disable_notifications(self) -> Optional[pulumi.Input[bool]]:
         """
-        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        When this setting is enabled, the admins won't receive any of the default Okta
+        administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "disable_notifications")
 
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
+    @disable_notifications.setter
+    def disable_notifications(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disable_notifications", value)
 
 
 @pulumi.input_type
-class _SignonState:
+class _UserAdminRolesState:
     def __init__(__self__, *,
-                 description: Optional[pulumi.Input[str]] = None,
-                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 priority: Optional[pulumi.Input[int]] = None,
-                 status: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering Signon resources.
-        :param pulumi.Input[str] description: Policy Description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
-        :param pulumi.Input[str] name: Policy Name.
-        :param pulumi.Input[int] priority: Priority of the policy.
-        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
-        """
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if groups_includeds is not None:
-            pulumi.set(__self__, "groups_includeds", groups_includeds)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if priority is not None:
-            pulumi.set(__self__, "priority", priority)
-        if status is not None:
-            pulumi.set(__self__, "status", status)
-
-    @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        """
-        Policy Description.
-        """
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
-
-    @property
-    @pulumi.getter(name="groupsIncludeds")
-    def groups_includeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+                 admin_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 disable_notifications: Optional[pulumi.Input[bool]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None):
         """
-        List of Group IDs to Include.
+        Input properties used for looking up and filtering UserAdminRoles resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] admin_roles: The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
+        :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
+               administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
+        :param pulumi.Input[str] user_id: Okta user ID.
         """
-        return pulumi.get(self, "groups_includeds")
-
-    @groups_includeds.setter
-    def groups_includeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "groups_includeds", value)
+        if admin_roles is not None:
+            pulumi.set(__self__, "admin_roles", admin_roles)
+        if disable_notifications is not None:
+            pulumi.set(__self__, "disable_notifications", disable_notifications)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="adminRoles")
+    def admin_roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Policy Name.
+        The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "admin_roles")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @admin_roles.setter
+    def admin_roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "admin_roles", value)
 
     @property
-    @pulumi.getter
-    def priority(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="disableNotifications")
+    def disable_notifications(self) -> Optional[pulumi.Input[bool]]:
         """
-        Priority of the policy.
+        When this setting is enabled, the admins won't receive any of the default Okta
+        administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         """
-        return pulumi.get(self, "priority")
+        return pulumi.get(self, "disable_notifications")
 
-    @priority.setter
-    def priority(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "priority", value)
+    @disable_notifications.setter
+    def disable_notifications(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disable_notifications", value)
 
     @property
-    @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        Okta user ID.
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "user_id")
 
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_id", value)
 
 
-class Signon(pulumi.CustomResource):
+class UserAdminRoles(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 priority: Optional[pulumi.Input[int]] = None,
-                 status: Optional[pulumi.Input[str]] = None,
+                 admin_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 disable_notifications: Optional[pulumi.Input[bool]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Creates a Sign On Policy.
+        Resource to manage a set of admin roles for a specific user.
 
-        This resource allows you to create and configure a Sign On Policy.
+        This resource allows you to manage admin roles for a single user, independent of the user schema itself.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.policy.Signon("example",
-            name="example",
-            status="ACTIVE",
-            description="Example",
-            groups_includeds=[everyone["id"]])
+        test = okta.user.User("test",
+            first_name="TestAcc",
+            last_name="Smith",
+            login="testAcc-replace_with_uuid@example.com",
+            email="testAcc-replace_with_uuid@example.com")
+        test_user_admin_roles = okta.UserAdminRoles("test",
+            user_id=test.id,
+            admin_roles=["APP_ADMIN"])
         ```
 
         ## Import
 
-        A Sign On Policy can be imported via the Okta ID.
+        Existing user admin roles can be imported via the Okta User ID.
 
         ```sh
-        $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
+        $ pulumi import okta:index/userAdminRoles:UserAdminRoles example &#60;user id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: Policy Description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
-        :param pulumi.Input[str] name: Policy Name.
-        :param pulumi.Input[int] priority: Priority of the policy.
-        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] admin_roles: The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
+        :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
+               administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
+        :param pulumi.Input[str] user_id: Okta user ID.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[SignonArgs] = None,
+                 args: UserAdminRolesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a Sign On Policy.
+        Resource to manage a set of admin roles for a specific user.
 
-        This resource allows you to create and configure a Sign On Policy.
+        This resource allows you to manage admin roles for a single user, independent of the user schema itself.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.policy.Signon("example",
-            name="example",
-            status="ACTIVE",
-            description="Example",
-            groups_includeds=[everyone["id"]])
+        test = okta.user.User("test",
+            first_name="TestAcc",
+            last_name="Smith",
+            login="testAcc-replace_with_uuid@example.com",
+            email="testAcc-replace_with_uuid@example.com")
+        test_user_admin_roles = okta.UserAdminRoles("test",
+            user_id=test.id,
+            admin_roles=["APP_ADMIN"])
         ```
 
         ## Import
 
-        A Sign On Policy can be imported via the Okta ID.
+        Existing user admin roles can be imported via the Okta User ID.
 
         ```sh
-        $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
+        $ pulumi import okta:index/userAdminRoles:UserAdminRoles example &#60;user id&#62;
         ```
 
         :param str resource_name: The name of the resource.
-        :param SignonArgs args: The arguments to use to populate this resource's properties.
+        :param UserAdminRolesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SignonArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserAdminRolesArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 priority: Optional[pulumi.Input[int]] = None,
-                 status: Optional[pulumi.Input[str]] = None,
+                 admin_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 disable_notifications: Optional[pulumi.Input[bool]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SignonArgs.__new__(SignonArgs)
+            __props__ = UserAdminRolesArgs.__new__(UserAdminRolesArgs)
 
-            __props__.__dict__["description"] = description
-            __props__.__dict__["groups_includeds"] = groups_includeds
-            __props__.__dict__["name"] = name
-            __props__.__dict__["priority"] = priority
-            __props__.__dict__["status"] = status
-        super(Signon, __self__).__init__(
-            'okta:policy/signon:Signon',
+            if admin_roles is None and not opts.urn:
+                raise TypeError("Missing required property 'admin_roles'")
+            __props__.__dict__["admin_roles"] = admin_roles
+            __props__.__dict__["disable_notifications"] = disable_notifications
+            if user_id is None and not opts.urn:
+                raise TypeError("Missing required property 'user_id'")
+            __props__.__dict__["user_id"] = user_id
+        super(UserAdminRoles, __self__).__init__(
+            'okta:index/userAdminRoles:UserAdminRoles',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            priority: Optional[pulumi.Input[int]] = None,
-            status: Optional[pulumi.Input[str]] = None) -> 'Signon':
+            admin_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            disable_notifications: Optional[pulumi.Input[bool]] = None,
+            user_id: Optional[pulumi.Input[str]] = None) -> 'UserAdminRoles':
         """
-        Get an existing Signon resource's state with the given name, id, and optional extra
+        Get an existing UserAdminRoles resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: Policy Description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
-        :param pulumi.Input[str] name: Policy Name.
-        :param pulumi.Input[int] priority: Priority of the policy.
-        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] admin_roles: The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
+        :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
+               administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
+        :param pulumi.Input[str] user_id: Okta user ID.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _SignonState.__new__(_SignonState)
-
-        __props__.__dict__["description"] = description
-        __props__.__dict__["groups_includeds"] = groups_includeds
-        __props__.__dict__["name"] = name
-        __props__.__dict__["priority"] = priority
-        __props__.__dict__["status"] = status
-        return Signon(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
-        """
-        Policy Description.
-        """
-        return pulumi.get(self, "description")
+        __props__ = _UserAdminRolesState.__new__(_UserAdminRolesState)
 
-    @property
-    @pulumi.getter(name="groupsIncludeds")
-    def groups_includeds(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        """
-        List of Group IDs to Include.
-        """
-        return pulumi.get(self, "groups_includeds")
+        __props__.__dict__["admin_roles"] = admin_roles
+        __props__.__dict__["disable_notifications"] = disable_notifications
+        __props__.__dict__["user_id"] = user_id
+        return UserAdminRoles(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="adminRoles")
+    def admin_roles(self) -> pulumi.Output[Sequence[str]]:
         """
-        Policy Name.
+        The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "admin_roles")
 
     @property
-    @pulumi.getter
-    def priority(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter(name="disableNotifications")
+    def disable_notifications(self) -> pulumi.Output[Optional[bool]]:
         """
-        Priority of the policy.
+        When this setting is enabled, the admins won't receive any of the default Okta
+        administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         """
-        return pulumi.get(self, "priority")
+        return pulumi.get(self, "disable_notifications")
 
     @property
-    @pulumi.getter
-    def status(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Output[str]:
         """
-        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        Okta user ID.
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "user_id")
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/provider.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/resource_set.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/role_subscription.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/template_sms.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/theme.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user/get_user.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user/get_users.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user/outputs.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user/user.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user/user_type.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1715926933
+Version: 4.9.0a1716406068
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1715926933/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,18 +17,21 @@
 pulumi_okta/auth_server_claim_default.py
 pulumi_okta/auth_server_default.py
 pulumi_okta/authenticator.py
 pulumi_okta/behaviour.py
 pulumi_okta/brand.py
 pulumi_okta/captcha.py
 pulumi_okta/captcha_org_wide_settings.py
+pulumi_okta/customized_signin_page.py
 pulumi_okta/domain.py
 pulumi_okta/domain_certificate.py
 pulumi_okta/domain_verification.py
 pulumi_okta/email_customization.py
+pulumi_okta/email_domain.py
+pulumi_okta/email_domain_verification.py
 pulumi_okta/email_sender.py
 pulumi_okta/email_sender_verification.py
 pulumi_okta/event_hook.py
 pulumi_okta/event_hook_verification.py
 pulumi_okta/factor_totp.py
 pulumi_okta/get_app_group_assignments.py
 pulumi_okta/get_app_signon_policy.py
@@ -36,37 +39,43 @@
 pulumi_okta/get_auth_server_claim.py
 pulumi_okta/get_auth_server_claims.py
 pulumi_okta/get_authenticator.py
 pulumi_okta/get_behaviour.py
 pulumi_okta/get_behaviours.py
 pulumi_okta/get_brand.py
 pulumi_okta/get_brands.py
+pulumi_okta/get_default_signin_page.py
+pulumi_okta/get_domain.py
 pulumi_okta/get_email_customization.py
 pulumi_okta/get_email_customizations.py
 pulumi_okta/get_groups.py
+pulumi_okta/get_log_stream.py
 pulumi_okta/get_network_zone.py
+pulumi_okta/get_org_metadata.py
 pulumi_okta/get_role_subscription.py
 pulumi_okta/get_template.py
 pulumi_okta/get_templates.py
 pulumi_okta/get_theme.py
 pulumi_okta/get_themes.py
 pulumi_okta/get_trusted_origins.py
 pulumi_okta/get_user_security_questions.py
 pulumi_okta/group_memberships.py
 pulumi_okta/group_schema_property.py
 pulumi_okta/link_definition.py
 pulumi_okta/link_value.py
+pulumi_okta/log_stream.py
 pulumi_okta/org_configuration.py
 pulumi_okta/org_support.py
 pulumi_okta/outputs.py
 pulumi_okta/policy_mfa_default.py
 pulumi_okta/policy_password_default.py
 pulumi_okta/policy_profile_enrollment.py
 pulumi_okta/policy_profile_enrollment_apps.py
 pulumi_okta/policy_rule_profile_enrollment.py
+pulumi_okta/preview_signin_page.py
 pulumi_okta/provider.py
 pulumi_okta/pulumi-plugin.json
 pulumi_okta/py.typed
 pulumi_okta/rate_limiting.py
 pulumi_okta/resource_set.py
 pulumi_okta/role_subscription.py
 pulumi_okta/security_notification_emails.py
@@ -132,26 +141,14 @@
 pulumi_okta/idp/get_oidc.py
 pulumi_okta/idp/get_saml.py
 pulumi_okta/idp/get_social.py
 pulumi_okta/idp/oidc.py
 pulumi_okta/idp/saml.py
 pulumi_okta/idp/saml_key.py
 pulumi_okta/idp/social.py
-pulumi_okta/index/__init__.py
-pulumi_okta/index/_inputs.py
-pulumi_okta/index/customized_signin_page.py
-pulumi_okta/index/email_domain.py
-pulumi_okta/index/email_domain_verification.py
-pulumi_okta/index/get_default_signin_page.py
-pulumi_okta/index/get_domain.py
-pulumi_okta/index/get_log_stream.py
-pulumi_okta/index/get_org_metadata.py
-pulumi_okta/index/log_stream.py
-pulumi_okta/index/outputs.py
-pulumi_okta/index/preview_signin_page.py
 pulumi_okta/inline/__init__.py
 pulumi_okta/inline/_inputs.py
 pulumi_okta/inline/hook.py
 pulumi_okta/inline/outputs.py
 pulumi_okta/network/__init__.py
 pulumi_okta/network/zone.py
 pulumi_okta/policy/__init__.py
```

### Comparing `pulumi_okta-4.9.0a1715926933/pyproject.toml` & `pulumi_okta-4.9.0a1716406068/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_okta"
   description = "A Pulumi package for creating and managing okta resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "okta"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.9.0a1715926933"
+  version = "4.9.0a1716406068"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-okta"
 
 [build-system]
```

