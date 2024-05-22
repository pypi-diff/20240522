# Comparing `tmp/types-hvac-2.1.0.20240514.tar.gz` & `tmp/types-hvac-2.2.0.20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-hvac-2.1.0.20240514.tar", last modified: Tue May 14 02:20:24 2024, max compression
+gzip compressed data, was "types-hvac-2.2.0.20240522.tar", last modified: Wed May 22 02:22:23 2024, max compression
```

## Comparing `types-hvac-2.1.0.20240514.tar` & `types-hvac-2.2.0.20240522.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-14 02:20:23.000000 types-hvac-2.1.0.20240514/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 02:20:23.000000 types-hvac-2.1.0.20240514/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.112275 types-hvac-2.1.0.20240514/hvac-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 02:20:23.000000 types-hvac-2.1.0.20240514/hvac-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/adapters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.112275 types-hvac-2.1.0.20240514/hvac-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.116275 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/approle.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/aws.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/azure.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/cert.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/gcp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/github.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/jwt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/ldap.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/legacy_mfa.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/oidc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/okta.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/radius.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/userpass.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.116275 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/active_directory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/aws.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/azure.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/consul.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/database.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/gcp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/identity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/kv.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/kv_v1.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/kv_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/pki.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/rabbitmq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/ssh.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/transit.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/audit.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/capabilities.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/health.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/init.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/key.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/leader.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/lease.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/mount.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/namespace.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/policies.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/policy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/quota.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/raft.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/seal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/system_backend_mixin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/wrapping.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/vault_api_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/vault_api_category.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/hvac-stubs/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/approle.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/aws.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/azure.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/gcp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/identity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/transit.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:23.000000 types-hvac-2.1.0.20240514/hvac-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/hvac-stubs/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-14 02:20:22.000000 types-hvac-2.1.0.20240514/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/types_hvac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:23.136911 types-hvac-2.2.0.20240522/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 02:22:22.000000 types-hvac-2.2.0.20240522/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 02:22:22.000000 types-hvac-2.2.0.20240522/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-22 02:22:23.136911 types-hvac-2.2.0.20240522/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:23.124911 types-hvac-2.2.0.20240522/hvac-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-22 02:22:22.000000 types-hvac-2.2.0.20240522/hvac-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/adapters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:23.124911 types-hvac-2.2.0.20240522/hvac-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:23.128911 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/approle.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/aws.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/azure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/cert.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/gcp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/github.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/jwt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/ldap.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/legacy_mfa.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/oidc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/okta.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/radius.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/userpass.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:23.128911 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/active_directory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/aws.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/azure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/consul.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/gcp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/identity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/kv.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/kv_v1.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/kv_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/ldap.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/pki.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/rabbitmq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/ssh.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/transit.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:23.132911 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/audit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/capabilities.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/health.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/init.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/key.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/leader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/lease.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/mount.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/namespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/policies.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/policy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/quota.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/raft.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/seal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/system_backend_mixin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/wrapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/vault_api_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/api/vault_api_category.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:23.132911 types-hvac-2.2.0.20240522/hvac-stubs/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/constants/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/constants/approle.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/constants/aws.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/constants/azure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/constants/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/constants/gcp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/constants/identity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/constants/transit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:22.000000 types-hvac-2.2.0.20240522/hvac-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:23.132911 types-hvac-2.2.0.20240522/hvac-stubs/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-22 02:22:00.000000 types-hvac-2.2.0.20240522/hvac-stubs/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:22:23.136911 types-hvac-2.2.0.20240522/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-22 02:22:22.000000 types-hvac-2.2.0.20240522/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:23.136911 types-hvac-2.2.0.20240522/types_hvac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-22 02:22:23.000000 types-hvac-2.2.0.20240522/types_hvac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-22 02:22:23.000000 types-hvac-2.2.0.20240522/types_hvac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:22:23.000000 types-hvac-2.2.0.20240522/types_hvac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 02:22:23.000000 types-hvac-2.2.0.20240522/types_hvac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 02:22:23.000000 types-hvac-2.2.0.20240522/types_hvac.egg-info/top_level.txt
```

### Comparing `types-hvac-2.1.0.20240514/PKG-INFO` & `types-hvac-2.2.0.20240522/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hvac
-Version: 2.1.0.20240514
+Version: 2.2.0.20240522
 Summary: Typing stubs for hvac
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hvac.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hvac`.
 
 This version of `types-hvac` aims to provide accurate annotations
-for `hvac==2.1.*`.
+for `hvac==2.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hvac. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3195f9fb1b4275144177441815e8132d4a600c83` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/adapters.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/adapters.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/__init__.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/approle.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/approle.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/aws.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/aws.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,25 @@
         access_key: Incomplete | None = None,
         secret_key: Incomplete | None = None,
         endpoint: Incomplete | None = None,
         iam_endpoint: Incomplete | None = None,
         sts_endpoint: Incomplete | None = None,
         iam_server_id_header_value: Incomplete | None = None,
         mount_point: str = "aws",
+        sts_region: str | None = None,
     ): ...
     def read_config(self, mount_point: str = "aws"): ...
     def delete_config(self, mount_point: str = "aws"): ...
     def configure_identity_integration(
-        self, iam_alias: Incomplete | None = None, ec2_alias: Incomplete | None = None, mount_point: str = "aws"
+        self,
+        iam_alias: Incomplete | None = None,
+        ec2_alias: Incomplete | None = None,
+        mount_point: str = "aws",
+        iam_metadata: str | list[str] | None = None,
+        ec2_metadata: str | list[str] | None = None,
     ): ...
     def read_identity_integration(self, mount_point: str = "aws"): ...
     def create_certificate_configuration(
         self, cert_name, aws_public_cert, document_type: Incomplete | None = None, mount_point: str = "aws"
     ): ...
     def read_certificate_configuration(self, cert_name, mount_point: str = "aws"): ...
     def delete_certificate_configuration(self, cert_name, mount_point: str = "aws"): ...
```

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/azure.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/azure.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/cert.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/cert.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/gcp.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/gcp.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/github.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/github.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/jwt.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/jwt.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         jwks_url: Incomplete | None = None,
         jwks_ca_pem: Incomplete | None = None,
         jwt_validation_pubkeys: Incomplete | None = None,
         bound_issuer: Incomplete | None = None,
         jwt_supported_algs: Incomplete | None = None,
         default_role: Incomplete | None = None,
         provider_config: Incomplete | None = None,
