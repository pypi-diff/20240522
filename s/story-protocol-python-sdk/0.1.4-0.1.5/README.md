# Comparing `tmp/story_protocol_python_sdk-0.1.4.tar.gz` & `tmp/story_protocol_python_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.1.4.tar", last modified: Tue May 21 21:55:08 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.1.5.tar", last modified: Wed May 22 18:52:02 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.1.4.tar` & `story_protocol_python_sdk-0.1.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.375246 story_protocol_python_sdk-0.1.4/
--rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      932 2024-05-21 21:55:08.374248 story_protocol_python_sdk-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.4/README.md
--rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 21:55:08.375246 story_protocol_python_sdk-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-21 21:55:00.000000 story_protocol_python_sdk-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.303220 story_protocol_python_sdk-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.315221 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/
--rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.334224 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.338221 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IPAssetRegistry/
--rw-rw-rw-   0        0        0    13409 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-rw-rw-   0        0        0     4546 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.341221 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
--rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.344221 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseRegistry/
--rw-rw-rw-   0        0        0    26905 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-rw-rw-   0        0        0     4230 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.348222 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseToken/
--rw-rw-rw-   0        0        0    23007 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
--rw-rw-rw-   0        0        0     1159 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.351226 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicensingModule/
--rw-rw-rw-   0        0        0    19697 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
--rw-rw-rw-   0        0        0     5246 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.354226 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/PILicenseTemplate/
--rw-rw-rw-   0        0        0    26246 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-rw-rw-   0        0        0     4625 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.358222 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyModule/
--rw-rw-rw-   0        0        0    16029 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-rw-rw-   0        0        0     1489 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.361224 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
--rw-rw-rw-   0        0        0    14037 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-rw-rw-   0        0        0     1183 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.365222 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/resources/
--rw-rw-rw-   0        0        0     6739 2024-05-21 21:20:33.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/resources/IPAsset.py
--rw-rw-rw-   0        0        0    16122 2024-05-21 21:21:25.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/resources/License.py
--rw-rw-rw-   0        0        0    12345 2024-05-21 21:21:50.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/resources/Royalty.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.371253 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/scripts/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/scripts/__init__.py
--rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/scripts/config.json
--rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/scripts/config_impl.json
--rw-rw-rw-   0        0        0     7361 2024-05-21 21:24:57.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/scripts/generate_client.py
--rw-rw-rw-   0        0        0     5288 2024-05-21 21:26:03.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/scripts/generate_client_impl.py
--rw-rw-rw-   0        0        0     1561 2024-05-21 21:48:50.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/story_client.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.373246 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/utils/license_terms.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:55:08.332220 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      932 2024-05-21 21:55:08.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2710 2024-05-21 21:55:08.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 21:55:08.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-21 21:55:08.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-21 21:55:08.000000 story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.752024 story_protocol_python_sdk-0.1.5/
+-rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      932 2024-05-22 18:52:02.750023 story_protocol_python_sdk-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.5/README.md
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 18:52:02.752024 story_protocol_python_sdk-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-22 18:50:15.000000 story_protocol_python_sdk-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.376131 story_protocol_python_sdk-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.395128 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/
+-rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.418129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.451129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-rw-rw-   0        0        0    13409 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-rw-rw-   0        0        0     4546 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.551129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.564131 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-rw-rw-   0        0        0    26905 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-rw-rw-   0        0        0     4230 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.590135 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-rw-rw-   0        0        0    23007 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-rw-rw-   0        0        0     1159 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.603130 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-rw-rw-   0        0        0    19697 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-rw-rw-   0        0        0     5246 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.616129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-rw-rw-   0        0        0    26246 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-rw-rw-   0        0        0     4625 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.635129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-rw-rw-   0        0        0    16029 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-rw-rw-   0        0        0     1489 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.660133 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-rw-rw-   0        0        0    14037 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-rw-rw-   0        0        0     1183 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.682130 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/
+-rw-rw-rw-   0        0        0     7087 2024-05-22 18:39:33.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-rw-rw-   0        0        0    16684 2024-05-22 18:40:50.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/License.py
+-rw-rw-rw-   0        0        0    12865 2024-05-22 18:41:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.743027 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/config.json
+-rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-rw-rw-   0        0        0     7361 2024-05-21 21:24:57.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-rw-rw-   0        0        0     5288 2024-05-21 21:26:03.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-rw-rw-   0        0        0     1561 2024-05-22 18:49:34.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/story_client.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.747027 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/utils/license_terms.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.416128 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      932 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2710 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.1.4/LICENSE` & `story_protocol_python_sdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/PKG-INFO` & `story_protocol_python_sdk-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: story_protocol_python_sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/resources/IPAsset.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/IPAsset.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,21 +38,25 @@
             ip_id = self._get_ip_id(token_contract, token_id)
             if self._is_registered(ip_id):
                 return {
                     'txHash': None,
                     'ipId': ip_id
                 }
 
