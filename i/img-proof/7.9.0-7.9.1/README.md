# Comparing `tmp/img-proof-7.9.0.tar.gz` & `tmp/img-proof-7.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img-proof-7.9.0.tar", last modified: Wed Mar 16 19:13:52 2022, max compression
+gzip compressed data, was "img-proof-7.9.1.tar", last modified: Wed Mar 16 20:47:38 2022, max compression
```

## Comparing `img-proof-7.9.0.tar` & `img-proof-7.9.1.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.756634 img-proof-7.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    25357 2022-03-16 19:13:42.000000 img-proof-7.9.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (121)     2460 2022-03-16 19:13:42.000000 img-proof-7.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    32403 2022-03-16 19:13:42.000000 img-proof-7.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-03-16 19:13:42.000000 img-proof-7.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-03-16 19:13:52.756634 img-proof-7.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4068 2022-03-16 19:13:42.000000 img-proof-7.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.744634 img-proof-7.9.0/img_proof/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/azure_creds_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/collect_items.py
--rw-r--r--   0 runner    (1001) docker     (121)     9600 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_aliyun.py
--rw-r--r--   0 runner    (1001) docker     (121)    19298 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_azure.py
--rw-r--r--   0 runner    (1001) docker     (121)    30063 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6716 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     6292 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_distro.py
--rw-r--r--   0 runner    (1001) docker     (121)     9825 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_ec2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_fedora.py
--rw-r--r--   0 runner    (1001) docker     (121)    20205 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_gce.py
--rw-r--r--   0 runner    (1001) docker     (121)    17404 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_oci.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_opensuse_leap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_redhat.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_rhel.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_sle_micro.py
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_sles.py
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_ssh.py
--rw-r--r--   0 runner    (1001) docker     (121)    16526 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/ipa_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.748634 img-proof-7.9.0/img_proof/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19801 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6097 2022-03-16 19:13:42.000000 img-proof-7.9.0/img_proof/scripts/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.748634 img-proof-7.9.0/img_proof.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-03-16 19:13:52.000000 img-proof-7.9.0/img_proof.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5735 2022-03-16 19:13:52.000000 img-proof-7.9.0/img_proof.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 19:13:52.000000 img-proof-7.9.0/img_proof.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-16 19:13:52.000000 img-proof-7.9.0/img_proof.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 19:13:52.000000 img-proof-7.9.0/img_proof.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-03-16 19:13:52.000000 img-proof-7.9.0/img_proof.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-16 19:13:52.000000 img-proof-7.9.0/img_proof.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-16 19:13:42.000000 img-proof-7.9.0/ipa-complete.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.748634 img-proof-7.9.0/package/
--rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-03-16 19:13:42.000000 img-proof-7.9.0/package/python3-img-proof.spec
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-03-16 19:13:42.000000 img-proof-7.9.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-03-16 19:13:42.000000 img-proof-7.9.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-03-16 19:13:42.000000 img-proof-7.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-03-16 19:13:52.756634 img-proof-7.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-03-16 19:13:42.000000 img-proof-7.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.748634 img-proof-7.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.748634 img-proof-7.9.0/tests/azure/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/azure/test-sa.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.748634 img-proof-7.9.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/.history
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/bad.results
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/config
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/config.noregion
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/empty.file
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/empty.history
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/eof.history
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/history.log
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/history.results
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/history2.log
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/history2.results
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/ida_test
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/ida_test.pub
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.748634 img-proof-7.9.0/tests/data/injection/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/injection/test_injection.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/invalid.history
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/test.results
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/tests/data/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests/test_broken.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests/test_image_desc.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests/test_pytest_json_results.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests/test_sles.py
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests/test_sles_desc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/tests/data/tests2/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests2/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/tests/data/tests3/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests3/test_image.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests3/test_image.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/tests/data/tests4/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/data/tests4/test_image_desc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/tests/ec2/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/ec2/.ec2utils.conf
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/ec2/.ec2utils.conf.nokey
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/tests/gce/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/gce/invalid-service-account.json
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/gce/service-account.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/tests/oci/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/oci/api_key.pem
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/oci/config
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_collect_items_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9008 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_alibaba.py
--rw-r--r--   0 runner    (1001) docker     (121)    12802 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_azure.py
--rw-r--r--   0 runner    (1001) docker     (121)    13164 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    23918 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_distro.py
--rw-r--r--   0 runner    (1001) docker     (121)    10490 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_ec2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_fedora_distro.py
--rw-r--r--   0 runner    (1001) docker     (121)    18115 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_gce.py
--rw-r--r--   0 runner    (1001) docker     (121)    21266 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_oci.py
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_opensuse_leap_distro.py
--rw-r--r--   0 runner    (1001) docker     (121)     4869 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_redhat_distro.py
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_rhel_distro.py
--rw-r--r--   0 runner    (1001) docker     (121)     4831 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_sles_distro.py
--rw-r--r--   0 runner    (1001) docker     (121)     3192 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_ssh.py
--rw-r--r--   0 runner    (1001) docker     (121)    11254 2022-03-16 19:13:42.000000 img-proof-7.9.0/tests/test_ipa_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-03-16 19:13:42.000000 img-proof-7.9.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.740634 img-proof-7.9.0/usr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.740634 img-proof-7.9.0/usr/share/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.740634 img-proof-7.9.0/usr/share/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.740634 img-proof-7.9.0/usr/share/lib/img_proof/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/usr/share/lib/img_proof/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Aliyun/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Aliyun/test_sles_aliyun.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Aliyun/test_sles_aliyun_services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.752634 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Azure/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure_accel_networking.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure_infiniband.py
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure_services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.756634 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_billing_code.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_byos.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_dracut_conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_network.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_no_billing_code.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_on_demand.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_services.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.756634 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/GCE/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/GCE/test_sles_gce.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/GCE/test_sles_gce_services.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/GCE/test_sles_gce_sev.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.756634 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/SAP/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/SAP/test_sles_sap.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/SAP/test_sles_sap_license.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/SAP/test_sles_sap_motd.py
--rw-r--r--   0 runner    (1001) docker     (121)    20211 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.756634 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/infra/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new_reg.py
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new_smt.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new_smt_reg.py
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/infra/test_sles_smt_failover.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/infra/test_sles_switch_smt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.756634 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/oci/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/oci/test_sles_oci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/oci/test_sles_oci_services.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_grow_root.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_guestregister.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_haveged.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_hostname.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_install_migration.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_kernel_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_license.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_lscpu.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_migration.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_motd.py
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_multipath_off.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_on_demand.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_repos.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_root_pass.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_smt_reg.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_wait_on_registration.py
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_zypper_migration.py
--rw-r--r--   0 runner    (1001) docker     (121)     6388 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 19:13:52.756634 img-proof-7.9.0/usr/share/lib/img_proof/tests/openSUSE_Leap/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/openSUSE_Leap/test_leap.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/openSUSE_Leap/test_leap_ec2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-03-16 19:13:42.000000 img-proof-7.9.0/usr/share/lib/img_proof/tests/openSUSE_Leap/test_leap_license.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    25442 2022-03-16 20:47:28.000000 img-proof-7.9.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2460 2022-03-16 20:47:28.000000 img-proof-7.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    32403 2022-03-16 20:47:28.000000 img-proof-7.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-03-16 20:47:28.000000 img-proof-7.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-03-16 20:47:38.369338 img-proof-7.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4068 2022-03-16 20:47:28.000000 img-proof-7.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.361338 img-proof-7.9.1/img_proof/
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/azure_creds_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/collect_items.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9600 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_aliyun.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19298 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_azure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30063 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6716 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6292 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_distro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9825 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_fedora.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20205 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_gce.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17404 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_oci.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_opensuse_leap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_redhat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_rhel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_sle_micro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_sles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16526 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/ipa_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.361338 img-proof-7.9.1/img_proof/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19801 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6097 2022-03-16 20:47:28.000000 img-proof-7.9.1/img_proof/scripts/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.361338 img-proof-7.9.1/img_proof.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-03-16 20:47:38.000000 img-proof-7.9.1/img_proof.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5735 2022-03-16 20:47:38.000000 img-proof-7.9.1/img_proof.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 20:47:38.000000 img-proof-7.9.1/img_proof.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-16 20:47:38.000000 img-proof-7.9.1/img_proof.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 20:47:38.000000 img-proof-7.9.1/img_proof.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-03-16 20:47:38.000000 img-proof-7.9.1/img_proof.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-16 20:47:38.000000 img-proof-7.9.1/img_proof.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-16 20:47:28.000000 img-proof-7.9.1/ipa-complete.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.361338 img-proof-7.9.1/package/
+-rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-03-16 20:47:28.000000 img-proof-7.9.1/package/python3-img-proof.spec
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-03-16 20:47:28.000000 img-proof-7.9.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-03-16 20:47:28.000000 img-proof-7.9.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-03-16 20:47:28.000000 img-proof-7.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-03-16 20:47:38.369338 img-proof-7.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-03-16 20:47:28.000000 img-proof-7.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.361338 img-proof-7.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/azure/
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/azure/test-sa.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/.history
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/bad.results
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/config
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/config.noregion
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/empty.file
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/empty.history
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/eof.history
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/history.log
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/history.results
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/history2.log
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/history2.results
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/ida_test
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/ida_test.pub
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/data/injection/
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/injection/test_injection.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/invalid.history
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/test.results
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests/test_broken.py
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests/test_image_desc.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests/test_pytest_json_results.py
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests/test_sles.py
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests/test_sles_desc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/data/tests2/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests2/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/data/tests3/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests3/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests3/test_image.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/data/tests4/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/data/tests4/test_image_desc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/ec2/
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/ec2/.ec2utils.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/ec2/.ec2utils.conf.nokey
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/gce/
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/gce/invalid-service-account.json
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/gce/service-account.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/tests/oci/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/oci/api_key.pem
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/oci/config
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_collect_items_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9008 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12802 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_azure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13164 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23918 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_distro.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10490 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_fedora_distro.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18800 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_gce.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21266 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_oci.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_opensuse_leap_distro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4869 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_redhat_distro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_rhel_distro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4831 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_sles_distro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3192 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11254 2022-03-16 20:47:28.000000 img-proof-7.9.1/tests/test_ipa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-03-16 20:47:28.000000 img-proof-7.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.357338 img-proof-7.9.1/usr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.357338 img-proof-7.9.1/usr/share/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.357338 img-proof-7.9.1/usr/share/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.357338 img-proof-7.9.1/usr/share/lib/img_proof/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.365338 img-proof-7.9.1/usr/share/lib/img_proof/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Aliyun/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Aliyun/test_sles_aliyun.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Aliyun/test_sles_aliyun_services.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Azure/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure_accel_networking.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure_infiniband.py
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure_services.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_billing_code.py
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_byos.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_dracut_conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_no_billing_code.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_on_demand.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_services.py
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/GCE/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/GCE/test_sles_gce.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/GCE/test_sles_gce_services.py
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/GCE/test_sles_gce_sev.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/SAP/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/SAP/test_sles_sap.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/SAP/test_sles_sap_license.py
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/SAP/test_sles_sap_motd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20211 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/infra/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new_reg.py
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new_smt.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new_smt_reg.py
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/infra/test_sles_smt_failover.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      941 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/infra/test_sles_switch_smt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/oci/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/oci/test_sles_oci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/oci/test_sles_oci_services.py
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_grow_root.py
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_guestregister.py
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_haveged.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_install_migration.py
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_kernel_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_license.py
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_lscpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_motd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_multipath_off.py
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_on_demand.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_repos.py
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_root_pass.py
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_smt_reg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_wait_on_registration.py
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_zypper_migration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6388 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:47:38.369338 img-proof-7.9.1/usr/share/lib/img_proof/tests/openSUSE_Leap/
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/openSUSE_Leap/test_leap.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/openSUSE_Leap/test_leap_ec2.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-03-16 20:47:28.000000 img-proof-7.9.1/usr/share/lib/img_proof/tests/openSUSE_Leap/test_leap_license.py
```

### Comparing `img-proof-7.9.0/CHANGES.md` & `img-proof-7.9.1/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v7.9.1 (2022-03-16)
+===================
+
+- Fix GCE auth tests to avoid auth request
+
 v7.9.0 (2022-03-16)
 ===================
 
 - Force GCE auth to provide a useful error message with invalid credentials
 
 v7.8.2 (2022-02-24)
 ===================
