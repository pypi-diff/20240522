# Comparing `tmp/alibabacloud_dingtalk-2.1.12.tar.gz` & `tmp/alibabacloud_dingtalk-2.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.12.tar", last modified: Sat May 18 17:22:34 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.13.tar", last modified: Wed May 22 02:53:25 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.1.12.tar` & `alibabacloud_dingtalk-2.1.13.tar`

### file list

```diff
@@ -1,429 +1,429 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/
--rw-r--r--   0 root         (0) root         (0)   131089 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2575 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2660 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10220 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15463 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25446 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    24061 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51732 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    55896 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11812 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23886 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69836 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   171793 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19974 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25370 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30918 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47170 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31278 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27481 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   114212 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   145728 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   248134 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413198 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53158 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    64382 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6152 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4135 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   306758 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   657929 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98018 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   115937 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11616 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9944 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191860 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   398319 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34906 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42901 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89960 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   237978 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10504 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88282 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124205 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185660 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   224275 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71002 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   126248 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   408970 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   425714 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25686 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43876 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40206 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44858 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21312 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30666 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23500 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10844 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14576 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6516 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10302 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   315868 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   638801 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5774 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7253 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37328 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46524 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   494304 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515207 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134392 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   150282 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16480 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15793 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70120 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56029 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79025 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81667 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   313048 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   322887 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260012 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   385294 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23366 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   168538 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   200479 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   672294 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   877133 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89270 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113792 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104118 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   121491 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22157 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20888 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   477634 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552235 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191008 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   320947 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21190 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28705 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42854 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53610 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5681 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5155 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12390 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9744 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98153 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137888 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20603 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18299 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84750 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124476 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   195023 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   271213 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   365994 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   376047 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28815 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33507 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107508 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    91958 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   815324 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   937150 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75114 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   157606 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78582 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108065 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   110044 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133326 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11628 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5990 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4381 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18311 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23610 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   181489 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   173547 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62895 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53887 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71486 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    63136 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42982 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44105 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10832 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7243 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107234 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   167406 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93818 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123438 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69184 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    59069 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35028 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68771 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   319400 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   411401 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21787 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30496 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44394 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164608 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172757 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115490 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105876 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   129630 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   168457 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47742 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46647 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   460426 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   551312 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38532 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26120 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54274 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95239 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   226462 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   350226 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70068 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95695 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16918 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28519 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84018 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152968 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17044 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16445 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17118 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22383 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16528 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17427 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91210 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135827 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92596 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   111817 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40437 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40791 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10216 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21704 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79864 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129013 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6226 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8459 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50430 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43338 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   252082 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   441259 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5688 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3678 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   590500 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   761218 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4472 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14206 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/
+-rw-r--r--   0 root         (0) root         (0)   132635 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2575 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2660 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10220 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15463 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25446 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    24061 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51732 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    55896 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11812 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23886 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69836 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   171793 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19974 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25370 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30918 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47170 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31278 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27481 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   114212 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   145728 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   248134 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413198 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53158 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    64382 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6152 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   306758 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   657929 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98018 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   115937 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11616 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191860 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   398319 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34906 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42901 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89960 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   237978 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10504 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88282 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124205 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185660 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   224275 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71002 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   126248 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   408970 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   425714 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25686 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43876 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40206 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44858 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21312 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30666 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23500 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10844 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14576 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6516 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10302 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   315868 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   638801 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5774 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7253 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37328 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46524 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494304 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515207 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134392 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   150282 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16480 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15793 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70120 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56029 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79025 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81667 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   313048 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   322887 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260012 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   385294 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23366 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   168538 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   200479 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   672294 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   877133 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89270 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113792 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104118 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   121491 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22157 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20888 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   477634 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552235 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191008 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   320947 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21190 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28705 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42854 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53610 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12390 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98153 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137888 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20603 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18299 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84750 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124476 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   195023 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   271289 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   396886 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413672 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28815 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33507 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107508 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    91958 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   815324 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   937150 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75114 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   157606 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78582 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108065 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   110044 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133326 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11628 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18311 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23610 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   181489 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   173547 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62895 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53887 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71486 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    63136 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42982 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44105 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10832 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107234 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   167406 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93818 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123438 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69184 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    59069 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35028 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68771 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   319400 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   411401 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21787 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30496 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44394 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164608 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172757 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115490 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105876 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129210 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   167086 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47742 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46647 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   460426 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   551312 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38532 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26120 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54274 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95239 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   226462 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   350226 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70068 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95695 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16918 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28519 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84018 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152968 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17044 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16445 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17118 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22383 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16528 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17427 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91210 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135827 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92596 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   111817 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40437 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40791 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10216 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21704 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79864 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129013 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8459 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50430 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43338 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   252082 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   441259 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3678 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   590500 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   761218 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4472 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14206 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/setup.py
```

