# Comparing `tmp/aws-encryption-sdk-3.2.0.tar.gz` & `tmp/aws-encryption-sdk-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-encryption-sdk-3.2.0.tar", last modified: Mon Mar 18 22:00:22 2024, max compression
+gzip compressed data, was "aws-encryption-sdk-3.3.0.tar", last modified: Tue May 21 22:46:51 2024, max compression
```

## Comparing `aws-encryption-sdk-3.2.0.tar` & `aws-encryption-sdk-3.3.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.422176 aws-encryption-sdk-3.2.0/
--rw-r--r--   0 root         (0) root         (0)    21187 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      222 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15343 2024-03-18 22:00:22.422176 aws-encryption-sdk-3.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14377 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.406176 aws-encryption-sdk-3.2.0/doc/
--rw-r--r--   0 root         (0) root         (0)     2072 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.406176 aws-encryption-sdk-3.2.0/examples/
--rw-r--r--   0 root         (0) root         (0)      622 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.410176 aws-encryption-sdk-3.2.0/examples/src/
--rw-r--r--   0 root         (0) root         (0)      627 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2785 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/basic_encryption.py
--rw-r--r--   0 root         (0) root         (0)     6964 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/basic_file_encryption_with_multiple_providers.py
--rw-r--r--   0 root         (0) root         (0)     4483 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/basic_file_encryption_with_raw_key_provider.py
--rw-r--r--   0 root         (0) root         (0)     3787 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/custom_kms_client_for_kms_provider.py
--rw-r--r--   0 root         (0) root         (0)     2539 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/data_key_caching_basic.py
--rw-r--r--   0 root         (0) root         (0)     3447 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/discovery_kms_provider.py
--rw-r--r--   0 root         (0) root         (0)     4648 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/mrk_aware_kms_provider.py
--rw-r--r--   0 root         (0) root         (0)     3153 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/multiple_kms_cmk.py
--rw-r--r--   0 root         (0) root         (0)     2653 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/one_kms_cmk.py
--rw-r--r--   0 root         (0) root         (0)     3150 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/one_kms_cmk_streaming_data.py
--rw-r--r--   0 root         (0) root         (0)     2843 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/one_kms_cmk_unsigned.py
--rw-r--r--   0 root         (0) root         (0)     2789 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/src/set_commitment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.410176 aws-encryption-sdk-3.2.0/examples/test/
--rw-r--r--   0 root         (0) root         (0)      627 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/examples_test_utils.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_basic_encryption.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_basic_file_encryption_with_multiple_providers.py
--rw-r--r--   0 root         (0) root         (0)     1187 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_basic_file_encryption_with_raw_key_provider.py
--rw-r--r--   0 root         (0) root         (0)      971 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_data_key_caching_basic.py
--rw-r--r--   0 root         (0) root         (0)     1082 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_discovery_kms_provider.py
--rw-r--r--   0 root         (0) root         (0)     1107 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_mrk_aware_kms_provider.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_multiple_kms_cmk.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_one_kms_cmk.py
--rw-r--r--   0 root         (0) root         (0)     1374 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_one_kms_cmk_streaming_data.py
--rw-r--r--   0 root         (0) root         (0)     1105 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_one_kms_cmk_unsigned.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/examples/test/test_i_set_commitment.py
--rw-r--r--   0 root         (0) root         (0)       63 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1341 2024-03-18 22:00:22.426176 aws-encryption-sdk-3.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1866 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.406176 aws-encryption-sdk-3.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.410176 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/
--rw-r--r--   0 root         (0) root         (0)    13858 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.414176 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/caches/
--rw-r--r--   0 root         (0) root         (0)     8063 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/caches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3001 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/caches/base.py
--rw-r--r--   0 root         (0) root         (0)     9502 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/caches/local.py
--rw-r--r--   0 root         (0) root         (0)     3094 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/caches/null.py
--rw-r--r--   0 root         (0) root         (0)     1725 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/compatability.py
--rw-r--r--   0 root         (0) root         (0)     4057 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14661 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/identifiers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.414176 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/
--rw-r--r--   0 root         (0) root         (0)      750 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7949 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/arn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.414176 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/
--rw-r--r--   0 root         (0) root         (0)      716 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/authentication.py
--rw-r--r--   0 root         (0) root         (0)     2792 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/data_keys.py
--rw-r--r--   0 root         (0) root         (0)     9130 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/elliptic_curve.py
--rw-r--r--   0 root         (0) root         (0)     5725 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/encryption.py
--rw-r--r--   0 root         (0) root         (0)     3686 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/iv.py
--rw-r--r--   0 root         (0) root         (0)     5499 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/wrapping_keys.py
--rw-r--r--   0 root         (0) root         (0)     2380 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/defaults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.414176 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/formatting/
--rw-r--r--   0 root         (0) root         (0)     4956 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/formatting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24770 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/formatting/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     6932 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/formatting/encryption_context.py
--rw-r--r--   0 root         (0) root         (0)    17553 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/formatting/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1482 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/str_ops.py
--rw-r--r--   0 root         (0) root         (0)     3030 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.414176 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/utils/
--rw-r--r--   0 root         (0) root         (0)     7163 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/utils/commitment.py
--rw-r--r--   0 root         (0) root         (0)     1453 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/utils/signature.py
--rw-r--r--   0 root         (0) root         (0)     3237 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/utils/streams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.414176 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/key_providers/
--rw-r--r--   0 root         (0) root         (0)      617 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/key_providers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26386 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/key_providers/base.py
--rw-r--r--   0 root         (0) root         (0)    49646 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/key_providers/kms.py
--rw-r--r--   0 root         (0) root         (0)     9766 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/key_providers/raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.414176 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/materials_managers/
--rw-r--r--   0 root         (0) root         (0)     5259 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/materials_managers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/materials_managers/base.py
--rw-r--r--   0 root         (0) root         (0)    11158 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/materials_managers/caching.py
--rw-r--r--   0 root         (0) root         (0)     7444 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/materials_managers/default.py
--rw-r--r--   0 root         (0) root         (0)    43244 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/streaming_client.py
--rw-r--r--   0 root         (0) root         (0)     5386 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.410176 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15343 2024-03-18 22:00:22.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5876 2024-03-18 22:00:22.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 22:00:22.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-03-18 22:00:22.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-18 22:00:22.000000 aws-encryption-sdk-3.2.0/src/aws_encryption_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.414176 aws-encryption-sdk-3.2.0/test/
--rw-r--r--   0 root         (0) root         (0)      561 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.418176 aws-encryption-sdk-3.2.0/test/functional/
--rw-r--r--   0 root         (0) root         (0)      561 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.418176 aws-encryption-sdk-3.2.0/test/functional/key_providers/
--rw-r--r--   0 root         (0) root         (0)      561 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/functional/key_providers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5018 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/functional/key_providers/test_base.py
--rw-r--r--   0 root         (0) root         (0)    39323 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/functional/test_f_aws_encryption_sdk_client.py
--rw-r--r--   0 root         (0) root         (0)    10906 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/functional/test_f_commitment.py
--rw-r--r--   0 root         (0) root         (0)     2623 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/functional/test_f_crypto.py
--rw-r--r--   0 root         (0) root         (0)     2244 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/functional/test_f_crypto_iv.py
--rw-r--r--   0 root         (0) root         (0)     7238 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/functional/test_f_xcompat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.418176 aws-encryption-sdk-3.2.0/test/integration/
--rw-r--r--   0 root         (0) root         (0)      561 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3792 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/integration/integration_test_utils.py
--rw-r--r--   0 root         (0) root         (0)    40325 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/integration/test_i_aws_encrytion_sdk_client.py
--rw-r--r--   0 root         (0) root         (0)     5778 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/integration/test_i_thread_safety.py
--rw-r--r--   0 root         (0) root         (0)     2845 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/integration/test_i_xcompat_kms.py
--rw-r--r--   0 root         (0) root         (0)     3518 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/integration/test_kat_commitment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.418176 aws-encryption-sdk-3.2.0/test/resources/
--rw-r--r--   0 root         (0) root         (0)   119431 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/resources/commitment-test-vectors.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 22:00:22.422176 aws-encryption-sdk-3.2.0/test/unit/
--rw-r--r--   0 root         (0) root         (0)      561 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1823 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_algorithm_suite.py
--rw-r--r--   0 root         (0) root         (0)    11865 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_arn.py
--rw-r--r--   0 root         (0) root         (0)     8942 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_caches.py
--rw-r--r--   0 root         (0) root         (0)     1256 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_caches_base.py
--rw-r--r--   0 root         (0) root         (0)     5970 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_caches_crypto_cache_entry.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_caches_local.py
--rw-r--r--   0 root         (0) root         (0)     2120 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_caches_null.py
--rw-r--r--   0 root         (0) root         (0)     5063 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_commitment.py
--rw-r--r--   0 root         (0) root         (0)     1340 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_compatability.py
--rw-r--r--   0 root         (0) root         (0)     3977 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_crypto.py
--rw-r--r--   0 root         (0) root         (0)     6427 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_crypto_authentication_signer.py
--rw-r--r--   0 root         (0) root         (0)     5625 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_crypto_authentication_verifier.py
--rw-r--r--   0 root         (0) root         (0)     4058 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_crypto_data_keys.py
--rw-r--r--   0 root         (0) root         (0)    14546 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_crypto_elliptic_curve.py
--rw-r--r--   0 root         (0) root         (0)     3976 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_crypto_encryption_decryptor.py
--rw-r--r--   0 root         (0) root         (0)     4263 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_crypto_encryption_encryptor.py
--rw-r--r--   0 root         (0) root         (0)     3677 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_crypto_prehashing_authenticator.py
--rw-r--r--   0 root         (0) root         (0)    12492 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_crypto_wrapping_keys.py
--rw-r--r--   0 root         (0) root         (0)     1475 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_defaults.py
--rw-r--r--   0 root         (0) root         (0)    22550 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_deserialize.py
--rw-r--r--   0 root         (0) root         (0)     6491 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_encryption_client.py
--rw-r--r--   0 root         (0) root         (0)     8715 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_encryption_context.py
--rw-r--r--   0 root         (0) root         (0)     2584 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_identifiers.py
--rw-r--r--   0 root         (0) root         (0)     2347 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_internal_structures.py
--rw-r--r--   0 root         (0) root         (0)     4082 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_material_managers.py
--rw-r--r--   0 root         (0) root         (0)     1189 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_material_managers_base.py
--rw-r--r--   0 root         (0) root         (0)    17744 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_material_managers_caching.py
--rw-r--r--   0 root         (0) root         (0)    20503 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_material_managers_default.py
--rw-r--r--   0 root         (0) root         (0)    14912 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_base_master_key.py
--rw-r--r--   0 root         (0) root         (0)     1780 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_base_master_key_config.py
--rw-r--r--   0 root         (0) root         (0)    30294 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_base_master_key_provider.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_base_master_key_provider_config.py
--rw-r--r--   0 root         (0) root         (0)    46845 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_kms_master_key.py
--rw-r--r--   0 root         (0) root         (0)     2294 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_kms_master_key_config.py
--rw-r--r--   0 root         (0) root         (0)    37194 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_kms_master_key_provider.py
--rw-r--r--   0 root         (0) root         (0)     2451 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_kms_master_key_provider_config.py
--rw-r--r--   0 root         (0) root         (0)     9762 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_raw_master_key.py
--rw-r--r--   0 root         (0) root         (0)     2145 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_raw_master_key_config.py
--rw-r--r--   0 root         (0) root         (0)     2758 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_providers_raw_master_key_provider.py
--rw-r--r--   0 root         (0) root         (0)    18454 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_serialize.py
--rw-r--r--   0 root         (0) root         (0)     5684 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_streaming_client_configs.py
--rw-r--r--   0 root         (0) root         (0)    17434 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_streaming_client_encryption_stream.py
--rw-r--r--   0 root         (0) root         (0)    37192 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_streaming_client_stream_decryptor.py
--rw-r--r--   0 root         (0) root         (0)    43872 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_streaming_client_stream_encryptor.py
--rw-r--r--   0 root         (0) root         (0)     4142 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_structures.py
--rw-r--r--   0 root         (0) root         (0)     2154 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_util_str_ops.py
--rw-r--r--   0 root         (0) root         (0)     2850 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_util_streams.py
--rw-r--r--   0 root         (0) root         (0)    13567 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    28041 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/test_values.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-03-18 21:59:39.000000 aws-encryption-sdk-3.2.0/test/unit/unit_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.812924 aws-encryption-sdk-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)    22241 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      222 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15446 2024-05-21 22:46:51.812924 aws-encryption-sdk-3.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14377 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.800924 aws-encryption-sdk-3.3.0/doc/
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.800924 aws-encryption-sdk-3.3.0/examples/
+-rw-r--r--   0 root         (0) root         (0)      167 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.800924 aws-encryption-sdk-3.3.0/examples/src/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/basic_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     6509 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/basic_file_encryption_with_multiple_providers.py
+-rw-r--r--   0 root         (0) root         (0)     4028 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/basic_file_encryption_with_raw_key_provider.py
+-rw-r--r--   0 root         (0) root         (0)     3332 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/custom_kms_client_for_kms_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/data_key_caching_basic.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/discovery_kms_provider.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/mrk_aware_kms_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/multiple_kms_cmk.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/one_kms_cmk.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/one_kms_cmk_streaming_data.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/one_kms_cmk_unsigned.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/src/set_commitment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.800924 aws-encryption-sdk-3.3.0/examples/test/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2919 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/examples_test_utils.py
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_basic_encryption.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_basic_file_encryption_with_multiple_providers.py
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_basic_file_encryption_with_raw_key_provider.py
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_data_key_caching_basic.py
+-rw-r--r--   0 root         (0) root         (0)      627 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_discovery_kms_provider.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_mrk_aware_kms_provider.py
+-rw-r--r--   0 root         (0) root         (0)      657 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_multiple_kms_cmk.py
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_one_kms_cmk.py
+-rw-r--r--   0 root         (0) root         (0)      914 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_one_kms_cmk_streaming_data.py
+-rw-r--r--   0 root         (0) root         (0)      650 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_one_kms_cmk_unsigned.py
+-rw-r--r--   0 root         (0) root         (0)      615 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/examples/test/test_i_set_commitment.py
+-rw-r--r--   0 root         (0) root         (0)       63 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-05-21 22:46:51.816924 aws-encryption-sdk-3.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1967 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.796924 aws-encryption-sdk-3.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.800924 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/
+-rw-r--r--   0 root         (0) root         (0)    13402 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.804924 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/caches/
+-rw-r--r--   0 root         (0) root         (0)     7608 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/caches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/caches/base.py
+-rw-r--r--   0 root         (0) root         (0)     9047 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/caches/local.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/caches/null.py
+-rw-r--r--   0 root         (0) root         (0)     1310 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/compatability.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14206 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/identifiers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.804924 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7494 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/arn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.804924 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6621 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/data_keys.py
+-rw-r--r--   0 root         (0) root         (0)     8675 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/elliptic_curve.py
+-rw-r--r--   0 root         (0) root         (0)     5270 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     3231 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/iv.py
+-rw-r--r--   0 root         (0) root         (0)     5202 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/wrapping_keys.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/defaults.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.804924 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/formatting/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/formatting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24315 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/formatting/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     6477 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/formatting/encryption_context.py
+-rw-r--r--   0 root         (0) root         (0)    17098 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/formatting/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/str_ops.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/structures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.804924 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/utils/
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/utils/commitment.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/utils/signature.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/utils/streams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.804924 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/key_providers/
+-rw-r--r--   0 root         (0) root         (0)      162 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/key_providers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25931 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/key_providers/base.py
+-rw-r--r--   0 root         (0) root         (0)    49191 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/key_providers/kms.py
+-rw-r--r--   0 root         (0) root         (0)     9311 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/key_providers/raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.804924 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/materials_managers/
+-rw-r--r--   0 root         (0) root         (0)     4804 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/materials_managers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/materials_managers/base.py
+-rw-r--r--   0 root         (0) root         (0)    10703 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/materials_managers/caching.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/materials_managers/default.py
+-rw-r--r--   0 root         (0) root         (0)    42789 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/streaming_client.py
+-rw-r--r--   0 root         (0) root         (0)     4931 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/structures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.804924 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15446 2024-05-21 22:46:51.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5876 2024-05-21 22:46:51.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 22:46:51.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-05-21 22:46:51.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-21 22:46:51.000000 aws-encryption-sdk-3.3.0/src/aws_encryption_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.808924 aws-encryption-sdk-3.3.0/test/
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.808924 aws-encryption-sdk-3.3.0/test/functional/
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/functional/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.808924 aws-encryption-sdk-3.3.0/test/functional/key_providers/
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/functional/key_providers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4563 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/functional/key_providers/test_base.py
+-rw-r--r--   0 root         (0) root         (0)    38868 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/functional/test_f_aws_encryption_sdk_client.py
+-rw-r--r--   0 root         (0) root         (0)    10451 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/functional/test_f_commitment.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/functional/test_f_crypto.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/functional/test_f_crypto_iv.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/functional/test_f_xcompat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.808924 aws-encryption-sdk-3.3.0/test/integration/
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/integration/integration_test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    39870 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/integration/test_i_aws_encrytion_sdk_client.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/integration/test_i_thread_safety.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/integration/test_i_xcompat_kms.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/integration/test_kat_commitment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.808924 aws-encryption-sdk-3.3.0/test/resources/
+-rw-r--r--   0 root         (0) root         (0)   119431 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/resources/commitment-test-vectors.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 22:46:51.812924 aws-encryption-sdk-3.3.0/test/unit/
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_algorithm_suite.py
+-rw-r--r--   0 root         (0) root         (0)    11410 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_arn.py
+-rw-r--r--   0 root         (0) root         (0)     8487 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_caches.py
+-rw-r--r--   0 root         (0) root         (0)      801 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_caches_base.py
+-rw-r--r--   0 root         (0) root         (0)     5515 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_caches_crypto_cache_entry.py
+-rw-r--r--   0 root         (0) root         (0)    10353 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_caches_local.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_caches_null.py
+-rw-r--r--   0 root         (0) root         (0)     4608 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_commitment.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_compatability.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_crypto.py
+-rw-r--r--   0 root         (0) root         (0)     5972 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_crypto_authentication_signer.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_crypto_authentication_verifier.py
+-rw-r--r--   0 root         (0) root         (0)     3603 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_crypto_data_keys.py
+-rw-r--r--   0 root         (0) root         (0)    14091 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_crypto_elliptic_curve.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_crypto_encryption_decryptor.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_crypto_encryption_encryptor.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_crypto_prehashing_authenticator.py
+-rw-r--r--   0 root         (0) root         (0)    12037 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_crypto_wrapping_keys.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_defaults.py
+-rw-r--r--   0 root         (0) root         (0)    22095 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     6036 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_encryption_client.py
+-rw-r--r--   0 root         (0) root         (0)     8260 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_encryption_context.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_identifiers.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_internal_structures.py
+-rw-r--r--   0 root         (0) root         (0)     3627 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_material_managers.py
+-rw-r--r--   0 root         (0) root         (0)      734 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_material_managers_base.py
+-rw-r--r--   0 root         (0) root         (0)    17289 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_material_managers_caching.py
+-rw-r--r--   0 root         (0) root         (0)    20048 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_material_managers_default.py
+-rw-r--r--   0 root         (0) root         (0)    14457 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_base_master_key.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_base_master_key_config.py
+-rw-r--r--   0 root         (0) root         (0)    29839 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_base_master_key_provider.py
+-rw-r--r--   0 root         (0) root         (0)      484 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_base_master_key_provider_config.py
+-rw-r--r--   0 root         (0) root         (0)    46390 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_kms_master_key.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_kms_master_key_config.py
+-rw-r--r--   0 root         (0) root         (0)    36739 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_kms_master_key_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_kms_master_key_provider_config.py
+-rw-r--r--   0 root         (0) root         (0)     9307 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_raw_master_key.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_raw_master_key_config.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_providers_raw_master_key_provider.py
+-rw-r--r--   0 root         (0) root         (0)    17999 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_serialize.py
+-rw-r--r--   0 root         (0) root         (0)     5229 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_streaming_client_configs.py
+-rw-r--r--   0 root         (0) root         (0)    16979 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_streaming_client_encryption_stream.py
+-rw-r--r--   0 root         (0) root         (0)    36737 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_streaming_client_stream_decryptor.py
+-rw-r--r--   0 root         (0) root         (0)    43417 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_streaming_client_stream_encryptor.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_structures.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_util_str_ops.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_util_streams.py
+-rw-r--r--   0 root         (0) root         (0)    13112 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    27586 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/test_values.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2024-05-21 22:46:12.000000 aws-encryption-sdk-3.3.0/test/unit/unit_test_utils.py
```

### Comparing `aws-encryption-sdk-3.2.0/CHANGELOG.rst` & `aws-encryption-sdk-3.3.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 *********
 Changelog
 *********
 