```

### Comparing `img-proof-7.9.0/CONTRIBUTING.md` & `img-proof-7.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/LICENSE` & `img-proof-7.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/PKG-INFO` & `img-proof-7.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img-proof
-Version: 7.9.0
+Version: 7.9.1
 Summary: Package for automated testing of cloud images.
 Home-page: https://github.com/SUSE-Enceladus/img-proof
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: img-proof img_proof
 Platform: UNKNOWN
```

### Comparing `img-proof-7.9.0/README.md` & `img-proof-7.9.1/README.md`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/__init__.py` & `img-proof-7.9.1/img_proof/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = """SUSE"""
 __email__ = 'public-cloud-dev@susecloud.net'
-__version__ = '7.9.0'
+__version__ = '7.9.1'
```

### Comparing `img-proof-7.9.0/img_proof/azure_creds_wrapper.py` & `img-proof-7.9.1/img_proof/azure_creds_wrapper.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/collect_items.py` & `img-proof-7.9.1/img_proof/collect_items.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_aliyun.py` & `img-proof-7.9.1/img_proof/ipa_aliyun.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_azure.py` & `img-proof-7.9.1/img_proof/ipa_azure.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_cloud.py` & `img-proof-7.9.1/img_proof/ipa_cloud.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_constants.py` & `img-proof-7.9.1/img_proof/ipa_constants.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_controller.py` & `img-proof-7.9.1/img_proof/ipa_controller.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_distro.py` & `img-proof-7.9.1/img_proof/ipa_distro.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_ec2.py` & `img-proof-7.9.1/img_proof/ipa_ec2.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_exceptions.py` & `img-proof-7.9.1/img_proof/ipa_exceptions.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_fedora.py` & `img-proof-7.9.1/img_proof/ipa_fedora.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_gce.py` & `img-proof-7.9.1/img_proof/ipa_gce.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_oci.py` & `img-proof-7.9.1/img_proof/ipa_oci.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_opensuse_leap.py` & `img-proof-7.9.1/img_proof/ipa_opensuse_leap.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_redhat.py` & `img-proof-7.9.1/img_proof/ipa_redhat.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_rhel.py` & `img-proof-7.9.1/img_proof/ipa_rhel.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_sle_micro.py` & `img-proof-7.9.1/img_proof/ipa_sle_micro.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_sles.py` & `img-proof-7.9.1/img_proof/ipa_sles.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_ssh.py` & `img-proof-7.9.1/img_proof/ipa_ssh.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/ipa_utils.py` & `img-proof-7.9.1/img_proof/ipa_utils.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/scripts/__init__.py` & `img-proof-7.9.1/img_proof/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/scripts/cli.py` & `img-proof-7.9.1/img_proof/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof/scripts/cli_utils.py` & `img-proof-7.9.1/img_proof/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/img_proof.egg-info/PKG-INFO` & `img-proof-7.9.1/img_proof.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img-proof
-Version: 7.9.0
+Version: 7.9.1
 Summary: Package for automated testing of cloud images.
 Home-page: https://github.com/SUSE-Enceladus/img-proof
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: img-proof img_proof
 Platform: UNKNOWN
