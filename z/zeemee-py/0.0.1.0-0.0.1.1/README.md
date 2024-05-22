# Comparing `tmp/zeemee_py-0.0.1.0.tar.gz` & `tmp/zeemee_py-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeemee_py-0.0.1.0.tar", last modified: Wed May 22 21:30:19 2024, max compression
+gzip compressed data, was "zeemee_py-0.0.1.1.tar", last modified: Wed May 22 21:30:50 2024, max compression
```

## Comparing `zeemee_py-0.0.1.0.tar` & `zeemee_py-0.0.1.1.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:19.035930 zeemee_py-0.0.1.0/
--rw-r--r--   0 mayur     (1002) mayur     (1002)       42 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/LICENSE
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3916 2024-05-22 21:30:19.035930 zeemee_py-0.0.1.0/PKG-INFO
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3214 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/README.md
--rw-r--r--   0 mayur     (1002) mayur     (1002)      787 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/pyproject.toml
--rw-r--r--   0 mayur     (1002) mayur     (1002)       38 2024-05-22 21:30:19.035930 zeemee_py-0.0.1.0/setup.cfg
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.939930 zeemee_py-0.0.1.0/src/
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.943930 zeemee_py-0.0.1.0/src/zeemee_py/
--rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/__init__.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.939930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.939930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.943930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4984 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_ap1_by_gender_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3810 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_ap1_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     9585 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_common_ap1_calculate_values.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1994 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2397 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1914 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2322 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6894 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     7224 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6834 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6910 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_for_old_cohort.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.943930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1345 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/function_ap1_perform_athena_update.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2607 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/function_ap1_recreate_full_table.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.939930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.947930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5494 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_ap2_by_gender_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3812 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_ap2_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2573 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    16874 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_campus_visit.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    16280 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_first_gen.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    17682 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_not_campus_visit.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    17076 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_not_first_gen.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1994 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2396 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1914 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2321 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6997 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     7224 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6910 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6900 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_for_old_cohort.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.947930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1345 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/function_ap2_perform_athena_update.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2607 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/function_ap2_recreate_full_table.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.939930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.947930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5494 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_ap3_by_gender_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3812 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_ap3_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2989 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6481 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_app_rate.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     7589 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_commitment_rate.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5580 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_melt_rate.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4276 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_missing_dates.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     9104 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_yield_rate.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1994 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2395 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1903 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2320 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6997 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     7224 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6910 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6900 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_for_old_cohort.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.947930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1345 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/function_ap3_perform_athena_update.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2607 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/function_ap3_recreate_full_table.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.947930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/athena_code/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     8157 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/athena_code/create_or_update_athena_tables_for_gold_schema.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.947930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/general_athena_table_update/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5764 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/general_athena_table_update/data_team_creation_and_updation.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1059 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/general_athena_table_update/get_column_details.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.951930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2631 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/create_zeemee_tp_college_combined_files.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3422 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_rawDataCurrent_details.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2886 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_rawDataCurrent_details_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2904 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_touchpoint_file_details.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3348 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_college_combined_files_details.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2556 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_college_combined_files_details_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      904 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_tp_and_college_file_details_in_one_table.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1293 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/query_athena_with_retry.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      760 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/query_athena_without_retry.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1741 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/send_slack_notifications.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.939930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.979930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2178 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3964 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_comm_match.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4591 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_non_dupe_ntr.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3762 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_organic.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4861 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_op1_by_gender_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3685 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_op1_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2003 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2501 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1912 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2416 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6796 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     7115 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6907 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     7080 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_for_old_cohort.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.979930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1321 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/function_op1_perform_athena_update.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2585 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/function_op1_recreate_full_table.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.939930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.983930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3717 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5488 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_accepted_community_entered_counts.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5391 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_applied_community_entered_counts.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5584 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_committed_community_entered_counts.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5487 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_enrolled_community_entered_counts.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5487 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_inquired_community_entered_counts.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4864 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_op2_by_gender_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3685 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_op2_create_one_school_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2004 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2501 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1913 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2416 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6797 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_by_gender_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     7115 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_by_gender_for_old_cohort.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6908 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_for_config_schools.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     7080 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_for_old_cohort.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.983930 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1321 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/function_op2_perform_athena_update.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2585 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/function_op2_recreate_full_table.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.983930 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/
--rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/__init__.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1304 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/connect_athena.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1125 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/connect_duckdb.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      620 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/connect_redshift.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      726 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_config.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      617 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_data_folder_path.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3153 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_latest_postwrangler_files.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3129 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_latest_touchpoints_files.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      571 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_org_additional_data_file.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      542 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_org_tracker.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1121 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_dataframe_to_s3.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      823 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_email.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1115 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_to_admin_and_make_visible.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      811 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_to_s3.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1022 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_to_slack.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.983930 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/
--rw-r--r--   0 mayur     (1002) mayur     (1002)      206 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/__init__.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.987930 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5391 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_calculate_individual_dfs_all_partner_additional_fields.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2254 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_main_all_partner_additional_fields.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    41477 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_redshift_update_all_partner_additional_fields.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    12115 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_URM_additional_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4382 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_accepted_entered_stage_additional_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4097 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_applied_comm_entered_additional_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     9815 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_campus_visit_additional_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    11490 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_caucasian_additional_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    10761 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_comm_matched_additional_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     8009 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_enrolled_comm_entered_additional_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     9816 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_first_gen_additional_fields.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    12511 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_known_race_additional_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    18983 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_non_FG_CV_and_URM.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    11249 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_race_ethnicity_distribution_additional_data.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.987930 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3996 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/function_calculate_individual_dfs_all_partner_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2913 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/function_main_all_partner_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    15332 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/function_redshift_update_all_partner_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     9086 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_01.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6561 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_02.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     7481 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_03.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6171 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_04.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     9664 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_05.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4012 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_06.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5501 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_07.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2248 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_08.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3716 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_09.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.987930 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/mau_30day_rolling_average/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1351 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/mau_30day_rolling_average/function_main_mau_30day_rolling_average.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3551 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/mau_30day_rolling_average/function_redshift_update_mau_30day_rolling_average.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2630 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/mau_30day_rolling_average/z_calculate_30day_rolling_average.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.987930 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/
--rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/_init_.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1990 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/function_calculate_individual_dfs_onepager_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1931 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/function_main_onepager_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     8120 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/function_redshift_update_onepager_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2619 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_comm_entered_preinquired.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2997 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_comm_match.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      941 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_community_funnel_counts.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3360 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_non_dupe_ntr.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2791 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_organic.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.987930 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/org_data_tracker/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5413 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/org_data_tracker/update_org_data_tracker_table.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.987930 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/organization_data/
--rw-r--r--   0 mayur     (1002) mayur     (1002)    10004 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/organization_data/update_organization_data_table.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.987930 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/prediction_model/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1201 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/prediction_model/function_main_prediction_model.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1976 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/prediction_model/z_clean_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3715 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/prediction_model/z_one_hot_encoding.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1239 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/prediction_model/z_scaling.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:18.991930 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/
--rw-r--r--   0 mayur     (1002) mayur     (1002)      954 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/alter_redshift_table.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      664 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/cancel_redshift_lock.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      371 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/cancel_redshift_query.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1803 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/create_redshift_table.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      404 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/delete_redshift_table.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      435 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/delete_row_redshift.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1224 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/modify_field_names_redshift.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      650 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/update_row_value_redshift.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      978 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/vaccum_redshift_tables.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:19.031931 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/touchpoint_dash/
--rw-r--r--   0 mayur     (1002) mayur     (1002)      977 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/touchpoint_dash/function_calculate_individual_dfs_touchpoint_dash.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1407 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/touchpoint_dash/function_main_touchpoint_dash.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    17005 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/touchpoint_dash/function_redshift_update_touchpoint_dash.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    26492 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/touchpoint_dash/z_calculate_values_01.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:19.031931 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/virtual_events/
--rw-r--r--   0 mayur     (1002) mayur     (1002)    13194 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/virtual_events/function_get_event_data.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)    10187 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/virtual_events/function_main_virtual_events.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3504 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/virtual_events/function_redshift_update_participants_table.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     5776 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/virtual_events/function_redshift_update_virtual_events_data_table.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:19.031931 zeemee_py-0.0.1.0/src/zeemee_py/reports/
--rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/__init__.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:19.031931 zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3000 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_create_schedule.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      583 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_delete_schedule.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1868 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_get_email_list.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1263 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_get_schedule_ids.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6959 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_main_snapshot_email.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:19.031931 zeemee_py-0.0.1.0/src/zeemee_py/reports/slack_reports/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3790 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/slack_reports/daily_new_accounts_slack_update.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:19.031931 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/
--rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/__init__.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2258 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_add_new_columns.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4047 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_create_engagement_data_df.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     6128 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_main_touchpoint.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2436 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_modify_column_values.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      847 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_touchpoint_query_from_touchpoint_table.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     4456 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_upload_to_destination.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      569 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_engaged_any_column.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1980 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_engaged_week_column.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1039 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_fname_lname_column.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      704 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_friendfinder_rmmatch_column.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      572 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_incsv_column.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      287 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_information_column.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3539 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_last_engaged_column.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1893 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_login_week_column.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     1327 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_year_term_type_partnercsv_columns.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     2008 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_modify_id_number_values.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)      768 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_upload_to_admin.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     8040 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_upload_to_sftp.py
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3213 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_upload_to_slate.py
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:19.035930 zeemee_py-0.0.1.0/src/zeemee_py.egg-info/
--rw-r--r--   0 mayur     (1002) mayur     (1002)     3916 2024-05-22 21:30:18.000000 zeemee_py-0.0.1.0/src/zeemee_py.egg-info/PKG-INFO
--rw-r--r--   0 mayur     (1002) mayur     (1002)    19090 2024-05-22 21:30:18.000000 zeemee_py-0.0.1.0/src/zeemee_py.egg-info/SOURCES.txt
--rw-r--r--   0 mayur     (1002) mayur     (1002)        1 2024-05-22 21:30:18.000000 zeemee_py-0.0.1.0/src/zeemee_py.egg-info/dependency_links.txt
--rw-r--r--   0 mayur     (1002) mayur     (1002)      127 2024-05-22 21:30:18.000000 zeemee_py-0.0.1.0/src/zeemee_py.egg-info/requires.txt
--rw-r--r--   0 mayur     (1002) mayur     (1002)       10 2024-05-22 21:30:18.000000 zeemee_py-0.0.1.0/src/zeemee_py.egg-info/top_level.txt
-drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:19.031931 zeemee_py-0.0.1.0/tests/
--rw-r--r--   0 mayur     (1002) mayur     (1002)      485 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.0/tests/test.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.780139 zeemee_py-0.0.1.1/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)       42 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/LICENSE
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3916 2024-05-22 21:30:50.780139 zeemee_py-0.0.1.1/PKG-INFO
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3214 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/README.md
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      787 2024-05-22 21:30:46.000000 zeemee_py-0.0.1.1/pyproject.toml
+-rw-r--r--   0 mayur     (1002) mayur     (1002)       38 2024-05-22 21:30:50.780139 zeemee_py-0.0.1.1/setup.cfg
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.680138 zeemee_py-0.0.1.1/src/
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.684138 zeemee_py-0.0.1.1/src/zeemee_py/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/__init__.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.684138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.684138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.688138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4984 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_ap1_by_gender_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3810 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_ap1_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     9585 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_common_ap1_calculate_values.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1994 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2397 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1914 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2322 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6894 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     7224 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6834 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6910 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_for_old_cohort.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.688138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1345 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/function_ap1_perform_athena_update.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2607 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/function_ap1_recreate_full_table.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.684138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.688138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5494 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_ap2_by_gender_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3812 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_ap2_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2573 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    16874 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_campus_visit.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    16280 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_first_gen.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    17682 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_not_campus_visit.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    17076 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_not_first_gen.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1994 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2396 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1914 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2321 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6997 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     7224 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6910 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6900 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_for_old_cohort.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.688138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1345 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/function_ap2_perform_athena_update.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2607 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/function_ap2_recreate_full_table.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.684138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.692138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5494 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_ap3_by_gender_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3812 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_ap3_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2989 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6481 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_app_rate.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     7589 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_commitment_rate.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5580 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_melt_rate.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4276 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_missing_dates.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     9104 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_yield_rate.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1994 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2395 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1903 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2320 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6997 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     7224 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6910 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6900 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_for_old_cohort.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.692138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1345 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/function_ap3_perform_athena_update.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2607 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/function_ap3_recreate_full_table.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.692138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/athena_code/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     8157 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/athena_code/create_or_update_athena_tables_for_gold_schema.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.692138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/general_athena_table_update/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5764 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/general_athena_table_update/data_team_creation_and_updation.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1059 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/general_athena_table_update/get_column_details.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.692138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2631 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/create_zeemee_tp_college_combined_files.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3422 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_rawDataCurrent_details.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2886 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_rawDataCurrent_details_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2904 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_touchpoint_file_details.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3348 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_college_combined_files_details.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2556 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_college_combined_files_details_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      904 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_tp_and_college_file_details_in_one_table.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1293 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/query_athena_with_retry.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      760 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/query_athena_without_retry.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1741 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/send_slack_notifications.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.684138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.724138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2178 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3964 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_comm_match.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4591 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_non_dupe_ntr.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3762 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_organic.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4861 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_op1_by_gender_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3685 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_op1_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2003 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2501 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1912 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2416 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6796 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     7115 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6907 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     7080 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_for_old_cohort.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.724138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1321 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/function_op1_perform_athena_update.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2585 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/function_op1_recreate_full_table.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.684138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.724138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3717 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5488 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_accepted_community_entered_counts.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5391 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_applied_community_entered_counts.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5584 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_committed_community_entered_counts.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5487 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_enrolled_community_entered_counts.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5487 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_inquired_community_entered_counts.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4864 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_op2_by_gender_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3685 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_op2_create_one_school_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2004 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2501 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1913 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2416 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6797 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_by_gender_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     7115 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_by_gender_for_old_cohort.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6908 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_for_config_schools.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     7080 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_for_old_cohort.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.724138 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1321 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/function_op2_perform_athena_update.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2585 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/function_op2_recreate_full_table.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.728138 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/__init__.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1304 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/connect_athena.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1125 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/connect_duckdb.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      620 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/connect_redshift.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      726 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_config.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      617 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_data_folder_path.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3153 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_latest_postwrangler_files.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3129 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_latest_touchpoints_files.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      571 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_org_additional_data_file.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      542 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_org_tracker.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1121 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_dataframe_to_s3.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      823 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_email.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1115 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_to_admin_and_make_visible.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      811 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_to_s3.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1022 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_to_slack.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.728138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      206 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/__init__.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.728138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5391 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_calculate_individual_dfs_all_partner_additional_fields.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2254 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_main_all_partner_additional_fields.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    41477 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_redshift_update_all_partner_additional_fields.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    12115 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_URM_additional_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4382 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_accepted_entered_stage_additional_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4097 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_applied_comm_entered_additional_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     9815 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_campus_visit_additional_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    11490 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_caucasian_additional_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    10761 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_comm_matched_additional_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     8009 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_enrolled_comm_entered_additional_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     9816 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_first_gen_additional_fields.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    12511 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_known_race_additional_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    18983 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_non_FG_CV_and_URM.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    11249 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_race_ethnicity_distribution_additional_data.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.732138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3996 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/function_calculate_individual_dfs_all_partner_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2913 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/function_main_all_partner_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    15332 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/function_redshift_update_all_partner_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     9086 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_01.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6561 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_02.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     7481 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_03.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6171 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_04.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     9664 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_05.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4012 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_06.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5501 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_07.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2248 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_08.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3716 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_09.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.732138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/mau_30day_rolling_average/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1351 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/mau_30day_rolling_average/function_main_mau_30day_rolling_average.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3551 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/mau_30day_rolling_average/function_redshift_update_mau_30day_rolling_average.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2630 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/mau_30day_rolling_average/z_calculate_30day_rolling_average.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.732138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/_init_.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1990 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/function_calculate_individual_dfs_onepager_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1931 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/function_main_onepager_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     8120 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/function_redshift_update_onepager_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2619 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_comm_entered_preinquired.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2997 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_comm_match.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      941 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_community_funnel_counts.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3360 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_non_dupe_ntr.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2791 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_organic.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.732138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/org_data_tracker/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5413 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/org_data_tracker/update_org_data_tracker_table.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.732138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/organization_data/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    10004 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/organization_data/update_organization_data_table.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.732138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/prediction_model/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1201 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/prediction_model/function_main_prediction_model.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1976 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/prediction_model/z_clean_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3715 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/prediction_model/z_one_hot_encoding.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1239 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/prediction_model/z_scaling.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.736138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      954 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/alter_redshift_table.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      664 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/cancel_redshift_lock.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      371 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/cancel_redshift_query.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1803 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/create_redshift_table.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      404 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/delete_redshift_table.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      435 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/delete_row_redshift.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1224 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/modify_field_names_redshift.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      650 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/update_row_value_redshift.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      978 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/vaccum_redshift_tables.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.736138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/touchpoint_dash/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      977 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/touchpoint_dash/function_calculate_individual_dfs_touchpoint_dash.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1407 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/touchpoint_dash/function_main_touchpoint_dash.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    17005 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/touchpoint_dash/function_redshift_update_touchpoint_dash.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    26492 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/touchpoint_dash/z_calculate_values_01.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.736138 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/virtual_events/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    13194 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/virtual_events/function_get_event_data.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    10187 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/virtual_events/function_main_virtual_events.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3504 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/virtual_events/function_redshift_update_participants_table.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     5776 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/virtual_events/function_redshift_update_virtual_events_data_table.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.736138 zeemee_py-0.0.1.1/src/zeemee_py/reports/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/__init__.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.736138 zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3000 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_create_schedule.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      583 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_delete_schedule.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1868 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_get_email_list.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1263 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_get_schedule_ids.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6959 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_main_snapshot_email.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.736138 zeemee_py-0.0.1.1/src/zeemee_py/reports/slack_reports/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3790 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/slack_reports/daily_new_accounts_slack_update.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.780139 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/__init__.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2258 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_add_new_columns.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4047 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_create_engagement_data_df.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     6128 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_main_touchpoint.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2436 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_modify_column_values.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      847 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_touchpoint_query_from_touchpoint_table.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     4456 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_upload_to_destination.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      569 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_engaged_any_column.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1980 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_engaged_week_column.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1039 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_fname_lname_column.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      704 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_friendfinder_rmmatch_column.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      572 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_incsv_column.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      287 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_information_column.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3539 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_last_engaged_column.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1893 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_login_week_column.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     1327 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_year_term_type_partnercsv_columns.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     2008 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_modify_id_number_values.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      768 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_upload_to_admin.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     8040 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_upload_to_sftp.py
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3213 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_upload_to_slate.py
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.780139 zeemee_py-0.0.1.1/src/zeemee_py.egg-info/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)     3916 2024-05-22 21:30:50.000000 zeemee_py-0.0.1.1/src/zeemee_py.egg-info/PKG-INFO
+-rw-r--r--   0 mayur     (1002) mayur     (1002)    19090 2024-05-22 21:30:50.000000 zeemee_py-0.0.1.1/src/zeemee_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mayur     (1002) mayur     (1002)        1 2024-05-22 21:30:50.000000 zeemee_py-0.0.1.1/src/zeemee_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      127 2024-05-22 21:30:50.000000 zeemee_py-0.0.1.1/src/zeemee_py.egg-info/requires.txt
+-rw-r--r--   0 mayur     (1002) mayur     (1002)       10 2024-05-22 21:30:50.000000 zeemee_py-0.0.1.1/src/zeemee_py.egg-info/top_level.txt
+drwxr-xr-x   0 mayur     (1002) mayur     (1002)        0 2024-05-22 21:30:50.780139 zeemee_py-0.0.1.1/tests/
+-rw-r--r--   0 mayur     (1002) mayur     (1002)      485 2024-05-22 21:12:02.000000 zeemee_py-0.0.1.1/tests/test.py
```

### Comparing `zeemee_py-0.0.1.0/PKG-INFO` & `zeemee_py-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeemee_py
-Version: 0.0.1.0
+Version: 0.0.1.1
 Summary: Python packages for ZeeMee data-team
 Author-email: Mayur Waghela <mayur@zeemee.com>
 Project-URL: Homepage, https://github.com/zeemee/data-team
 Project-URL: Issues, https://github.com/zeemee/data-team/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.8