### Comparing `alibabacloud_dingtalk-2.1.12/ChangeLog.md` & `alibabacloud_dingtalk-2.1.13/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-05-18 Version: 2.1.12
+- Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-05-14 Version: 2.1.11
 - Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-05-09 Version: 2.1.10
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-26 Version: 2.0.99
```

### Comparing `alibabacloud_dingtalk-2.1.12/LICENSE` & `alibabacloud_dingtalk-2.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/PKG-INFO` & `alibabacloud_dingtalk-2.1.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.1.12
+Version: 2.1.13
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.12/README-CN.md` & `alibabacloud_dingtalk-2.1.13/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/README.md` & `alibabacloud_dingtalk-2.1.13/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1453,17 +1453,19 @@
     def __init__(
         self,
         app_agent_id: int = None,
         field_filter_list: List[str] = None,
         text_2select_convert: bool = None,
         user_id_list: List[str] = None,
     ):
+        # This parameter is required.
         self.app_agent_id = app_agent_id
         self.field_filter_list = field_filter_list
         self.text_2select_convert = text_2select_convert
+        # This parameter is required.
         self.user_id_list = user_id_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4307,14 +4307,376 @@
         
         @return: ListOrgTextEmotionResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkim__1__0_models.ListOrgTextEmotionHeaders()
         return await self.list_org_text_emotion_with_options_async(headers, runtime)
 