+
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = self.ip_asset_registry_client.build_register_transaction(
                 self.chain_id, token_contract, token_id, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
-                    'gasPrice': self.web3.to_wei('300', 'gwei')  # Adjusted gas price for faster processing
+                    'gasPrice': current_gas_price
                 }
             )
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
 
             # Send the transaction
@@ -85,21 +89,24 @@
                 raise ValueError("There must be 1 or 2 parent IP IDs.")
 
             # Check if license terms are attached to parent IPs
             for parent_id, terms_id in zip(parent_ip_ids, license_terms_ids):
                 if not self.license_registry_client.hasIpAttachedLicenseTerms(parent_id, license_template, terms_id):
                     raise ValueError(f"License terms id {terms_id} must be attached to the parent ipId {parent_id} before registering derivative.")
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = self.licensing_module_client.build_registerDerivative_transaction(
                 child_ip_id, parent_ip_ids, license_terms_ids, license_template, '0x0000000000000000000000000000000000000000', {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
-                    'gasPrice': self.web3.to_wei('100', 'gwei')
+                    'gasPrice': current_gas_price
                 }
             )
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
 
             # Send the transaction
@@ -121,21 +128,24 @@
 
             # Ensure license token IDs are owned by the caller
             for token_id in license_token_ids:
                 token_owner = self.license_token_client.ownerOf(token_id)
                 if token_owner.lower() != self.account.address.lower():
                     raise ValueError(f"License token id {token_id} must be owned by the caller.")
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = self.licensing_module_client.build_registerDerivativeWithLicenseTokens_transaction(
                 child_ip_id, license_token_ids, '0x0000000000000000000000000000000000000000', {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
-                    'gasPrice': self.web3.to_wei('300', 'gwei')
+                    'gasPrice': current_gas_price
                 }
             )
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
 
             # Send the transaction
