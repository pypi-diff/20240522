# Comparing `tmp/patent_client-5.0.8.tar.gz` & `tmp/patent_client-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_client-5.0.8.tar", max compression
+gzip compressed data, was "patent_client-5.0.9.tar", max compression
```

## Comparing `patent_client-5.0.8.tar` & `patent_client-5.0.9.tar`

### file list

```diff
@@ -1,409 +1,409 @@
--rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.8/LICENSE
--rw-r--r--   0        0        0     6283 2024-05-02 17:06:23.093538 patent_client-5.0.8/README.md
--rw-r--r--   0        0        0     1739 2024-05-03 17:25:00.646245 patent_client-5.0.8/patent_client/__init__.py
--rw-r--r--   0        0        0      833 2024-05-02 17:06:23.121290 patent_client-5.0.8/patent_client/_async/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.8/patent_client/_async/epo/__init__.py
--rw-r--r--   0        0        0      214 2024-05-01 18:05:47.951425 patent_client-5.0.8/patent_client/_async/epo/ops/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.8/patent_client/_async/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      360 2024-05-03 17:25:00.646675 patent_client-5.0.8/patent_client/_async/epo/ops/family/api.py
--rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.8/patent_client/_async/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.8/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.8/patent_client/_async/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.8/patent_client/_async/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.8/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      356 2024-05-03 17:25:00.646963 patent_client-5.0.8/patent_client/_async/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1119 2024-05-01 18:05:47.952437 patent_client-5.0.8/patent_client/_async/epo/ops/family/model.py
--rw-r--r--   0        0        0      519 2024-05-01 18:05:47.952767 patent_client-5.0.8/patent_client/_async/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1503 2024-05-03 17:25:00.647248 patent_client-5.0.8/patent_client/_async/epo/ops/family/schema.py
--rw-r--r--   0        0        0      527 2024-05-01 18:05:47.953647 patent_client-5.0.8/patent_client/_async/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.8/patent_client/_async/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      359 2024-05-02 17:06:23.121738 patent_client-5.0.8/patent_client/_async/epo/ops/legal/api.py
--rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.8/patent_client/_async/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0      467 2024-05-03 17:25:00.653744 patent_client-5.0.8/patent_client/_async/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2375 2024-05-01 18:05:47.954191 patent_client-5.0.8/patent_client/_async/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5434 2024-05-03 17:25:00.657228 patent_client-5.0.8/patent_client/_async/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.8/patent_client/_async/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4018 2024-05-03 17:25:00.661652 patent_client-5.0.8/patent_client/_async/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1216 2024-05-01 18:05:47.954968 patent_client-5.0.8/patent_client/_async/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.8/patent_client/_async/epo/ops/legal/util.py
--rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.8/patent_client/_async/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1415 2024-05-02 17:06:23.125551 patent_client-5.0.8/patent_client/_async/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     1806 2024-05-01 18:05:47.955307 patent_client-5.0.8/patent_client/_async/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1117 2024-05-01 18:05:47.955516 patent_client-5.0.8/patent_client/_async/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.8/patent_client/_async/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.8/patent_client/_async/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0      763 2024-05-01 18:05:47.955715 patent_client-5.0.8/patent_client/_async/epo/ops/number_service/model.py
--rw-r--r--   0        0        0      952 2024-05-01 18:05:47.955921 patent_client-5.0.8/patent_client/_async/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.8/patent_client/_async/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5472 2024-05-03 17:25:00.661893 patent_client-5.0.8/patent_client/_async/epo/ops/published/api.py
--rw-r--r--   0        0        0     2699 2024-05-03 17:25:00.662175 patent_client-5.0.8/patent_client/_async/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.8/patent_client/_async/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6174 2024-05-03 19:08:07.224593 patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    20102 2024-05-03 19:08:07.228235 patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18516 2024-05-03 19:08:07.239602 patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3204 2024-05-03 17:25:00.662696 patent_client-5.0.8/patent_client/_async/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2411 2024-05-03 17:25:00.662959 patent_client-5.0.8/patent_client/_async/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      321 2024-05-01 18:05:47.957189 patent_client-5.0.8/patent_client/_async/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     2754 2024-05-01 18:05:47.957413 patent_client-5.0.8/patent_client/_async/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1050 2024-05-01 18:05:47.957672 patent_client-5.0.8/patent_client/_async/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2078 2024-05-03 17:25:00.663177 patent_client-5.0.8/patent_client/_async/epo/ops/published/model/images.py
--rw-r--r--   0        0        0      843 2024-05-01 18:05:47.958081 patent_client-5.0.8/patent_client/_async/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      285 2024-05-01 18:05:47.958344 patent_client-5.0.8/patent_client/_async/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     3934 2024-05-03 17:25:00.663421 patent_client-5.0.8/patent_client/_async/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0      874 2024-05-01 18:05:47.958917 patent_client-5.0.8/patent_client/_async/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     1640 2024-05-03 17:25:00.664113 patent_client-5.0.8/patent_client/_async/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.8/patent_client/_async/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3160 2024-05-03 17:25:00.664661 patent_client-5.0.8/patent_client/_async/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-05-03 19:08:07.371916 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-05-03 19:08:07.376377 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.8/patent_client/_async/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3478 2024-05-03 17:25:00.664935 patent_client-5.0.8/patent_client/_async/epo/ops/session.py
--rw-r--r--   0        0        0     2881 2024-05-03 17:25:00.665195 patent_client-5.0.8/patent_client/_async/epo/ops/util.py
--rw-r--r--   0        0        0     3220 2024-05-03 17:25:00.665599 patent_client-5.0.8/patent_client/_async/http_client.py
--rw-r--r--   0        0        0      201 2024-05-02 17:06:23.136948 patent_client-5.0.8/patent_client/_async/odp.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.8/patent_client/_async/uspto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.8/patent_client/_async/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2538 2024-05-03 17:25:00.665812 patent_client-5.0.8/patent_client/_async/uspto/assignment/api.py
--rw-r--r--   0        0        0      921 2024-05-02 17:06:23.137157 patent_client-5.0.8/patent_client/_async/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     3595 2024-05-03 17:25:00.666143 patent_client-5.0.8/patent_client/_async/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.8/patent_client/_async/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3424 2024-05-03 17:25:00.666449 patent_client-5.0.8/patent_client/_async/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4158 2024-05-03 17:25:00.666715 patent_client-5.0.8/patent_client/_async/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5500 2024-05-03 17:25:00.666971 patent_client-5.0.8/patent_client/_async/uspto/assignment/model.py
--rw-r--r--   0        0        0     1932 2024-05-01 18:05:47.962761 patent_client-5.0.8/patent_client/_async/uspto/assignment/model_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.8/patent_client/_async/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3182 2024-05-03 17:25:00.667431 patent_client-5.0.8/patent_client/_async/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1100 2024-05-01 18:05:47.963236 patent_client-5.0.8/patent_client/_async/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     2781 2024-05-01 18:05:47.963445 patent_client-5.0.8/patent_client/_async/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1707 2024-05-01 18:05:47.963660 patent_client-5.0.8/patent_client/_async/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1553 2024-05-03 17:25:00.667735 patent_client-5.0.8/patent_client/_async/uspto/bulk_data/model.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2109 2024-05-01 18:05:47.964054 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1143 2024-05-01 18:05:47.964243 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     1762 2024-05-03 17:25:00.667994 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     6897 2024-05-03 17:25:00.668558 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3738 2024-05-01 18:05:47.970105 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6031 2024-05-03 17:25:00.668826 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5252 2024-05-01 18:05:47.970651 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.8/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0        1 2024-05-01 18:05:47.970962 patent_client-5.0.8/patent_client/_async/uspto/odp/__init__.py
--rw-r--r--   0        0        0     6187 2024-05-03 18:56:17.340414 patent_client-5.0.8/patent_client/_async/uspto/odp/api.py
--rw-r--r--   0        0        0     2818 2024-05-03 17:25:00.669417 patent_client-5.0.8/patent_client/_async/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     5815 2024-05-03 18:56:17.114385 patent_client-5.0.8/patent_client/_async/uspto/odp/manager.py
--rw-r--r--   0        0        0     2127 2024-05-03 18:56:17.339737 patent_client-5.0.8/patent_client/_async/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    19876 2024-05-03 19:08:40.407498 patent_client-5.0.8/patent_client/_async/uspto/odp/model.py
--rw-r--r--   0        0        0    12577 2024-05-03 19:08:40.555304 patent_client-5.0.8/patent_client/_async/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2396 2024-05-01 18:05:47.972634 patent_client-5.0.8/patent_client/_async/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.8/patent_client/_async/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      475 2024-05-01 18:05:47.972937 patent_client-5.0.8/patent_client/_async/uspto/odp/util.py
--rw-r--r--   0        0        0      132 2024-05-01 18:05:47.973121 patent_client-5.0.8/patent_client/_async/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4501 2024-05-01 18:05:47.973352 patent_client-5.0.8/patent_client/_async/uspto/peds/api.py
--rw-r--r--   0        0        0      683 2024-05-03 17:25:00.670577 patent_client-5.0.8/patent_client/_async/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.8/patent_client/_async/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0     8619 2024-05-03 17:25:00.673086 patent_client-5.0.8/patent_client/_async/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8191 2024-05-03 17:25:00.673373 patent_client-5.0.8/patent_client/_async/uspto/peds/manager.py
--rw-r--r--   0        0        0     9623 2024-05-03 17:25:00.673653 patent_client-5.0.8/patent_client/_async/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    14958 2024-05-03 17:25:00.673984 patent_client-5.0.8/patent_client/_async/uspto/peds/model.py
--rw-r--r--   0        0        0     6116 2024-05-01 18:05:47.974623 patent_client-5.0.8/patent_client/_async/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.8/patent_client/_async/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      188 2024-05-02 17:06:23.210126 patent_client-5.0.8/patent_client/_async/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10134 2024-05-03 17:25:00.674181 patent_client-5.0.8/patent_client/_async/uspto/ptab/api.py
--rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.8/patent_client/_async/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.8/patent_client/_async/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.8/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2025 2024-05-03 17:25:00.674454 patent_client-5.0.8/patent_client/_async/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2249 2024-05-03 17:25:00.674630 patent_client-5.0.8/patent_client/_async/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8382 2024-05-03 17:25:00.674990 patent_client-5.0.8/patent_client/_async/uspto/ptab/model.py
--rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.8/patent_client/_async/uspto/ptab/util.py
--rw-r--r--   0        0        0      326 2024-05-02 17:06:23.210541 patent_client-5.0.8/patent_client/_async/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     6921 2024-05-03 17:25:00.675209 patent_client-5.0.8/patent_client/_async/uspto/public_search/api.py
--rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.8/patent_client/_async/uspto/public_search/api_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.8/patent_client/_async/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2066 2024-05-01 18:05:47.981591 patent_client-5.0.8/patent_client/_async/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     6548 2024-05-03 17:25:00.680068 patent_client-5.0.8/patent_client/_async/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     1594 2024-05-01 18:05:47.983719 patent_client-5.0.8/patent_client/_async/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1035 2024-05-02 17:06:23.211161 patent_client-5.0.8/patent_client/_async/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.8/patent_client/_async/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-05-03 19:08:09.632336 patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4132 2024-05-03 17:25:00.680395 patent_client-5.0.8/patent_client/_async/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7627 2024-05-03 17:25:00.680977 patent_client-5.0.8/patent_client/_async/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      554 2024-05-03 17:25:00.681546 patent_client-5.0.8/patent_client/_async/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3091 2024-05-03 17:25:00.681713 patent_client-5.0.8/patent_client/_async/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7574 2024-05-03 17:25:00.681893 patent_client-5.0.8/patent_client/_async/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2243 2024-05-03 17:25:00.682051 patent_client-5.0.8/patent_client/_async/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1535 2024-05-02 17:06:23.211470 patent_client-5.0.8/patent_client/_async/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4498 2024-05-03 17:25:00.682225 patent_client-5.0.8/patent_client/_async/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.8/patent_client/_async/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4056 2024-05-03 17:25:00.682391 patent_client-5.0.8/patent_client/_async/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.8/patent_client/_async/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.8/patent_client/_async/uspto/public_search/util.py
--rw-r--r--   0        0        0     1249 2024-05-03 19:07:58.356029 patent_client-5.0.8/patent_client/_sync/__init__.py
--rw-r--r--   0        0        0      416 2024-05-03 19:07:58.918971 patent_client-5.0.8/patent_client/_sync/epo/__init__.py
--rw-r--r--   0        0        0      630 2024-05-03 19:07:58.930646 patent_client-5.0.8/patent_client/_sync/epo/ops/__init__.py
--rw-r--r--   0        0        0      416 2024-05-03 19:07:58.947993 patent_client-5.0.8/patent_client/_sync/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      764 2024-05-03 19:07:58.951037 patent_client-5.0.8/patent_client/_sync/epo/ops/family/api.py
--rw-r--r--   0        0        0      839 2024-05-03 19:08:41.001990 patent_client-5.0.8/patent_client/_sync/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-05-03 19:07:58.958136 patent_client-5.0.8/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-05-03 19:07:58.958426 patent_client-5.0.8/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-05-03 19:07:58.959117 patent_client-5.0.8/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-05-03 19:07:58.958758 patent_client-5.0.8/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      750 2024-05-03 19:07:58.953267 patent_client-5.0.8/patent_client/_sync/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1535 2024-05-03 19:07:58.950132 patent_client-5.0.8/patent_client/_sync/epo/ops/family/model.py
--rw-r--r--   0        0        0      887 2024-05-03 19:08:40.986449 patent_client-5.0.8/patent_client/_sync/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1919 2024-05-03 19:07:58.955892 patent_client-5.0.8/patent_client/_sync/epo/ops/family/schema.py
--rw-r--r--   0        0        0      943 2024-05-03 19:07:58.947829 patent_client-5.0.8/patent_client/_sync/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0      416 2024-05-03 19:07:59.048390 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      763 2024-05-03 19:07:59.053311 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/api.py
--rw-r--r--   0        0        0      688 2024-05-03 19:08:41.003907 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-05-03 19:07:59.083882 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-05-03 19:07:59.082163 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-05-03 19:07:59.083495 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-05-03 19:07:59.082496 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-05-03 19:07:59.082754 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-05-03 19:07:59.083096 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-05-03 19:07:59.081053 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0      847 2024-05-03 19:08:40.554626 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2791 2024-05-03 19:07:59.052457 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5767 2024-05-03 19:08:40.531684 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      866 2024-05-03 19:08:41.005042 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4434 2024-05-03 19:07:59.070800 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1632 2024-05-03 19:07:59.047514 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      530 2024-05-03 19:07:59.047999 patent_client-5.0.8/patent_client/_sync/epo/ops/legal/util.py
--rw-r--r--   0        0        0      483 2024-05-03 19:07:58.931519 patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1819 2024-05-03 19:07:58.935606 patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     2023 2024-05-03 19:08:40.553863 patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1533 2024-05-03 19:07:58.938020 patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-05-03 19:07:58.930953 patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-05-03 19:07:58.935754 patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0     1179 2024-05-03 19:07:58.933183 patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/model.py
--rw-r--r--   0        0        0     1368 2024-05-03 19:07:58.943318 patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0      416 2024-05-03 19:07:58.969025 patent_client-5.0.8/patent_client/_sync/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5742 2024-05-03 19:08:40.554760 patent_client-5.0.8/patent_client/_sync/epo/ops/published/api.py
--rw-r--r--   0        0        0     2878 2024-05-03 19:08:40.995502 patent_client-5.0.8/patent_client/_sync/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1917 2024-05-03 19:07:58.971495 patent_client-5.0.8/patent_client/_sync/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-05-03 19:07:59.043721 patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6174 2024-05-03 19:08:26.915184 patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-05-03 19:07:59.042807 patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-05-03 19:07:59.043133 patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    20102 2024-05-03 19:08:26.918533 patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18516 2024-05-03 19:08:26.929284 patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3494 2024-05-03 19:07:58.990416 patent_client-5.0.8/patent_client/_sync/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2383 2024-05-03 19:08:40.554169 patent_client-5.0.8/patent_client/_sync/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      737 2024-05-03 19:07:59.029642 patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     3170 2024-05-03 19:07:59.034326 patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1466 2024-05-03 19:07:59.042057 patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2470 2024-05-03 19:07:59.038161 patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/images.py
--rw-r--r--   0        0        0     1259 2024-05-03 19:07:59.039904 patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      701 2024-05-03 19:07:59.015580 patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     4350 2024-05-03 19:07:59.022076 patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0     1290 2024-05-03 19:07:59.028646 patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     2056 2024-05-03 19:07:59.025156 patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0     1066 2024-05-03 19:07:59.026537 patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3576 2024-05-03 19:07:58.968746 patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-05-03 19:07:58.991870 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-05-03 19:07:58.992900 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-05-03 19:07:58.992607 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-05-03 19:07:58.992166 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-05-03 19:08:27.058853 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-05-03 19:07:58.994509 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-05-03 19:08:27.062675 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-05-03 19:07:58.993503 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-05-03 19:07:58.991266 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-05-03 19:07:58.995891 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-05-03 19:07:58.995231 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-05-03 19:07:58.997175 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-05-03 19:07:58.997793 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-05-03 19:07:58.996384 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-05-03 19:07:58.996637 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-05-03 19:07:58.996923 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-05-03 19:07:58.995497 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-05-03 19:07:58.994931 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-05-03 19:07:58.997459 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-05-03 19:07:58.990879 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-05-03 19:07:58.993140 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-05-03 19:07:58.994272 patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3872 2024-05-03 19:07:58.930033 patent_client-5.0.8/patent_client/_sync/epo/ops/session.py
--rw-r--r--   0        0        0     3129 2024-05-03 19:08:40.996973 patent_client-5.0.8/patent_client/_sync/epo/ops/util.py
--rw-r--r--   0        0        0     3597 2024-05-03 19:07:58.353686 patent_client-5.0.8/patent_client/_sync/http_client.py
--rw-r--r--   0        0        0      616 2024-05-03 19:07:58.357610 patent_client-5.0.8/patent_client/_sync/odp.py
--rw-r--r--   0        0        0      416 2024-05-03 19:07:58.357943 patent_client-5.0.8/patent_client/_sync/uspto/__init__.py
--rw-r--r--   0        0        0      416 2024-05-03 19:07:58.539892 patent_client-5.0.8/patent_client/_sync/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2922 2024-05-03 19:07:58.553285 patent_client-5.0.8/patent_client/_sync/uspto/assignment/api.py
--rw-r--r--   0        0        0     1256 2024-05-03 19:08:41.010456 patent_client-5.0.8/patent_client/_sync/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     4011 2024-05-03 19:07:58.539673 patent_client-5.0.8/patent_client/_sync/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1565 2024-05-03 19:07:58.556971 patent_client-5.0.8/patent_client/_sync/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-05-03 19:07:58.582002 patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-05-03 19:07:58.582313 patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-05-03 19:07:58.575369 patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-05-03 19:07:58.577461 patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-05-03 19:07:58.575868 patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-05-03 19:07:58.581583 patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3766 2024-05-03 19:08:40.554751 patent_client-5.0.8/patent_client/_sync/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4209 2024-05-03 19:08:40.979619 patent_client-5.0.8/patent_client/_sync/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5904 2024-05-03 19:07:58.548615 patent_client-5.0.8/patent_client/_sync/uspto/assignment/model.py
--rw-r--r--   0        0        0     2348 2024-05-03 19:07:58.534045 patent_client-5.0.8/patent_client/_sync/uspto/assignment/model_test.py
--rw-r--r--   0        0        0      416 2024-05-03 19:07:58.362830 patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3549 2024-05-03 19:07:58.372078 patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1364 2024-05-03 19:08:40.554194 patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     3099 2024-05-03 19:08:40.554401 patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1923 2024-05-03 19:08:40.978695 patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1957 2024-05-03 19:07:58.366144 patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/model.py
--rw-r--r--   0        0        0      416 2024-05-03 19:07:58.793755 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2470 2024-05-03 19:08:40.554873 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1445 2024-05-03 19:08:41.009941 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-05-03 19:07:58.793478 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     2132 2024-05-03 19:07:58.813427 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     7139 2024-05-03 19:08:41.009357 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3741 2024-05-03 19:08:40.553566 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6447 2024-05-03 19:07:58.793091 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5668 2024-05-03 19:07:58.783861 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-05-03 19:07:58.813772 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-05-03 19:07:58.814429 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-05-03 19:07:58.814788 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-05-03 19:07:58.814085 patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0      417 2024-05-03 19:07:58.609359 patent_client-5.0.8/patent_client/_sync/uspto/odp/__init__.py
--rw-r--r--   0        0        0     6449 2024-05-03 19:08:40.554870 patent_client-5.0.8/patent_client/_sync/uspto/odp/api.py
--rw-r--r--   0        0        0     2871 2024-05-03 19:08:40.553326 patent_client-5.0.8/patent_client/_sync/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-05-03 19:07:58.676641 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-05-03 19:07:58.678471 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-05-03 19:07:58.676367 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-05-03 19:07:58.678049 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-05-03 19:07:58.676004 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-05-03 19:07:58.674810 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-05-03 19:07:58.676952 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-05-03 19:07:58.678644 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-05-03 19:07:58.675046 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-05-03 19:07:58.675823 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-05-03 19:07:58.677270 patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     5953 2024-05-03 19:08:40.553979 patent_client-5.0.8/patent_client/_sync/uspto/odp/manager.py
--rw-r--r--   0        0        0     2169 2024-05-03 19:08:40.554477 patent_client-5.0.8/patent_client/_sync/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    20058 2024-05-03 19:08:40.994670 patent_client-5.0.8/patent_client/_sync/uspto/odp/model.py
--rw-r--r--   0        0        0    12993 2024-05-03 19:08:40.555532 patent_client-5.0.8/patent_client/_sync/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2812 2024-05-03 19:07:58.607648 patent_client-5.0.8/patent_client/_sync/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-05-03 19:07:58.608994 patent_client-5.0.8/patent_client/_sync/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      891 2024-05-03 19:07:58.608667 patent_client-5.0.8/patent_client/_sync/uspto/odp/util.py
--rw-r--r--   0        0        0      548 2024-05-03 19:07:58.703873 patent_client-5.0.8/patent_client/_sync/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4838 2024-05-03 19:07:58.734377 patent_client-5.0.8/patent_client/_sync/uspto/peds/api.py
--rw-r--r--   0        0        0      986 2024-05-03 19:08:40.555230 patent_client-5.0.8/patent_client/_sync/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-05-03 19:07:58.769474 patent_client-5.0.8/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0     8619 2024-05-03 19:07:58.769151 patent_client-5.0.8/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8510 2024-05-03 19:07:58.748484 patent_client-5.0.8/patent_client/_sync/uspto/peds/manager.py
--rw-r--r--   0        0        0     9245 2024-05-03 19:08:40.553571 patent_client-5.0.8/patent_client/_sync/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    15280 2024-05-03 19:08:41.007694 patent_client-5.0.8/patent_client/_sync/uspto/peds/model.py
--rw-r--r--   0        0        0     6532 2024-05-03 19:07:58.703074 patent_client-5.0.8/patent_client/_sync/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-05-03 19:07:58.693803 patent_client-5.0.8/patent_client/_sync/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      604 2024-05-03 19:07:58.878526 patent_client-5.0.8/patent_client/_sync/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10513 2024-05-03 19:07:58.905772 patent_client-5.0.8/patent_client/_sync/uspto/ptab/api.py
--rw-r--r--   0        0        0      992 2024-05-03 19:08:40.554956 patent_client-5.0.8/patent_client/_sync/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-05-03 19:07:58.917837 patent_client-5.0.8/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-05-03 19:07:58.918422 patent_client-5.0.8/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2407 2024-05-03 19:07:58.910876 patent_client-5.0.8/patent_client/_sync/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2270 2024-05-03 19:08:40.553535 patent_client-5.0.8/patent_client/_sync/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8786 2024-05-03 19:07:58.891149 patent_client-5.0.8/patent_client/_sync/uspto/ptab/model.py
--rw-r--r--   0        0        0      658 2024-05-03 19:07:58.877731 patent_client-5.0.8/patent_client/_sync/uspto/ptab/util.py
--rw-r--r--   0        0        0      742 2024-05-03 19:07:58.415849 patent_client-5.0.8/patent_client/_sync/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     7172 2024-05-03 19:07:58.426137 patent_client-5.0.8/patent_client/_sync/uspto/public_search/api.py
--rw-r--r--   0        0        0      667 2024-05-03 19:08:40.554193 patent_client-5.0.8/patent_client/_sync/uspto/public_search/api_test.py
--rw-r--r--   0        0        0      416 2024-05-03 19:07:58.509098 patent_client-5.0.8/patent_client/_sync/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2482 2024-05-03 19:07:58.512319 patent_client-5.0.8/patent_client/_sync/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     6964 2024-05-03 19:07:58.524815 patent_client-5.0.8/patent_client/_sync/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     2010 2024-05-03 19:07:58.514724 patent_client-5.0.8/patent_client/_sync/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1451 2024-05-03 19:07:58.429228 patent_client-5.0.8/patent_client/_sync/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-05-03 19:07:58.415039 patent_client-5.0.8/patent_client/_sync/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-05-03 19:07:58.503602 patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-05-03 19:07:58.504639 patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-05-03 19:07:58.507554 patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-05-03 19:07:58.507094 patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-05-03 19:08:29.323723 patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-05-03 19:07:58.490240 patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4475 2024-05-03 19:08:40.987691 patent_client-5.0.8/patent_client/_sync/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7113 2024-05-03 19:08:40.553694 patent_client-5.0.8/patent_client/_sync/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      970 2024-05-03 19:07:58.466071 patent_client-5.0.8/patent_client/_sync/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3495 2024-05-03 19:07:58.471151 patent_client-5.0.8/patent_client/_sync/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7978 2024-05-03 19:07:58.486934 patent_client-5.0.8/patent_client/_sync/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2659 2024-05-03 19:07:58.475001 patent_client-5.0.8/patent_client/_sync/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1951 2024-05-03 19:07:58.399855 patent_client-5.0.8/patent_client/_sync/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4914 2024-05-03 19:07:58.413604 patent_client-5.0.8/patent_client/_sync/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-05-03 19:07:58.384665 patent_client-5.0.8/patent_client/_sync/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4472 2024-05-03 19:07:58.406643 patent_client-5.0.8/patent_client/_sync/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-05-03 19:07:58.436433 patent_client-5.0.8/patent_client/_sync/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      689 2024-05-03 19:07:58.414522 patent_client-5.0.8/patent_client/_sync/uspto/public_search/util.py
--rw-r--r--   0        0        0      121 2024-05-03 17:27:31.159772 patent_client-5.0.8/patent_client/odp.py
--rw-r--r--   0        0        0     6027 2024-05-03 17:25:00.874498 patent_client-5.0.8/patent_client/parser.py
--rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.8/patent_client/patches.py
--rw-r--r--   0        0        0     3262 2024-05-03 17:25:00.874850 patent_client-5.0.8/patent_client/session.py
--rw-r--r--   0        0        0      685 2024-05-01 18:05:48.010111 patent_client-5.0.8/patent_client/settings.py
--rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.8/patent_client/test_parser.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.8/patent_client/util/__init__.py
--rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.8/patent_client/util/asyncio_util.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.8/patent_client/util/claims/__init__.py
--rw-r--r--   0        0        0     4313 2024-05-03 19:08:30.230688 patent_client-5.0.8/patent_client/util/claims/examples/multiple_dependent.json
--rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.8/patent_client/util/claims/examples/multiple_dependent.txt
--rw-r--r--   0        0        0     6924 2024-05-03 19:08:30.233717 patent_client-5.0.8/patent_client/util/claims/examples/published_claims.json
--rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.8/patent_client/util/claims/examples/published_claims.txt
--rw-r--r--   0        0        0      735 2024-05-02 17:06:23.356360 patent_client-5.0.8/patent_client/util/claims/model.py
--rw-r--r--   0        0        0     3522 2024-05-03 17:25:00.875271 patent_client-5.0.8/patent_client/util/claims/parser.py
--rw-r--r--   0        0        0      939 2024-05-01 18:05:48.010826 patent_client-5.0.8/patent_client/util/claims/parser_test.py
--rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.8/patent_client/util/format.py
--rw-r--r--   0        0        0     9700 2024-05-03 17:25:00.875510 patent_client-5.0.8/patent_client/util/manager.py
--rw-r--r--   0        0        0     3062 2024-05-03 17:25:00.875751 patent_client-5.0.8/patent_client/util/pydantic_util.py
--rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.8/patent_client/util/request_util.py
--rw-r--r--   0        0        0     1233 2024-05-03 17:25:00.876102 patent_client-5.0.8/patent_client/util/test.py
--rw-r--r--   0        0        0       22 2024-05-03 19:08:51.818528 patent_client-5.0.8/patent_client/version.py
--rw-r--r--   0        0        0     3407 2024-05-03 19:08:51.819109 patent_client-5.0.8/pyproject.toml
--rw-r--r--   0        0        0     7880 1970-01-01 00:00:00.000000 patent_client-5.0.8/PKG-INFO
+-rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.9/LICENSE
+-rw-r--r--   0        0        0     6283 2024-05-02 17:06:23.093538 patent_client-5.0.9/README.md
+-rw-r--r--   0        0        0     1739 2024-05-03 17:25:00.646245 patent_client-5.0.9/patent_client/__init__.py
+-rw-r--r--   0        0        0      833 2024-05-02 17:06:23.121290 patent_client-5.0.9/patent_client/_async/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.9/patent_client/_async/epo/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-01 18:05:47.951425 patent_client-5.0.9/patent_client/_async/epo/ops/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.9/patent_client/_async/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-03 17:25:00.646675 patent_client-5.0.9/patent_client/_async/epo/ops/family/api.py
+-rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.9/patent_client/_async/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.9/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.9/patent_client/_async/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.9/patent_client/_async/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.9/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      356 2024-05-03 17:25:00.646963 patent_client-5.0.9/patent_client/_async/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1119 2024-05-01 18:05:47.952437 patent_client-5.0.9/patent_client/_async/epo/ops/family/model.py
+-rw-r--r--   0        0        0      519 2024-05-01 18:05:47.952767 patent_client-5.0.9/patent_client/_async/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1503 2024-05-03 17:25:00.647248 patent_client-5.0.9/patent_client/_async/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      527 2024-05-01 18:05:47.953647 patent_client-5.0.9/patent_client/_async/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.9/patent_client/_async/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-02 17:06:23.121738 patent_client-5.0.9/patent_client/_async/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.9/patent_client/_async/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      467 2024-05-03 17:25:00.653744 patent_client-5.0.9/patent_client/_async/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2375 2024-05-01 18:05:47.954191 patent_client-5.0.9/patent_client/_async/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5434 2024-05-03 17:25:00.657228 patent_client-5.0.9/patent_client/_async/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.9/patent_client/_async/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4018 2024-05-03 17:25:00.661652 patent_client-5.0.9/patent_client/_async/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1216 2024-05-01 18:05:47.954968 patent_client-5.0.9/patent_client/_async/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.9/patent_client/_async/epo/ops/legal/util.py
+-rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.9/patent_client/_async/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1415 2024-05-02 17:06:23.125551 patent_client-5.0.9/patent_client/_async/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     1806 2024-05-01 18:05:47.955307 patent_client-5.0.9/patent_client/_async/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1117 2024-05-01 18:05:47.955516 patent_client-5.0.9/patent_client/_async/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.9/patent_client/_async/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.9/patent_client/_async/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0      763 2024-05-01 18:05:47.955715 patent_client-5.0.9/patent_client/_async/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0      952 2024-05-01 18:05:47.955921 patent_client-5.0.9/patent_client/_async/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.9/patent_client/_async/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5472 2024-05-03 17:25:00.661893 patent_client-5.0.9/patent_client/_async/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2699 2024-05-03 17:25:00.662175 patent_client-5.0.9/patent_client/_async/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.9/patent_client/_async/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-03 19:08:07.224593 patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-03 19:08:07.228235 patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18516 2024-05-03 19:08:07.239602 patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3204 2024-05-03 17:25:00.662696 patent_client-5.0.9/patent_client/_async/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2411 2024-05-03 17:25:00.662959 patent_client-5.0.9/patent_client/_async/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      321 2024-05-01 18:05:47.957189 patent_client-5.0.9/patent_client/_async/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     2754 2024-05-01 18:05:47.957413 patent_client-5.0.9/patent_client/_async/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1050 2024-05-01 18:05:47.957672 patent_client-5.0.9/patent_client/_async/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2078 2024-05-03 17:25:00.663177 patent_client-5.0.9/patent_client/_async/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0      843 2024-05-01 18:05:47.958081 patent_client-5.0.9/patent_client/_async/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      285 2024-05-01 18:05:47.958344 patent_client-5.0.9/patent_client/_async/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     3934 2024-05-03 17:25:00.663421 patent_client-5.0.9/patent_client/_async/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0      874 2024-05-01 18:05:47.958917 patent_client-5.0.9/patent_client/_async/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     1640 2024-05-03 17:25:00.664113 patent_client-5.0.9/patent_client/_async/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.9/patent_client/_async/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3160 2024-05-03 17:25:00.664661 patent_client-5.0.9/patent_client/_async/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-03 19:08:07.371916 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-03 19:08:07.376377 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.9/patent_client/_async/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3478 2024-05-03 17:25:00.664935 patent_client-5.0.9/patent_client/_async/epo/ops/session.py
+-rw-r--r--   0        0        0     2881 2024-05-03 17:25:00.665195 patent_client-5.0.9/patent_client/_async/epo/ops/util.py
+-rw-r--r--   0        0        0     3220 2024-05-03 17:25:00.665599 patent_client-5.0.9/patent_client/_async/http_client.py
+-rw-r--r--   0        0        0      201 2024-05-02 17:06:23.136948 patent_client-5.0.9/patent_client/_async/odp.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.9/patent_client/_async/uspto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.9/patent_client/_async/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2538 2024-05-03 17:25:00.665812 patent_client-5.0.9/patent_client/_async/uspto/assignment/api.py
+-rw-r--r--   0        0        0      921 2024-05-02 17:06:23.137157 patent_client-5.0.9/patent_client/_async/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     3595 2024-05-03 17:25:00.666143 patent_client-5.0.9/patent_client/_async/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.9/patent_client/_async/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3424 2024-05-03 17:25:00.666449 patent_client-5.0.9/patent_client/_async/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4158 2024-05-03 17:25:00.666715 patent_client-5.0.9/patent_client/_async/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5500 2024-05-03 17:25:00.666971 patent_client-5.0.9/patent_client/_async/uspto/assignment/model.py
+-rw-r--r--   0        0        0     1932 2024-05-01 18:05:47.962761 patent_client-5.0.9/patent_client/_async/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.9/patent_client/_async/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3182 2024-05-03 17:25:00.667431 patent_client-5.0.9/patent_client/_async/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1100 2024-05-01 18:05:47.963236 patent_client-5.0.9/patent_client/_async/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     2781 2024-05-01 18:05:47.963445 patent_client-5.0.9/patent_client/_async/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1707 2024-05-01 18:05:47.963660 patent_client-5.0.9/patent_client/_async/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1553 2024-05-03 17:25:00.667735 patent_client-5.0.9/patent_client/_async/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2109 2024-05-01 18:05:47.964054 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1143 2024-05-01 18:05:47.964243 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     1762 2024-05-03 17:25:00.667994 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     6897 2024-05-03 17:25:00.668558 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3738 2024-05-01 18:05:47.970105 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6031 2024-05-03 17:25:00.668826 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5252 2024-05-01 18:05:47.970651 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.9/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0        1 2024-05-01 18:05:47.970962 patent_client-5.0.9/patent_client/_async/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     6187 2024-05-03 18:56:17.340414 patent_client-5.0.9/patent_client/_async/uspto/odp/api.py
+-rw-r--r--   0        0        0     2818 2024-05-03 17:25:00.669417 patent_client-5.0.9/patent_client/_async/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     5815 2024-05-03 18:56:17.114385 patent_client-5.0.9/patent_client/_async/uspto/odp/manager.py
+-rw-r--r--   0        0        0     2127 2024-05-03 18:56:17.339737 patent_client-5.0.9/patent_client/_async/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    20030 2024-05-03 19:19:32.465419 patent_client-5.0.9/patent_client/_async/uspto/odp/model.py
+-rw-r--r--   0        0        0    12674 2024-05-03 19:20:52.911779 patent_client-5.0.9/patent_client/_async/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2396 2024-05-01 18:05:47.972634 patent_client-5.0.9/patent_client/_async/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.9/patent_client/_async/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      475 2024-05-01 18:05:47.972937 patent_client-5.0.9/patent_client/_async/uspto/odp/util.py
+-rw-r--r--   0        0        0      132 2024-05-01 18:05:47.973121 patent_client-5.0.9/patent_client/_async/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4501 2024-05-01 18:05:47.973352 patent_client-5.0.9/patent_client/_async/uspto/peds/api.py
+-rw-r--r--   0        0        0      683 2024-05-03 17:25:00.670577 patent_client-5.0.9/patent_client/_async/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.9/patent_client/_async/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8619 2024-05-03 17:25:00.673086 patent_client-5.0.9/patent_client/_async/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8191 2024-05-03 17:25:00.673373 patent_client-5.0.9/patent_client/_async/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9623 2024-05-03 17:25:00.673653 patent_client-5.0.9/patent_client/_async/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    14958 2024-05-03 17:25:00.673984 patent_client-5.0.9/patent_client/_async/uspto/peds/model.py
+-rw-r--r--   0        0        0     6116 2024-05-01 18:05:47.974623 patent_client-5.0.9/patent_client/_async/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.9/patent_client/_async/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      188 2024-05-02 17:06:23.210126 patent_client-5.0.9/patent_client/_async/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10134 2024-05-03 17:25:00.674181 patent_client-5.0.9/patent_client/_async/uspto/ptab/api.py
+-rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.9/patent_client/_async/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.9/patent_client/_async/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.9/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2025 2024-05-03 17:25:00.674454 patent_client-5.0.9/patent_client/_async/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2249 2024-05-03 17:25:00.674630 patent_client-5.0.9/patent_client/_async/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8382 2024-05-03 17:25:00.674990 patent_client-5.0.9/patent_client/_async/uspto/ptab/model.py
+-rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.9/patent_client/_async/uspto/ptab/util.py
+-rw-r--r--   0        0        0      326 2024-05-02 17:06:23.210541 patent_client-5.0.9/patent_client/_async/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     6921 2024-05-03 17:25:00.675209 patent_client-5.0.9/patent_client/_async/uspto/public_search/api.py
+-rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.9/patent_client/_async/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.9/patent_client/_async/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2066 2024-05-01 18:05:47.981591 patent_client-5.0.9/patent_client/_async/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     6548 2024-05-03 17:25:00.680068 patent_client-5.0.9/patent_client/_async/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     1594 2024-05-01 18:05:47.983719 patent_client-5.0.9/patent_client/_async/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1035 2024-05-02 17:06:23.211161 patent_client-5.0.9/patent_client/_async/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.9/patent_client/_async/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-03 19:08:09.632336 patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4132 2024-05-03 17:25:00.680395 patent_client-5.0.9/patent_client/_async/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7627 2024-05-03 17:25:00.680977 patent_client-5.0.9/patent_client/_async/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      554 2024-05-03 17:25:00.681546 patent_client-5.0.9/patent_client/_async/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3091 2024-05-03 17:25:00.681713 patent_client-5.0.9/patent_client/_async/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7574 2024-05-03 17:25:00.681893 patent_client-5.0.9/patent_client/_async/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2243 2024-05-03 17:25:00.682051 patent_client-5.0.9/patent_client/_async/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1535 2024-05-02 17:06:23.211470 patent_client-5.0.9/patent_client/_async/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4498 2024-05-03 17:25:00.682225 patent_client-5.0.9/patent_client/_async/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.9/patent_client/_async/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4056 2024-05-03 17:25:00.682391 patent_client-5.0.9/patent_client/_async/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.9/patent_client/_async/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.9/patent_client/_async/uspto/public_search/util.py
+-rw-r--r--   0        0        0     1249 2024-05-03 19:07:58.356029 patent_client-5.0.9/patent_client/_sync/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-03 19:07:58.918971 patent_client-5.0.9/patent_client/_sync/epo/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-03 19:07:58.930646 patent_client-5.0.9/patent_client/_sync/epo/ops/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-03 19:07:58.947993 patent_client-5.0.9/patent_client/_sync/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-03 19:07:58.951037 patent_client-5.0.9/patent_client/_sync/epo/ops/family/api.py
+-rw-r--r--   0        0        0      839 2024-05-03 19:08:41.001990 patent_client-5.0.9/patent_client/_sync/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-05-03 19:07:58.958136 patent_client-5.0.9/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-05-03 19:07:58.958426 patent_client-5.0.9/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-05-03 19:07:58.959117 patent_client-5.0.9/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-05-03 19:07:58.958758 patent_client-5.0.9/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      750 2024-05-03 19:07:58.953267 patent_client-5.0.9/patent_client/_sync/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1535 2024-05-03 19:07:58.950132 patent_client-5.0.9/patent_client/_sync/epo/ops/family/model.py
+-rw-r--r--   0        0        0      887 2024-05-03 19:08:40.986449 patent_client-5.0.9/patent_client/_sync/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1919 2024-05-03 19:07:58.955892 patent_client-5.0.9/patent_client/_sync/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      943 2024-05-03 19:07:58.947829 patent_client-5.0.9/patent_client/_sync/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0      416 2024-05-03 19:07:59.048390 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-03 19:07:59.053311 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      688 2024-05-03 19:08:41.003907 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-05-03 19:07:59.083882 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-05-03 19:07:59.082163 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-05-03 19:07:59.083495 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-05-03 19:07:59.082496 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-05-03 19:07:59.082754 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-05-03 19:07:59.083096 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-05-03 19:07:59.081053 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      847 2024-05-03 19:08:40.554626 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2791 2024-05-03 19:07:59.052457 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5767 2024-05-03 19:08:40.531684 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      866 2024-05-03 19:08:41.005042 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4434 2024-05-03 19:07:59.070800 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1632 2024-05-03 19:07:59.047514 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      530 2024-05-03 19:07:59.047999 patent_client-5.0.9/patent_client/_sync/epo/ops/legal/util.py
+-rw-r--r--   0        0        0      483 2024-05-03 19:07:58.931519 patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1819 2024-05-03 19:07:58.935606 patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     2023 2024-05-03 19:08:40.553863 patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1533 2024-05-03 19:07:58.938020 patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-05-03 19:07:58.930953 patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-05-03 19:07:58.935754 patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0     1179 2024-05-03 19:07:58.933183 patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0     1368 2024-05-03 19:07:58.943318 patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0      416 2024-05-03 19:07:58.969025 patent_client-5.0.9/patent_client/_sync/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5742 2024-05-03 19:08:40.554760 patent_client-5.0.9/patent_client/_sync/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2878 2024-05-03 19:08:40.995502 patent_client-5.0.9/patent_client/_sync/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1917 2024-05-03 19:07:58.971495 patent_client-5.0.9/patent_client/_sync/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-05-03 19:07:59.043721 patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-03 19:08:26.915184 patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-05-03 19:07:59.042807 patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-05-03 19:07:59.043133 patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-03 19:08:26.918533 patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18516 2024-05-03 19:08:26.929284 patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3494 2024-05-03 19:07:58.990416 patent_client-5.0.9/patent_client/_sync/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2383 2024-05-03 19:08:40.554169 patent_client-5.0.9/patent_client/_sync/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      737 2024-05-03 19:07:59.029642 patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     3170 2024-05-03 19:07:59.034326 patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1466 2024-05-03 19:07:59.042057 patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2470 2024-05-03 19:07:59.038161 patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0     1259 2024-05-03 19:07:59.039904 patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      701 2024-05-03 19:07:59.015580 patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     4350 2024-05-03 19:07:59.022076 patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0     1290 2024-05-03 19:07:59.028646 patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     2056 2024-05-03 19:07:59.025156 patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0     1066 2024-05-03 19:07:59.026537 patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3576 2024-05-03 19:07:58.968746 patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-05-03 19:07:58.991870 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-05-03 19:07:58.992900 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-05-03 19:07:58.992607 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-05-03 19:07:58.992166 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-03 19:08:27.058853 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-05-03 19:07:58.994509 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-03 19:08:27.062675 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-05-03 19:07:58.993503 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-05-03 19:07:58.991266 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-05-03 19:07:58.995891 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-05-03 19:07:58.995231 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-05-03 19:07:58.997175 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-05-03 19:07:58.997793 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-05-03 19:07:58.996384 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-05-03 19:07:58.996637 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-05-03 19:07:58.996923 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-05-03 19:07:58.995497 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-05-03 19:07:58.994931 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-05-03 19:07:58.997459 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-05-03 19:07:58.990879 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-05-03 19:07:58.993140 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-05-03 19:07:58.994272 patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3872 2024-05-03 19:07:58.930033 patent_client-5.0.9/patent_client/_sync/epo/ops/session.py
+-rw-r--r--   0        0        0     3129 2024-05-03 19:08:40.996973 patent_client-5.0.9/patent_client/_sync/epo/ops/util.py
+-rw-r--r--   0        0        0     3597 2024-05-03 19:07:58.353686 patent_client-5.0.9/patent_client/_sync/http_client.py
+-rw-r--r--   0        0        0      616 2024-05-03 19:07:58.357610 patent_client-5.0.9/patent_client/_sync/odp.py
+-rw-r--r--   0        0        0      416 2024-05-03 19:07:58.357943 patent_client-5.0.9/patent_client/_sync/uspto/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-03 19:07:58.539892 patent_client-5.0.9/patent_client/_sync/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2922 2024-05-03 19:07:58.553285 patent_client-5.0.9/patent_client/_sync/uspto/assignment/api.py
+-rw-r--r--   0        0        0     1256 2024-05-03 19:08:41.010456 patent_client-5.0.9/patent_client/_sync/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     4011 2024-05-03 19:07:58.539673 patent_client-5.0.9/patent_client/_sync/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1565 2024-05-03 19:07:58.556971 patent_client-5.0.9/patent_client/_sync/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-05-03 19:07:58.582002 patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-05-03 19:07:58.582313 patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-05-03 19:07:58.575369 patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-05-03 19:07:58.577461 patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-05-03 19:07:58.575868 patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-05-03 19:07:58.581583 patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3766 2024-05-03 19:08:40.554751 patent_client-5.0.9/patent_client/_sync/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4209 2024-05-03 19:08:40.979619 patent_client-5.0.9/patent_client/_sync/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5904 2024-05-03 19:07:58.548615 patent_client-5.0.9/patent_client/_sync/uspto/assignment/model.py
+-rw-r--r--   0        0        0     2348 2024-05-03 19:07:58.534045 patent_client-5.0.9/patent_client/_sync/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0      416 2024-05-03 19:07:58.362830 patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3549 2024-05-03 19:07:58.372078 patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1364 2024-05-03 19:08:40.554194 patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     3099 2024-05-03 19:08:40.554401 patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1923 2024-05-03 19:08:40.978695 patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1957 2024-05-03 19:07:58.366144 patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0      416 2024-05-03 19:07:58.793755 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2470 2024-05-03 19:08:40.554873 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1445 2024-05-03 19:08:41.009941 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-05-03 19:07:58.793478 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     2132 2024-05-03 19:07:58.813427 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     7139 2024-05-03 19:08:41.009357 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3741 2024-05-03 19:08:40.553566 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6447 2024-05-03 19:07:58.793091 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5668 2024-05-03 19:07:58.783861 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-05-03 19:07:58.813772 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-05-03 19:07:58.814429 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-05-03 19:07:58.814788 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-05-03 19:07:58.814085 patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0      417 2024-05-03 19:07:58.609359 patent_client-5.0.9/patent_client/_sync/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     6449 2024-05-03 19:08:40.554870 patent_client-5.0.9/patent_client/_sync/uspto/odp/api.py
+-rw-r--r--   0        0        0     2871 2024-05-03 19:08:40.553326 patent_client-5.0.9/patent_client/_sync/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-05-03 19:07:58.676641 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-05-03 19:07:58.678471 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-05-03 19:07:58.676367 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-05-03 19:07:58.678049 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-05-03 19:07:58.676004 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-05-03 19:07:58.674810 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-05-03 19:07:58.676952 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-05-03 19:07:58.678644 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-05-03 19:07:58.675046 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-05-03 19:07:58.675823 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-05-03 19:07:58.677270 patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     5953 2024-05-03 19:08:40.553979 patent_client-5.0.9/patent_client/_sync/uspto/odp/manager.py
+-rw-r--r--   0        0        0     2169 2024-05-03 19:08:40.554477 patent_client-5.0.9/patent_client/_sync/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    20058 2024-05-03 19:08:40.994670 patent_client-5.0.9/patent_client/_sync/uspto/odp/model.py
+-rw-r--r--   0        0        0    12993 2024-05-03 19:08:40.555532 patent_client-5.0.9/patent_client/_sync/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2812 2024-05-03 19:07:58.607648 patent_client-5.0.9/patent_client/_sync/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-05-03 19:07:58.608994 patent_client-5.0.9/patent_client/_sync/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      891 2024-05-03 19:07:58.608667 patent_client-5.0.9/patent_client/_sync/uspto/odp/util.py
+-rw-r--r--   0        0        0      548 2024-05-03 19:07:58.703873 patent_client-5.0.9/patent_client/_sync/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4838 2024-05-03 19:07:58.734377 patent_client-5.0.9/patent_client/_sync/uspto/peds/api.py
+-rw-r--r--   0        0        0      986 2024-05-03 19:08:40.555230 patent_client-5.0.9/patent_client/_sync/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-05-03 19:07:58.769474 patent_client-5.0.9/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8619 2024-05-03 19:07:58.769151 patent_client-5.0.9/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8510 2024-05-03 19:07:58.748484 patent_client-5.0.9/patent_client/_sync/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9245 2024-05-03 19:08:40.553571 patent_client-5.0.9/patent_client/_sync/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    15280 2024-05-03 19:08:41.007694 patent_client-5.0.9/patent_client/_sync/uspto/peds/model.py
+-rw-r--r--   0        0        0     6532 2024-05-03 19:07:58.703074 patent_client-5.0.9/patent_client/_sync/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-05-03 19:07:58.693803 patent_client-5.0.9/patent_client/_sync/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      604 2024-05-03 19:07:58.878526 patent_client-5.0.9/patent_client/_sync/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10513 2024-05-03 19:07:58.905772 patent_client-5.0.9/patent_client/_sync/uspto/ptab/api.py
+-rw-r--r--   0        0        0      992 2024-05-03 19:08:40.554956 patent_client-5.0.9/patent_client/_sync/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-05-03 19:07:58.917837 patent_client-5.0.9/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-05-03 19:07:58.918422 patent_client-5.0.9/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2407 2024-05-03 19:07:58.910876 patent_client-5.0.9/patent_client/_sync/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2270 2024-05-03 19:08:40.553535 patent_client-5.0.9/patent_client/_sync/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8786 2024-05-03 19:07:58.891149 patent_client-5.0.9/patent_client/_sync/uspto/ptab/model.py
+-rw-r--r--   0        0        0      658 2024-05-03 19:07:58.877731 patent_client-5.0.9/patent_client/_sync/uspto/ptab/util.py
+-rw-r--r--   0        0        0      742 2024-05-03 19:07:58.415849 patent_client-5.0.9/patent_client/_sync/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     7172 2024-05-03 19:07:58.426137 patent_client-5.0.9/patent_client/_sync/uspto/public_search/api.py
+-rw-r--r--   0        0        0      667 2024-05-03 19:08:40.554193 patent_client-5.0.9/patent_client/_sync/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0      416 2024-05-03 19:07:58.509098 patent_client-5.0.9/patent_client/_sync/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2482 2024-05-03 19:07:58.512319 patent_client-5.0.9/patent_client/_sync/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     6964 2024-05-03 19:07:58.524815 patent_client-5.0.9/patent_client/_sync/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     2010 2024-05-03 19:07:58.514724 patent_client-5.0.9/patent_client/_sync/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1451 2024-05-03 19:07:58.429228 patent_client-5.0.9/patent_client/_sync/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-05-03 19:07:58.415039 patent_client-5.0.9/patent_client/_sync/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-05-03 19:07:58.503602 patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-05-03 19:07:58.504639 patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-05-03 19:07:58.507554 patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-05-03 19:07:58.507094 patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-03 19:08:29.323723 patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-05-03 19:07:58.490240 patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4475 2024-05-03 19:08:40.987691 patent_client-5.0.9/patent_client/_sync/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7113 2024-05-03 19:08:40.553694 patent_client-5.0.9/patent_client/_sync/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      970 2024-05-03 19:07:58.466071 patent_client-5.0.9/patent_client/_sync/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3495 2024-05-03 19:07:58.471151 patent_client-5.0.9/patent_client/_sync/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7978 2024-05-03 19:07:58.486934 patent_client-5.0.9/patent_client/_sync/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2659 2024-05-03 19:07:58.475001 patent_client-5.0.9/patent_client/_sync/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1951 2024-05-03 19:07:58.399855 patent_client-5.0.9/patent_client/_sync/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4914 2024-05-03 19:07:58.413604 patent_client-5.0.9/patent_client/_sync/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-05-03 19:07:58.384665 patent_client-5.0.9/patent_client/_sync/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4472 2024-05-03 19:07:58.406643 patent_client-5.0.9/patent_client/_sync/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-05-03 19:07:58.436433 patent_client-5.0.9/patent_client/_sync/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      689 2024-05-03 19:07:58.414522 patent_client-5.0.9/patent_client/_sync/uspto/public_search/util.py
+-rw-r--r--   0        0        0      121 2024-05-03 17:27:31.159772 patent_client-5.0.9/patent_client/odp.py
+-rw-r--r--   0        0        0     6027 2024-05-03 17:25:00.874498 patent_client-5.0.9/patent_client/parser.py
+-rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.9/patent_client/patches.py
+-rw-r--r--   0        0        0     3262 2024-05-03 17:25:00.874850 patent_client-5.0.9/patent_client/session.py
+-rw-r--r--   0        0        0      685 2024-05-01 18:05:48.010111 patent_client-5.0.9/patent_client/settings.py
+-rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.9/patent_client/test_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.9/patent_client/util/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.9/patent_client/util/asyncio_util.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.9/patent_client/util/claims/__init__.py
+-rw-r--r--   0        0        0     4313 2024-05-03 19:08:30.230688 patent_client-5.0.9/patent_client/util/claims/examples/multiple_dependent.json
+-rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.9/patent_client/util/claims/examples/multiple_dependent.txt
+-rw-r--r--   0        0        0     6924 2024-05-03 19:08:30.233717 patent_client-5.0.9/patent_client/util/claims/examples/published_claims.json
+-rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.9/patent_client/util/claims/examples/published_claims.txt
+-rw-r--r--   0        0        0      735 2024-05-02 17:06:23.356360 patent_client-5.0.9/patent_client/util/claims/model.py
+-rw-r--r--   0        0        0     3522 2024-05-03 17:25:00.875271 patent_client-5.0.9/patent_client/util/claims/parser.py
+-rw-r--r--   0        0        0      939 2024-05-01 18:05:48.010826 patent_client-5.0.9/patent_client/util/claims/parser_test.py
+-rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.9/patent_client/util/format.py
+-rw-r--r--   0        0        0     9700 2024-05-03 17:25:00.875510 patent_client-5.0.9/patent_client/util/manager.py
+-rw-r--r--   0        0        0     3062 2024-05-03 17:25:00.875751 patent_client-5.0.9/patent_client/util/pydantic_util.py
+-rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.9/patent_client/util/request_util.py
+-rw-r--r--   0        0        0     1233 2024-05-03 17:25:00.876102 patent_client-5.0.9/patent_client/util/test.py
+-rw-r--r--   0        0        0       22 2024-05-03 19:21:03.879182 patent_client-5.0.9/patent_client/version.py
+-rw-r--r--   0        0        0     3407 2024-05-03 19:21:03.879515 patent_client-5.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7880 1970-01-01 00:00:00.000000 patent_client-5.0.9/PKG-INFO
```

### Comparing `patent_client-5.0.8/LICENSE` & `patent_client-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/README.md` & `patent_client-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/__init__.py` & `patent_client-5.0.9/patent_client/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/__init__.py` & `patent_client-5.0.9/patent_client/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/family/model.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/family/model_test.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/family/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/family/schema.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/family/schema_test.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/model.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/national_codes.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/national_codes.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/schema.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/legal/schema_test.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/number_service/api.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/number_service/api_test.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/number_service/errors.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/number_service/errors.txt` & `patent_client-5.0.9/patent_client/_async/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/number_service/messages.txt` & `patent_client-5.0.9/patent_client/_async/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/number_service/model.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/number_service/schema.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/api.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/api_test.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/cql.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/fixtures/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/manager.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/manager_test.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/model/biblio.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/model/fulltext.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/model/images.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/model/search.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/schema/biblio.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/schema/images.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/schema/search.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/schema_test.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/claims_example.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/description_example.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/image_example.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/published/test/search_example.xml` & `patent_client-5.0.9/patent_client/_async/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/session.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/epo/ops/util.py` & `patent_client-5.0.9/patent_client/_async/epo/ops/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/http_client.py` & `patent_client-5.0.9/patent_client/_async/http_client.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/api.py` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/api_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/convert.py` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/convert.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/convert_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/manager.py` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/manager_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/model.py` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/assignment/model_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/bulk_data/api.py` & `patent_client-5.0.9/patent_client/_async/uspto/bulk_data/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/bulk_data/api_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/bulk_data/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/bulk_data/manager.py` & `patent_client-5.0.9/patent_client/_async/uspto/bulk_data/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/bulk_data/manager_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/bulk_data/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/bulk_data/model.py` & `patent_client-5.0.9/patent_client/_async/uspto/bulk_data/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/api.py` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/api_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/manager.py` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/model.py` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/model_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/query.py` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/query_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/test/app.json` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.9/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/api.py` & `patent_client-5.0.9/patent_client/_async/uspto/odp/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/api_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/odp/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/application.json` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/documents.json` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/search.json` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.9/patent_client/_async/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/manager.py` & `patent_client-5.0.9/patent_client/_async/uspto/odp/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/manager_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/odp/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/model.py` & `patent_client-5.0.9/patent_client/_async/uspto/odp/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,15 @@
     atty_docket_num: Optional[str] = Field(alias="docketNumber", default=None)
     appl_id: Optional[str] = Field(alias="applicationNumberText", default=None)
     first_inventor_name: Optional[str] = Field(alias="firstInventorName", default=None)
     first_applicant_name: Optional[str] = Field(alias="firstApplicantName", default=None)
     cpc_classifications: list[str] = Field(alias="cpcClassificationBag", default_factory=list)
     entity_status: Optional[str] = Field(alias="businessEntityStatusCategory", default=None)
     app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber", default=None)