-        path: Incomplete | None = None,
+        path: str | None = None,
+        namespace_in_state: bool | None = None,
     ): ...
     def read_config(self, path: Incomplete | None = None): ...
     def create_role(
         self,
         name,
         user_claim,
         allowed_redirect_uris,
```

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/kubernetes.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/kubernetes.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/ldap.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/ldap.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/legacy_mfa.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/legacy_mfa.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/oidc.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/oidc.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/okta.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/okta.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/radius.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/radius.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/token.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/token.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/userpass.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/auth_methods/userpass.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/__init__.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from hvac.api.secrets_engines.azure import Azure as Azure
 from hvac.api.secrets_engines.database import Database as Database
 from hvac.api.secrets_engines.gcp import Gcp as Gcp
 from hvac.api.secrets_engines.identity import Identity as Identity
 from hvac.api.secrets_engines.kv import Kv as Kv
 from hvac.api.secrets_engines.kv_v1 import KvV1 as KvV1
 from hvac.api.secrets_engines.kv_v2 import KvV2 as KvV2
+from hvac.api.secrets_engines.ldap import Ldap as Ldap
 from hvac.api.secrets_engines.pki import Pki as Pki
 from hvac.api.secrets_engines.rabbitmq import RabbitMQ as RabbitMQ
 from hvac.api.secrets_engines.ssh import Ssh as Ssh
 from hvac.api.secrets_engines.transform import Transform as Transform
 from hvac.api.secrets_engines.transit import Transit as Transit
 from hvac.api.vault_api_category import VaultApiCategory
 
@@ -21,14 +22,15 @@
     "Azure",
     "Gcp",
     "ActiveDirectory",
     "Identity",
     "Kv",
     "KvV1",
     "KvV2",
+    "Ldap",
     "Pki",
     "Transform",
     "Transit",
     "SecretsEngines",
     "Database",
     "RabbitMQ",
     "Ssh",
```

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/active_directory.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/active_directory.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/aws.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/aws.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/azure.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/azure.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/consul.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/consul.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/database.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/database.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/gcp.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/gcp.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/identity.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/identity.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from _typeshed import Incomplete
 
 from hvac.api.vault_api_base import VaultApiBase
 
-DEFAULT_MOUNT_POINT: str
 logger: Incomplete
 
 class Identity(VaultApiBase):
     def create_or_update_entity(
         self,
         name,
         entity_id: Incomplete | None = None,
```

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/kv_v2.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/kv_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/pki.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/pki.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/rabbitmq.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/rabbitmq.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/ssh.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/ssh.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/transform.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/transform.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/transit.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/secrets_engines/transit.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,24 +38,26 @@
         plaintext: Incomplete | None = None,
         context: Incomplete | None = None,
         key_version: Incomplete | None = None,
         nonce: Incomplete | None = None,
         batch_input: Incomplete | None = None,
         type: Incomplete | None = None,
         convergent_encryption: Incomplete | None = None,
-        mount_point="transit",
+        mount_point: str = "transit",
+        associated_data: str | None = None,
     ): ...
     def decrypt_data(
         self,
         name,
         ciphertext: Incomplete | None = None,
         context: Incomplete | None = None,
         nonce: Incomplete | None = None,
         batch_input: Incomplete | None = None,
-        mount_point="transit",
+        mount_point: str = "transit",
+        associated_data: str | None = None,
     ): ...
     def rewrap_data(
         self,
         name,
         ciphertext,
         context: Incomplete | None = None,
         key_version: Incomplete | None = None,
```

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/__init__.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/audit.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/audit.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/auth.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/health.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/health.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/init.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/init.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/key.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/key.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/mount.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/mount.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/policies.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/policies.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/quota.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/quota.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/raft.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/system_backend/raft.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/api/vault_api_category.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/api/vault_api_category.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/exceptions.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/exceptions.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         json: object | None = ...,
     ) -> Self: ...
 
 class InvalidRequest(VaultError): ...
 class Unauthorized(VaultError): ...
 class Forbidden(VaultError): ...
 class InvalidPath(VaultError): ...
+class UnsupportedOperation(VaultError): ...
+class PreconditionFailed(VaultError): ...
 class RateLimitExceeded(VaultError): ...
 class InternalServerError(VaultError): ...
 class VaultNotInitialized(VaultError): ...
 class VaultDown(VaultError): ...
 class UnexpectedError(VaultError): ...
 class BadGateway(VaultError): ...
 class ParamValidationError(VaultError): ...
```

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/utils.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/hvac-stubs/v1/__init__.pyi` & `types-hvac-2.2.0.20240522/hvac-stubs/v1/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240514/setup.py` & `types-hvac-2.2.0.20240522/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hvac`.
 
 This version of `types-hvac` aims to provide accurate annotations
-for `hvac==2.1.*`.
+for `hvac==2.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hvac. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3195f9fb1b4275144177441815e8132d4a600c83` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.1.0.20240514",
+      version="2.2.0.20240522",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hvac.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-requests'],
       packages=['hvac-stubs'],
-      package_data={'hvac-stubs': ['__init__.pyi', 'adapters.pyi', 'api/__init__.pyi', 'api/auth_methods/__init__.pyi', 'api/auth_methods/approle.pyi', 'api/auth_methods/aws.pyi', 'api/auth_methods/azure.pyi', 'api/auth_methods/cert.pyi', 'api/auth_methods/gcp.pyi', 'api/auth_methods/github.pyi', 'api/auth_methods/jwt.pyi', 'api/auth_methods/kubernetes.pyi', 'api/auth_methods/ldap.pyi', 'api/auth_methods/legacy_mfa.pyi', 'api/auth_methods/oidc.pyi', 'api/auth_methods/okta.pyi', 'api/auth_methods/radius.pyi', 'api/auth_methods/token.pyi', 'api/auth_methods/userpass.pyi', 'api/secrets_engines/__init__.pyi', 'api/secrets_engines/active_directory.pyi', 'api/secrets_engines/aws.pyi', 'api/secrets_engines/azure.pyi', 'api/secrets_engines/consul.pyi', 'api/secrets_engines/database.pyi', 'api/secrets_engines/gcp.pyi', 'api/secrets_engines/identity.pyi', 'api/secrets_engines/kv.pyi', 'api/secrets_engines/kv_v1.pyi', 'api/secrets_engines/kv_v2.pyi', 'api/secrets_engines/pki.pyi', 'api/secrets_engines/rabbitmq.pyi', 'api/secrets_engines/ssh.pyi', 'api/secrets_engines/transform.pyi', 'api/secrets_engines/transit.pyi', 'api/system_backend/__init__.pyi', 'api/system_backend/audit.pyi', 'api/system_backend/auth.pyi', 'api/system_backend/capabilities.pyi', 'api/system_backend/health.pyi', 'api/system_backend/init.pyi', 'api/system_backend/key.pyi', 'api/system_backend/leader.pyi', 'api/system_backend/lease.pyi', 'api/system_backend/mount.pyi', 'api/system_backend/namespace.pyi', 'api/system_backend/policies.pyi', 'api/system_backend/policy.pyi', 'api/system_backend/quota.pyi', 'api/system_backend/raft.pyi', 'api/system_backend/seal.pyi', 'api/system_backend/system_backend_mixin.pyi', 'api/system_backend/wrapping.pyi', 'api/vault_api_base.pyi', 'api/vault_api_category.pyi', 'aws_utils.pyi', 'constants/__init__.pyi', 'constants/approle.pyi', 'constants/aws.pyi', 'constants/azure.pyi', 'constants/client.pyi', 'constants/gcp.pyi', 'constants/identity.pyi', 'constants/transit.pyi', 'exceptions.pyi', 'utils.pyi', 'v1/__init__.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'hvac-stubs': ['__init__.pyi', 'adapters.pyi', 'api/__init__.pyi', 'api/auth_methods/__init__.pyi', 'api/auth_methods/approle.pyi', 'api/auth_methods/aws.pyi', 'api/auth_methods/azure.pyi', 'api/auth_methods/cert.pyi', 'api/auth_methods/gcp.pyi', 'api/auth_methods/github.pyi', 'api/auth_methods/jwt.pyi', 'api/auth_methods/kubernetes.pyi', 'api/auth_methods/ldap.pyi', 'api/auth_methods/legacy_mfa.pyi', 'api/auth_methods/oidc.pyi', 'api/auth_methods/okta.pyi', 'api/auth_methods/radius.pyi', 'api/auth_methods/token.pyi', 'api/auth_methods/userpass.pyi', 'api/secrets_engines/__init__.pyi', 'api/secrets_engines/active_directory.pyi', 'api/secrets_engines/aws.pyi', 'api/secrets_engines/azure.pyi', 'api/secrets_engines/consul.pyi', 'api/secrets_engines/database.pyi', 'api/secrets_engines/gcp.pyi', 'api/secrets_engines/identity.pyi', 'api/secrets_engines/kv.pyi', 'api/secrets_engines/kv_v1.pyi', 'api/secrets_engines/kv_v2.pyi', 'api/secrets_engines/ldap.pyi', 'api/secrets_engines/pki.pyi', 'api/secrets_engines/rabbitmq.pyi', 'api/secrets_engines/ssh.pyi', 'api/secrets_engines/transform.pyi', 'api/secrets_engines/transit.pyi', 'api/system_backend/__init__.pyi', 'api/system_backend/audit.pyi', 'api/system_backend/auth.pyi', 'api/system_backend/capabilities.pyi', 'api/system_backend/health.pyi', 'api/system_backend/init.pyi', 'api/system_backend/key.pyi', 'api/system_backend/leader.pyi', 'api/system_backend/lease.pyi', 'api/system_backend/mount.pyi', 'api/system_backend/namespace.pyi', 'api/system_backend/policies.pyi', 'api/system_backend/policy.pyi', 'api/system_backend/quota.pyi', 'api/system_backend/raft.pyi', 'api/system_backend/seal.pyi', 'api/system_backend/system_backend_mixin.pyi', 'api/system_backend/wrapping.pyi', 'api/vault_api_base.pyi', 'api/vault_api_category.pyi', 'aws_utils.pyi', 'constants/__init__.pyi', 'constants/approle.pyi', 'constants/aws.pyi', 'constants/azure.pyi', 'constants/client.pyi', 'constants/gcp.pyi', 'constants/identity.pyi', 'constants/transit.pyi', 'exceptions.pyi', 'utils.pyi', 'v1/__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-hvac-2.1.0.20240514/types_hvac.egg-info/PKG-INFO` & `types-hvac-2.2.0.20240522/types_hvac.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hvac
-Version: 2.1.0.20240514
+Version: 2.2.0.20240522
 Summary: Typing stubs for hvac
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hvac.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hvac`.
 
 This version of `types-hvac` aims to provide accurate annotations
-for `hvac==2.1.*`.
+for `hvac==2.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hvac. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3195f9fb1b4275144177441815e8132d4a600c83` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-hvac-2.1.0.20240514/types_hvac.egg-info/SOURCES.txt` & `types-hvac-2.2.0.20240522/types_hvac.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 hvac-stubs/api/secrets_engines/consul.pyi
 hvac-stubs/api/secrets_engines/database.pyi
 hvac-stubs/api/secrets_engines/gcp.pyi
 hvac-stubs/api/secrets_engines/identity.pyi
 hvac-stubs/api/secrets_engines/kv.pyi
 hvac-stubs/api/secrets_engines/kv_v1.pyi
 hvac-stubs/api/secrets_engines/kv_v2.pyi
+hvac-stubs/api/secrets_engines/ldap.pyi
 hvac-stubs/api/secrets_engines/pki.pyi
 hvac-stubs/api/secrets_engines/rabbitmq.pyi
 hvac-stubs/api/secrets_engines/ssh.pyi
 hvac-stubs/api/secrets_engines/transform.pyi
 hvac-stubs/api/secrets_engines/transit.pyi
 hvac-stubs/api/system_backend/__init__.pyi
 hvac-stubs/api/system_backend/audit.pyi
```