```

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/resources/License.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/License.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,21 +35,24 @@
 
             # Check if the license terms are already registered
             license_terms_id = self._get_license_terms_id(license_terms)
             # logger.info(f"License terms ID: {license_terms_id}")
             if (license_terms_id is not None) and (license_terms_id != 0):
                 return {'licenseTermsId': license_terms_id}
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = self.license_template_client.build_registerLicenseTerms_transaction(
                 license_terms, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
-                    'gasPrice': self.web3.to_wei('100', 'gwei')  # Adjusted gas price for faster processing
+                    'gasPrice': current_gas_price
                 }
             )
             # logger.info(f"Transaction: {transaction}")
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
@@ -88,21 +91,24 @@
 
             # Check if the license terms are already registered
             license_terms_id = self._get_license_terms_id(complete_license_terms)
             # logger.info(f"License terms ID: {license_terms_id}")
             if (license_terms_id is not None) and (license_terms_id != 0):
                 return {'licenseTermsId': license_terms_id}
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = self.license_template_client.build_registerLicenseTerms_transaction(
                 complete_license_terms, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
-                    'gasPrice': self.web3.to_wei('100', 'gwei')  # Adjusted gas price for faster processing
+                    'gasPrice': current_gas_price
                 }
             )
             # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
@@ -145,21 +151,24 @@
 
             # Check if the license terms are already registered
             license_terms_id = self._get_license_terms_id(complete_license_terms)
             # logger.info(f"License terms ID: {license_terms_id}")
             if license_terms_id and license_terms_id != 0:
                 return {'licenseTermsId': license_terms_id}
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = self.license_template_client.build_registerLicenseTerms_transaction(
                 complete_license_terms, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
-                    'gasPrice': self.web3.to_wei('100', 'gwei')
+                    'gasPrice': current_gas_price
                 }
             )
             # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
@@ -215,21 +224,24 @@
                 raise ValueError(f"License terms id {license_terms_id} do not exist.")
 
             # Check if the license terms are already attached to the IP
             is_attached_license_terms = self.license_registry_client.hasIpAttachedLicenseTerms(ip_id, license_template, license_terms_id)
             if is_attached_license_terms:
                 raise ValueError(f"License terms id {license_terms_id} is already attached to the IP with id {ip_id}.")
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = self.licensing_module_client.build_attachLicenseTerms_transaction(
                 ip_id, license_template, license_terms_id, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
-                    'gasPrice': self.web3.to_wei('100', 'gwei')
+                    'gasPrice': current_gas_price
                 }
             )
             # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
@@ -271,21 +283,24 @@
                 raise ValueError(f"License terms id {license_terms_id} do not exist.")
 
             # Check if the license terms are attached to the IP
             is_attached_license_terms = self.license_registry_client.hasIpAttachedLicenseTerms(licensor_ip_id, license_template, license_terms_id)
             if not is_attached_license_terms:
                 raise ValueError(f"License terms id {license_terms_id} is not attached to the IP with id {licensor_ip_id}.")
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = self.licensing_module_client.build_mintLicenseTokens_transaction(
                 licensor_ip_id, license_template, license_terms_id, amount, receiver, '0x0000000000000000000000000000000000000000', {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
-                    'gasPrice': self.web3.to_wei('100', 'gwei')
+                    'gasPrice': current_gas_price
                 }
             )
             # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
```

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/resources/Royalty.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/Royalty.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,20 +32,23 @@
             # print("gonna check for royalty vault addy")
             proxy_address = self._getRoyaltyVaultAddress(child_ip_id)
             # print("The proxy address: ", proxy_address)
 
             # Initialize the IP Royalty Vault client with the proxy address
             ip_royalty_vault_client = IpRoyaltyVaultImplClient(self.web3, contract_address=proxy_address)
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = ip_royalty_vault_client.build_collectRoyaltyTokens_transaction(parent_ip_id, {
                 'from': self.account.address,
                 'nonce': self.web3.eth.get_transaction_count(self.account.address),
                 'gas': 2000000,
-                'gasPrice': self.web3.to_wei('300', 'gwei')
+                'gasPrice': current_gas_price
             })
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
@@ -101,20 +104,23 @@
             proxy_address = self._getRoyaltyVaultAddress(child_ip_id)
             # logger.info(f"The proxy address: {proxy_address}")
             #print("Thne proxy addres: ", proxy_address)
 
             # Initialize the IP Royalty Vault client with the proxy address
             ip_royalty_vault_client = IpRoyaltyVaultImplClient(self.web3, contract_address=proxy_address)
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = ip_royalty_vault_client.build_snapshot_transaction({
                 'from': self.account.address,
                 'nonce': self.web3.eth.get_transaction_count(self.account.address),
                 'gas': 2000000,
-                'gasPrice': self.web3.to_wei('300', 'gwei')
+                'gasPrice': current_gas_price
             })
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
@@ -181,20 +187,23 @@
                 raise ValueError(f"The receiver IP with id {receiver_ip_id} is not registered.")
 
             # Check if the payer IP is registered
             is_payer_registered = self.ip_asset_registry_client.isRegistered(payer_ip_id)
             if not is_payer_registered:
                 raise ValueError(f"The payer IP with id {payer_ip_id} is not registered.")
             
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = self.royalty_module_client.build_payRoyaltyOnBehalf_transaction(receiver_ip_id, payer_ip_id, token, amount, {
                 'from': self.account.address,
                 'nonce': self.web3.eth.get_transaction_count(self.account.address),
                 'gas': 2000000,
-                'gasPrice': self.web3.to_wei('300', 'gwei')
+                'gasPrice': current_gas_price
             })
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
@@ -220,20 +229,23 @@
             proxy_address = self._getRoyaltyVaultAddress(child_ip_id)
             # logger.info(f"The proxy address: {proxy_address}")
             # print("The proxy addres: ", proxy_address)
 
             # Initialize the IP Royalty Vault client with the proxy address
             ip_royalty_vault_client = IpRoyaltyVaultImplClient(self.web3, contract_address=proxy_address)
 
+            # Fetch the current average gas price from the node plus 10%
+            current_gas_price = int(self.web3.eth.gas_price * 1.1)
+
             # Build the transaction
             transaction = ip_royalty_vault_client.build_claimRevenueBySnapshotBatch_transaction(snapshotIds, token, {
                 'from': self.account.address,
                 'nonce': self.web3.eth.get_transaction_count(self.account.address),
                 'gas': 2000000,
-                'gasPrice': self.web3.to_wei('300', 'gwei')
+                'gasPrice': current_gas_price
             })
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
```

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/scripts/config.json` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/scripts/generate_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/story_client.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/story_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk/utils/license_terms.py` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/utils/license_terms.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk.egg-info/PKG-INFO` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: story-protocol-python-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.1.4/src/story_protocol_python_sdk.egg-info/SOURCES.txt` & `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

