# Comparing `tmp/bc-detect-secrets-1.5.8.tar.gz` & `tmp/bc-detect-secrets-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bc-detect-secrets-1.5.8.tar", last modified: Wed Apr 24 15:24:44 2024, max compression
+gzip compressed data, was "bc-detect-secrets-1.5.9.tar", last modified: Mon Apr 29 11:09:31 2024, max compression
```

## Comparing `bc-detect-secrets-1.5.8.tar` & `bc-detect-secrets-1.5.9.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.141841 bc-detect-secrets-1.5.8/
--rw-r--r--   0 root         (0) root         (0)    10834 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    23718 2024-04-24 15:24:44.141841 bc-detect-secrets-1.5.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    22435 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.141841 bc-detect-secrets-1.5.8/bc_detect_secrets.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23718 2024-04-24 15:24:44.000000 bc-detect-secrets-1.5.8/bc_detect_secrets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3189 2024-04-24 15:24:44.000000 bc-detect-secrets-1.5.8/bc_detect_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 15:24:44.000000 bc-detect-secrets-1.5.8/bc_detect_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2024-04-24 15:24:44.000000 bc-detect-secrets-1.5.8/bc_detect_secrets.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-24 15:24:44.000000 bc-detect-secrets-1.5.8/bc_detect_secrets.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-24 15:24:44.000000 bc-detect-secrets-1.5.8/bc_detect_secrets.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.129840 bc-detect-secrets-1.5.8/detect_secrets/
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)       85 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/__main__.py
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-24 15:24:41.000000 bc-detect-secrets-1.5.8/detect_secrets/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.129840 bc-detect-secrets-1.5.8/detect_secrets/audit/
--rw-r--r--   0 root         (0) root         (0)      212 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/audit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5172 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/audit/analytics.py
--rw-r--r--   0 root         (0) root         (0)     3352 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/audit/audit.py
--rw-r--r--   0 root         (0) root         (0)     6816 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/audit/common.py
--rw-r--r--   0 root         (0) root         (0)     8798 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/audit/compare.py
--rw-r--r--   0 root         (0) root         (0)     4078 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/audit/io.py
--rw-r--r--   0 root         (0) root         (0)     1544 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/audit/iterator.py
--rw-r--r--   0 root         (0) root         (0)     3014 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/audit/report.py
--rw-r--r--   0 root         (0) root         (0)      566 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.133841 bc-detect-secrets-1.5.8/detect_secrets/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/baseline.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.133841 bc-detect-secrets-1.5.8/detect_secrets/core/plugins/
--rw-r--r--   0 root         (0) root         (0)       41 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2560 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/plugins/initialize.py
--rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/plugins/util.py
--rw-r--r--   0 root         (0) root         (0)     5821 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/potential_secret.py
--rw-r--r--   0 root         (0) root         (0)    16864 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/scan.py
--rw-r--r--   0 root         (0) root         (0)    11603 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/secrets_collection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.133841 bc-detect-secrets-1.5.8/detect_secrets/core/upgrades/
--rw-r--r--   0 root         (0) root         (0)      337 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/upgrades/__init__.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/upgrades/v0_12.py
--rw-r--r--   0 root         (0) root         (0)     4215 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/upgrades/v1_0.py
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/upgrades/v1_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.133841 bc-detect-secrets-1.5.8/detect_secrets/core/usage/
--rw-r--r--   0 root         (0) root         (0)     6386 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/usage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3199 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/usage/audit.py
--rw-r--r--   0 root         (0) root         (0)     1026 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/usage/baseline.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/usage/common.py
--rw-r--r--   0 root         (0) root         (0)     8280 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/usage/filters.py
--rw-r--r--   0 root         (0) root         (0)     5335 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/usage/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3188 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/core/usage/scan.py
--rw-r--r--   0 root         (0) root         (0)     1279 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/custom_types.py
--rw-r--r--   0 root         (0) root         (0)      960 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.133841 bc-detect-secrets-1.5.8/detect_secrets/filters/
--rw-r--r--   0 root         (0) root         (0)      205 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/filters/allowlist.py
--rw-r--r--   0 root         (0) root         (0)     1826 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/filters/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.133841 bc-detect-secrets-1.5.8/detect_secrets/filters/gibberish/
--rw-r--r--   0 root         (0) root         (0)     3324 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/filters/gibberish/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/filters/gibberish/rfc.model
--rw-r--r--   0 root         (0) root         (0)     6388 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/filters/heuristic.py
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/filters/regex.py
--rw-r--r--   0 root         (0) root         (0)     1827 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/filters/util.py
--rw-r--r--   0 root         (0) root         (0)     2308 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/filters/wordlist.py
--rw-r--r--   0 root         (0) root         (0)     5181 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.137841 bc-detect-secrets-1.5.8/detect_secrets/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      519 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     5731 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/aws.py
--rw-r--r--   0 root         (0) root         (0)     2477 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/azure_storage_key.py
--rw-r--r--   0 root         (0) root         (0)     8398 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/base.py
--rw-r--r--   0 root         (0) root         (0)      793 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     3866 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/cloudant.py
--rw-r--r--   0 root         (0) root         (0)      589 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/discord.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/github_token.py
--rw-r--r--   0 root         (0) root         (0)     7480 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/high_entropy_strings.py
--rw-r--r--   0 root         (0) root         (0)     2608 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/ibm_cloud_iam.py
--rw-r--r--   0 root         (0) root         (0)     5377 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/ibm_cos_hmac.py
--rw-r--r--   0 root         (0) root         (0)     1494 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/jwt.py
--rw-r--r--   0 root         (0) root         (0)    12533 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/keyword.py
--rw-r--r--   0 root         (0) root         (0)      992 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/mailchimp.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/npm.py
--rw-r--r--   0 root         (0) root         (0)     4586 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/private_key.py
--rw-r--r--   0 root         (0) root         (0)      457 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/sendgrid.py
--rw-r--r--   0 root         (0) root         (0)     1437 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/slack.py
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/softlayer.py
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/square_oauth.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/stripe.py
--rw-r--r--   0 root         (0) root         (0)      436 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/plugins/twilio.py
--rw-r--r--   0 root         (0) root         (0)     4748 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/pre_commit_hook.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/py.typed
--rw-r--r--   0 root         (0) root         (0)    10312 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.137841 bc-detect-secrets-1.5.8/detect_secrets/transformers/
--rw-r--r--   0 root         (0) root         (0)     1279 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1396 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/transformers/base.py
--rw-r--r--   0 root         (0) root         (0)     8689 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/transformers/config.py
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/transformers/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12310 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/transformers/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:24:44.141841 bc-detect-secrets-1.5.8/detect_secrets/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/util/code_snippet.py
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/util/color.py
--rw-r--r--   0 root         (0) root         (0)     1348 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/util/filetype.py
--rw-r--r--   0 root         (0) root         (0)     1765 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/util/git.py
--rw-r--r--   0 root         (0) root         (0)     3701 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/util/importlib.py
--rw-r--r--   0 root         (0) root         (0)     2752 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/util/inject.py
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/util/path.py
--rw-r--r--   0 root         (0) root         (0)     1388 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/detect_secrets/util/semver.py
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      476 2024-04-24 15:24:44.141841 bc-detect-secrets-1.5.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2146 2024-04-24 15:24:40.000000 bc-detect-secrets-1.5.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.504197 bc-detect-secrets-1.5.9/
+-rw-r--r--   0 root         (0) root         (0)    10834 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    23718 2024-04-29 11:09:31.504197 bc-detect-secrets-1.5.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    22435 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.504197 bc-detect-secrets-1.5.9/bc_detect_secrets.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23718 2024-04-29 11:09:31.000000 bc-detect-secrets-1.5.9/bc_detect_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3189 2024-04-29 11:09:31.000000 bc-detect-secrets-1.5.9/bc_detect_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 11:09:31.000000 bc-detect-secrets-1.5.9/bc_detect_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-29 11:09:31.000000 bc-detect-secrets-1.5.9/bc_detect_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-29 11:09:31.000000 bc-detect-secrets-1.5.9/bc_detect_secrets.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-29 11:09:31.000000 bc-detect-secrets-1.5.9/bc_detect_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.492197 bc-detect-secrets-1.5.9/detect_secrets/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       85 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-29 11:09:29.000000 bc-detect-secrets-1.5.9/detect_secrets/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.492197 bc-detect-secrets-1.5.9/detect_secrets/audit/
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/audit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5172 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/audit/analytics.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/audit/audit.py
+-rw-r--r--   0 root         (0) root         (0)     6816 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/audit/common.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/audit/compare.py
+-rw-r--r--   0 root         (0) root         (0)     4078 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/audit/io.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/audit/iterator.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/audit/report.py
+-rw-r--r--   0 root         (0) root         (0)      566 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.496197 bc-detect-secrets-1.5.9/detect_secrets/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/baseline.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.496197 bc-detect-secrets-1.5.9/detect_secrets/core/plugins/
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/plugins/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/plugins/util.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/potential_secret.py
+-rw-r--r--   0 root         (0) root         (0)    16864 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/scan.py
+-rw-r--r--   0 root         (0) root         (0)    11603 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/secrets_collection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.496197 bc-detect-secrets-1.5.9/detect_secrets/core/upgrades/
+-rw-r--r--   0 root         (0) root         (0)      337 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/upgrades/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/upgrades/v0_12.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/upgrades/v1_0.py
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/upgrades/v1_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.496197 bc-detect-secrets-1.5.9/detect_secrets/core/usage/
+-rw-r--r--   0 root         (0) root         (0)     6386 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/usage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/usage/audit.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/usage/baseline.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/usage/common.py
+-rw-r--r--   0 root         (0) root         (0)     8280 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/usage/filters.py
+-rw-r--r--   0 root         (0) root         (0)     5335 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/usage/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/core/usage/scan.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/custom_types.py
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.496197 bc-detect-secrets-1.5.9/detect_secrets/filters/
+-rw-r--r--   0 root         (0) root         (0)      205 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/filters/allowlist.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/filters/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.496197 bc-detect-secrets-1.5.9/detect_secrets/filters/gibberish/
+-rw-r--r--   0 root         (0) root         (0)     3324 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/filters/gibberish/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/filters/gibberish/rfc.model
+-rw-r--r--   0 root         (0) root         (0)     6388 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/filters/heuristic.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/filters/regex.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/filters/util.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/filters/wordlist.py
+-rw-r--r--   0 root         (0) root         (0)     5181 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.500197 bc-detect-secrets-1.5.9/detect_secrets/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      519 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     5731 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/aws.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/azure_storage_key.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/base.py
+-rw-r--r--   0 root         (0) root         (0)      793 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/cloudant.py
+-rw-r--r--   0 root         (0) root         (0)      589 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/discord.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/github_token.py
+-rw-r--r--   0 root         (0) root         (0)     7481 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/high_entropy_strings.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/ibm_cloud_iam.py
+-rw-r--r--   0 root         (0) root         (0)     5377 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/ibm_cos_hmac.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/jwt.py
+-rw-r--r--   0 root         (0) root         (0)    12533 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      992 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/mailchimp.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/npm.py
+-rw-r--r--   0 root         (0) root         (0)     4586 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/private_key.py
+-rw-r--r--   0 root         (0) root         (0)      457 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/sendgrid.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/slack.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/softlayer.py
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/square_oauth.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/stripe.py
+-rw-r--r--   0 root         (0) root         (0)      436 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/plugins/twilio.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/pre_commit_hook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10312 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.500197 bc-detect-secrets-1.5.9/detect_secrets/transformers/
+-rw-r--r--   0 root         (0) root         (0)     1279 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/transformers/base.py
+-rw-r--r--   0 root         (0) root         (0)     8689 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/transformers/config.py
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/transformers/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12310 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/transformers/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:09:31.504197 bc-detect-secrets-1.5.9/detect_secrets/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/util/code_snippet.py
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/util/color.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/util/filetype.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/util/git.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/util/importlib.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/util/inject.py
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/detect_secrets/util/semver.py
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-29 11:09:31.504197 bc-detect-secrets-1.5.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-04-29 11:09:28.000000 bc-detect-secrets-1.5.9/setup.py
```

### Comparing `bc-detect-secrets-1.5.8/LICENSE` & `bc-detect-secrets-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/PKG-INFO` & `bc-detect-secrets-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc-detect-secrets
-Version: 1.5.8
+Version: 1.5.9
 Summary: Tool for detecting secrets in the codebase
 Home-page: https://github.com/bridgecrewio/detect-secrets
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Keywords: secret-management,pre-commit,security,entropy-checks
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `bc-detect-secrets-1.5.8/README.md` & `bc-detect-secrets-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/bc_detect_secrets.egg-info/PKG-INFO` & `bc-detect-secrets-1.5.9/bc_detect_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc-detect-secrets
-Version: 1.5.8
+Version: 1.5.9
 Summary: Tool for detecting secrets in the codebase
 Home-page: https://github.com/bridgecrewio/detect-secrets
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Keywords: secret-management,pre-commit,security,entropy-checks
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `bc-detect-secrets-1.5.8/bc_detect_secrets.egg-info/SOURCES.txt` & `bc-detect-secrets-1.5.9/bc_detect_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/audit/analytics.py` & `bc-detect-secrets-1.5.9/detect_secrets/audit/analytics.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/audit/audit.py` & `bc-detect-secrets-1.5.9/detect_secrets/audit/audit.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/audit/common.py` & `bc-detect-secrets-1.5.9/detect_secrets/audit/common.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/audit/compare.py` & `bc-detect-secrets-1.5.9/detect_secrets/audit/compare.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/audit/io.py` & `bc-detect-secrets-1.5.9/detect_secrets/audit/io.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/audit/iterator.py` & `bc-detect-secrets-1.5.9/detect_secrets/audit/iterator.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/audit/report.py` & `bc-detect-secrets-1.5.9/detect_secrets/audit/report.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/constants.py` & `bc-detect-secrets-1.5.9/detect_secrets/constants.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/baseline.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/baseline.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/log.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/log.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/plugins/initialize.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/plugins/initialize.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/plugins/util.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/plugins/util.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/potential_secret.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/potential_secret.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/scan.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/scan.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/secrets_collection.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/secrets_collection.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/upgrades/v1_0.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/upgrades/v1_0.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/upgrades/v1_1.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/upgrades/v1_1.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/usage/__init__.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/usage/audit.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/usage/audit.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/usage/baseline.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/usage/baseline.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/usage/common.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/usage/common.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/usage/filters.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/usage/filters.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/usage/plugins.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/usage/plugins.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/core/usage/scan.py` & `bc-detect-secrets-1.5.9/detect_secrets/core/usage/scan.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/custom_types.py` & `bc-detect-secrets-1.5.9/detect_secrets/custom_types.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/exceptions.py` & `bc-detect-secrets-1.5.9/detect_secrets/exceptions.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/filters/allowlist.py` & `bc-detect-secrets-1.5.9/detect_secrets/filters/allowlist.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/filters/common.py` & `bc-detect-secrets-1.5.9/detect_secrets/filters/common.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/filters/gibberish/__init__.py` & `bc-detect-secrets-1.5.9/detect_secrets/filters/gibberish/__init__.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/filters/gibberish/rfc.model` & `bc-detect-secrets-1.5.9/detect_secrets/filters/gibberish/rfc.model`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/filters/heuristic.py` & `bc-detect-secrets-1.5.9/detect_secrets/filters/heuristic.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/filters/regex.py` & `bc-detect-secrets-1.5.9/detect_secrets/filters/regex.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/filters/util.py` & `bc-detect-secrets-1.5.9/detect_secrets/filters/util.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/filters/wordlist.py` & `bc-detect-secrets-1.5.9/detect_secrets/filters/wordlist.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/main.py` & `bc-detect-secrets-1.5.9/detect_secrets/main.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/artifactory.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/artifactory.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/aws.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/aws.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/azure_storage_key.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/azure_storage_key.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/base.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/base.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/basic_auth.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/basic_auth.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/cloudant.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/cloudant.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/discord.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/discord.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/high_entropy_strings.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/high_entropy_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             )
 
         self.charset = charset
         self.entropy_limit = limit
 
         # We require quoted strings to reduce noise.
         # NOTE: We need this to be a capturing group, so back-reference can work.
-        self.regex = re.compile(r'([\'":=])\s*([{}]+)([\'"]?)'.format(re.escape(charset)))
+        self.regex = re.compile(r'([\'":=])\s*([{}]+)([\'"]|$)'.format(re.escape(charset)))
 
     def analyze_string(self, string: str) -> Generator[str, None, None]:
         for result in self.regex.findall(string):
             if isinstance(result, tuple):
                 # This occurs on the default regex, but not on the eager regex.
                 result = result[1]
```

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/ibm_cloud_iam.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/ibm_cloud_iam.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/ibm_cos_hmac.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/ibm_cos_hmac.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/jwt.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/jwt.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/keyword.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/keyword.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/mailchimp.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/mailchimp.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/private_key.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/private_key.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/slack.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/slack.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/softlayer.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/softlayer.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/plugins/stripe.py` & `bc-detect-secrets-1.5.9/detect_secrets/plugins/stripe.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/pre_commit_hook.py` & `bc-detect-secrets-1.5.9/detect_secrets/pre_commit_hook.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/settings.py` & `bc-detect-secrets-1.5.9/detect_secrets/settings.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/transformers/__init__.py` & `bc-detect-secrets-1.5.9/detect_secrets/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/transformers/base.py` & `bc-detect-secrets-1.5.9/detect_secrets/transformers/base.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/transformers/config.py` & `bc-detect-secrets-1.5.9/detect_secrets/transformers/config.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/transformers/yaml.py` & `bc-detect-secrets-1.5.9/detect_secrets/transformers/yaml.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/util/code_snippet.py` & `bc-detect-secrets-1.5.9/detect_secrets/util/code_snippet.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/util/color.py` & `bc-detect-secrets-1.5.9/detect_secrets/util/color.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/util/filetype.py` & `bc-detect-secrets-1.5.9/detect_secrets/util/filetype.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/util/git.py` & `bc-detect-secrets-1.5.9/detect_secrets/util/git.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/util/importlib.py` & `bc-detect-secrets-1.5.9/detect_secrets/util/importlib.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/util/inject.py` & `bc-detect-secrets-1.5.9/detect_secrets/util/inject.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/detect_secrets/util/semver.py` & `bc-detect-secrets-1.5.9/detect_secrets/util/semver.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/pyproject.toml` & `bc-detect-secrets-1.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.5.8/setup.py` & `bc-detect-secrets-1.5.9/setup.py`

 * *Files identical despite different names*