```

### Comparing `img-proof-7.9.0/img_proof.egg-info/SOURCES.txt` & `img-proof-7.9.1/img_proof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/package/python3-img-proof.spec` & `img-proof-7.9.1/package/python3-img-proof.spec`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Please submit bugfixes or comments via https://bugs.opensuse.org/
 #
 
 
 %bcond_without test
 Name:           python3-img-proof
-Version:        7.9.0
+Version:        7.9.1
 Release:        0
 Summary:        Command line and API for testing custom images
 License:        GPL-3.0-or-later
 Group:          Development/Languages/Python
 URL:            https://github.com/SUSE-Enceladus/img-proof
 Source:         https://files.pythonhosted.org/packages/source/i/img-proof/img-proof-%{version}.tar.gz
 BuildRequires:  python-rpm-macros
@@ -64,26 +64,26 @@
 Requires:       python3-google-auth
 Requires:       python3-oci-sdk
 Requires:       python3-paramiko
 Requires:       python3-pytest
 Requires:       python3-pytest-testinfra
 Requires:       python3-pytest-json-report
 BuildArch:      noarch
-Obsoletes:      python3-ipa < 7.9.0
+Obsoletes:      python3-ipa < 7.9.1
 
 %description
 img-proof provides a command line utility to test images in
 the Public Cloud (AWS, Azure, GCE, etc.).
 
 %package tests
 Summary:        Infrastructure tests for img-proof
 Group:          Development/Languages/Python
 Requires:       python3-susepubliccloudinfo
 PreReq:         python3-img-proof = %{version}
-Obsoletes:      python3-ipa-tests < 7.9.0
+Obsoletes:      python3-ipa-tests < 7.9.1
 
 %description tests
 Directory of infrastructure tests for testing images.
 
 %prep
 %setup -q -n img-proof-%{version}
```