```

### Comparing `zeemee_py-0.0.1.0/README.md` & `zeemee_py-0.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/pyproject.toml` & `zeemee_py-0.0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.5.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zeemee_py"
-version = "0.0.1.0"
+version = "0.0.1.1"
 authors = [
   { name="Mayur Waghela", email="mayur@zeemee.com" },
 ]
 description = "Python packages for ZeeMee data-team"
 readme = "README.md"
 requires-python = ">=3.11.8"
 classifiers = [
```

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_ap1_by_gender_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_ap1_by_gender_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_ap1_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_ap1_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_common_ap1_calculate_values.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/function_common_ap1_calculate_values.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/main_stitch_ap1_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_data_processing/process_ap1_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/function_ap1_perform_athena_update.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/function_ap1_perform_athena_update.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/function_ap1_recreate_full_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part1/ap1_module_table_update/function_ap1_recreate_full_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_ap2_by_gender_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_ap2_by_gender_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_ap2_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_ap2_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_campus_visit.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_campus_visit.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_first_gen.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_first_gen.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_not_campus_visit.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_not_campus_visit.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_not_first_gen.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/function_common_ap2_calculate_values_not_first_gen.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/main_stitch_ap2_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_data_processing/process_ap2_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/function_ap2_perform_athena_update.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/function_ap2_perform_athena_update.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/function_ap2_recreate_full_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part2/ap2_module_table_update/function_ap2_recreate_full_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_ap3_by_gender_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_ap3_by_gender_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_ap3_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_ap3_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_app_rate.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_app_rate.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_commitment_rate.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_commitment_rate.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_melt_rate.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_melt_rate.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_missing_dates.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_missing_dates.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_yield_rate.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/function_common_ap3_calculate_values_yield_rate.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/main_stitch_ap3_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_data_processing/process_ap3_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/function_ap3_perform_athena_update.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/function_ap3_perform_athena_update.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/function_ap3_recreate_full_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/all_partner_data_part3/ap3_module_table_update/function_ap3_recreate_full_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/athena_code/create_or_update_athena_tables_for_gold_schema.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/athena_code/create_or_update_athena_tables_for_gold_schema.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/general_athena_table_update/data_team_creation_and_updation.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/general_athena_table_update/data_team_creation_and_updation.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/general_athena_table_update/get_column_details.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/general_athena_table_update/get_column_details.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/create_zeemee_tp_college_combined_files.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/create_zeemee_tp_college_combined_files.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_rawDataCurrent_details.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_rawDataCurrent_details.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_rawDataCurrent_details_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_rawDataCurrent_details_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_touchpoint_file_details.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_touchpoint_file_details.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_college_combined_files_details.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_college_combined_files_details.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_college_combined_files_details_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_college_combined_files_details_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_tp_and_college_file_details_in_one_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/get_zeemee_tp_and_college_file_details_in_one_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/query_athena_with_retry.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/query_athena_with_retry.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/query_athena_without_retry.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/query_athena_without_retry.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/helper_functions/send_slack_notifications.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/helper_functions/send_slack_notifications.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_comm_match.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_comm_match.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_non_dupe_ntr.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_non_dupe_ntr.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_organic.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_common_op1_calculate_values_organic.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_op1_by_gender_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_op1_by_gender_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_op1_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/function_op1_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/main_stitch_op1_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_data_processing/process_op1_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/function_op1_perform_athena_update.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/function_op1_perform_athena_update.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/function_op1_recreate_full_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part1/op1_module_table_update/function_op1_recreate_full_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_accepted_community_entered_counts.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_accepted_community_entered_counts.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_applied_community_entered_counts.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_applied_community_entered_counts.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_committed_community_entered_counts.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_committed_community_entered_counts.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_enrolled_community_entered_counts.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_enrolled_community_entered_counts.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_inquired_community_entered_counts.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_common_op2_calculate_values_inquired_community_entered_counts.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_op2_by_gender_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_op2_by_gender_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_op2_create_one_school_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/function_op2_create_one_school_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/main_stitch_op2_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_by_gender_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_by_gender_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_by_gender_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_by_gender_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_for_config_schools.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_for_config_schools.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_for_old_cohort.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_data_processing/process_op2_for_old_cohort.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/function_op2_perform_athena_update.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/function_op2_perform_athena_update.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/function_op2_recreate_full_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/data_team_etl/one_pager_data_part2/op2_module_table_update/function_op2_recreate_full_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/connect_athena.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/connect_athena.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/connect_duckdb.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/connect_duckdb.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/connect_redshift.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/connect_redshift.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_config.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_config.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_data_folder_path.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_data_folder_path.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_latest_postwrangler_files.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_latest_postwrangler_files.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_latest_touchpoints_files.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_latest_touchpoints_files.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_org_additional_data_file.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_org_additional_data_file.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/get_org_tracker.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/get_org_tracker.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_dataframe_to_s3.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_dataframe_to_s3.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_email.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_email.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_to_admin_and_make_visible.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_to_admin_and_make_visible.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_to_s3.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_to_s3.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/helper_functions/send_to_slack.py` & `zeemee_py-0.0.1.1/src/zeemee_py/helper_functions/send_to_slack.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_calculate_individual_dfs_all_partner_additional_fields.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_calculate_individual_dfs_all_partner_additional_fields.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_main_all_partner_additional_fields.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_main_all_partner_additional_fields.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_redshift_update_all_partner_additional_fields.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/function_redshift_update_all_partner_additional_fields.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_URM_additional_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_URM_additional_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_accepted_entered_stage_additional_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_accepted_entered_stage_additional_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_applied_comm_entered_additional_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_applied_comm_entered_additional_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_campus_visit_additional_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_campus_visit_additional_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_caucasian_additional_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_caucasian_additional_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_comm_matched_additional_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_comm_matched_additional_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_enrolled_comm_entered_additional_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_enrolled_comm_entered_additional_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_first_gen_additional_fields.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_first_gen_additional_fields.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_known_race_additional_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_known_race_additional_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_non_FG_CV_and_URM.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_non_FG_CV_and_URM.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_race_ethnicity_distribution_additional_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_additional_fields/z_race_ethnicity_distribution_additional_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/function_calculate_individual_dfs_all_partner_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/function_calculate_individual_dfs_all_partner_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/function_main_all_partner_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/function_main_all_partner_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/function_redshift_update_all_partner_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/function_redshift_update_all_partner_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_01.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_01.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_02.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_02.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_03.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_03.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_04.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_04.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_05.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_05.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_06.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_06.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_07.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_07.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_08.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_08.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_09.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/all_partner_data/z_calculate_values_09.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/mau_30day_rolling_average/function_main_mau_30day_rolling_average.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/mau_30day_rolling_average/function_main_mau_30day_rolling_average.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/mau_30day_rolling_average/function_redshift_update_mau_30day_rolling_average.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/mau_30day_rolling_average/function_redshift_update_mau_30day_rolling_average.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/mau_30day_rolling_average/z_calculate_30day_rolling_average.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/mau_30day_rolling_average/z_calculate_30day_rolling_average.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/function_calculate_individual_dfs_onepager_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/function_calculate_individual_dfs_onepager_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/function_main_onepager_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/function_main_onepager_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/function_redshift_update_onepager_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/function_redshift_update_onepager_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_comm_entered_preinquired.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_comm_entered_preinquired.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_comm_match.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_comm_match.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_community_funnel_counts.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_community_funnel_counts.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_non_dupe_ntr.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_non_dupe_ntr.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/one_pager_data/z_organic.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/one_pager_data/z_organic.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/org_data_tracker/update_org_data_tracker_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/org_data_tracker/update_org_data_tracker_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/organization_data/update_organization_data_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/organization_data/update_organization_data_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/prediction_model/function_main_prediction_model.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/prediction_model/function_main_prediction_model.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/prediction_model/z_clean_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/prediction_model/z_clean_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/prediction_model/z_one_hot_encoding.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/prediction_model/z_one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/prediction_model/z_scaling.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/prediction_model/z_scaling.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/alter_redshift_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/alter_redshift_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/cancel_redshift_lock.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/cancel_redshift_lock.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/create_redshift_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/create_redshift_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/modify_field_names_redshift.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/modify_field_names_redshift.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/update_row_value_redshift.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/update_row_value_redshift.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/redshift_dev_scripts/vaccum_redshift_tables.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/redshift_dev_scripts/vaccum_redshift_tables.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/touchpoint_dash/function_calculate_individual_dfs_touchpoint_dash.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/touchpoint_dash/function_calculate_individual_dfs_touchpoint_dash.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/touchpoint_dash/function_main_touchpoint_dash.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/touchpoint_dash/function_main_touchpoint_dash.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/touchpoint_dash/function_redshift_update_touchpoint_dash.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/touchpoint_dash/function_redshift_update_touchpoint_dash.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/touchpoint_dash/z_calculate_values_01.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/touchpoint_dash/z_calculate_values_01.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/virtual_events/function_get_event_data.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/virtual_events/function_get_event_data.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/virtual_events/function_main_virtual_events.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/virtual_events/function_main_virtual_events.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/virtual_events/function_redshift_update_participants_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/virtual_events/function_redshift_update_participants_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/redshift_updates/virtual_events/function_redshift_update_virtual_events_data_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/redshift_updates/virtual_events/function_redshift_update_virtual_events_data_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_create_schedule.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_create_schedule.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_delete_schedule.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_delete_schedule.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_get_email_list.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_get_email_list.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_get_schedule_ids.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_get_schedule_ids.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/holistics_snapshot_email/function_main_snapshot_email.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/holistics_snapshot_email/function_main_snapshot_email.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/slack_reports/daily_new_accounts_slack_update.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/slack_reports/daily_new_accounts_slack_update.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_add_new_columns.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_add_new_columns.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_create_engagement_data_df.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_create_engagement_data_df.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_main_touchpoint.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_main_touchpoint.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_modify_column_values.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_modify_column_values.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_touchpoint_query_from_touchpoint_table.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_touchpoint_query_from_touchpoint_table.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/function_upload_to_destination.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/function_upload_to_destination.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_engaged_any_column.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_engaged_any_column.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_engaged_week_column.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_engaged_week_column.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_fname_lname_column.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_fname_lname_column.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_friendfinder_rmmatch_column.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_friendfinder_rmmatch_column.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_incsv_column.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_incsv_column.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_last_engaged_column.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_last_engaged_column.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_login_week_column.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_login_week_column.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_create_year_term_type_partnercsv_columns.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_create_year_term_type_partnercsv_columns.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_modify_id_number_values.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_modify_id_number_values.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_upload_to_admin.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_upload_to_admin.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_upload_to_sftp.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_upload_to_sftp.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py/reports/touchpoint_report/z_upload_to_slate.py` & `zeemee_py-0.0.1.1/src/zeemee_py/reports/touchpoint_report/z_upload_to_slate.py`

 * *Files identical despite different names*

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py.egg-info/PKG-INFO` & `zeemee_py-0.0.1.1/src/zeemee_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeemee_py
-Version: 0.0.1.0
+Version: 0.0.1.1
 Summary: Python packages for ZeeMee data-team
 Author-email: Mayur Waghela <mayur@zeemee.com>
 Project-URL: Homepage, https://github.com/zeemee/data-team
 Project-URL: Issues, https://github.com/zeemee/data-team/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.8
```

### Comparing `zeemee_py-0.0.1.0/src/zeemee_py.egg-info/SOURCES.txt` & `zeemee_py-0.0.1.1/src/zeemee_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