+    def open_inner_group_transfer_to_dept_group_with_options(
+        self,
+        request: dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupRequest,
+        headers: dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupResponse:
+        """
+        @summary 内部群转部门群
+        
+        @param request: OpenInnerGroupTransferToDeptGroupRequest
+        @param headers: OpenInnerGroupTransferToDeptGroupHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenInnerGroupTransferToDeptGroupResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.dept_id):
+            body['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='OpenInnerGroupTransferToDeptGroup',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/innerGroups/transferToDeptGroups',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def open_inner_group_transfer_to_dept_group_with_options_async(
+        self,
+        request: dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupRequest,
+        headers: dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupResponse:
+        """
+        @summary 内部群转部门群
+        
+        @param request: OpenInnerGroupTransferToDeptGroupRequest
+        @param headers: OpenInnerGroupTransferToDeptGroupHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenInnerGroupTransferToDeptGroupResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.dept_id):
+            body['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='OpenInnerGroupTransferToDeptGroup',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/innerGroups/transferToDeptGroups',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def open_inner_group_transfer_to_dept_group(
+        self,
+        request: dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupRequest,
+    ) -> dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupResponse:
+        """
+        @summary 内部群转部门群
+        
+        @param request: OpenInnerGroupTransferToDeptGroupRequest
+        @return: OpenInnerGroupTransferToDeptGroupResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupHeaders()
+        return self.open_inner_group_transfer_to_dept_group_with_options(request, headers, runtime)
+
+    async def open_inner_group_transfer_to_dept_group_async(
+        self,
+        request: dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupRequest,
+    ) -> dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupResponse:
+        """
+        @summary 内部群转部门群
+        
+        @param request: OpenInnerGroupTransferToDeptGroupRequest
+        @return: OpenInnerGroupTransferToDeptGroupResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.OpenInnerGroupTransferToDeptGroupHeaders()
+        return await self.open_inner_group_transfer_to_dept_group_with_options_async(request, headers, runtime)
+
+    def open_search_group_list_with_options(
+        self,
+        request: dingtalkim__1__0_models.OpenSearchGroupListRequest,
+        headers: dingtalkim__1__0_models.OpenSearchGroupListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.OpenSearchGroupListResponse:
+        """
+        @summary 群搜索
+        
+        @param request: OpenSearchGroupListRequest
+        @param headers: OpenSearchGroupListHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenSearchGroupListResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.keyword):
+            body['keyword'] = request.keyword
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='OpenSearchGroupList',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/groups/search',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.OpenSearchGroupListResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def open_search_group_list_with_options_async(
+        self,
+        request: dingtalkim__1__0_models.OpenSearchGroupListRequest,
+        headers: dingtalkim__1__0_models.OpenSearchGroupListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.OpenSearchGroupListResponse:
+        """
+        @summary 群搜索
+        
+        @param request: OpenSearchGroupListRequest
+        @param headers: OpenSearchGroupListHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenSearchGroupListResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.keyword):
+            body['keyword'] = request.keyword
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='OpenSearchGroupList',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/groups/search',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.OpenSearchGroupListResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def open_search_group_list(
+        self,
+        request: dingtalkim__1__0_models.OpenSearchGroupListRequest,
+    ) -> dingtalkim__1__0_models.OpenSearchGroupListResponse:
+        """
+        @summary 群搜索
+        
+        @param request: OpenSearchGroupListRequest
+        @return: OpenSearchGroupListResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.OpenSearchGroupListHeaders()
+        return self.open_search_group_list_with_options(request, headers, runtime)
+
+    async def open_search_group_list_async(
+        self,
+        request: dingtalkim__1__0_models.OpenSearchGroupListRequest,
+    ) -> dingtalkim__1__0_models.OpenSearchGroupListResponse:
+        """
+        @summary 群搜索
+        
+        @param request: OpenSearchGroupListRequest
+        @return: OpenSearchGroupListResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.OpenSearchGroupListHeaders()
+        return await self.open_search_group_list_with_options_async(request, headers, runtime)
+
+    def open_user_send_card_message_with_options(
+        self,
+        request: dingtalkim__1__0_models.OpenUserSendCardMessageRequest,
+        headers: dingtalkim__1__0_models.OpenUserSendCardMessageHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.OpenUserSendCardMessageResponse:
+        """
+        @summary 以个人身份发送卡片消息
+        
+        @param request: OpenUserSendCardMessageRequest
+        @param headers: OpenUserSendCardMessageHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenUserSendCardMessageResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.card_content):
+            body['cardContent'] = request.card_content
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.receive_user_id):
+            body['receiveUserId'] = request.receive_user_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='OpenUserSendCardMessage',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/cardMessages/users/send',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.OpenUserSendCardMessageResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def open_user_send_card_message_with_options_async(
+        self,
+        request: dingtalkim__1__0_models.OpenUserSendCardMessageRequest,
+        headers: dingtalkim__1__0_models.OpenUserSendCardMessageHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.OpenUserSendCardMessageResponse:
+        """
+        @summary 以个人身份发送卡片消息
+        
+        @param request: OpenUserSendCardMessageRequest
+        @param headers: OpenUserSendCardMessageHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenUserSendCardMessageResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.card_content):
+            body['cardContent'] = request.card_content
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.receive_user_id):
+            body['receiveUserId'] = request.receive_user_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='OpenUserSendCardMessage',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/cardMessages/users/send',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.OpenUserSendCardMessageResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def open_user_send_card_message(
+        self,
+        request: dingtalkim__1__0_models.OpenUserSendCardMessageRequest,
+    ) -> dingtalkim__1__0_models.OpenUserSendCardMessageResponse:
+        """
+        @summary 以个人身份发送卡片消息
+        
+        @param request: OpenUserSendCardMessageRequest
+        @return: OpenUserSendCardMessageResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.OpenUserSendCardMessageHeaders()
+        return self.open_user_send_card_message_with_options(request, headers, runtime)
+
+    async def open_user_send_card_message_async(
+        self,
+        request: dingtalkim__1__0_models.OpenUserSendCardMessageRequest,
+    ) -> dingtalkim__1__0_models.OpenUserSendCardMessageResponse:
+        """
+        @summary 以个人身份发送卡片消息
+        
+        @param request: OpenUserSendCardMessageRequest
+        @return: OpenUserSendCardMessageResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.OpenUserSendCardMessageHeaders()
+        return await self.open_user_send_card_message_with_options_async(request, headers, runtime)
+
     def query_group_info_by_member_auth_with_options(
         self,
         request: dingtalkim__1__0_models.QueryGroupInfoByMemberAuthRequest,
         headers: dingtalkim__1__0_models.QueryGroupInfoByMemberAuthHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkim__1__0_models.QueryGroupInfoByMemberAuthResponse:
         """
@@ -4775,14 +5137,254 @@
         @param request: QueryGroupMuteStatusRequest
         @return: QueryGroupMuteStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkim__1__0_models.QueryGroupMuteStatusHeaders()
         return await self.query_group_mute_status_with_options_async(request, headers, runtime)
 
+    def query_inner_group_member_list_with_options(
+        self,
+        request: dingtalkim__1__0_models.QueryInnerGroupMemberListRequest,
+        headers: dingtalkim__1__0_models.QueryInnerGroupMemberListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.QueryInnerGroupMemberListResponse:
+        """
+        @summary 读取群成员列表
+        
+        @param request: QueryInnerGroupMemberListRequest
+        @param headers: QueryInnerGroupMemberListHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryInnerGroupMemberListResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QueryInnerGroupMemberList',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/innerGroups/memberLists/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.QueryInnerGroupMemberListResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_inner_group_member_list_with_options_async(
+        self,
+        request: dingtalkim__1__0_models.QueryInnerGroupMemberListRequest,
+        headers: dingtalkim__1__0_models.QueryInnerGroupMemberListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.QueryInnerGroupMemberListResponse:
+        """
+        @summary 读取群成员列表
+        
+        @param request: QueryInnerGroupMemberListRequest
+        @param headers: QueryInnerGroupMemberListHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryInnerGroupMemberListResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QueryInnerGroupMemberList',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/innerGroups/memberLists/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.QueryInnerGroupMemberListResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_inner_group_member_list(
+        self,
+        request: dingtalkim__1__0_models.QueryInnerGroupMemberListRequest,
+    ) -> dingtalkim__1__0_models.QueryInnerGroupMemberListResponse:
+        """
+        @summary 读取群成员列表
+        
+        @param request: QueryInnerGroupMemberListRequest
+        @return: QueryInnerGroupMemberListResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.QueryInnerGroupMemberListHeaders()
+        return self.query_inner_group_member_list_with_options(request, headers, runtime)
+
+    async def query_inner_group_member_list_async(
+        self,
+        request: dingtalkim__1__0_models.QueryInnerGroupMemberListRequest,
+    ) -> dingtalkim__1__0_models.QueryInnerGroupMemberListResponse:
+        """
+        @summary 读取群成员列表
+        
+        @param request: QueryInnerGroupMemberListRequest
+        @return: QueryInnerGroupMemberListResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.QueryInnerGroupMemberListHeaders()
+        return await self.query_inner_group_member_list_with_options_async(request, headers, runtime)
+
+    def query_inner_group_recent_list_with_options(
+        self,
+        request: dingtalkim__1__0_models.QueryInnerGroupRecentListRequest,
+        headers: dingtalkim__1__0_models.QueryInnerGroupRecentListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.QueryInnerGroupRecentListResponse:
+        """
+        @summary 查询最近活跃的企业内部群列表
+        
+        @param request: QueryInnerGroupRecentListRequest
+        @param headers: QueryInnerGroupRecentListHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryInnerGroupRecentListResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryInnerGroupRecentList',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/innerGroups/recentLists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.QueryInnerGroupRecentListResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_inner_group_recent_list_with_options_async(
+        self,
+        request: dingtalkim__1__0_models.QueryInnerGroupRecentListRequest,
+        headers: dingtalkim__1__0_models.QueryInnerGroupRecentListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.QueryInnerGroupRecentListResponse:
+        """
+        @summary 查询最近活跃的企业内部群列表
+        
+        @param request: QueryInnerGroupRecentListRequest
+        @param headers: QueryInnerGroupRecentListHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryInnerGroupRecentListResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryInnerGroupRecentList',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/innerGroups/recentLists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.QueryInnerGroupRecentListResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_inner_group_recent_list(
+        self,
+        request: dingtalkim__1__0_models.QueryInnerGroupRecentListRequest,
+    ) -> dingtalkim__1__0_models.QueryInnerGroupRecentListResponse:
+        """
+        @summary 查询最近活跃的企业内部群列表
+        
+        @param request: QueryInnerGroupRecentListRequest
+        @return: QueryInnerGroupRecentListResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.QueryInnerGroupRecentListHeaders()
+        return self.query_inner_group_recent_list_with_options(request, headers, runtime)
+
+    async def query_inner_group_recent_list_async(
+        self,
+        request: dingtalkim__1__0_models.QueryInnerGroupRecentListRequest,
+    ) -> dingtalkim__1__0_models.QueryInnerGroupRecentListResponse:
+        """
+        @summary 查询最近活跃的企业内部群列表
+        
+        @param request: QueryInnerGroupRecentListRequest
+        @return: QueryInnerGroupRecentListResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.QueryInnerGroupRecentListHeaders()
+        return await self.query_inner_group_recent_list_with_options_async(request, headers, runtime)
+
     def query_members_of_group_role_with_options(
         self,
         request: dingtalkim__1__0_models.QueryMembersOfGroupRoleRequest,
         headers: dingtalkim__1__0_models.QueryMembersOfGroupRoleHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkim__1__0_models.QueryMembersOfGroupRoleResponse:
         """
@@ -4897,14 +5499,128 @@
         @param request: QueryMembersOfGroupRoleRequest
         @return: QueryMembersOfGroupRoleResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkim__1__0_models.QueryMembersOfGroupRoleHeaders()
         return await self.query_members_of_group_role_with_options_async(request, headers, runtime)
 
+    def query_recent_conversations_with_options(
+        self,
+        request: dingtalkim__1__0_models.QueryRecentConversationsRequest,
+        headers: dingtalkim__1__0_models.QueryRecentConversationsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.QueryRecentConversationsResponse:
+        """
+        @summary 获取最近联系人及群组
+        
+        @param request: QueryRecentConversationsRequest
+        @param headers: QueryRecentConversationsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryRecentConversationsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryRecentConversations',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/conversations/recentLists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.QueryRecentConversationsResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_recent_conversations_with_options_async(
+        self,
+        request: dingtalkim__1__0_models.QueryRecentConversationsRequest,
+        headers: dingtalkim__1__0_models.QueryRecentConversationsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__1__0_models.QueryRecentConversationsResponse:
+        """
+        @summary 获取最近联系人及群组
+        
+        @param request: QueryRecentConversationsRequest
+        @param headers: QueryRecentConversationsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryRecentConversationsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryRecentConversations',
+            version='im_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/im/conversations/recentLists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__1__0_models.QueryRecentConversationsResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_recent_conversations(
+        self,
+        request: dingtalkim__1__0_models.QueryRecentConversationsRequest,
+    ) -> dingtalkim__1__0_models.QueryRecentConversationsResponse:
+        """
+        @summary 获取最近联系人及群组
+        
+        @param request: QueryRecentConversationsRequest
+        @return: QueryRecentConversationsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.QueryRecentConversationsHeaders()
+        return self.query_recent_conversations_with_options(request, headers, runtime)
+
+    async def query_recent_conversations_async(
+        self,
+        request: dingtalkim__1__0_models.QueryRecentConversationsRequest,
+    ) -> dingtalkim__1__0_models.QueryRecentConversationsResponse:
+        """
+        @summary 获取最近联系人及群组
+        
+        @param request: QueryRecentConversationsRequest
+        @return: QueryRecentConversationsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__1__0_models.QueryRecentConversationsHeaders()
+        return await self.query_recent_conversations_with_options_async(request, headers, runtime)
+
     def query_scene_group_template_robot_with_options(
         self,
         request: dingtalkim__1__0_models.QuerySceneGroupTemplateRobotRequest,
         headers: dingtalkim__1__0_models.QuerySceneGroupTemplateRobotHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkim__1__0_models.QuerySceneGroupTemplateRobotResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6157,14 +6157,599 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListOrgTextEmotionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class OpenInnerGroupTransferToDeptGroupHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class OpenInnerGroupTransferToDeptGroupRequest(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+        open_conversation_id: str = None,
+    ):
+        # This parameter is required.
+        self.dept_id = dept_id
+        # This parameter is required.
+        self.open_conversation_id = open_conversation_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        return self
+
+
+class OpenInnerGroupTransferToDeptGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class OpenInnerGroupTransferToDeptGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: OpenInnerGroupTransferToDeptGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = OpenInnerGroupTransferToDeptGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class OpenSearchGroupListHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class OpenSearchGroupListRequest(TeaModel):
+    def __init__(
+        self,
+        keyword: str = None,
+        user_id: str = None,
+    ):
+        self.keyword = keyword
+        # This parameter is required.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.keyword is not None:
+            result['keyword'] = self.keyword
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('keyword') is not None:
+            self.keyword = m.get('keyword')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class OpenSearchGroupListResponseBodyResultGroupList(TeaModel):
+    def __init__(
+        self,
+        icon: str = None,
+        member_count: int = None,
+        open_conversation_id: str = None,
+        tag: str = None,
+        title: str = None,
+    ):
+        self.icon = icon
+        self.member_count = member_count
+        self.open_conversation_id = open_conversation_id
+        self.tag = tag
+        self.title = title
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.icon is not None:
+            result['icon'] = self.icon
+        if self.member_count is not None:
+            result['memberCount'] = self.member_count
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.tag is not None:
+            result['tag'] = self.tag
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('icon') is not None:
+            self.icon = m.get('icon')
+        if m.get('memberCount') is not None:
+            self.member_count = m.get('memberCount')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('tag') is not None:
+            self.tag = m.get('tag')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class OpenSearchGroupListResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        group_list: List[OpenSearchGroupListResponseBodyResultGroupList] = None,
+    ):
+        self.group_list = group_list
+
+    def validate(self):
+        if self.group_list:
+            for k in self.group_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['groupList'] = []
+        if self.group_list is not None:
+            for k in self.group_list:
+                result['groupList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.group_list = []
+        if m.get('groupList') is not None:
+            for k in m.get('groupList'):
+                temp_model = OpenSearchGroupListResponseBodyResultGroupList()
+                self.group_list.append(temp_model.from_map(k))
+        return self
+
+
+class OpenSearchGroupListResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: OpenSearchGroupListResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = OpenSearchGroupListResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class OpenSearchGroupListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: OpenSearchGroupListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = OpenSearchGroupListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class OpenUserSendCardMessageHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class OpenUserSendCardMessageRequestCardContent(TeaModel):
+    def __init__(
+        self,
+        last_message: str = None,
+        out_track_id: str = None,
+    ):
+        # This parameter is required.
+        self.last_message = last_message
+        # This parameter is required.
+        self.out_track_id = out_track_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.last_message is not None:
+            result['lastMessage'] = self.last_message
+        if self.out_track_id is not None:
+            result['outTrackId'] = self.out_track_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('lastMessage') is not None:
+            self.last_message = m.get('lastMessage')
+        if m.get('outTrackId') is not None:
+            self.out_track_id = m.get('outTrackId')
+        return self
+
+
+class OpenUserSendCardMessageRequest(TeaModel):
+    def __init__(
+        self,
+        card_content: OpenUserSendCardMessageRequestCardContent = None,
+        open_conversation_id: str = None,
+        receive_user_id: str = None,
+        user_id: str = None,
+    ):
+        # This parameter is required.
+        self.card_content = card_content
+        self.open_conversation_id = open_conversation_id
+        self.receive_user_id = receive_user_id
+        # This parameter is required.
+        self.user_id = user_id
+
+    def validate(self):
+        if self.card_content:
+            self.card_content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.card_content is not None:
+            result['cardContent'] = self.card_content.to_map()
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.receive_user_id is not None:
+            result['receiveUserId'] = self.receive_user_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('cardContent') is not None:
+            temp_model = OpenUserSendCardMessageRequestCardContent()
+            self.card_content = temp_model.from_map(m['cardContent'])
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('receiveUserId') is not None:
+            self.receive_user_id = m.get('receiveUserId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class OpenUserSendCardMessageResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        open_task_id: str = None,
+    ):
+        self.open_task_id = open_task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.open_task_id is not None:
+            result['openTaskId'] = self.open_task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('openTaskId') is not None:
+            self.open_task_id = m.get('openTaskId')
+        return self
+
+
+class OpenUserSendCardMessageResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: OpenUserSendCardMessageResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = OpenUserSendCardMessageResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class OpenUserSendCardMessageResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: OpenUserSendCardMessageResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = OpenUserSendCardMessageResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryGroupInfoByMemberAuthHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -6868,14 +7453,423 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryGroupMuteStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryInnerGroupMemberListHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryInnerGroupMemberListRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: int = None,
+        open_conversation_id: str = None,
+        user_id: str = None,
+    ):
+        # This parameter is required.
+        self.max_results = max_results
+        # This parameter is required.
+        self.next_token = next_token
+        # This parameter is required.
+        self.open_conversation_id = open_conversation_id
+        # This parameter is required.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class QueryInnerGroupMemberListResponseBodyList(TeaModel):
+    def __init__(
+        self,
+        icon: str = None,
+        name: str = None,
+        nick_name: str = None,
+        user_id: str = None,
+    ):
+        self.icon = icon
+        self.name = name
+        self.nick_name = nick_name
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.icon is not None:
+            result['icon'] = self.icon
+        if self.name is not None:
+            result['name'] = self.name
+        if self.nick_name is not None:
+            result['nickName'] = self.nick_name
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('icon') is not None:
+            self.icon = m.get('icon')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('nickName') is not None:
+            self.nick_name = m.get('nickName')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class QueryInnerGroupMemberListResponseBody(TeaModel):
+    def __init__(
+        self,
+        has_more: bool = None,
+        list: List[QueryInnerGroupMemberListResponseBodyList] = None,
+        next_token: int = None,
+        success: bool = None,
+    ):
+        self.has_more = has_more
+        self.list = list
+        self.next_token = next_token
+        self.success = success
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = QueryInnerGroupMemberListResponseBodyList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class QueryInnerGroupMemberListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryInnerGroupMemberListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryInnerGroupMemberListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class QueryInnerGroupRecentListHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryInnerGroupRecentListRequest(TeaModel):
+    def __init__(
+        self,
+        user_id: str = None,
+    ):
+        # This parameter is required.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class QueryInnerGroupRecentListResponseBodyGroupInfos(TeaModel):
+    def __init__(
+        self,
+        icon: str = None,
+        member_amount: str = None,
+        open_conversation_id: str = None,
+        title: str = None,
+    ):
+        self.icon = icon
+        self.member_amount = member_amount
+        self.open_conversation_id = open_conversation_id
+        self.title = title
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.icon is not None:
+            result['icon'] = self.icon
+        if self.member_amount is not None:
+            result['memberAmount'] = self.member_amount
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('icon') is not None:
+            self.icon = m.get('icon')
+        if m.get('memberAmount') is not None:
+            self.member_amount = m.get('memberAmount')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class QueryInnerGroupRecentListResponseBody(TeaModel):
+    def __init__(
+        self,
+        group_infos: List[QueryInnerGroupRecentListResponseBodyGroupInfos] = None,
+        success: bool = None,
+    ):
+        self.group_infos = group_infos
+        self.success = success
+
+    def validate(self):
+        if self.group_infos:
+            for k in self.group_infos:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['groupInfos'] = []
+        if self.group_infos is not None:
+            for k in self.group_infos:
+                result['groupInfos'].append(k.to_map() if k else None)
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.group_infos = []
+        if m.get('groupInfos') is not None:
+            for k in m.get('groupInfos'):
+                temp_model = QueryInnerGroupRecentListResponseBodyGroupInfos()
+                self.group_infos.append(temp_model.from_map(k))
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class QueryInnerGroupRecentListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryInnerGroupRecentListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryInnerGroupRecentListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryMembersOfGroupRoleHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -7010,14 +8004,263 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryMembersOfGroupRoleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryRecentConversationsHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryRecentConversationsRequest(TeaModel):
+    def __init__(
+        self,
+        user_id: str = None,
+    ):
+        # This parameter is required.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class QueryRecentConversationsResponseBodyResultConversationList(TeaModel):
+    def __init__(
+        self,
+        conversation_type: int = None,
+        icon: str = None,
+        member_count: str = None,
+        name: str = None,
+        nick_name: str = None,
+        open_conversation_id: str = None,
+        title: str = None,
+        user_id: str = None,
+    ):
+        # This parameter is required.
+        self.conversation_type = conversation_type
+        # This parameter is required.
+        self.icon = icon
+        # This parameter is required.
+        self.member_count = member_count
+        # This parameter is required.
+        self.name = name
+        # This parameter is required.
+        self.nick_name = nick_name
+        # This parameter is required.
+        self.open_conversation_id = open_conversation_id
+        # This parameter is required.
+        self.title = title
+        # This parameter is required.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.conversation_type is not None:
+            result['conversationType'] = self.conversation_type
+        if self.icon is not None:
+            result['icon'] = self.icon
+        if self.member_count is not None:
+            result['memberCount'] = self.member_count
+        if self.name is not None:
+            result['name'] = self.name
+        if self.nick_name is not None:
+            result['nickName'] = self.nick_name
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.title is not None:
+            result['title'] = self.title
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('conversationType') is not None:
+            self.conversation_type = m.get('conversationType')
+        if m.get('icon') is not None:
+            self.icon = m.get('icon')
+        if m.get('memberCount') is not None:
+            self.member_count = m.get('memberCount')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('nickName') is not None:
+            self.nick_name = m.get('nickName')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class QueryRecentConversationsResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        conversation_list: List[QueryRecentConversationsResponseBodyResultConversationList] = None,
+    ):
+        self.conversation_list = conversation_list
+
+    def validate(self):
+        if self.conversation_list:
+            for k in self.conversation_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['conversationList'] = []
+        if self.conversation_list is not None:
+            for k in self.conversation_list:
+                result['conversationList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.conversation_list = []
+        if m.get('conversationList') is not None:
+            for k in m.get('conversationList'):
+                temp_model = QueryRecentConversationsResponseBodyResultConversationList()
+                self.conversation_list.append(temp_model.from_map(k))
+        return self
+
+
+class QueryRecentConversationsResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: QueryRecentConversationsResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = QueryRecentConversationsResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class QueryRecentConversationsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryRecentConversationsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryRecentConversationsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QuerySceneGroupTemplateRobotHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -847,42 +847,40 @@
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkrooms__1__0_models.DeleteMeetingRoomHeaders()
         return await self.delete_meeting_room_with_options_async(room_id, request, headers, runtime)
 
     def delete_meeting_room_control_panel_with_options(
         self,
-        tmp_req: dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelRequest,
+        request: dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelRequest,
         headers: dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelResponse:
         """
         @summary 删除会议室配置
         
-        @param tmp_req: DeleteMeetingRoomControlPanelRequest
+        @param request: DeleteMeetingRoomControlPanelRequest
         @param headers: DeleteMeetingRoomControlPanelHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteMeetingRoomControlPanelResponse
         """
-        UtilClient.validate_model(tmp_req)
-        request = dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.body):
-            request.body_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.body, 'body', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.body_shrink):
-            query['body'] = request.body_shrink
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.room_ids):
+            body['roomIds'] = request.room_ids
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteMeetingRoomControlPanel',
             version='rooms_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/rooms/panels/remove',
             method='POST',
