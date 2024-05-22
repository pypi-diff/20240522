# Comparing `tmp/yao-0.1.4.tar.gz` & `tmp/yao-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yao-0.1.4.tar", last modified: Thu Oct  5 08:41:06 2023, max compression
+gzip compressed data, was "yao-0.1.5.tar", last modified: Wed May 22 13:46:18 2024, max compression
```

## Comparing `yao-0.1.4.tar` & `yao-0.1.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.431404 yao-0.1.4/
--rw-r--r--   0 ke         (501) wheel        (0)      844 2023-10-05 08:41:06.431143 yao-0.1.4/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)       38 2023-10-05 08:41:06.431454 yao-0.1.4/setup.cfg
--rw-r--r--   0 ke         (501) wheel        (0)     1021 2023-10-05 08:38:18.000000 yao-0.1.4/setup.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.422903 yao-0.1.4/yao/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)    22069 2023-09-13 01:10:14.000000 yao-0.1.4/yao/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     2235 2023-08-21 01:15:12.000000 yao-0.1.4/yao/db.py
--rw-r--r--   0 ke         (501) wheel        (0)     9293 2023-09-21 09:33:31.000000 yao-0.1.4/yao/depends.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.424096 yao-0.1.4/yao/function/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/__init__.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.424830 yao-0.1.4/yao/function/annex/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/annex/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      187 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/annex/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11252 2023-09-21 09:29:53.000000 yao-0.1.4/yao/function/annex/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1669 2023-08-26 01:31:22.000000 yao-0.1.4/yao/function/annex/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.425411 yao-0.1.4/yao/function/appointment/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/appointment/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/appointment/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/appointment/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1506 2023-08-30 08:53:19.000000 yao-0.1.4/yao/function/appointment/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.426034 yao-0.1.4/yao/function/company/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/company/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      192 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/company/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/company/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/company/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.426745 yao-0.1.4/yao/function/department/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/department/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      189 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/department/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/department/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1250 2023-08-26 01:30:38.000000 yao-0.1.4/yao/function/department/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.427317 yao-0.1.4/yao/function/log/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/log/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      169 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/log/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/log/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/log/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)      746 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     9412 2023-08-31 07:41:39.000000 yao-0.1.4/yao/function/model.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.428024 yao-0.1.4/yao/function/permission/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/permission/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      199 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/permission/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     8272 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/permission/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     2305 2023-08-26 01:30:06.000000 yao-0.1.4/yao/function/permission/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.429049 yao-0.1.4/yao/function/queue/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/queue/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      159 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/queue/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     6333 2023-09-15 11:26:42.000000 yao-0.1.4/yao/function/queue/helper.py
--rw-r--r--   0 ke         (501) wheel        (0)     4161 2023-10-05 08:22:34.000000 yao-0.1.4/yao/function/queue/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     2037 2023-10-05 08:22:00.000000 yao-0.1.4/yao/function/queue/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)      547 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/queue/type.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.430050 yao-0.1.4/yao/function/user/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/user/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     2275 2023-08-21 01:15:12.000000 yao-0.1.4/yao/function/user/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    16522 2023-09-21 09:43:22.000000 yao-0.1.4/yao/function/user/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     4163 2023-08-31 07:54:17.000000 yao-0.1.4/yao/function/user/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-08-29 09:37:50.000000 yao-0.1.4/yao/helpers.py
--rw-r--r--   0 ke         (501) wheel        (0)    13890 2023-09-05 10:13:54.000000 yao-0.1.4/yao/method.py
--rw-r--r--   0 ke         (501) wheel        (0)     2818 2023-09-21 09:25:38.000000 yao-0.1.4/yao/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.430301 yao-0.1.4/yao/wxamp/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.4/yao/wxamp/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)    11593 2023-09-15 11:26:25.000000 yao-0.1.4/yao/wxamp/base.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.430666 yao-0.1.4/yao/wxmp/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-09-05 09:17:16.000000 yao-0.1.4/yao/wxmp/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     7119 2023-09-15 11:26:16.000000 yao-0.1.4/yao/wxmp/base.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-10-05 08:41:06.423651 yao-0.1.4/yao.egg-info/
--rw-r--r--   0 ke         (501) wheel        (0)      844 2023-10-05 08:41:06.000000 yao-0.1.4/yao.egg-info/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)     1412 2023-10-05 08:41:06.000000 yao-0.1.4/yao.egg-info/SOURCES.txt
--rw-r--r--   0 ke         (501) wheel        (0)        1 2023-10-05 08:41:06.000000 yao-0.1.4/yao.egg-info/dependency_links.txt
--rw-r--r--   0 ke         (501) wheel        (0)      209 2023-10-05 08:41:06.000000 yao-0.1.4/yao.egg-info/requires.txt
--rw-r--r--   0 ke         (501) wheel        (0)        4 2023-10-05 08:41:06.000000 yao-0.1.4/yao.egg-info/top_level.txt
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.457650 yao-0.1.5/
+-rw-r--r--   0 ke         (501) wheel        (0)      872 2024-05-22 13:46:18.457374 yao-0.1.5/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)       38 2024-05-22 13:46:18.457693 yao-0.1.5/setup.cfg
+-rw-r--r--   0 ke         (501) wheel        (0)     1045 2024-05-22 13:44:30.000000 yao-0.1.5/setup.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.447767 yao-0.1.5/yao/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)    22069 2023-09-13 01:10:14.000000 yao-0.1.5/yao/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2235 2023-08-21 01:15:12.000000 yao-0.1.5/yao/db.py
+-rw-r--r--   0 ke         (501) wheel        (0)     9293 2023-09-21 09:33:31.000000 yao-0.1.5/yao/depends.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.449383 yao-0.1.5/yao/function/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/__init__.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.450305 yao-0.1.5/yao/function/annex/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/annex/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      187 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/annex/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11257 2023-10-12 01:56:14.000000 yao-0.1.5/yao/function/annex/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1669 2023-08-26 01:31:22.000000 yao-0.1.5/yao/function/annex/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.451034 yao-0.1.5/yao/function/appointment/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/appointment/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/appointment/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/appointment/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1506 2023-08-30 08:53:19.000000 yao-0.1.5/yao/function/appointment/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.451630 yao-0.1.5/yao/function/company/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/company/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      192 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/company/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/company/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/company/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.452354 yao-0.1.5/yao/function/department/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/department/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      189 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/department/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/department/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1250 2023-08-26 01:30:38.000000 yao-0.1.5/yao/function/department/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.453034 yao-0.1.5/yao/function/log/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/log/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      169 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/log/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/log/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/log/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      746 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     9616 2023-10-31 06:01:56.000000 yao-0.1.5/yao/function/model.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.453757 yao-0.1.5/yao/function/permission/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/permission/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      199 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/permission/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8272 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/permission/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2305 2023-08-26 01:30:06.000000 yao-0.1.5/yao/function/permission/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.454903 yao-0.1.5/yao/function/queue/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/queue/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      159 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/queue/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     6333 2023-09-15 11:26:42.000000 yao-0.1.5/yao/function/queue/helper.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4161 2023-10-05 08:22:34.000000 yao-0.1.5/yao/function/queue/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2037 2023-10-05 08:22:00.000000 yao-0.1.5/yao/function/queue/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      547 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/queue/type.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.455941 yao-0.1.5/yao/function/user/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/user/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2275 2023-08-21 01:15:12.000000 yao-0.1.5/yao/function/user/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    17229 2023-10-17 08:39:05.000000 yao-0.1.5/yao/function/user/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4251 2023-10-17 07:55:35.000000 yao-0.1.5/yao/function/user/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-08-29 09:37:50.000000 yao-0.1.5/yao/helpers.py
+-rw-r--r--   0 ke         (501) wheel        (0)    14409 2023-10-26 02:49:43.000000 yao-0.1.5/yao/method.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2818 2023-09-21 09:25:38.000000 yao-0.1.5/yao/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.456283 yao-0.1.5/yao/wxamp/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-08-21 01:15:12.000000 yao-0.1.5/yao/wxamp/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11593 2023-09-15 11:26:25.000000 yao-0.1.5/yao/wxamp/base.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.456761 yao-0.1.5/yao/wxmp/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-09-05 09:17:16.000000 yao-0.1.5/yao/wxmp/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     7826 2023-10-13 10:00:25.000000 yao-0.1.5/yao/wxmp/base.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2024-05-22 13:46:18.457004 yao-0.1.5/yao.egg-info/
+-rw-r--r--   0 ke         (501) wheel        (0)      872 2024-05-22 13:46:18.000000 yao-0.1.5/yao.egg-info/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)     1412 2024-05-22 13:46:18.000000 yao-0.1.5/yao.egg-info/SOURCES.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        1 2024-05-22 13:46:18.000000 yao-0.1.5/yao.egg-info/dependency_links.txt
+-rw-r--r--   0 ke         (501) wheel        (0)      222 2024-05-22 13:46:18.000000 yao-0.1.5/yao.egg-info/requires.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        4 2024-05-22 13:46:18.000000 yao-0.1.5/yao.egg-info/top_level.txt
```

### Comparing `yao-0.1.4/PKG-INFO` & `yao-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: yao
-Version: 0.1.4
+Version: 0.1.5
 Summary: Production
 Home-page: https://github.com/lsshu/yao
 Author: Lsshu
 Author-email: admin@lsshu.cn
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi[all]==0.83.0
 Requires-Dist: python-jose[cryptography]==3.3.0