+3.3.0 -- 2024-05-20
+===================
+
+Deprecation
+-----------
+The AWS Encryption SDK for Python no longer supports Python 3.7
+as of version 3.3; only Python 3.8+ is supported.
+
+Fixes
+-----------
+* fix: Handle errors when decrypting multiple EDKs with raw RSA MKPs (#672 (https://github.com/aws/aws-encryption-sdk-python/pull/672))
+* chore: Updated description of decrypt() usage in src/aws_encryption_sdk/__init__.py (#660 (https://github.com/aws/aws-encryption-sdk-python/pull/660))
+* fix(CI): removed appveyor.yml (#668 (https://github.com/aws/aws-encryption-sdk-python/pull/668))
+* fix(CI): updated ci_test-vector-handler.yaml and ci_tests.yaml (#665 (https://github.com/aws/aws-encryption-sdk-python/pull/665))
+
+Maintenance
+-----------
+* feat: remove Python3.7 support (#648 (https://github.com/aws/aws-encryption-sdk-python/pull/648))
+* chore: Update copyright headers (#677 (https://github.com/aws/aws-encryption-sdk-python/pull/677))
+* chore(CFN): Changes for MPL TestVectors (#653 (https://github.com/aws/aws-encryption-sdk-python/pull/653))
+
 3.2.0 -- 2024-03-18
 ===================
 
 Features
 -----------
 * test Python 3.12 in CI (#623 (https://github.com/josecorella/aws-encryption-sdk-python/issues/623)) (93a67d8 (https://github.com/josecorella/aws-encryption-sdk-python/commit/93a67d8a3806f560ead950e6d8898e53c4c4f9df))
 * update requirements and README (#638 (https://github.com/josecorella/aws-encryption-sdk-python/issues/638)) (bcead77 (https://github.com/josecorella/aws-encryption-sdk-python/commit/bcead776b022566ad8211a08e1a458375b23a356))
```

### Comparing `aws-encryption-sdk-3.2.0/LICENSE` & `aws-encryption-sdk-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-encryption-sdk-3.2.0/PKG-INFO` & `aws-encryption-sdk-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: aws-encryption-sdk
-Version: 3.2.0
+Version: 3.3.0
 Summary: AWS Encryption SDK implementation for Python
 Home-page: https://github.com/aws/aws-encryption-sdk-python
 Author: Amazon Web Services
 Author-email: aws-cryptools@amazon.com
 Maintainer: Amazon Web Services
 License: Apache License 2.0
 Keywords: aws-encryption-sdk aws kms encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 License-File: LICENSE
 
 ##################
 aws-encryption-sdk
@@ -54,15 +56,15 @@
 
 ***************
 Getting Started
 ***************
 Required Prerequisites
 ======================
 
-* Python 3.7+
+* Python 3.8+
 * cryptography >= 3.4.6
 * boto3 >= 1.10.0
 * attrs
 
 Installation
 ============
```

### Comparing `aws-encryption-sdk-3.2.0/README.rst` & `aws-encryption-sdk-3.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ***************
 Getting Started
 ***************
 Required Prerequisites
 ======================
 
-* Python 3.7+
+* Python 3.8+
 * cryptography >= 3.4.6
 * boto3 >= 1.10.0
 * attrs
 
 Installation
 ============
```

### Comparing `aws-encryption-sdk-3.2.0/doc/conf.py` & `aws-encryption-sdk-3.3.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `aws-encryption-sdk-3.2.0/doc/index.rst` & `aws-encryption-sdk-3.3.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `aws-encryption-sdk-3.2.0/examples/src/basic_encryption.py` & `aws-encryption-sdk-3.3.0/examples/src/basic_encryption.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing basic encryption and decryption of a value already in memory."""
 import aws_encryption_sdk
 from aws_encryption_sdk import CommitmentPolicy
 
 
 def cycle_string(key_arn, source_plaintext, botocore_session=None):
     """Encrypts and then decrypts a string under a KMS customer master key (CMK).
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/basic_file_encryption_with_multiple_providers.py` & `aws-encryption-sdk-3.3.0/examples/src/basic_file_encryption_with_multiple_providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing creation of a RawMasterKeyProvider, how to use multiple
 master key providers to encrypt, and demonstrating that each master key
 provider can then be used independently to decrypt the same encrypted message.
 """
 import filecmp
 import os
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/basic_file_encryption_with_raw_key_provider.py` & `aws-encryption-sdk-3.3.0/examples/src/basic_file_encryption_with_raw_key_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing creation and use of a RawMasterKeyProvider."""
 import filecmp
 import os
 
 import aws_encryption_sdk
 from aws_encryption_sdk.identifiers import Algorithm, CommitmentPolicy, EncryptionKeyType, WrappingAlgorithm
 from aws_encryption_sdk.internal.crypto.wrapping_keys import WrappingKey
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/custom_kms_client_for_kms_provider.py` & `aws-encryption-sdk-3.3.0/examples/src/custom_kms_client_for_kms_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing how to customize the AWS KMS Client."""
 import boto3
 from botocore.config import Config
 
 import aws_encryption_sdk
 from aws_encryption_sdk import CommitmentPolicy
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/data_key_caching_basic.py` & `aws-encryption-sdk-3.3.0/examples/src/data_key_caching_basic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example of encryption with data key caching."""
 import aws_encryption_sdk
 from aws_encryption_sdk import CommitmentPolicy
 
 
 def encrypt_with_caching(kms_cmk_arn, max_age_in_cache, cache_capacity):
     """Encrypts a string using an AWS KMS customer master key (CMK) and data key caching.
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/discovery_kms_provider.py` & `aws-encryption-sdk-3.3.0/examples/src/discovery_kms_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing encryption of a value already in memory using one KMS CMK, then decryption of the ciphertext using
 a DiscoveryAwsKmsMasterKeyProvider.
 """
 import aws_encryption_sdk
 from aws_encryption_sdk import CommitmentPolicy
 from aws_encryption_sdk.internal.arn import arn_from_str
 from aws_encryption_sdk.key_providers.kms import DiscoveryFilter
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/mrk_aware_kms_provider.py` & `aws-encryption-sdk-3.3.0/examples/src/mrk_aware_kms_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2021 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing encryption of a value already in memory using one KMS CMK, then decryption of the ciphertext using
 a DiscoveryAwsKmsMasterKeyProvider.
 """
 
 import aws_encryption_sdk
 from aws_encryption_sdk import CommitmentPolicy
 from aws_encryption_sdk.internal.arn import arn_from_str
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/multiple_kms_cmk.py` & `aws-encryption-sdk-3.3.0/examples/src/multiple_kms_cmk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing basic encryption and decryption of a value already in memory using one KMS CMK."""
 import aws_encryption_sdk
 from aws_encryption_sdk import CommitmentPolicy
 
 
 def encrypt_decrypt(key_arns, source_plaintext, botocore_session=None):
     """Encrypts and then decrypts a string under two KMS customer master keys (CMK).
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/one_kms_cmk.py` & `aws-encryption-sdk-3.3.0/examples/src/one_kms_cmk.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing basic encryption and decryption of a value already in memory using one KMS CMK."""
 import aws_encryption_sdk
 from aws_encryption_sdk import CommitmentPolicy
 
 
 def encrypt_decrypt(key_arn, source_plaintext, botocore_session=None):
     """Encrypts and then decrypts a string under one KMS customer master key (CMK).
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/one_kms_cmk_streaming_data.py` & `aws-encryption-sdk-3.3.0/examples/src/one_kms_cmk_streaming_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing basic encryption and decryption of streaming data in memory using one KMS CMK."""
 import filecmp
 
 import aws_encryption_sdk
 from aws_encryption_sdk import CommitmentPolicy
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/one_kms_cmk_unsigned.py` & `aws-encryption-sdk-3.3.0/examples/src/one_kms_cmk_unsigned.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing basic encryption and decryption of a value already in memory
 using one AWS KMS CMK with an unsigned algorithm.
 
 Note: We recommend using an algorithm with signing as an AWS Encryption SDK best practice.
 """
 import aws_encryption_sdk
 from aws_encryption_sdk import StrictAwsKmsMasterKeyProvider
```

### Comparing `aws-encryption-sdk-3.2.0/examples/src/set_commitment.py` & `aws-encryption-sdk-3.3.0/examples/src/set_commitment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Example showing how to disable commitment.
 
 Note: This configuration should only be used as part of a migration from version 1.x to 2.x, or for advanced users
 with specialized requirements. We recommend that AWS Encryption SDK users enable commitment whenever possible.
 """
 import aws_encryption_sdk
 from aws_encryption_sdk import CommitmentPolicy
```

### Comparing `aws-encryption-sdk-3.2.0/examples/test/examples_test_utils.py` & `aws-encryption-sdk-3.3.0/examples/test/examples_test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Helper utilities for use while testing examples."""
 import os
 import sys
 
 os.environ["AWS_ENCRYPTION_SDK_EXAMPLES_TESTING"] = "yes"
 sys.path.extend([os.sep.join([os.path.dirname(__file__), "..", "..", "test", "integration"])])
```

### Comparing `aws-encryption-sdk-3.2.0/setup.cfg` & `aws-encryption-sdk-3.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aws-encryption-sdk-3.2.0/setup.py` & `aws-encryption-sdk-3.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,17 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Security",
         "Topic :: Security :: Cryptography",
     ],
 )
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/__init__.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """High level AWS Encryption SDK client functions."""
 # Below are imported for ease of use by implementors
 import warnings
 
 import attr
 
 from aws_encryption_sdk.caches.local import LocalCryptoMaterialsCache  # noqa
@@ -160,15 +150,15 @@
 
             >>> import aws_encryption_sdk
             >>> client = aws_encryption_sdk.EncryptionSDKClient()
             >>> kms_key_provider = aws_encryption_sdk.StrictAwsKmsMasterKeyProvider(key_ids=[
             ...     'arn:aws:kms:us-east-1:2222222222222:key/22222222-2222-2222-2222-222222222222',
             ...     'arn:aws:kms:us-east-1:3333333333333:key/33333333-3333-3333-3333-333333333333'
             ... ])
-            >>> my_ciphertext, encryptor_header = client.decrypt(
+            >>> my_plaintext, decryptor_header = client.decrypt(
             ...     source=my_ciphertext,
             ...     key_provider=kms_key_provider
             ... )
 
         :param config: Client configuration object (config or individual parameters required)
         :type config: aws_encryption_sdk.streaming_client.DecryptorConfig
         :param source: Source data to encrypt or decrypt
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/caches/__init__.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/caches/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Common functions and structures for use in cryptographic materials caches.
 
 .. versionadded:: 1.3.0
 """
 import time
 from threading import Lock
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/caches/local.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/caches/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Local, in-memory, LRU, cryptographic materials cache for use with caching cryptographic materials providers."""
 import logging
 import weakref
 from collections import OrderedDict, deque
 from threading import RLock
 
 import attr
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/caches/null.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/caches/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,57 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
-"""Null cache: a cache which does not cache."""
-from ..exceptions import CacheKeyError
-from . import CryptoMaterialsCacheEntry
-from .base import CryptoMaterialsCache
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
+"""Base class interface for caches for use with caching crypto material managers."""
+import abc
 
+import six
 
-class NullCryptoMaterialsCache(CryptoMaterialsCache):
-    """Null cache: a cache which does not cache.
+
+@six.add_metaclass(abc.ABCMeta)
+class CryptoMaterialsCache(object):
+    """Parent interface for crypto materials caches.
 
     .. versionadded:: 1.3.0
     """
 
+    @abc.abstractmethod
     def put_encryption_materials(self, cache_key, encryption_materials, plaintext_length, entry_hints=None):
-        """Does not add encryption materials to the cache since there is no cache to which to add them.
+        """Adds encryption materials to the cache.
 
         :param bytes cache_key: Identifier for entries in cache
         :param encryption_materials: Encryption materials to add to cache
         :type encryption_materials: aws_encryption_sdk.materials_managers.EncryptionMaterials
         :param int plaintext_length: Length of plaintext associated with this request to the cache
         :param entry_hints: Metadata to associate with entry (optional)
         :type entry_hints: aws_encryption_sdk.caches.CryptoCacheEntryHints
-        :rtype: aws_encryption_sdk.caches.CryptoMaterialsCacheEntry
+        :rtype: aws_encryption_sdk.caches.CryptoCacheEntry
         """
-        return CryptoMaterialsCacheEntry(cache_key=cache_key, value=encryption_materials)
 
+    @abc.abstractmethod
     def put_decryption_materials(self, cache_key, decryption_materials):
-        """Does not add decryption materials to the cache since there is no cache to which to add them.
+        """Adds decryption materials to the cache
 
         :param bytes cache_key: Identifier for entries in cache
         :param decryption_materials: Decryption materials to add to cache
         :type decryption_materials: aws_encryption_sdk.materials_managers.DecryptionMaterials
-        :rtype: aws_encryption_sdk.caches.CryptoMaterialsCacheEntry
+        :rtype: aws_encryption_sdk.caches.CryptoCacheEntry
         """
-        return CryptoMaterialsCacheEntry(cache_key=cache_key, value=decryption_materials)
 
+    @abc.abstractmethod
     def get_encryption_materials(self, cache_key, plaintext_length):
-        """Always raises a CacheKeyError.
+        """Locates exactly one available encryption materials cache entry for the specified cache_key,
+        incrementing the entry's usage stats prior to returning it to the caller.
 
         :param bytes cache_key: Cache ID for which to locate cache entries
         :param int plaintext_length: Bytes to be encrypted by the encryption materials
         :rtype: aws_encryption_sdk.caches.CryptoCacheEntry
-        :raises CacheKeyError: when called
+        :raises CacheKeyError: if no values found in cache for cache_key
         """
-        raise CacheKeyError("Key not found in cache")
 
+    @abc.abstractmethod
     def get_decryption_materials(self, cache_key):
-        """Always raises a CacheKeyError.
+        """Locates exactly one available decryption materials cache entry for the specified cache_key.
 
         :param bytes cache_key: Cache ID for which to locate cache entries
         :rtype: aws_encryption_sdk.caches.CryptoCacheEntry
-        :raises CacheKeyError: when called
+        :raises CacheKeyError: if no values found in cache for cache_key
         """
-        raise CacheKeyError("Key not found in cache")
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/exceptions.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Contains exception classes for AWS Encryption SDK."""
 
 
 class AWSEncryptionSDKClientError(Exception):
     """General exception class for AWS Encryption SDK."""
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/identifiers.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/identifiers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """AWS Encryption SDK native data structures for defining implementation-specific characteristics."""
 import struct
 from enum import Enum
 
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec, padding, rsa
 from cryptography.hazmat.primitives.ciphers import algorithms, modes
@@ -23,15 +13,15 @@
 
 try:  # Python 3.5.0 and 3.5.1 have incompatible typing modules
     from typing import Optional  # noqa pylint: disable=unused-import
 except ImportError:  # pragma: no cover
     # We only actually need these imports when running the mypy checks
     pass
 
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 USER_AGENT_SUFFIX = "AwsEncryptionSdkPython/{}".format(__version__)
 
 
 class EncryptionSuite(Enum):
     """Static definition of encryption algorithm details.
 
     .. warning:: These members must only be used as part of an AlgorithmSuite.
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/arn.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/arn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Utility class for processing Amazon Resource Names (ARNs)"""
 
 from aws_encryption_sdk.exceptions import MalformedArnError
 
 
 class Arn(object):
     """Arn to identify AWS resources. See https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/authentication.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Contains authentication primitives."""
 import base64
 import logging
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import ec
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/elliptic_curve.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/elliptic_curve.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Contains elliptic curve functionality."""
 import logging
 from collections import namedtuple
 
 import six
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import ec
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/encryption.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/encryption.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Contains encryption primitives and helper functions."""
 import logging
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.ciphers import Cipher
 
 from ..structures import EncryptedData
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/iv.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/iv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """
 Helper functions used for generating deterministic initialization vectors (IVs).
 
 Deterministic IVs are used to reduce the probability of IV/message-key pair collisions when caching
 data keys.
 
 Prior to introducing caching, a statement could safely be made that every encrypt call resulted in a new
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/crypto/wrapping_keys.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/crypto/wrapping_keys.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Contains wrapping key primitives."""
 import logging
 import os
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 
@@ -94,17 +84,20 @@
         :param dict encryption_context: Encryption context to use in decryption
         :returns: Plaintext of data key
         :rtype: bytes
         """
         if self.wrapping_key_type is EncryptionKeyType.PUBLIC:
             raise IncorrectMasterKeyError("Public key cannot decrypt")
         if self.wrapping_key_type is EncryptionKeyType.PRIVATE:
-            return self._wrapping_key.decrypt(
-                ciphertext=encrypted_wrapped_data_key.ciphertext, padding=self.wrapping_algorithm.padding
-            )
+            try:
+                return self._wrapping_key.decrypt(
+                    ciphertext=encrypted_wrapped_data_key.ciphertext, padding=self.wrapping_algorithm.padding
+                )
+            except ValueError:
+                raise IncorrectMasterKeyError("_wrapping_key cannot decrypt provided ciphertext")
         serialized_encryption_context = serialize_encryption_context(encryption_context=encryption_context)
         return decrypt(
             algorithm=self.wrapping_algorithm.algorithm,
             key=self._derived_wrapping_key,
             encrypted_data=encrypted_wrapped_data_key,
             associated_data=serialized_encryption_context,
         )
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/defaults.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/defaults.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Default values for AWS Encryption SDK."""
 import io
 
 import aws_encryption_sdk.identifiers
 
 #: Default chunk size to read data from sources in streaming clients
 LINE_LENGTH = io.DEFAULT_BUFFER_SIZE
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/formatting/__init__.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/formatting/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Formatting functions for aws_encryption_sdk."""
 from .serialize import serialize_header
 
 
 def header_length(header):
     """Calculates the ciphertext message header length, given a complete header.
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/formatting/deserialize.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/formatting/deserialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Components for handling AWS Encryption SDK message deserialization."""
 from __future__ import division
 
 import io
 import logging
 import struct
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/formatting/encryption_context.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/formatting/encryption_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """
 Components for handling serialization and deserialization of
 encryption context data in AWS Encryption SDK messages.
 """
 import codecs
 import logging
 import struct
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/formatting/serialize.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/formatting/serialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Components for handling AWS Encryption SDK message serialization."""
 import logging
 import struct
 
 import aws_encryption_sdk.internal.defaults
 import aws_encryption_sdk.internal.formatting.encryption_context
 from aws_encryption_sdk.exceptions import SerializationError
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/structures.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/structures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Public data structures for aws_encryption_sdk."""
 import attr
 import six
 
 
 @attr.s(hash=True)
 class EncryptedData(object):
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/utils/__init__.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Helper utility functions for AWS Encryption SDK."""
 import io
 import logging
 import os
 
 import six
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/utils/commitment.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/utils/commitment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Helper functions for validating commitment policies and algorithms for the AWS Encryption SDK."""
 from aws_encryption_sdk.exceptions import ActionNotAllowedError
 from aws_encryption_sdk.identifiers import CommitmentPolicy
 
 TROUBLESHOOTING_URL = "https://docs.aws.amazon.com/encryption-sdk/latest/developer-guide/troubleshooting-migration.html"
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/internal/utils/streams.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/internal/utils/streams.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Helper stream utility objects for AWS Encryption SDK."""
 import io
 
 from wrapt import ObjectProxy
 
 from aws_encryption_sdk.exceptions import ActionNotAllowedError
 from aws_encryption_sdk.internal.str_ops import to_bytes
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/key_providers/base.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/key_providers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Base class interface for Master Key Providers."""
 import abc
 import logging
 
 import attr
 import six
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/key_providers/kms.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/key_providers/kms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Master Key Providers for use with AWS KMS"""
 import abc
 import functools
 import itertools
 import logging
 
 import attr
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/key_providers/raw.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/key_providers/raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Resources required for Raw Master Keys."""
 import abc
 import logging
 import os
 
 import attr
 import six
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/materials_managers/__init__.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/materials_managers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Primitive structures for use when interacting with crypto material managers.
 
 .. versionadded:: 1.3.0
 """
 import attr
 import six
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/materials_managers/base.py` & `aws-encryption-sdk-3.3.0/test/unit/test_caches_null.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
-"""Base class interface for crypto material managers."""
-import abc
-
-import six
-
-
-@six.add_metaclass(abc.ABCMeta)
-class CryptoMaterialsManager(object):
-    """Parent interface for crypto material manager classes.
-
-    .. versionadded:: 1.3.0
-    """
-
-    @abc.abstractmethod
-    def get_encryption_materials(self, request):
-        """Provides encryption materials appropriate for the request.
-
-        .. note::
-            Must be implemented by specific CryptoMaterialsManager implementations.
-
-        :param request: encryption materials request
-        :type request: aws_encryption_sdk.materials_managers.EncryptionMaterialsRequest
-        :returns: encryption materials
-        :rtype: aws_encryption_sdk.materials_managers.EncryptionMaterials
-        """
-
-    @abc.abstractmethod
-    def decrypt_materials(self, request):
-        """Provides decryption materials appropriate for the request.
-
-        .. note::
-            Must be implemented by specific CryptoMaterialsManager implementations.
-
-        :param request: decrypt materials request
-        :type request: aws_encryption_sdk.materials_managers.DecryptionMaterialsRequest
-        :returns: decryption materials
-        :rtype: aws_encryption_sdk.materials_managers.DecryptionMaterials
-        """
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
+"""Unit testing suite for NullCryptoMaterialsCache"""
+import pytest
+from mock import MagicMock
+
+from aws_encryption_sdk.caches import CryptoMaterialsCacheEntry
+from aws_encryption_sdk.caches.null import NullCryptoMaterialsCache
+from aws_encryption_sdk.exceptions import CacheKeyError
+from aws_encryption_sdk.materials_managers import DecryptionMaterials, EncryptionMaterials
+
+pytestmark = [pytest.mark.unit, pytest.mark.local]
+
+
+def test_put_encryption_materials():
+    cache_key = b"ex_cache_key"
+    value = MagicMock(__class__=EncryptionMaterials)
+    check_value = CryptoMaterialsCacheEntry(cache_key=cache_key, value=value)
+    cache = NullCryptoMaterialsCache()
+
+    test = cache.put_encryption_materials(
+        cache_key=cache_key, encryption_materials=value, plaintext_length=0, entry_hints=None
+    )
+
+    assert test == check_value
+
+
+def test_put_decryption_materials():
+    cache_key = b"ex_cache_key"
+    value = MagicMock(__class__=DecryptionMaterials)
+    check_value = CryptoMaterialsCacheEntry(cache_key=cache_key, value=value)
+    cache = NullCryptoMaterialsCache()
+
+    test = cache.put_decryption_materials(cache_key=cache_key, decryption_materials=value)
+
+    assert test == check_value
+
+
+@pytest.mark.parametrize(
+    "method_name, args", (("get_encryption_materials", (None, None)), ("get_decryption_materials", (None,)))
+)
+def test_gets(method_name, args):
+    test = NullCryptoMaterialsCache()
+
+    with pytest.raises(CacheKeyError) as excinfo:
+        getattr(test, method_name)(*args)
+
+    excinfo.match(r"Key not found in cache")
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/materials_managers/caching.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/materials_managers/caching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Caching crypto material manager."""
 import logging
 import uuid
 
 import attr
 import six
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/materials_managers/default.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/materials_managers/default.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Default crypto material manager class."""
 import logging
 
 import attr
 
 from ..exceptions import MasterKeyProviderError, SerializationError
 from ..identifiers import CommitmentPolicy
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/streaming_client.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/streaming_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """High level AWS Encryption SDK client for streaming objects."""
 from __future__ import division
 
 import abc
 import hmac
 import io
 import logging
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk/structures.py` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Public data structures for aws_encryption_sdk."""
 import attr
 import six
 
 import aws_encryption_sdk.identifiers
 from aws_encryption_sdk.internal.str_ops import to_bytes, to_str
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk.egg-info/PKG-INFO` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: aws-encryption-sdk
-Version: 3.2.0
+Version: 3.3.0
 Summary: AWS Encryption SDK implementation for Python
 Home-page: https://github.com/aws/aws-encryption-sdk-python
 Author: Amazon Web Services
 Author-email: aws-cryptools@amazon.com
 Maintainer: Amazon Web Services
 License: Apache License 2.0
 Keywords: aws-encryption-sdk aws kms encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 License-File: LICENSE
 
 ##################
 aws-encryption-sdk
@@ -54,15 +56,15 @@
 
 ***************
 Getting Started
 ***************
 Required Prerequisites
 ======================
 
-* Python 3.7+
+* Python 3.8+
 * cryptography >= 3.4.6
 * boto3 >= 1.10.0
 * attrs
 
 Installation
 ============
```

### Comparing `aws-encryption-sdk-3.2.0/src/aws_encryption_sdk.egg-info/SOURCES.txt` & `aws-encryption-sdk-3.3.0/src/aws_encryption_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-encryption-sdk-3.2.0/test/functional/key_providers/test_base.py` & `aws-encryption-sdk-3.3.0/test/functional/key_providers/test_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Functional tests for ``aws_encryption_sdk.key_providers.base``."""
 import itertools
 
 import attr
 import pytest
 
 from aws_encryption_sdk.exceptions import InvalidKeyIdError
```

### Comparing `aws-encryption-sdk-3.2.0/test/functional/test_f_aws_encryption_sdk_client.py` & `aws-encryption-sdk-3.3.0/test/functional/test_f_aws_encryption_sdk_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Functional test suite for aws_encryption_sdk.kms_thick_client"""
 from __future__ import division
 
 import io
 import logging
 
 import attr
```

### Comparing `aws-encryption-sdk-3.2.0/test/functional/test_f_commitment.py` & `aws-encryption-sdk-3.3.0/test/functional/test_f_commitment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Functional test suite for functionality related to key commitment."""
 from test.functional.test_f_aws_encryption_sdk_client import fake_kms_key_provider
 
 import attr
 import pytest
 import six
```

### Comparing `aws-encryption-sdk-3.2.0/test/functional/test_f_crypto.py` & `aws-encryption-sdk-3.3.0/test/functional/test_f_crypto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Functional test suite for Elliptic Curve static length signature calculation."""
 import pytest
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec
 
 import aws_encryption_sdk
```

### Comparing `aws-encryption-sdk-3.2.0/test/functional/test_f_xcompat.py` & `aws-encryption-sdk-3.3.0/test/functional/test_f_xcompat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Functional test suite testing decryption of known good test files encrypted using static RawMasterKeyProvider."""
 import base64
 import json
 import logging
 import os
 import sys
 from collections import defaultdict
```

### Comparing `aws-encryption-sdk-3.2.0/test/integration/integration_test_utils.py` & `aws-encryption-sdk-3.3.0/test/integration/integration_test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Utility functions to handle configuration and credentials setup for integration tests."""
 import os
 
 import botocore.session
 
 from aws_encryption_sdk.key_providers.kms import StrictAwsKmsMasterKeyProvider
```

### Comparing `aws-encryption-sdk-3.2.0/test/integration/test_i_aws_encrytion_sdk_client.py` & `aws-encryption-sdk-3.3.0/test/integration/test_i_aws_encrytion_sdk_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Integration test suite for `aws_encryption_sdk`."""
 import io
 import logging
 
 import pytest
 from botocore.exceptions import BotoCoreError
```

### Comparing `aws-encryption-sdk-3.2.0/test/integration/test_i_thread_safety.py` & `aws-encryption-sdk-3.3.0/test/integration/test_i_thread_safety.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Basic sanity check for ``aws_encryption_sdk`` client behavior when threading."""
 from __future__ import division
 
 import copy
 import threading
 import time
 from random import SystemRandom
```

### Comparing `aws-encryption-sdk-3.2.0/test/integration/test_kat_commitment.py` & `aws-encryption-sdk-3.3.0/test/integration/test_kat_commitment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Known answer test suite for functionality related to key commitment."""
 import base64
 import json
 import os
 import sys
 from test.functional.test_f_commitment import StaticRawMasterKeyProvider
```

### Comparing `aws-encryption-sdk-3.2.0/test/resources/commitment-test-vectors.json` & `aws-encryption-sdk-3.3.0/test/resources/commitment-test-vectors.json`

 * *Files identical despite different names*

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_arn.py` & `aws-encryption-sdk-3.3.0/test/unit/test_arn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.internal.arn functions."""
 import pytest
 
 from aws_encryption_sdk.exceptions import MalformedArnError
 from aws_encryption_sdk.internal.arn import arn_from_str, is_valid_mrk_arn_str, is_valid_mrk_identifier
 
 pytestmark = [pytest.mark.unit, pytest.mark.local]
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_caches.py` & `aws-encryption-sdk-3.3.0/test/unit/test_caches.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.caches common functions."""
 import struct
 from base64 import b64decode
 
 import pytest
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_caches_crypto_cache_entry.py` & `aws-encryption-sdk-3.3.0/test/unit/test_caches_crypto_cache_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for CryptoMaterialsCacheEntry and CryptoMaterialsCacheEntryHints"""
 import pytest
 from mock import MagicMock
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 import aws_encryption_sdk.caches
 from aws_encryption_sdk.caches import CryptoMaterialsCacheEntry, CryptoMaterialsCacheEntryHints
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_caches_local.py` & `aws-encryption-sdk-3.3.0/test/unit/test_caches_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit testing suite for LocalCryptoMaterialsCache"""
 import weakref
 from collections import OrderedDict, deque
 
 import pytest
 from mock import MagicMock, call, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_commitment.py` & `aws-encryption-sdk-3.3.0/test/unit/test_commitment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit testing suite for commitment utility functions"""
 import pytest
 from mock import MagicMock
 
 from aws_encryption_sdk.exceptions import ActionNotAllowedError
 from aws_encryption_sdk.identifiers import Algorithm, CommitmentPolicy
 from aws_encryption_sdk.internal.utils.commitment import (
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_crypto.py` & `aws-encryption-sdk-3.3.0/test/unit/test_crypto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.internal.crypto"""
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import ec
 
 VALUES = {
     "iv": b"asdfzxcvqwer",
     "tag": b"asdfzxcvqwerasdf",
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_crypto_authentication_signer.py` & `aws-encryption-sdk-3.3.0/test/unit/test_crypto_authentication_signer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for ``aws_encryption_sdk.internal.crypto.authentication.Signer``."""
 import pytest
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 import aws_encryption_sdk.internal.crypto.authentication
 from aws_encryption_sdk.internal.crypto.authentication import Signer
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_crypto_authentication_verifier.py` & `aws-encryption-sdk-3.3.0/test/unit/test_crypto_authentication_verifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for ``aws_encryption_sdk.internal.crypto.authentication.Verifier``."""
 import pytest
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 import aws_encryption_sdk.internal.crypto.authentication
 from aws_encryption_sdk.internal.crypto.authentication import Verifier
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_crypto_data_keys.py` & `aws-encryption-sdk-3.3.0/test/unit/test_crypto_data_keys.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for ``aws_encryption_sdk.internal.crypto.data_keys``."""
 import pytest
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 from aws_encryption_sdk.internal.crypto import data_keys
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_crypto_elliptic_curve.py` & `aws-encryption-sdk-3.3.0/test/unit/test_crypto_elliptic_curve.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for ``aws_encryption_sdk.internal.crypto.elliptic_curve``."""
 import sys
 
 import pytest
 from cryptography.hazmat.primitives.asymmetric import ec
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_crypto_encryption_decryptor.py` & `aws-encryption-sdk-3.3.0/test/unit/test_crypto_encryption_decryptor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for ``aws_encryption_sdk.internal.crypto.encryption.Decryptor``."""
 import pytest
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 import aws_encryption_sdk.internal.crypto.encryption
 from aws_encryption_sdk.internal.crypto.encryption import Decryptor, decrypt
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_crypto_encryption_encryptor.py` & `aws-encryption-sdk-3.3.0/test/unit/test_crypto_encryption_encryptor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for ``aws_encryption_sdk.internal.crypto.encryption.Encryptor``."""
 import pytest
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 import aws_encryption_sdk.internal.crypto.encryption
 from aws_encryption_sdk.internal.crypto.encryption import Encryptor, encrypt
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_crypto_prehashing_authenticator.py` & `aws-encryption-sdk-3.3.0/test/unit/test_crypto_prehashing_authenticator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for ``aws_encryption_sdk.internal.crypto._PrehashingAuthenticater``."""
 import pytest
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 import aws_encryption_sdk.internal.crypto.authentication
 from aws_encryption_sdk.exceptions import NotSupportedError
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_crypto_wrapping_keys.py` & `aws-encryption-sdk-3.3.0/test/unit/test_crypto_wrapping_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for ``aws_encryption_sdk.internal.crypto.wrapping_keys``."""
 import pytest
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 import aws_encryption_sdk.internal.crypto.wrapping_keys
 from aws_encryption_sdk.exceptions import IncorrectMasterKeyError, InvalidDataKeyError
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_deserialize.py` & `aws-encryption-sdk-3.3.0/test/unit/test_deserialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.deserialize"""
 import io
 import struct
 
 import pytest
 from cryptography.exceptions import InvalidTag
 from mock import MagicMock, patch, sentinel
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_encryption_client.py` & `aws-encryption-sdk-3.3.0/test/unit/test_encryption_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.EncryptionSDKClient"""
 import warnings
 
 import pytest
 from mock import MagicMock
 
 import aws_encryption_sdk
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_encryption_context.py` & `aws-encryption-sdk-3.3.0/test/unit/test_encryption_context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.internal.formatting.encryption_context"""
 import pytest
 
 import aws_encryption_sdk.internal.defaults
 import aws_encryption_sdk.internal.formatting.encryption_context
 from aws_encryption_sdk.exceptions import SerializationError
 from aws_encryption_sdk.identifiers import ContentAADString
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_internal_structures.py` & `aws-encryption-sdk-3.3.0/test/unit/test_internal_structures.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.internal.structures"""
 import pytest
 
 from aws_encryption_sdk.internal.structures import (
     EncryptedData,
     MessageFooter,
     MessageFrameBody,
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_material_managers.py` & `aws-encryption-sdk-3.3.0/test/unit/test_material_managers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Test suite for aws_encryption_sdk.materials_managers"""
 import pytest
 from mock import MagicMock
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 from aws_encryption_sdk.identifiers import Algorithm, CommitmentPolicy
 from aws_encryption_sdk.internal.utils.streams import ROStream
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_material_managers_caching.py` & `aws-encryption-sdk-3.3.0/test/unit/test_material_managers_caching.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for CachingCryptoMaterialsManager"""
 
 import pytest
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 import aws_encryption_sdk.materials_managers.caching
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_material_managers_default.py` & `aws-encryption-sdk-3.3.0/test/unit/test_material_managers_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Test suite for aws_encryption_sdk.materials_managers.default"""
 
 import pytest
 from mock import MagicMock, sentinel
 from pytest_mock import mocker  # noqa pylint: disable=unused-import
 
 import aws_encryption_sdk.materials_managers.default
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_providers_base_master_key.py` & `aws-encryption-sdk-3.3.0/test/unit/test_providers_base_master_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Test suite for aws_encryption_sdk.key_providers.base.MasterKey"""
 import attr
 import pytest
 from mock import MagicMock, patch, sentinel
 
 from aws_encryption_sdk.exceptions import ConfigMismatchError, IncorrectMasterKeyError, InvalidKeyIdError
 from aws_encryption_sdk.internal.defaults import ALGORITHM
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_providers_base_master_key_config.py` & `aws-encryption-sdk-3.3.0/test/unit/test_providers_base_master_key_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite to validate aws_encryption_sdk.key_providers.base.MasterKeyConfig"""
 import pytest
 
 from aws_encryption_sdk.key_providers.base import MasterKeyConfig
 
 from .unit_test_utils import all_invalid_kwargs, all_valid_kwargs
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_providers_base_master_key_provider.py` & `aws-encryption-sdk-3.3.0/test/unit/test_providers_base_master_key_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Test suite for aws_encryption_sdk.key_providers.base.MasterKeyProvider"""
 import attr
 import pytest
 from mock import MagicMock, PropertyMock, call, patch, sentinel
 
 from aws_encryption_sdk.exceptions import (
     DecryptKeyError,
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_providers_kms_master_key.py` & `aws-encryption-sdk-3.3.0/test/unit/test_providers_kms_master_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.key_providers.kms.KMSMasterKey"""
 import botocore.client
 import pytest
 from botocore.exceptions import ClientError
 from mock import MagicMock, patch, sentinel
 
 from aws_encryption_sdk.exceptions import DecryptKeyError, EncryptKeyError, GenerateKeyError, MalformedArnError
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_providers_kms_master_key_config.py` & `aws-encryption-sdk-3.3.0/test/unit/test_providers_kms_master_key_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite to validate aws_encryption_sdk.key_providers.kms.KMSMasterKeyConfig"""
 import boto3
 import pytest
 
 from aws_encryption_sdk.key_providers.base import MasterKeyConfig
 from aws_encryption_sdk.key_providers.kms import _PROVIDER_ID, KMSMasterKeyConfig
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_providers_kms_master_key_provider.py` & `aws-encryption-sdk-3.3.0/test/unit/test_providers_kms_master_key_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite from aws_encryption_sdk.key_providers.kms.KMSMasterKeyProvider"""
 import botocore.client
 import botocore.session
 import pytest
 from mock import ANY, MagicMock, call, patch, sentinel
 
 from aws_encryption_sdk.exceptions import (
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_providers_kms_master_key_provider_config.py` & `aws-encryption-sdk-3.3.0/test/unit/test_providers_kms_master_key_provider_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite to validate aws_encryption_sdk.key_providers.kms.KMSMasterKeyProviderConfig"""
 import botocore.session
 import pytest
 
 from aws_encryption_sdk.key_providers.base import MasterKeyProviderConfig
 from aws_encryption_sdk.key_providers.kms import KMSMasterKeyProviderConfig
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_providers_raw_master_key.py` & `aws-encryption-sdk-3.3.0/test/unit/test_providers_raw_master_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Test suite for aws_encryption_sdk.key_providers.raw.RawMasterKey"""
 import pytest
 from mock import MagicMock, patch, sentinel
 
 from aws_encryption_sdk.identifiers import Algorithm, WrappingAlgorithm
 from aws_encryption_sdk.internal.crypto.wrapping_keys import WrappingKey
 from aws_encryption_sdk.key_providers.base import MasterKey
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_serialize.py` & `aws-encryption-sdk-3.3.0/test/unit/test_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.internal.formatting.serialize"""
 import pytest
 from mock import MagicMock, patch, sentinel
 
 import aws_encryption_sdk.internal.formatting.serialize
 from aws_encryption_sdk.exceptions import SerializationError
 from aws_encryption_sdk.identifiers import ContentAADString, SerializationVersion
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_streaming_client_configs.py` & `aws-encryption-sdk-3.3.0/test/unit/test_streaming_client_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite to validate aws_encryption_sdk.streaming_client config classes."""
 import io
 
 import pytest
 import six
 
 from aws_encryption_sdk import CommitmentPolicy
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_streaming_client_encryption_stream.py` & `aws-encryption-sdk-3.3.0/test/unit/test_streaming_client_encryption_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.streaming_client._EncryptionStream"""
 import copy
 import io
 
 import attr
 import pytest
 from mock import MagicMock, PropertyMock, call, patch, sentinel
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_streaming_client_stream_decryptor.py` & `aws-encryption-sdk-3.3.0/test/unit/test_streaming_client_stream_decryptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.streaming_client.StreamDecryptor"""
 import io
 
 import pytest
 from mock import MagicMock, call, patch, sentinel
 
 from aws_encryption_sdk.exceptions import (
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_streaming_client_stream_encryptor.py` & `aws-encryption-sdk-3.3.0/test/unit/test_streaming_client_stream_encryptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.streaming_client.StreamEncryptor"""
 import io
 
 import pytest
 import six
 from mock import MagicMock, call, patch, sentinel
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_structures.py` & `aws-encryption-sdk-3.3.0/test/unit/test_structures.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.structures"""
 import pytest
 
 from aws_encryption_sdk.identifiers import Algorithm, ContentType, ObjectType, SerializationVersion
 from aws_encryption_sdk.structures import DataKey, EncryptedDataKey, MasterKeyInfo, MessageHeader, RawDataKey
 
 from .unit_test_utils import all_invalid_kwargs, all_valid_kwargs
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_util_streams.py` & `aws-encryption-sdk-3.3.0/test/unit/test_util_streams.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Unit test suite for aws_encryption_sdk.internal.utils.streams"""
 import io
 
 import pytest
 
 from aws_encryption_sdk.exceptions import ActionNotAllowedError
 from aws_encryption_sdk.internal.str_ops import to_bytes, to_str
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_utils.py` & `aws-encryption-sdk-3.3.0/test/unit/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,10 @@
 # coding: utf-8
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Test suite for aws_encryption_sdk.internal.utils"""
 import io
 
 import pytest
 from mock import MagicMock, patch, sentinel
 
 import aws_encryption_sdk.identifiers
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/test_values.py` & `aws-encryption-sdk-3.3.0/test/unit/test_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Values to use in various unit test suites."""
 import copy
 import struct
 
 import six
 from mock import MagicMock
```

### Comparing `aws-encryption-sdk-3.2.0/test/unit/unit_test_utils.py` & `aws-encryption-sdk-3.3.0/test/unit/unit_test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-# http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
+# Copyright Amazon.com Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 """Utility functions to handle common test framework functions."""
 import copy
 import io
 import itertools
 
 from aws_encryption_sdk.internal.utils.streams import InsistentReaderBytesIO
```

