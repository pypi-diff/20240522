# Comparing `tmp/linktest-2.8.3.tar.gz` & `tmp/linktest-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.8.3.tar", last modified: Fri May 17 06:34:38 2024, max compression
+gzip compressed data, was "linktest-2.8.4.tar", last modified: Wed May 22 08:26:48 2024, max compression
```

## Comparing `linktest-2.8.3.tar` & `linktest-2.8.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-17 06:34:38.444645 linktest-2.8.3/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-17 06:34:38.444367 linktest-2.8.3/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-17 06:34:38.442035 linktest-2.8.3/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-17 06:28:08.000000 linktest-2.8.3/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/auto_generate_testcase_list-backup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    28841 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10326 2024-05-17 06:28:03.000000 linktest-2.8.3/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38554 2024-05-17 06:31:46.000000 linktest-2.8.3/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8899 2024-05-17 06:30:10.000000 linktest-2.8.3/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102436 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4811 2024-05-17 06:31:14.000000 linktest-2.8.3/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-17 06:28:14.000000 linktest-2.8.3/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-17 06:34:38.444009 linktest-2.8.3/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1498 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-17 06:34:38.444695 linktest-2.8.3/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-17 06:34:33.000000 linktest-2.8.3/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-22 08:26:48.355761 linktest-2.8.4/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-22 08:26:48.355485 linktest-2.8.4/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-22 08:26:48.351803 linktest-2.8.4/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-22 08:23:18.000000 linktest-2.8.4/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/auto_generate_testcase_list-backup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    28841 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10326 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38554 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8899 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102436 2024-05-22 08:21:55.000000 linktest-2.8.4/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4811 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-22 08:23:23.000000 linktest-2.8.4/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-22 08:26:48.355097 linktest-2.8.4/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1498 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-22 08:26:48.355814 linktest-2.8.4/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-22 08:26:42.000000 linktest-2.8.4/setup.py
```

### Comparing `linktest-2.8.3/linktest/appium_utils.py` & `linktest-2.8.4/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/auto_generate_testcase_list-backup.py` & `linktest-2.8.4/linktest/auto_generate_testcase_list-backup.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/auto_generate_testcase_list.py` & `linktest-2.8.4/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.8.4/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/base_testcase.py` & `linktest-2.8.4/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/clean_data.py` & `linktest-2.8.4/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/conver_xml_into_db.py` & `linktest-2.8.4/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/database_helper.py` & `linktest-2.8.4/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/date_utilities.py` & `linktest-2.8.4/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/doctor.py` & `linktest-2.8.4/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/framework_log.py` & `linktest-2.8.4/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/generate_html_log.py` & `linktest-2.8.4/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/get_adb_devices.py` & `linktest-2.8.4/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/get_ios_devices_list.py` & `linktest-2.8.4/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/get_platform_info.py` & `linktest-2.8.4/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/get_project_info.py` & `linktest-2.8.4/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/html_report.py` & `linktest-2.8.4/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/logged_requests.py` & `linktest-2.8.4/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/main.py` & `linktest-2.8.4/linktest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1475,15 +1475,15 @@
     for item in args:
         if item.find("=") != -1:
             item, value = item.split('=')[0].upper().lstrip().rstrip(), item.split('=')[1]
             print(item, "=", value)
             if item == '' or value == '':
                 continue
 
-            if item == 'ENV' or item == 'ENVIORNMENT':
+            if item == 'ENV' or item == 'ENVIRONMENT':
                 if value.lower() == 'dev':
                     update_config_str += 'ENVIRONMENT = Environment.DEV &'
                 if value.lower() == 'qa':
                     update_config_str += 'ENVIRONMENT = Environment.QA & '
                 if value.lower() == 'uat':
                     update_config_str += 'ENVIRONMENT = Environment.UAT & '
                 if value.lower() == 'sit':
```

### Comparing `linktest-2.8.3/linktest/memory_usage.py` & `linktest-2.8.4/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/re_func.py` & `linktest-2.8.4/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/run.py` & `linktest-2.8.4/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/run_testcase_thread.py` & `linktest-2.8.4/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/scp_report_to_specified_path.py` & `linktest-2.8.4/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/selenium_helper.py` & `linktest-2.8.4/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/timeout_thread.py` & `linktest-2.8.4/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/ui_testcase.py` & `linktest-2.8.4/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/update_config.py` & `linktest-2.8.4/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/webdriver_wrapper.py` & `linktest-2.8.4/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/webdriver_wrapper_chrome.py` & `linktest-2.8.4/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/webdriver_wrapper_edge.py` & `linktest-2.8.4/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/webdriver_wrapper_firefox.py` & `linktest-2.8.4/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/webdriver_wrapper_ie.py` & `linktest-2.8.4/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/webdriver_wrapper_safari.py` & `linktest-2.8.4/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest/xml_report.py` & `linktest-2.8.4/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.3/linktest.egg-info/SOURCES.txt` & `linktest-2.8.4/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