+    patent_number: Optional[str] = Field(alias="patentNumber", default=None)
     status: Optional[str] = Field(alias="applicationStatusDescriptionText", default=None)
     status_date: Optional[datetime.date] = Field(alias="applicationStatusDate", default=None)
     status_code: Optional[int] = Field(alias="applicationStatusCode", default=None)
 
     @async_property
     async def bibliographic_data(self) -> "USApplicationBiblio":
         return await self._get_model(".model.USApplicationBiblio").objects.get(appl_id=self.appl_id)
@@ -335,14 +336,15 @@
     atty_docket_num: Optional[str] = Field(alias="docketNumber", default=None)
     appl_id: Optional[str] = Field(alias="applicationNumberText", default=None)
     first_inventor_name: Optional[str] = Field(alias="firstInventorName", default=None)
     first_applicant_name: Optional[str] = Field(alias="firstApplicantName", default=None)
     cpc_classifications: list[str] = Field(alias="cpcClassificationBag", default_factory=list)
     entity_status: Optional[str] = Field(alias="businessEntityStatusCategory", default=None)
     app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber", default=None)
+    patent_number: Optional[str] = Field(alias="patentNumber", default=None)
 
     app_type_code: Optional[str] = Field(alias="applicationTypeCode", default=None)
     national_stage_indicator: Optional[YNBool] = Field(alias="nationalStageIndicator", default=None)
 
     status: Optional[str] = Field(alias="applicationStatusDescriptionText", default=None)
     status_date: Optional[datetime.date] = Field(alias="applicationStatusDate", default=None)
     status_code: Optional[int] = Field(alias="applicationStatusCode", default=None)