-Requires-Dist: passlib[bcrypt]
+Requires-Dist: passlib==1.7.4
+Requires-Dist: bcrypt==4.0.1
 Requires-Dist: SQLAlchemy==1.4.46
 Requires-Dist: Pillow
 Requires-Dist: PyMySQL==1.0.2
 Requires-Dist: sqlalchemy-mptt==0.2.5
 Requires-Dist: user-agents==2.2.0
 Requires-Dist: requests
 Requires-Dist: openpyxl
```

### Comparing `yao-0.1.4/setup.py` & `yao-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yao",
-    version="0.1.4",
+    version="0.1.5",
     description="Production",
     python_requires=">=3.8",
     author="Lsshu",
     author_email="admin@lsshu.cn",
     url="https://github.com/lsshu/yao",
     packages=find_packages(),
     long_description=long_description,
@@ -19,15 +19,16 @@
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
         "Development Status :: 3 - Alpha",
     ],
     install_requires=[
         "fastapi[all]==0.83.0",
         "python-jose[cryptography]==3.3.0",
-        "passlib[bcrypt]",
+        "passlib==1.7.4",
+        "bcrypt==4.0.1",
         "SQLAlchemy==1.4.46",
         "Pillow",
         "PyMySQL==1.0.2",
         "sqlalchemy-mptt==0.2.5",
         "user-agents==2.2.0",
         "requests",
         "openpyxl",
```

### Comparing `yao-0.1.4/yao/crud.py` & `yao-0.1.5/yao/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/db.py` & `yao-0.1.5/yao/db.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/depends.py` & `yao-0.1.5/yao/depends.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/annex/main.py` & `yao-0.1.5/yao/function/annex/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 img = Image.open(path)
                 width, height = img.size
             except:
                 width, height = (0, 0)
             CrudFunctionAnnexe.init().store(session=session,
                                             item=SchemasFunctionAnnexeStoreUpdate(
                                                 prefix=auth.prefix,
-                                                filename=file.filename,
+                                                filename=file.filename[:50],
                                                 content_type=file.content_type,
                                                 md5=md5, path=path, size=size, width=width, height=height))
             db_model = CrudFunctionAnnexe.init().first(session=session, where=("md5", md5))
     return Schemas(data=SchemasFunctionAnnexeResponse(**db_model.to_dict()))
 
 
 @route('/_M_.ueditor', module=name, router=router, methods=['get'])
```

### Comparing `yao-0.1.4/yao/function/annex/schema.py` & `yao-0.1.5/yao/function/annex/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/appointment/crud.py` & `yao-0.1.5/yao/function/appointment/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/appointment/main.py` & `yao-0.1.5/yao/function/appointment/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/appointment/schema.py` & `yao-0.1.5/yao/function/appointment/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/company/main.py` & `yao-0.1.5/yao/function/company/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/company/schema.py` & `yao-0.1.5/yao/function/company/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/department/main.py` & `yao-0.1.5/yao/function/department/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/department/schema.py` & `yao-0.1.5/yao/function/department/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/log/main.py` & `yao-0.1.5/yao/function/log/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/log/schema.py` & `yao-0.1.5/yao/function/log/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/main.py` & `yao-0.1.5/yao/function/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/model.py` & `yao-0.1.5/yao/function/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+import os
 from sqlalchemy import Column, String, Boolean, Text, Integer, ForeignKey, event, Table, JSON, TIMESTAMP
 from sqlalchemy.orm import relationship, declared_attr
 from sqlalchemy_mptt.mixins import BaseNestedSets
 
 from yao.method import plural
 from yao.db import Model, Engine
 
+try:
+    from config import STATIC_URL
+except:
+    STATIC_URL = "/"
+
 name = __name__[:__name__.rfind(".")].capitalize()
 
 """职能信息"""
 function_name = plural("%s" % name)
 
 """公司信息"""
 function_company_name = plural("%s.company" % name)
@@ -95,16 +101,16 @@
 
 class ModelFunctionPermissions(BaseModel, BaseNestedSets):
     """ 权限 """
     __tablename__ = function_permission_table_name
     sqlalchemy_mptt_pk_name = "uuid"
     name = Column(String(15), unique=True, nullable=False, comment="名称")
     icon = Column(String(20), nullable=True, comment="ICO")
-    scope = Column(String(50), nullable=False, unique=True, comment="Scope")
-    path = Column(String(50), nullable=False, comment="Path")
+    scope = Column(String(80), nullable=False, unique=True, comment="Scope")
+    path = Column(String(80), nullable=False, comment="Path")
     is_menu = Column(Boolean, default=True, comment="是否为菜单")
     is_action = Column(Boolean, default=True, comment="是否为动作权限")
 
 
 @event.listens_for(ModelFunctionPermissions.scope, 'set')
 def permission_receive_before_insert(target, value: str, old_value, initiator):
     target.path = "/%s" % value.replace('.', '/').lower()
@@ -150,14 +156,22 @@
     appointments = relationship(ModelFunctionAppointments, backref='function_users', secondary=Table(
         "%s_user_has_appointments" % function_name.replace('.', '_'),
         Model.metadata,
         Column('app_id', Integer, ForeignKey("%s.id" % function_appointment_table_name, ondelete="CASCADE"), primary_key=True, comment="职位"),
         Column('use_id', Integer, ForeignKey("%s.id" % function_user_table_name, ondelete="CASCADE"), primary_key=True, comment="用户"),
     ))
 
+    @property
+    def auth_mp_code_path(self):
+        """
+        真实路径
+        :return:
+        """
+        return os.path.join(STATIC_URL, "api/auth/mp/code", self.uuid)
+
 
 class ModelFunctionAnnexes(BaseCompanyModel):
     """ 附件 """
     __tablename__ = function_annex_table_name
 
     filename = Column(String(50), nullable=False, comment="文件名")
     content_type = Column(String(100), nullable=False, comment="类型")
@@ -165,16 +179,14 @@
     md5 = Column(String(32), nullable=True, comment="md5", index=True)
     size = Column(Integer, nullable=False, comment="SIZE")
     width = Column(String(100), nullable=True, comment="宽")
     height = Column(String(190), nullable=True, comment="高")
 
     @property
     def preview_path(self):
-        import os
-        from config import STATIC_URL
         return os.path.join(STATIC_URL, self.path)
 
 
 class ModelFunctionLogs(BaseCompanyModel):
     """ 日志 """
     __tablename__ = function_log_table_name
     scope = Column(String(100), nullable=True, comment="scope")
```

### Comparing `yao-0.1.4/yao/function/permission/main.py` & `yao-0.1.5/yao/function/permission/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/permission/schema.py` & `yao-0.1.5/yao/function/permission/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/queue/helper.py` & `yao-0.1.5/yao/function/queue/helper.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/queue/main.py` & `yao-0.1.5/yao/function/queue/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/queue/schema.py` & `yao-0.1.5/yao/function/queue/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/queue/type.py` & `yao-0.1.5/yao/function/queue/type.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/user/crud.py` & `yao-0.1.5/yao/function/user/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/function/user/main.py` & `yao-0.1.5/yao/function/user/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+import os
+from urllib.parse import urljoin
 from typing import List, Optional
 
 from fastapi import APIRouter, Depends, Security, HTTPException, status
+from fastapi.responses import FileResponse
+
 from fastapi.responses import HTMLResponse
 from fastapi.security import OAuth2PasswordRequestForm
 from sqlalchemy.orm import Session
 
+from yao.method import get_qrcode
+
 try:
     from config import OAUTH_ADMIN_USERS, DEFAULT_FUNCTION_COMPANY
 except:
     # 默认公司
     DEFAULT_FUNCTION_COMPANY = {
         "name": "默认",
         "prefix_name": "site",
@@ -310,15 +316,15 @@
             CrudFunctionUser.init().update(session=session, uuid=item.scene, item=_item, exclude_unset=True, event=True, close=True)
             return Schemas(data="已经成功获取到授权，可以关闭当前窗口！")
     except:
         return SchemasError(data="授权出错！")
 
 
 @router.get('/auth/mp/{user_uuid}', name="get {}".format(name))
-async def mp_auth(user_uuid: str, session: Session = Depends(_session)):
+async def mp_auth(user_uuid: str):
     """
     :param user_uuid
     :param session
     :return:
     """
     try:
         from config import HOME_URL
@@ -389,7 +395,28 @@
             </head>
             <body>
             <h1 style="text-align: center;margin:100px auto;width:100%;color:red">授权出错！</h1>
             </body>
             </html>
             """
     return HTMLResponse(content=content, status_code=200)
+
+
+@router.get('/auth/mp/code/{user_uuid}', name="get {}".format(name))
+async def mp_auth_code(user_uuid: str):
+    try:
+        from config import HOME_URL
+    except:
+        HOME_URL = "/"
+    try:
+        from config import ROOT_PATH
+    except:
+        ROOT_PATH = "/temp/"
+    try:
+        from config import UPLOAD_DIR
+    except:
+        UPLOAD_DIR = "static"
+    path = os.path.join(ROOT_PATH, UPLOAD_DIR, "runtime", ".user.auth.mp.code.png")
+    is_success = get_qrcode(data=urljoin(HOME_URL, "/api/auth/mp/%s" % user_uuid), path=path)
+    if is_success:
+        return FileResponse(path)
+    return SchemasError()
```

### Comparing `yao-0.1.4/yao/function/user/schema.py` & `yao-0.1.5/yao/function/user/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     prefix: Optional[str] = None
     username: Optional[str] = None
     user_phone: Optional[str] = None
     permissions: Optional[List[SchemasFunctionResponse]] = None
     appointments: Optional[List[SchemasFunctionMiniAppointmentResponse]] = None
     children: Optional[List['SchemasFunctionUserResponse']] = None
     children_ids: Optional[list] = None
+    auth_mp_code_path: Optional[str] = None
     available: Optional[bool] = True
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
 
     remarks: Optional[str] = None  # 备注
     sort: Optional[int] = None  # 排序
     status: Optional[bool] = None  # 状态
@@ -34,14 +35,15 @@
 class SchemasFunctionUserMiniResponse(BaseModel):
     """授权用户 返回"""
     uuid: Optional[str] = None
     prefix: Optional[str] = None
     username: Optional[str] = None
     user_phone: Optional[str] = None
     available: Optional[bool] = True
+    auth_mp_code_path: Optional[str] = None
 
     remarks: Optional[str] = None  # 备注
     sort: Optional[int] = None  # 排序
     status: Optional[bool] = None  # 状态
 
     class Config:
         orm_mode = True
```

### Comparing `yao-0.1.4/yao/helpers.py` & `yao-0.1.5/yao/helpers.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/method.py` & `yao-0.1.5/yao/method.py`

 * *Files 2% similar despite different names*

```diff
@@ -526,7 +526,25 @@
     qr.add_data(data)
     # 填充数据并生成二维码
     qr.make(fit=True)
     img = qr.make_image(fill_color=img_fill_color, back_color=img_back_color)
     # 保存二维码图片
     img.save(path)
     return True
+
+
+def clean_icode(text, restr=''):
+    """
+    过滤表情
+    Args:
+        text:
+        restr:
+
+    Returns:
+
+    """
+    try:
+        # co = re.compile(u'['u'\U0001F300-\U0001F64F' u'\U0001F680-\U0001F6FF' u'\u2600-\u2B55]+')
+        co = re.compile(u'['u'\U0001F300-\U0001F64F' u'\U0001F680-\U0001F6FF' u'\u2600-\u2B55' u'\U00010000-\U0010ffff]+')
+    except re.error:
+        co = re.compile(u'('u'\ud83c[\udf00-\udfff]|'u'\ud83d[\udc00-\ude4f\ude80-\udeff]|'u'[\u2600-\u2B55])+')
+    return co.sub(restr, text)
```

### Comparing `yao-0.1.4/yao/schema.py` & `yao-0.1.5/yao/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/wxamp/base.py` & `yao-0.1.5/yao/wxamp/base.py`

 * *Files identical despite different names*

### Comparing `yao-0.1.4/yao/wxmp/base.py` & `yao-0.1.5/yao/wxmp/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -192,20 +192,41 @@
         else:
             bytes_content = self.__get_file_content(path, mode=read_mode)
             return json.loads(bytes_content)
 
 #
 # if __name__ == '__main__':
 #     from config import MPAPPID, MPAPPSECRET
+#     from app.stats.mp_template_config import user_copy_glance_template_id
 #
 #     mp = MP(app_id=MPAPPID, app_secret=MPAPPSECRET)
-#     print(mp.message(openid="o9vB96AmVEZCLO09jPaplvvRDlok", template_id="8BNzzuBzXd_ttcr2KHAbDEuJLyQ5IVKXYR1YiRLJ2Sk", data={
-#         "thing2": {
-#             "value": "公司高抛"
-#         },
-#         "thing3": {
-#             "value": "软件园43号楼"
-#         },
-#         "time5": {
-#             "value": "2022年12月27日 13:48:43"
-#         },
-#     }))
+#     # print(mp.message(openid="o9vB96AmVEZCLO09jPaplvvRDlok", template_id="8BNzzuBzXd_ttcr2KHAbDEuJLyQ5IVKXYR1YiRLJ2Sk", data={
+#     #     "thing2": {
+#     #         "value": "公司高抛"
+#     #     },
+#     #     "thing3": {
+#     #         "value": "软件园43号楼"
+#     #     },
+#     #     "time5": {
+#     #         "value": "2022年12月27日 13:48:43"
+#     #     },
+#     # }))
+#     # print(mp.message(openid="o9vB96AmVEZCLO09jPaplvvRDlok", template_id=user_copy_glance_template_id, data={
+#     #     "thing1": {
+#     #         "value": "复制"
+#     #     },
+#     #     "thing3": {
+#     #         "value": "林银瑶"
+#     #     },
+#     #     "phone_number2": {
+#     #         "value": "13800138000"
+#     #     },
+#     #     "time7": {
+#     #         "value": "2022年12月27日 13:48:43"
+#     #     },
+#     #     "thing3": {
+#     #         "value": "预约服务"
+#     #     },
+#     #     "thing4": {
+#     #         "value": "预约来源"
+#     #     },
+#     # }))
```

### Comparing `yao-0.1.4/yao.egg-info/PKG-INFO` & `yao-0.1.5/yao.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: yao
-Version: 0.1.4
+Version: 0.1.5
 Summary: Production
 Home-page: https://github.com/lsshu/yao
 Author: Lsshu
 Author-email: admin@lsshu.cn
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi[all]==0.83.0
 Requires-Dist: python-jose[cryptography]==3.3.0
-Requires-Dist: passlib[bcrypt]
+Requires-Dist: passlib==1.7.4
+Requires-Dist: bcrypt==4.0.1
 Requires-Dist: SQLAlchemy==1.4.46
 Requires-Dist: Pillow
 Requires-Dist: PyMySQL==1.0.2
 Requires-Dist: sqlalchemy-mptt==0.2.5
 Requires-Dist: user-agents==2.2.0
 Requires-Dist: requests
 Requires-Dist: openpyxl
```

### Comparing `yao-0.1.4/yao.egg-info/SOURCES.txt` & `yao-0.1.5/yao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