### Comparing `img-proof-7.9.0/setup.py` & `img-proof-7.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     'tox',
     'tox-pyenv'
 ]
 
 
 setup(
     name='img-proof',
-    version='7.9.0',
+    version='7.9.1',
     description="Package for automated testing of cloud images.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SUSE",
     author_email='public-cloud-dev@susecloud.net',
     url='https://github.com/SUSE-Enceladus/img-proof',
     packages=find_packages(),
```

### Comparing `img-proof-7.9.0/tests/data/ida_test` & `img-proof-7.9.1/tests/data/ida_test`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/data/test.results` & `img-proof-7.9.1/tests/data/test.results`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_collect_items_plugin.py` & `img-proof-7.9.1/tests/test_collect_items_plugin.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_alibaba.py` & `img-proof-7.9.1/tests/test_ipa_alibaba.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_azure.py` & `img-proof-7.9.1/tests/test_ipa_azure.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_cli.py` & `img-proof-7.9.1/tests/test_ipa_cli.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_cli_utils.py` & `img-proof-7.9.1/tests/test_ipa_cli_utils.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_cloud.py` & `img-proof-7.9.1/tests/test_ipa_cloud.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_controller.py` & `img-proof-7.9.1/tests/test_ipa_controller.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_distro.py` & `img-proof-7.9.1/tests/test_ipa_distro.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_ec2.py` & `img-proof-7.9.1/tests/test_ipa_ec2.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_fedora_distro.py` & `img-proof-7.9.1/tests/test_ipa_fedora_distro.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_gce.py` & `img-proof-7.9.1/tests/test_ipa_gce.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,23 +45,25 @@
 
     return HttpError(resp, json.dumps(content).encode())
 
 
 class TestGCECloud(object):
     """Test GCE cloud class."""
 
+    @patch('img_proof.ipa_gce.AuthorizedSession')
     @patch('img_proof.ipa_gce.service_account')
     @patch.object(GCECloud, '_validate_region')
     @patch('img_proof.ipa_gce.discovery')
     def setup_method(
         self,
         method,
         mock_discovery,
         mock_validate_region,
-        mock_service_account
+        mock_service_account,
+        mock_auth_session
     ):
         """Set up kwargs dict."""
         self.kwargs = {
             'config': 'tests/data/config',
             'distro_name': 'SLES',
             'image_id': 'fakeimage',
             'no_default_test_dirs': True,
@@ -115,14 +117,32 @@
             self.cloud._get_credentials()
 
         msg = 'Service account JSON file is invalid for GCE. ' \
             'client_email key is expected. See getting started ' \
             'docs for information on GCE configuration.'
         assert str(error.value) == msg
 
+    @patch('img_proof.ipa_gce.AuthorizedSession')
+    @patch('img_proof.ipa_gce.service_account')
+    def test_gce_get_creds_invalid(
+        self,
+        mock_service_account,
+        mock_auth_session
+    ):
+        """Test get credentials method with exception."""
+        session = MagicMock()
+        session.get.side_effect = Exception('Invalid creds!')
+        mock_auth_session.return_value = session
+
+        with pytest.raises(GCECloudException) as error:
+            self.cloud._get_credentials()
+
+        msg = 'GCP authentication failed: Invalid creds!'
+        assert str(error.value) == msg
+
     def test_gce_get_instance(self):
         """Test gce get instance method."""
         instance = MagicMock()
         instances_obj = MagicMock()
         operation = MagicMock()
         operation.execute.return_value = instance
         instances_obj.get.return_value = operation
```

### Comparing `img-proof-7.9.0/tests/test_ipa_oci.py` & `img-proof-7.9.1/tests/test_ipa_oci.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_opensuse_leap_distro.py` & `img-proof-7.9.1/tests/test_ipa_opensuse_leap_distro.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_redhat_distro.py` & `img-proof-7.9.1/tests/test_ipa_redhat_distro.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_rhel_distro.py` & `img-proof-7.9.1/tests/test_ipa_rhel_distro.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_sles_distro.py` & `img-proof-7.9.1/tests/test_ipa_sles_distro.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_ssh.py` & `img-proof-7.9.1/tests/test_ipa_ssh.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/tests/test_ipa_utils.py` & `img-proof-7.9.1/tests/test_ipa_utils.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Aliyun/test_sles_aliyun_services.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Aliyun/test_sles_aliyun_services.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure_services.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/Azure/test_sles_azure_services.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_dracut_conf.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_dracut_conf.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_network.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_network.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_services.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/EC2/test_sles_ec2_services.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/GCE/test_sles_gce_services.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/GCE/test_sles_gce_services.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/SAP/test_sles_sap_license.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/SAP/test_sles_sap_license.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/conftest.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/conftest.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new_smt_reg.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/infra/test_sles_force_new_smt_reg.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/infra/test_sles_switch_smt.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/infra/test_sles_switch_smt.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/oci/test_sles_oci_services.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/oci/test_sles_oci_services.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_grow_root.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_grow_root.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_kernel_version.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_kernel_version.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_license.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_license.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_repos.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_repos.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_smt_reg.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_smt_reg.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/SLES/test_sles_wait_on_registration.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/SLES/test_sles_wait_on_registration.py`

 * *Files identical despite different names*

### Comparing `img-proof-7.9.0/usr/share/lib/img_proof/tests/conftest.py` & `img-proof-7.9.1/usr/share/lib/img_proof/tests/conftest.py`

 * *Files identical despite different names*