```

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/model_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/odp/model_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,15 @@
     assert application_biblio.first_inventor_name == "Marvin Wang"
     assert application_biblio.first_applicant_name == "The General Hospital Corporation"
     assert len(application_biblio.cpc_classifications) > 0
     assert application_biblio.entity_status == "Small"
     assert application_biblio.status == "Abandoned  --  Failure to Respond to an Office Action"
     assert application_biblio.status_date == datetime.date.fromisoformat("2018-10-02")
     assert application_biblio.status_code is None
+    assert application_biblio.patent_number is None
 
 
 def test_application_object(fixture_dir):
     data = json.loads((fixture_dir / "application.json").read_text())
     application_data = data["patentBag"][0]
     application = USApplication(**application_data)
 
@@ -237,14 +238,15 @@
     assert len(application.attorneys.attorneys) > 0
     assert len(application.transactions) > 0
     assert len(application.parent_applications) > 0
     assert len(application.child_applications) > 0
     assert application.status == "Abandoned  --  Failure to Respond to an Office Action"
     assert application.status_date == datetime.date.fromisoformat("2018-10-02")
     assert application.status_code == 161
+    assert application.patent_number is None
 
 
 def test_search_model():
     model = SearchRequest(rangeFilters=[{"field": "filingDate"}])
     assert model.rangeFilters[0].field == "filingDate"
     assert model.rangeFilters[0].valueFrom == "1776-07-04"
     assert model.rangeFilters[0].valueTo == datetime.date.today().isoformat()
```

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/query.py` & `patent_client-5.0.9/patent_client/_async/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/odp/query_fields.csv` & `patent_client-5.0.9/patent_client/_async/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/peds/api.py` & `patent_client-5.0.9/patent_client/_async/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/peds/api_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/peds/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.9/patent_client/_async/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/peds/fixtures/app_1_output.json` & `patent_client-5.0.9/patent_client/_async/uspto/peds/fixtures/app_1_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/peds/manager.py` & `patent_client-5.0.9/patent_client/_async/uspto/peds/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/peds/manager_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/peds/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/peds/model.py` & `patent_client-5.0.9/patent_client/_async/uspto/peds/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/peds/query.py` & `patent_client-5.0.9/patent_client/_async/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/peds/search_index.csv` & `patent_client-5.0.9/patent_client/_async/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/ptab/api.py` & `patent_client-5.0.9/patent_client/_async/uspto/ptab/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/ptab/api_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/ptab/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.9/patent_client/_async/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.9/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/ptab/manager.py` & `patent_client-5.0.9/patent_client/_async/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/ptab/manager_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/ptab/model.py` & `patent_client-5.0.9/patent_client/_async/uspto/ptab/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/api.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/convert/biblio.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/convert/document.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/convert/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/convert/shared.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/convert_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/count_query.json` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/manager.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/manager_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/model/__init__.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/model/biblio.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/model/document.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/model/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/model/shared.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/model/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/model_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/query.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/query_config.csv` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/query_test.py` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_async/uspto/public_search/search_query.json` & `patent_client-5.0.9/patent_client/_async/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/__init__.py` & `patent_client-5.0.9/patent_client/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/__init__.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/api.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/api_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/manager.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/model.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/model_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/schema.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/family/schema_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/api.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/api_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/manager.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/model.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/national_codes.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/national_codes.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/national_codes_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/national_codes_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/schema.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/schema_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/legal/util.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/legal/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/api.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/api_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/errors.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/errors.txt` & `patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/messages.txt` & `patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/model.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/number_service/schema.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/api.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/api_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/cql.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/fixtures/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/manager.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/manager_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/__init__.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/biblio.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/fulltext.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/images.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/model/search.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/__init__.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/biblio.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/images.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema/search.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/schema_test.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/claims_example.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/description_example.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/image_example.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/published/test/search_example.xml` & `patent_client-5.0.9/patent_client/_sync/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/session.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/epo/ops/util.py` & `patent_client-5.0.9/patent_client/_sync/epo/ops/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/http_client.py` & `patent_client-5.0.9/patent_client/_sync/http_client.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/odp.py` & `patent_client-5.0.9/patent_client/_sync/odp.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/api.py` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/api_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/convert.py` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/convert.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/convert_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/manager.py` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/manager_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/model.py` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/assignment/model_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/api.py` & `patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/api_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/manager.py` & `patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/manager_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/bulk_data/model.py` & `patent_client-5.0.9/patent_client/_sync/uspto/bulk_data/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/api.py` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/api_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/manager.py` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/model.py` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/model_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/query.py` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/query_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/test/app.json` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.9/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/api.py` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/api_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/application.json` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/documents.json` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/search.json` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/manager.py` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/manager_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/model.py` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/model_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/query.py` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/query_fields.csv` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/odp/util.py` & `patent_client-5.0.9/patent_client/_sync/uspto/odp/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/__init__.py` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/api.py` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/api_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/fixtures/app_1_output.json` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/fixtures/app_1_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/manager.py` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/manager_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/model.py` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/query.py` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/peds/search_index.csv` & `patent_client-5.0.9/patent_client/_sync/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/ptab/__init__.py` & `patent_client-5.0.9/patent_client/_sync/uspto/ptab/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/ptab/api.py` & `patent_client-5.0.9/patent_client/_sync/uspto/ptab/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/ptab/api_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/ptab/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.9/patent_client/_sync/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.9/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/ptab/manager.py` & `patent_client-5.0.9/patent_client/_sync/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/ptab/manager_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/ptab/model.py` & `patent_client-5.0.9/patent_client/_sync/uspto/ptab/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/ptab/util.py` & `patent_client-5.0.9/patent_client/_sync/uspto/ptab/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/__init__.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/api.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/api_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/convert/biblio.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/convert/document.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/convert/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/convert/shared.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/convert_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/count_query.json` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/manager.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/manager_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/model/__init__.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/model/biblio.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/model/document.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/model/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/model/shared.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/model/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/model_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/query.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/query_config.csv` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/query_test.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/search_query.json` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/_sync/uspto/public_search/util.py` & `patent_client-5.0.9/patent_client/_sync/uspto/public_search/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/parser.py` & `patent_client-5.0.9/patent_client/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/session.py` & `patent_client-5.0.9/patent_client/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/settings.py` & `patent_client-5.0.9/patent_client/settings.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/test_parser.py` & `patent_client-5.0.9/patent_client/test_parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/asyncio_util.py` & `patent_client-5.0.9/patent_client/util/asyncio_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/claims/examples/multiple_dependent.json` & `patent_client-5.0.9/patent_client/util/claims/examples/multiple_dependent.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/claims/examples/multiple_dependent.txt` & `patent_client-5.0.9/patent_client/util/claims/examples/multiple_dependent.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/claims/examples/published_claims.json` & `patent_client-5.0.9/patent_client/util/claims/examples/published_claims.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/claims/examples/published_claims.txt` & `patent_client-5.0.9/patent_client/util/claims/examples/published_claims.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/claims/model.py` & `patent_client-5.0.9/patent_client/util/claims/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/claims/parser.py` & `patent_client-5.0.9/patent_client/util/claims/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/claims/parser_test.py` & `patent_client-5.0.9/patent_client/util/claims/parser_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/format.py` & `patent_client-5.0.9/patent_client/util/format.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/manager.py` & `patent_client-5.0.9/patent_client/util/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/pydantic_util.py` & `patent_client-5.0.9/patent_client/util/pydantic_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/request_util.py` & `patent_client-5.0.9/patent_client/util/request_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/patent_client/util/test.py` & `patent_client-5.0.9/patent_client/util/test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.8/pyproject.toml` & `patent_client-5.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent_client"
-version = "5.0.8"
+version = "5.0.9"
 description = "A set of ORM-style clients for publicly available intellectual property data"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 documentation = "https://patent-client.readthedocs.io"
 homepage = "https://github.com/parkerhancock/patent_client"
 repository = "https://github.com/parkerhancock/patent_client"
```

### Comparing `patent_client-5.0.8/PKG-INFO` & `patent_client-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patent-client
-Version: 5.0.8
+Version: 5.0.9
 Summary: A set of ORM-style clients for publicly available intellectual property data
 Home-page: https://github.com/parkerhancock/patent_client
 License: Apache Software License 2.0
 Keywords: patent,intellectual property,usitc,epo,ops,trademark,inpadoc,337
 Author: Parker Hancock
 Author-email: 633163+parkerhancock@users.noreply.github.com
 Requires-Python: >=3.9,<3.13
```

