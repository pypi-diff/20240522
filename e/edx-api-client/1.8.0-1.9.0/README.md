# Comparing `tmp/edx-api-client-1.8.0.tar.gz` & `tmp/edx-api-client-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/edx-api-client-1.8.0.tar", last modified: Wed Aug 16 14:21:05 2023, max compression
+gzip compressed data, was "dist/edx-api-client-1.9.0.tar", last modified: Wed May 22 07:04:16 2024, max compression
```

## Comparing `edx-api-client-1.8.0.tar` & `edx-api-client-1.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.047924 edx-api-client-1.8.0/
--rw-------   0 u15935   (15935) dyno     (15935)       38 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/DESCRIPTION
--rw-------   0 u15935   (15935) dyno     (15935)    34520 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/LICENSE
--rw-------   0 u15935   (15935) dyno     (15935)      281 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/MANIFEST.in
--rw-------   0 u15935   (15935) dyno     (15935)      346 2023-08-16 14:21:05.047924 edx-api-client-1.8.0/PKG-INFO
--rw-------   0 u15935   (15935) dyno     (15935)     1417 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/README.md
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/
--rw-------   0 u15935   (15935) dyno     (15935)      104 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/__init__.py
--rw-------   0 u15935   (15935) dyno     (15935)      814 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/bulk_user_retirement.py
--rw-------   0 u15935   (15935) dyno     (15935)     1574 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/ccx.py
--rw-------   0 u15935   (15935) dyno     (15935)      657 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/ccx_test.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/certificates/
--rw-------   0 u15935   (15935) dyno     (15935)     2480 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/certificates/__init__.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/certificates/fixtures/
--rw-------   0 u15935   (15935) dyno     (15935)      668 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/certificates/fixtures/certificates.json
--rw-------   0 u15935   (15935) dyno     (15935)     3560 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/certificates/models.py
--rw-------   0 u15935   (15935) dyno     (15935)     5033 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/certificates/models_test.py
--rw-------   0 u15935   (15935) dyno     (15935)     3354 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/client.py
--rw-------   0 u15935   (15935) dyno     (15935)      613 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/client_test.py
--rw-------   0 u15935   (15935) dyno     (15935)      102 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/constants.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/course_detail/
--rw-------   0 u15935   (15935) dyno     (15935)     2350 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/course_detail/__init__.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/course_detail/fixtures/
--rw-------   0 u15935   (15935) dyno     (15935)      965 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/course_detail/fixtures/course_detail.json
--rw-------   0 u15935   (15935) dyno     (15935)      316 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/course_detail/fixtures/course_mode.json
--rw-------   0 u15935   (15935) dyno     (15935)     5630 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/course_detail/models.py
--rw-------   0 u15935   (15935) dyno     (15935)     5259 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/course_detail/models_test.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/course_structure/
--rw-------   0 u15935   (15935) dyno     (15935)     1045 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/course_structure/__init__.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/course_structure/fixtures/
--rw-------   0 u15935   (15935) dyno     (15935)    99969 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/course_structure/fixtures/course_structure.json
--rw-------   0 u15935   (15935) dyno     (15935)     1793 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/course_structure/models.py
--rw-------   0 u15935   (15935) dyno     (15935)     2012 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/course_structure/models_test.py
--rw-------   0 u15935   (15935) dyno     (15935)     1554 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/email_settings.py
--rw-------   0 u15935   (15935) dyno     (15935)     1369 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/email_settings_test.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/enrollments/
--rw-------   0 u15935   (15935) dyno     (15935)     8179 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/enrollments/__init__.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/enrollments/fixtures/
--rw-------   0 u15935   (15935) dyno     (15935)      793 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/enrollments/fixtures/enrollments_list.json
--rw-------   0 u15935   (15935) dyno     (15935)     1760 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/enrollments/fixtures/user_enrollments.json
--rw-------   0 u15935   (15935) dyno     (15935)     6481 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/enrollments/init_test.py
--rw-------   0 u15935   (15935) dyno     (15935)     7323 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/enrollments/models.py
--rw-------   0 u15935   (15935) dyno     (15935)     7667 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/enrollments/models_test.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/fixtures/
--rw-------   0 u15935   (15935) dyno     (15935)      471 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/fixtures/ccx_create_response.json
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/grades/
--rw-------   0 u15935   (15935) dyno     (15935)     3794 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/grades/__init__.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.043924 edx-api-client-1.8.0/edx_api/grades/fixtures/
--rw-------   0 u15935   (15935) dyno     (15935)      350 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/grades/fixtures/course_grades_hawthorn.json
--rw-------   0 u15935   (15935) dyno     (15935)      460 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/grades/fixtures/course_grades_ironwood_p1.json
--rw-------   0 u15935   (15935) dyno     (15935)      462 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/grades/fixtures/course_grades_ironwood_p2.json
--rw-------   0 u15935   (15935) dyno     (15935)      342 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/grades/fixtures/current_grades.json
--rw-------   0 u15935   (15935) dyno     (15935)     3536 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/grades/init_test.py
--rw-------   0 u15935   (15935) dyno     (15935)     4184 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/grades/models.py
--rw-------   0 u15935   (15935) dyno     (15935)     5563 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/grades/models_test.py
--rw-------   0 u15935   (15935) dyno     (15935)    16088 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/integration_test.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.047924 edx-api-client-1.8.0/edx_api/user_info/
--rw-------   0 u15935   (15935) dyno     (15935)     1984 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/user_info/__init__.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.047924 edx-api-client-1.8.0/edx_api/user_info/fixtures/
--rw-------   0 u15935   (15935) dyno     (15935)      186 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/user_info/fixtures/user_info.json
--rw-------   0 u15935   (15935) dyno     (15935)      715 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/user_info/models.py
--rw-------   0 u15935   (15935) dyno     (15935)     1165 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/edx_api/user_info/models_test.py
-drwx------   0 u15935   (15935) dyno     (15935)        0 2023-08-16 14:21:05.047924 edx-api-client-1.8.0/edx_api_client.egg-info/
--rw-------   0 u15935   (15935) dyno     (15935)      346 2023-08-16 14:21:04.000000 edx-api-client-1.8.0/edx_api_client.egg-info/PKG-INFO
--rw-------   0 u15935   (15935) dyno     (15935)     1748 2023-08-16 14:21:05.000000 edx-api-client-1.8.0/edx_api_client.egg-info/SOURCES.txt
--rw-------   0 u15935   (15935) dyno     (15935)        1 2023-08-16 14:21:04.000000 edx-api-client-1.8.0/edx_api_client.egg-info/dependency_links.txt
--rw-------   0 u15935   (15935) dyno     (15935)       61 2023-08-16 14:21:04.000000 edx-api-client-1.8.0/edx_api_client.egg-info/requires.txt
--rw-------   0 u15935   (15935) dyno     (15935)        8 2023-08-16 14:21:04.000000 edx-api-client-1.8.0/edx_api_client.egg-info/top_level.txt
--rw-------   0 u15935   (15935) dyno     (15935)       47 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/requirements.txt
--rw-------   0 u15935   (15935) dyno     (15935)      163 2023-08-16 14:21:05.047924 edx-api-client-1.8.0/setup.cfg
--rw-------   0 u15935   (15935) dyno     (15935)     1009 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/setup.py
--rw-------   0 u15935   (15935) dyno     (15935)      224 2023-08-16 14:20:55.000000 edx-api-client-1.8.0/tox.ini
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.144921 edx-api-client-1.9.0/
+-rw-------   0 u33214   (33214) dyno     (33214)       38 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/DESCRIPTION
+-rw-------   0 u33214   (33214) dyno     (33214)    34520 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/LICENSE
+-rw-------   0 u33214   (33214) dyno     (33214)      281 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/MANIFEST.in
+-rw-r--r--   0 u33214   (33214) dyno     (33214)      461 2024-05-22 07:04:16.144921 edx-api-client-1.9.0/PKG-INFO
+-rw-------   0 u33214   (33214) dyno     (33214)     1342 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/README.md
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.136921 edx-api-client-1.9.0/edx_api/
+-rw-------   0 u33214   (33214) dyno     (33214)      104 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/__init__.py
+-rw-------   0 u33214   (33214) dyno     (33214)      814 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/bulk_user_retirement.py
+-rw-------   0 u33214   (33214) dyno     (33214)     1574 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/ccx.py
+-rw-------   0 u33214   (33214) dyno     (33214)      657 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/ccx_test.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.136921 edx-api-client-1.9.0/edx_api/certificates/
+-rw-------   0 u33214   (33214) dyno     (33214)     2480 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/certificates/__init__.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.136921 edx-api-client-1.9.0/edx_api/certificates/fixtures/
+-rw-------   0 u33214   (33214) dyno     (33214)      668 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/certificates/fixtures/certificates.json
+-rw-------   0 u33214   (33214) dyno     (33214)     3560 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/certificates/models.py
+-rw-------   0 u33214   (33214) dyno     (33214)     5033 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/certificates/models_test.py
+-rw-------   0 u33214   (33214) dyno     (33214)     3287 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/client.py
+-rw-------   0 u33214   (33214) dyno     (33214)      499 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/client_test.py
+-rw-------   0 u33214   (33214) dyno     (33214)      102 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/constants.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.136921 edx-api-client-1.9.0/edx_api/course_detail/
+-rw-------   0 u33214   (33214) dyno     (33214)     2350 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/course_detail/__init__.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.136921 edx-api-client-1.9.0/edx_api/course_detail/fixtures/
+-rw-------   0 u33214   (33214) dyno     (33214)      965 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/course_detail/fixtures/course_detail.json
+-rw-------   0 u33214   (33214) dyno     (33214)      316 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/course_detail/fixtures/course_mode.json
+-rw-------   0 u33214   (33214) dyno     (33214)     5630 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/course_detail/models.py
+-rw-------   0 u33214   (33214) dyno     (33214)     5259 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/course_detail/models_test.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.136921 edx-api-client-1.9.0/edx_api/course_structure/
+-rw-------   0 u33214   (33214) dyno     (33214)     1045 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/course_structure/__init__.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.136921 edx-api-client-1.9.0/edx_api/course_structure/fixtures/
+-rw-------   0 u33214   (33214) dyno     (33214)    99969 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/course_structure/fixtures/course_structure.json
+-rw-------   0 u33214   (33214) dyno     (33214)     1793 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/course_structure/models.py
+-rw-------   0 u33214   (33214) dyno     (33214)     2012 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/course_structure/models_test.py
+-rw-------   0 u33214   (33214) dyno     (33214)     1554 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/email_settings.py
+-rw-------   0 u33214   (33214) dyno     (33214)     1369 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/email_settings_test.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.140921 edx-api-client-1.9.0/edx_api/enrollments/
+-rw-------   0 u33214   (33214) dyno     (33214)     8192 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/enrollments/__init__.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.140921 edx-api-client-1.9.0/edx_api/enrollments/fixtures/
+-rw-------   0 u33214   (33214) dyno     (33214)      793 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/enrollments/fixtures/enrollments_list.json
+-rw-------   0 u33214   (33214) dyno     (33214)     1760 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/enrollments/fixtures/user_enrollments.json
+-rw-------   0 u33214   (33214) dyno     (33214)     6570 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/enrollments/init_test.py
+-rw-------   0 u33214   (33214) dyno     (33214)     7323 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/enrollments/models.py
+-rw-------   0 u33214   (33214) dyno     (33214)     7667 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/enrollments/models_test.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.140921 edx-api-client-1.9.0/edx_api/fixtures/
+-rw-------   0 u33214   (33214) dyno     (33214)      471 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/fixtures/ccx_create_response.json
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.140921 edx-api-client-1.9.0/edx_api/grades/
+-rw-------   0 u33214   (33214) dyno     (33214)     3794 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/grades/__init__.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.140921 edx-api-client-1.9.0/edx_api/grades/fixtures/
+-rw-------   0 u33214   (33214) dyno     (33214)      350 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/grades/fixtures/course_grades_hawthorn.json
+-rw-------   0 u33214   (33214) dyno     (33214)      460 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/grades/fixtures/course_grades_ironwood_p1.json
+-rw-------   0 u33214   (33214) dyno     (33214)      462 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/grades/fixtures/course_grades_ironwood_p2.json
+-rw-------   0 u33214   (33214) dyno     (33214)      342 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/grades/fixtures/current_grades.json
+-rw-------   0 u33214   (33214) dyno     (33214)     3536 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/grades/init_test.py
+-rw-------   0 u33214   (33214) dyno     (33214)     4184 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/grades/models.py
+-rw-------   0 u33214   (33214) dyno     (33214)     5563 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/grades/models_test.py
+-rw-------   0 u33214   (33214) dyno     (33214)    15937 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/integration_test.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.140921 edx-api-client-1.9.0/edx_api/user_info/
+-rw-------   0 u33214   (33214) dyno     (33214)     1984 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/user_info/__init__.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.140921 edx-api-client-1.9.0/edx_api/user_info/fixtures/
+-rw-------   0 u33214   (33214) dyno     (33214)      186 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/user_info/fixtures/user_info.json
+-rw-------   0 u33214   (33214) dyno     (33214)      715 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/user_info/models.py
+-rw-------   0 u33214   (33214) dyno     (33214)     1165 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/edx_api/user_info/models_test.py
+drwx------   0 u33214   (33214) dyno     (33214)        0 2024-05-22 07:04:16.144921 edx-api-client-1.9.0/edx_api_client.egg-info/
+-rw-r--r--   0 u33214   (33214) dyno     (33214)      461 2024-05-22 07:04:16.000000 edx-api-client-1.9.0/edx_api_client.egg-info/PKG-INFO
+-rw-------   0 u33214   (33214) dyno     (33214)     1748 2024-05-22 07:04:16.000000 edx-api-client-1.9.0/edx_api_client.egg-info/SOURCES.txt
+-rw-------   0 u33214   (33214) dyno     (33214)        1 2024-05-22 07:04:16.000000 edx-api-client-1.9.0/edx_api_client.egg-info/dependency_links.txt
+-rw-------   0 u33214   (33214) dyno     (33214)       61 2024-05-22 07:04:16.000000 edx-api-client-1.9.0/edx_api_client.egg-info/requires.txt
+-rw-------   0 u33214   (33214) dyno     (33214)        8 2024-05-22 07:04:16.000000 edx-api-client-1.9.0/edx_api_client.egg-info/top_level.txt
+-rw-------   0 u33214   (33214) dyno     (33214)       47 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/requirements.txt
+-rw-------   0 u33214   (33214) dyno     (33214)      163 2024-05-22 07:04:16.144921 edx-api-client-1.9.0/setup.cfg
+-rw-------   0 u33214   (33214) dyno     (33214)     1009 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/setup.py
+-rw-------   0 u33214   (33214) dyno     (33214)      224 2024-05-22 07:04:04.000000 edx-api-client-1.9.0/tox.ini
```

### Comparing `edx-api-client-1.8.0/LICENSE` & `edx-api-client-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/README.md` & `edx-api-client-1.9.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -30,14 +30,13 @@
 variable `OAUTHLIB_INSECURE_TRANSPORT=1`. This will skip the HTTPS
 validation which is required by the OAuth spec.
 
 Your edx demo course (course id `course-v1:edX+DemoX+Demo_Course`)
 must be enabled for CCX.
 
 The Course Enrollment integration tests have the following requirements:
-- The `API_KEY` value must match the `settings.EDX_API_TOKEN` value in LMS
 - The user assigned to that `ACCESS_TOKEN` must be an admin in the edX demo course.
   Adding a user as an admin can be done in Studio (url: `<studio_url>/course_team/course-v1:edX+DemoX+Demo_Course`
 
 ## Release Notes
 
 See the RELEASE.rst file
```

### Comparing `edx-api-client-1.8.0/edx_api/bulk_user_retirement.py` & `edx-api-client-1.9.0/edx_api/bulk_user_retirement.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/ccx.py` & `edx-api-client-1.9.0/edx_api/ccx.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/ccx_test.py` & `edx-api-client-1.9.0/edx_api/ccx_test.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/certificates/__init__.py` & `edx-api-client-1.9.0/edx_api/certificates/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/certificates/fixtures/certificates.json` & `edx-api-client-1.9.0/edx_api/certificates/fixtures/certificates.json`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/certificates/models.py` & `edx-api-client-1.9.0/edx_api/certificates/models.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/certificates/models_test.py` & `edx-api-client-1.9.0/edx_api/certificates/models_test.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/client.py` & `edx-api-client-1.9.0/edx_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         # TODO(abrahms): Perhaps pull this out into a factory function for
         # generating an EdxApi instance with the proper requester & credentials.
         session = requests.session()
         session.headers.update(
             {
                 "Authorization": "{} {}".format(
                     token_type, self.credentials["access_token"]
-                ),
-                "X-EdX-Api-Key": self.credentials.get("api_key"),
+                )
             }
         )
 
         old_request = session.request
 
         def patched_request(*args, **kwargs):
             """
```

### Comparing `edx-api-client-1.8.0/edx_api/course_detail/__init__.py` & `edx-api-client-1.9.0/edx_api/course_detail/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/course_detail/fixtures/course_detail.json` & `edx-api-client-1.9.0/edx_api/course_detail/fixtures/course_detail.json`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/course_detail/models.py` & `edx-api-client-1.9.0/edx_api/course_detail/models.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/course_detail/models_test.py` & `edx-api-client-1.9.0/edx_api/course_detail/models_test.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/course_structure/__init__.py` & `edx-api-client-1.9.0/edx_api/course_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/course_structure/fixtures/course_structure.json` & `edx-api-client-1.9.0/edx_api/course_structure/fixtures/course_structure.json`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/course_structure/models.py` & `edx-api-client-1.9.0/edx_api/course_structure/models.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/course_structure/models_test.py` & `edx-api-client-1.9.0/edx_api/course_structure/models_test.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/email_settings.py` & `edx-api-client-1.9.0/edx_api/email_settings.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/email_settings_test.py` & `edx-api-client-1.9.0/edx_api/email_settings_test.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/enrollments/__init__.py` & `edx-api-client-1.9.0/edx_api/enrollments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,28 +197,31 @@
         # So this function should only be called on behalf of a Staff user
         return self.create_student_enrollment(
             course_id,
             mode=ENROLLMENT_MODE_VERIFIED,
             username=username
         )
 
-    def deactivate_enrollment(self, course_id):
+    def deactivate_enrollment(self, course_id, username=None):
         """
         Deactivates an enrollment in the given course for the user
-        whose access token was provided to the API client (in other words, the
-        user will be unenrolled)
 
         Args:
             course_id (str): An edX course id.
+            username (str): Username.
 
         Returns:
             Enrollment: object representing the deactivated student enrollment
         """
+
+        params = {
+            "course_details": {"course_id": course_id},
+            "is_active": False,
+        }
+        if username:
+            params['user'] = username
         resp = self.requester.post(
             urljoin(self.base_url, self.enrollment_url),
-            json={
-                "course_details": {"course_id": course_id},
-                "is_active": False,
-            }
+            json=params
         )
         resp.raise_for_status()
         return Enrollment(resp.json())
```

### Comparing `edx-api-client-1.8.0/edx_api/enrollments/fixtures/enrollments_list.json` & `edx-api-client-1.9.0/edx_api/enrollments/fixtures/enrollments_list.json`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/enrollments/fixtures/user_enrollments.json` & `edx-api-client-1.9.0/edx_api/enrollments/fixtures/user_enrollments.json`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/enrollments/init_test.py` & `edx-api-client-1.9.0/edx_api/enrollments/init_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,18 +168,22 @@
     def test_deactivate_enrollment(self, request_mock):
         """
         Test that deactivate_enrollment calls the enrollment endpoint with the correct request
         body and returns the deactivated enrollment
         """
         request_mock.post(self.enrollment_url, json=self.enrollments_json[0])
         course_id = 'course_id'
-        returned_enrollment = self.enrollment_client.deactivate_enrollment(course_id=course_id)
+        user = 'user'
+        returned_enrollment = self.enrollment_client.deactivate_enrollment(
+            course_id=course_id, username=user
+        )
         self.assertDictEqual(
             request_mock.last_request.json(),
             {
                 'course_details': {
                     'course_id': course_id
                 },
-                'is_active': False
+                'is_active': False,
+                'user': user
             }
         )
         assert returned_enrollment.json == self.enrollments_json[0]
```

### Comparing `edx-api-client-1.8.0/edx_api/enrollments/models.py` & `edx-api-client-1.9.0/edx_api/enrollments/models.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/enrollments/models_test.py` & `edx-api-client-1.9.0/edx_api/enrollments/models_test.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/grades/__init__.py` & `edx-api-client-1.9.0/edx_api/grades/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/grades/init_test.py` & `edx-api-client-1.9.0/edx_api/grades/init_test.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/grades/models.py` & `edx-api-client-1.9.0/edx_api/grades/models.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/grades/models_test.py` & `edx-api-client-1.9.0/edx_api/grades/models_test.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/integration_test.py` & `edx-api-client-1.9.0/edx_api/integration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 from urllib.parse import urljoin
 
 from edx_api.constants import ENROLLMENT_MODE_AUDIT, ENROLLMENT_MODE_VERIFIED
 from edx_api.client import EdxApi
 
 
 ACCESS_TOKEN = os.getenv('ACCESS_TOKEN')
-API_KEY = os.getenv('API_KEY')
 BASE_URL = os.getenv('BASE_URL', 'http://localhost:18000/')
 ENROLLMENT_CREATION_COURSE_ID = os.getenv('ENROLLMENT_CREATION_COURSE_ID')
 
 # pylint: disable=invalid-name
 require_integration_settings = pytest.mark.skipif(
     not ACCESS_TOKEN or not BASE_URL,
     reason="You must specify the credential env vars"
@@ -107,15 +106,15 @@
 
 @require_integration_settings
 def test_course_structure():
     """
     Pull down the course structure and validate it has the correct entries.
     This test assumes that the used user can access the course.
     """
-    api = EdxApi({'access_token': ACCESS_TOKEN, 'api_key': API_KEY}, base_url=BASE_URL)
+    api = EdxApi({'access_token': ACCESS_TOKEN}, base_url=BASE_URL)
     structure = api.course_structure.course_blocks('course-v1:edX+DemoX+Demo_Course', 'staff')
 
     titles = [
         block.title for block in structure.root.children
         if block.visible
     ]
 
@@ -131,15 +130,15 @@
 
 @require_integration_settings
 def test_enrollments():
     """
     Enrolls the user in a course and then pulls down the enrollments for the user.
     This assumes that the course in the edX instance is available for enrollment.
     """
-    api = EdxApi({'access_token': ACCESS_TOKEN, 'api_key': API_KEY}, base_url=BASE_URL)
+    api = EdxApi({'access_token': ACCESS_TOKEN}, base_url=BASE_URL)
 
     # the enrollment will be done manually until
     # a client to enroll the student is implemented
     requester = api.get_requester()
     requester.post(
         urljoin(BASE_URL, '/api/enrollment/v1/enrollment'),
         json={"course_details": {"course_id": 'course-v1:edX+DemoX+Demo_Course'}}
@@ -156,45 +155,45 @@
 
 
 @require_integration_settings_course_id
 def test_create_verified_enrollment():
     """
     Integration test to enroll the user in a course with `verified` mode
     """
-    api = EdxApi({'access_token': ACCESS_TOKEN, 'api_key': API_KEY}, base_url=BASE_URL)
+    api = EdxApi({'access_token': ACCESS_TOKEN}, base_url=BASE_URL)
     enrollment = api.enrollments.create_student_enrollment(
         course_id=ENROLLMENT_CREATION_COURSE_ID,
         mode=ENROLLMENT_MODE_VERIFIED,
         username="staff"
     )
     assert enrollment.course_id == ENROLLMENT_CREATION_COURSE_ID
     assert enrollment.mode == ENROLLMENT_MODE_VERIFIED
 
 
 @require_integration_settings_course_id
 def test_create_audit_enrollment():
     """
     Integration test to enroll the user in a course with `audit` mode
     """
-    api = EdxApi({'access_token': ACCESS_TOKEN, 'api_key': API_KEY}, base_url=BASE_URL)
+    api = EdxApi({'access_token': ACCESS_TOKEN}, base_url=BASE_URL)
     enrollment = api.enrollments.create_student_enrollment(
         course_id=ENROLLMENT_CREATION_COURSE_ID,
         mode=ENROLLMENT_MODE_AUDIT,
         username="staff"
     )
     assert enrollment.course_id == ENROLLMENT_CREATION_COURSE_ID
     assert enrollment.mode == ENROLLMENT_MODE_AUDIT
 
 
 @require_integration_settings_course_id
 def test_deactivate_enrollment():
     """
     Integration test to enroll then deactivate a user in a course
     """
-    api = EdxApi({'access_token': ACCESS_TOKEN, 'api_key': API_KEY}, base_url=BASE_URL)
+    api = EdxApi({'access_token': ACCESS_TOKEN}, base_url=BASE_URL)
     api.enrollments.create_student_enrollment(
         course_id=ENROLLMENT_CREATION_COURSE_ID,
         mode=ENROLLMENT_MODE_AUDIT
     )
     deactivated_enrollment = api.enrollments.deactivate_enrollment(
         course_id=ENROLLMENT_CREATION_COURSE_ID
     )
@@ -203,15 +202,15 @@
 
 
 @require_integration_settings_course_id
 def test_create_enrollment_timeout():
     """
      Asserts request timeout error on enrollment api
     """
-    api = EdxApi({'access_token': ACCESS_TOKEN, 'api_key': API_KEY}, base_url=BASE_URL)
+    api = EdxApi({'access_token': ACCESS_TOKEN}, base_url=BASE_URL)
     enrollments = api.enrollments
     with patch.object(enrollments.requester, 'post', autospec=True) as post:
         post.side_effect = mocked_timeout
         with pytest.raises(Timeout):
             enrollments.create_student_enrollment(ENROLLMENT_CREATION_COURSE_ID)
```

### Comparing `edx-api-client-1.8.0/edx_api/user_info/__init__.py` & `edx-api-client-1.9.0/edx_api/user_info/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/user_info/models.py` & `edx-api-client-1.9.0/edx_api/user_info/models.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api/user_info/models_test.py` & `edx-api-client-1.9.0/edx_api/user_info/models_test.py`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/edx_api_client.egg-info/SOURCES.txt` & `edx-api-client-1.9.0/edx_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-api-client-1.8.0/setup.py` & `edx-api-client-1.9.0/setup.py`

 * *Files identical despite different names*

