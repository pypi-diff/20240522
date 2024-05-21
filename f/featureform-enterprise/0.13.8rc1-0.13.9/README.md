# Comparing `tmp/featureform_enterprise-0.13.8rc1.tar.gz` & `tmp/featureform_enterprise-0.13.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featureform_enterprise-0.13.8rc1.tar", last modified: Tue May 14 18:43:11 2024, max compression
+gzip compressed data, was "featureform_enterprise-0.13.9.tar", last modified: Fri May 17 20:04:10 2024, max compression
```

## Comparing `featureform_enterprise-0.13.8rc1.tar` & `featureform_enterprise-0.13.9.tar`

### file list

```diff
@@ -1,411 +1,411 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.734175 featureform_enterprise-0.13.8rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-14 18:43:11.734175 featureform_enterprise-0.13.8rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-14 18:43:11.734175 featureform_enterprise-0.13.8rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.606175 featureform_enterprise-0.13.8rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.614175 featureform_enterprise-0.13.8rc1/src/featureform/
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    38226 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.602175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.614175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.614175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/[type]/
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/[type]/[entity].html
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/[type].html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.602175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.606175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.614175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.614175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/Whp2ynQYI3B1VGRrjktEB/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.694175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (127)    83441 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
--rw-r--r--   0 runner    (1001) docker     (127)    73108 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
--rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
--rw-r--r--   0 runner    (1001) docker     (127)   199780 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
--rw-r--r--   0 runner    (1001) docker     (127)   130088 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
--rw-r--r--   0 runner    (1001) docker     (127)   108180 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.702175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.702175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-2f83fe1ff7f9d94c.js
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
--rw-r--r--   0 runner    (1001) docker     (127)  4255345 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/_app-574fe43e4223620b.js
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.702175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.706175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.706175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/
--rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.706175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/query-5a171bd499b8d4eb.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/search-abfa6bb494904a10.js
--rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-70243ca2c0452223.js
--rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.706175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
--rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.7b558400037bbf48.js
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.79939abf3c1e11a8.js
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.dbf25fee2d30d81a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.503837d41162f24d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.9a929c1c9b2638ee.js
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.1f58545eb203e18f.js
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.5a6e695471cb4195.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.e90979a55a3b2795.js
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.cb40bb8da99d6066.js
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js
--rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a9e892235dc65f7b.js
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.a271ae92c5d426c4.js
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.bb3235d2b44fb9b3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js
--rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.b941e6f1f8370030.js
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.706175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.706175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    81048 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.706175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.706175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.706175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.710175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/group/
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/group/[groupName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/groups.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.710175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/role/
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/role/[roleName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/roles.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.710175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/user/
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/user/[userName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/users.html
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/connections.html
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/query.html
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.718175 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Capital_One_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Kubernetes_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Postgresql_elephant.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Redis_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Snowflake_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/amazon_dynamoDB.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/amazon_redshift.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/amazon_s3.svg
--rw-r--r--   0 runner    (1001) docker     (127)    26573 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/apache_cassandra.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60161 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/apache_hadoop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/azure_storage_accounts.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/base_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/clearIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/clickhouse-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    35853 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/creature.png
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/file_store.svg
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/google_bigquery.svg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/google_cloud_storage.svg
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/google_firestore.svg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/localmode.png
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/mongoDB.svg
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/offline_store.svg
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/online_store.svg
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/owner_bubble.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)   175958 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/welcomebackground.png
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-14 18:43:07.000000 featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/tasks.html
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.722175 featureform_enterprise-0.13.8rc1/src/featureform/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.722175 featureform_enterprise-0.13.8rc1/src/featureform/proto/
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-14 18:42:16.000000 featureform_enterprise-0.13.8rc1/src/featureform/proto/metadata.proto
--rw-r--r--   0 runner    (1001) docker     (127)    31926 2024-05-14 18:42:17.000000 featureform_enterprise-0.13.8rc1/src/featureform/proto/metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-14 18:42:17.000000 featureform_enterprise-0.13.8rc1/src/featureform/proto/metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   112884 2024-05-14 18:42:17.000000 featureform_enterprise-0.13.8rc1/src/featureform/proto/metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-14 18:42:16.000000 featureform_enterprise-0.13.8rc1/src/featureform/proto/serving.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-05-14 18:42:17.000000 featureform_enterprise-0.13.8rc1/src/featureform/proto/serving_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-14 18:42:17.000000 featureform_enterprise-0.13.8rc1/src/featureform/proto/serving_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-05-14 18:42:17.000000 featureform_enterprise-0.13.8rc1/src/featureform/proto/serving_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)   203890 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    84275 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    30878 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/status_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/type_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    33892 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/variant_names_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/src/featureform/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.730175 featureform_enterprise-0.13.8rc1/src/featureform_enterprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-14 18:43:11.000000 featureform_enterprise-0.13.8rc1/src/featureform_enterprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34961 2024-05-14 18:43:11.000000 featureform_enterprise-0.13.8rc1/src/featureform_enterprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:43:11.000000 featureform_enterprise-0.13.8rc1/src/featureform_enterprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 18:43:11.000000 featureform_enterprise-0.13.8rc1/src/featureform_enterprise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 18:43:11.000000 featureform_enterprise-0.13.8rc1/src/featureform_enterprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 18:43:11.000000 featureform_enterprise-0.13.8rc1/src/featureform_enterprise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:11.730175 featureform_enterprise-0.13.8rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_autogenerated_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_class_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    43785 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_executor_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_getting_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_multi_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_ondemand_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_resource_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_serving_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_source_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_source_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_spark_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    28897 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_tags_and_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_training_set_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-14 18:41:30.000000 featureform_enterprise-0.13.8rc1/tests/test_updating_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.646153 featureform_enterprise-0.13.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-17 20:04:10.646153 featureform_enterprise-0.13.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-17 20:04:10.650153 featureform_enterprise-0.13.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.562153 featureform_enterprise-0.13.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.570153 featureform_enterprise-0.13.9/src/featureform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.562153 featureform_enterprise-0.13.9/src/featureform/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.570153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.570153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type]/
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type]/[entity].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type].html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.562153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.562153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.570153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.618153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (127)    83441 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    73108 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
+-rw-r--r--   0 runner    (1001) docker     (127)   199780 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
+-rw-r--r--   0 runner    (1001) docker     (127)   130088 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
+-rw-r--r--   0 runner    (1001) docker     (127)   108180 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-2f83fe1ff7f9d94c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4255345 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/_app-574fe43e4223620b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/
+-rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/query-5a171bd499b8d4eb.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/search-abfa6bb494904a10.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-70243ca2c0452223.js
+-rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
+-rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.7b558400037bbf48.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.79939abf3c1e11a8.js
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.dbf25fee2d30d81a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.503837d41162f24d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.9a929c1c9b2638ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.1f58545eb203e18f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.5a6e695471cb4195.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.e90979a55a3b2795.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.cb40bb8da99d6066.js
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a9e892235dc65f7b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.a271ae92c5d426c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.bb3235d2b44fb9b3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.b941e6f1f8370030.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    81048 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/group/
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/group/[groupName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/groups.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/role/
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/role/[roleName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/roles.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/user/[userName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/users.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/connections.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.638153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Capital_One_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Kubernetes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Postgresql_elephant.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Redis_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Snowflake_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_dynamoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_redshift.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_s3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26573 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apache_cassandra.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60161 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apache_hadoop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/azure_storage_accounts.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/base_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/clearIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/clickhouse-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    35853 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/creature.png
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/file_store.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_bigquery.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_cloud_storage.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_firestore.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/localmode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/mongoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/offline_store.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/online_store.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/owner_bubble.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   175958 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/welcomebackground.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.638153 featureform_enterprise-0.13.9/src/featureform/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.642153 featureform_enterprise-0.13.9/src/featureform/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-17 20:03:16.000000 featureform_enterprise-0.13.9/src/featureform/proto/metadata.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    31926 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   112884 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-17 20:03:16.000000 featureform_enterprise-0.13.9/src/featureform/proto/serving.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   203902 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84275 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30878 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/status_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/type_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33892 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/variant_names_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.646153 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34961 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.646153 featureform_enterprise-0.13.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_autogenerated_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_class_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43785 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_executor_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_getting_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_multi_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_ondemand_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_resource_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_serving_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_source_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_source_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_spark_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28897 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_tags_and_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_training_set_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_updating_provider.py
```

### Comparing `featureform_enterprise-0.13.8rc1/LICENSE` & `featureform_enterprise-0.13.9/LICENSE`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/PKG-INFO` & `featureform_enterprise-0.13.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform-enterprise
-Version: 0.13.8rc1
+Version: 0.13.9
 Summary: Package for the Featureform Enterprise Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/featureform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `featureform_enterprise-0.13.8rc1/README.md` & `featureform_enterprise-0.13.9/README.md`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/setup.cfg` & `featureform_enterprise-0.13.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = featureform-enterprise
-version = 0.13.8-rc1
+version = 0.13.9
 author = FeatureForm, Inc.
 author_email = hello@featureform.com
 description = Package for the Featureform Enterprise Feature Store
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://featureform.com
 project_urls =
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/__init__.py` & `featureform_enterprise-0.13.9/src/featureform/__init__.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/cli.py` & `featureform_enterprise-0.13.9/src/featureform/cli.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/client.py` & `featureform_enterprise-0.13.9/src/featureform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
             config=config,
             tags=[tag for tag in tags.tag] or [],
             properties={key: value for key, value in properties.property.items()} or {},
         )
 
     def __get_provider(self, name):
         # Get a single provider
-        return next(self._stub.GetProviders(iter([pb.Provider(name=name)])))
+        return next(self._stub.GetProviders(iter([pb.Name(name=name)])))
 
     def get_postgres(self, name):
         """Get a Postgres provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
         postgres = client.get_postgres("postgres-quickstart")
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/404.html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type]/[entity].html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/404-8d282ae638ce5722.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-2f83fe1ff7f9d94c.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/[type]/[entity].html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/users.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-2f83fe1ff7f9d94c.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/users","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/[type].html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/groups.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-7bfcb609b1affd61.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/groups","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-2f83fe1ff7f9d94c.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-2f83fe1ff7f9d94c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/_app-574fe43e4223620b.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/_app-574fe43e4223620b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-70243ca2c0452223.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-70243ca2c0452223.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/group/[groupName].html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/group/[groupName].html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/group/%5BgroupName%5D-4ba8b6abfb4b13ca.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/group/%5BgroupName%5D-4ba8b6abfb4b13ca.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/group/[groupName]","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/group/[groupName]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/groups.html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/tasks.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/tasks-70243ca2c0452223.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/groups","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/tasks","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/role/[roleName].html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/role/%5BroleName%5D-a4f4cefefad41418.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/index-142e8557e4889163.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/role/[roleName]","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/roles.html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/roles.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/roles-a560426c6514c003.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/roles-a560426c6514c003.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/roles","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/roles","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/user/[userName].html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/user/[userName].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/user/%5BuserName%5D-5a66d4c05c9e7453.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/user/%5BuserName%5D-5a66d4c05c9e7453.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/user/[userName]","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/user/[userName]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/admin/users.html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/search-abfa6bb494904a10.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/users","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/connections.html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/query.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/connections-f98076127418a04b.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/query-5a171bd499b8d4eb.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/query","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/index.html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type].html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/index-142e8557e4889163.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-7bfcb609b1affd61.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/query.html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/role/[roleName].html`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/query-5a171bd499b8d4eb.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/role/%5BroleName%5D-a4f4cefefad41418.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/query","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/role/[roleName]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/search.html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/connections.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/search-abfa6bb494904a10.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/connections-f98076127418a04b.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Apache_Spark_logo.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Apache_Spark_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Capital_One_logo.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Capital_One_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Featureform_logo_pink.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Featureform_logo_pink.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Kubernetes_logo.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Kubernetes_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Postgresql_elephant.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Postgresql_elephant.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Redis_Logo.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Redis_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/Snowflake_Logo.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Snowflake_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/amazon_dynamoDB.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_dynamoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/amazon_redshift.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_redshift.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/amazon_s3.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_s3.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/apache_cassandra.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apache_cassandra.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/apache_hadoop.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apache_hadoop.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/apple-touch-icon.png` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/azure_storage_accounts.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/azure_storage_accounts.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/base_logo.png` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/base_logo.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/clearIcon.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/clearIcon.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/clickhouse-logo.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/clickhouse-logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/creature.png` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/creature.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/favicon.ico` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/google_bigquery.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_bigquery.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/google_cloud_storage.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_cloud_storage.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/google_firestore.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_firestore.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/logo192.png` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/logo192.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/logo512.png` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/logo512.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/mongoDB.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/mongoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/offline_store.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/offline_store.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/safari-pinned-tab.svg` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/static/welcomebackground.png` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/welcomebackground.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/dashboard/out/tasks.html` & `featureform_enterprise-0.13.9/src/featureform/dashboard/out/404.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/tasks-70243ca2c0452223.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js" defer=""></script><script src="/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/404-8d282ae638ce5722.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/tasks","query":{},"buildId":"Whp2ynQYI3B1VGRrjktEB","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/deploy.py` & `featureform_enterprise-0.13.9/src/featureform/deploy.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/enums.py` & `featureform_enterprise-0.13.9/src/featureform/enums.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/exceptions.py` & `featureform_enterprise-0.13.9/src/featureform/exceptions.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/format.py` & `featureform_enterprise-0.13.9/src/featureform/format.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/get.py` & `featureform_enterprise-0.13.9/src/featureform/get.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/grpc_client.py` & `featureform_enterprise-0.13.9/src/featureform/grpc_client.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/lib/auth.py` & `featureform_enterprise-0.13.9/src/featureform/lib/auth.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/list.py` & `featureform_enterprise-0.13.9/src/featureform/list.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/proto/metadata.proto` & `featureform_enterprise-0.13.9/src/featureform/proto/metadata.proto`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/proto/metadata_pb2.py` & `featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/proto/metadata_pb2.pyi` & `featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/proto/metadata_pb2_grpc.py` & `featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/proto/serving.proto` & `featureform_enterprise-0.13.9/src/featureform/proto/serving.proto`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/proto/serving_pb2.py` & `featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/proto/serving_pb2.pyi` & `featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/proto/serving_pb2_grpc.py` & `featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/register.py` & `featureform_enterprise-0.13.9/src/featureform/register.py`

 * *Files 0% similar despite different names*

```diff
@@ -5152,15 +5152,15 @@
             status=source.status.Status._enum_type.values[source.status.status].name,
             tags=[],
             properties={},
             source_text=(
                 definition.source_text if type(definition) == DFTransformation else ""
             ),
         )
-        return ColumnSourceRegistrar(self, source_variant)
+        return ColumnSourceRegistrar(global_registrar, source_variant)
 
     def _get_source_definition(self, source):
         if source.primaryData.table.name:
             return PrimaryData(SQLTable(source.primaryData.table.name))
         elif source.transformation:
             return self._get_transformation_definition(source)
         else:
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/resources.py` & `featureform_enterprise-0.13.9/src/featureform/resources.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/search.py` & `featureform_enterprise-0.13.9/src/featureform/search.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/serving.py` & `featureform_enterprise-0.13.9/src/featureform/serving.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/status_display.py` & `featureform_enterprise-0.13.9/src/featureform/status_display.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/tls.py` & `featureform_enterprise-0.13.9/src/featureform/tls.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/train_test_split.py` & `featureform_enterprise-0.13.9/src/featureform/train_test_split.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/type_objects.py` & `featureform_enterprise-0.13.9/src/featureform/type_objects.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/types.py` & `featureform_enterprise-0.13.9/src/featureform/types.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/variant_names_generator.py` & `featureform_enterprise-0.13.9/src/featureform/variant_names_generator.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform/version.py` & `featureform_enterprise-0.13.9/src/featureform/version.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform_enterprise.egg-info/PKG-INFO` & `featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform-enterprise
-Version: 0.13.8rc1
+Version: 0.13.9
 Summary: Package for the Featureform Enterprise Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/featureform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `featureform_enterprise-0.13.8rc1/src/featureform_enterprise.egg-info/SOURCES.txt` & `featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,14 @@
 src/featureform/dashboard/out/robots.txt
 src/featureform/dashboard/out/search.html
 src/featureform/dashboard/out/site.webmanifest
 src/featureform/dashboard/out/tasks.html
 src/featureform/dashboard/out/[type]/[entity].html
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-src/featureform/dashboard/out/_next/static/Whp2ynQYI3B1VGRrjktEB/_buildManifest.js
-src/featureform/dashboard/out/_next/static/Whp2ynQYI3B1VGRrjktEB/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
 src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
 src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
 src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
 src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
 src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
 src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
@@ -293,14 +291,16 @@
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
 src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
 src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
 src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
 src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
 src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
+src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js
+src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js
 src/featureform/dashboard/out/admin/groups.html
 src/featureform/dashboard/out/admin/roles.html
 src/featureform/dashboard/out/admin/users.html
 src/featureform/dashboard/out/admin/group/[groupName].html
 src/featureform/dashboard/out/admin/role/[roleName].html
 src/featureform/dashboard/out/admin/user/[userName].html
 src/featureform/dashboard/out/static/Apache_Spark_logo.svg
```

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_auth.py` & `featureform_enterprise-0.13.9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_autogenerated_variants.py` & `featureform_enterprise-0.13.9/tests/test_autogenerated_variants.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_class_api.py` & `featureform_enterprise-0.13.9/tests/test_class_api.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_cli.py` & `featureform_enterprise-0.13.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_client.py` & `featureform_enterprise-0.13.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_deploy.py` & `featureform_enterprise-0.13.9/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_enums.py` & `featureform_enterprise-0.13.9/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_executor_resources.py` & `featureform_enterprise-0.13.9/tests/test_executor_resources.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_getting_model.py` & `featureform_enterprise-0.13.9/tests/test_getting_model.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_multi_feature.py` & `featureform_enterprise-0.13.9/tests/test_multi_feature.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_ondemand_features.py` & `featureform_enterprise-0.13.9/tests/test_ondemand_features.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_parse.py` & `featureform_enterprise-0.13.9/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_resource_registration.py` & `featureform_enterprise-0.13.9/tests/test_resource_registration.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_search.py` & `featureform_enterprise-0.13.9/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_serving_model.py` & `featureform_enterprise-0.13.9/tests/test_serving_model.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_source_columns.py` & `featureform_enterprise-0.13.9/tests/test_source_columns.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_source_dataframe.py` & `featureform_enterprise-0.13.9/tests/test_source_dataframe.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_spark_provider.py` & `featureform_enterprise-0.13.9/tests/test_spark_provider.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_tags_and_properties.py` & `featureform_enterprise-0.13.9/tests/test_tags_and_properties.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_train_test_split.py` & `featureform_enterprise-0.13.9/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_training_set_dataframe.py` & `featureform_enterprise-0.13.9/tests/test_training_set_dataframe.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.8rc1/tests/test_updating_provider.py` & `featureform_enterprise-0.13.9/tests/test_updating_provider.py`

 * *Files identical despite different names*