@@ -894,42 +892,40 @@
         return TeaCore.from_map(
             dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelResponse(),
             self.execute(params, req, runtime)
         )
 
     async def delete_meeting_room_control_panel_with_options_async(
         self,
-        tmp_req: dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelRequest,
+        request: dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelRequest,
         headers: dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelResponse:
         """
         @summary 删除会议室配置
         
-        @param tmp_req: DeleteMeetingRoomControlPanelRequest
+        @param request: DeleteMeetingRoomControlPanelRequest
         @param headers: DeleteMeetingRoomControlPanelHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteMeetingRoomControlPanelResponse
         """
-        UtilClient.validate_model(tmp_req)
-        request = dingtalkrooms__1__0_models.DeleteMeetingRoomControlPanelShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.body):
-            request.body_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.body, 'body', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.body_shrink):
-            query['body'] = request.body_shrink
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.room_ids):
+            body['roomIds'] = request.room_ids
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteMeetingRoomControlPanel',
             version='rooms_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/rooms/panels/remove',
             method='POST',
```

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1224,15 +1224,15 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class DeleteMeetingRoomControlPanelRequestBody(TeaModel):
+class DeleteMeetingRoomControlPanelRequest(TeaModel):
     def __init__(
         self,
         room_ids: List[str] = None,
         union_id: str = None,
     ):
         # This parameter is required.
         self.room_ids = room_ids
@@ -1259,70 +1259,14 @@
         if m.get('roomIds') is not None:
             self.room_ids = m.get('roomIds')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
         return self
 
 
-class DeleteMeetingRoomControlPanelRequest(TeaModel):
-    def __init__(
-        self,
-        body: DeleteMeetingRoomControlPanelRequestBody = None,
-    ):
-        self.body = body
-
-    def validate(self):
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('body') is not None:
-            temp_model = DeleteMeetingRoomControlPanelRequestBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class DeleteMeetingRoomControlPanelShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        body_shrink: str = None,
-    ):
-        self.body_shrink = body_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.body_shrink is not None:
-            result['body'] = self.body_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('body') is not None:
-            self.body_shrink = m.get('body')
-        return self
-
-
 class DeleteMeetingRoomControlPanelResponseBody(TeaModel):
     def __init__(
         self,
         result: str = None,
     ):
         self.result = result
```

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.1.12
+Version: 2.1.13
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.12/setup.py` & `alibabacloud_dingtalk-2.1.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 18/05/2024
+Created on 22/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

