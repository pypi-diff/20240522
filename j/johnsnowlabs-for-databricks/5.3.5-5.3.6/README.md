# Comparing `tmp/johnsnowlabs_for_databricks-5.3.5.tar.gz` & `tmp/johnsnowlabs_for_databricks-5.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs_for_databricks-5.3.5.tar", last modified: Fri May 10 22:45:51 2024, max compression
+gzip compressed data, was "johnsnowlabs_for_databricks-5.3.6.tar", last modified: Tue May 21 22:46:27 2024, max compression
```

## Comparing `johnsnowlabs_for_databricks-5.3.5.tar` & `johnsnowlabs_for_databricks-5.3.6.tar`

### file list

```diff
@@ -1,114 +1,216 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.555700 johnsnowlabs_for_databricks-5.3.5/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2024-05-10 21:41:30.000000 johnsnowlabs_for_databricks-5.3.5/LICENSE
--rw-r--r--   0 ckl       (1000) ckl       (1000)     9572 2024-05-10 22:45:51.555700 johnsnowlabs_for_databricks-5.3.5/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8310 2024-05-10 21:41:30.000000 johnsnowlabs_for_databricks-5.3.5/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.547700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1042 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.547700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9326 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.547700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.547700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2680 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    28916 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/endpoints.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    20814 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     7591 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/marketplace.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    21829 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/marketplace_offering.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12197 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.547700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/docker/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/docker/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       84 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/docker/docker_template.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13516 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/docker/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.547700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/emr/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/emr/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      376 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/emr/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11474 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/emr/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1850 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/emr/utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4164 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/emr/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.547700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/glue/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/glue/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2809 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/glue/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3191 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/glue/utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.551700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/benchmark_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6100 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/endpoint_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      690 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/generate_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      832 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      317 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/load_predict_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      908 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2124 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    20668 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11364 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.551700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3192 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/offline_install.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.551700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/snowflake/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/snowflake/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11410 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/snowflake/work_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5673 2024-05-10 22:14:31.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/finance.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.551700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.551700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      547 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    18435 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    14001 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6757 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5614 2024-05-10 22:14:31.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       56 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/llm.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5630 2024-05-10 22:14:31.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1849 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.551700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4945 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    34057 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      121 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/serve.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2935 2024-05-10 22:16:17.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.555700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      997 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/boto_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6668 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4845 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3221 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10596 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4423 2024-05-10 21:52:48.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3109 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/s3_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8495 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.555700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3465 2024-05-10 21:52:48.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:51.555700 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs_for_databricks.egg-info/
--rw-r--r--   0 ckl       (1000) ckl       (1000)     9572 2024-05-10 22:45:51.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs_for_databricks.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3923 2024-05-10 22:45:51.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs_for_databricks.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-10 22:45:51.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs_for_databricks.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2024-05-10 22:45:51.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs_for_databricks.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2024-05-10 22:45:51.000000 johnsnowlabs_for_databricks-5.3.5/johnsnowlabs_for_databricks.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2024-05-10 22:45:51.555700 johnsnowlabs_for_databricks-5.3.5/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2028 2024-05-10 21:41:33.000000 johnsnowlabs_for_databricks-5.3.5/setup_johnsnowlabs_for_databricks.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.168007 johnsnowlabs_for_databricks-5.3.6/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2024-05-17 08:39:14.000000 johnsnowlabs_for_databricks-5.3.6/LICENSE
+-rw-r--r--   0 ckl       (1000) ckl       (1000)     9572 2024-05-21 22:46:27.168007 johnsnowlabs_for_databricks-5.3.6/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8310 2024-05-17 08:39:14.000000 johnsnowlabs_for_databricks-5.3.6/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.152007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1042 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.152007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9326 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2680 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    28916 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/endpoints.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20830 2024-05-21 22:45:10.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     7591 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/marketplace.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    21829 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/marketplace_offering.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12197 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/docker/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/docker/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       84 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/docker/docker_template.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13516 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/docker/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/emr/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/emr/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      376 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/emr/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11474 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/emr/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1850 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/emr/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4164 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/emr/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/glue/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/glue/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2809 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/glue/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3191 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/glue/utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/benchmark_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6100 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/endpoint_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      690 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/generate_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      832 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      317 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/load_predict_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      908 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2124 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20668 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11364 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3192 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/offline_install.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/snowflake/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/snowflake/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11410 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/snowflake/work_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5673 2024-05-21 15:47:39.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/finance.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/embedding_retrieval/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      547 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/embedding_retrieval/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    18435 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    14001 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6757 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/embedding_retrieval/utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.156007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1042 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9326 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2680 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    28916 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/databricks/endpoints.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20814 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     7591 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/databricks/marketplace.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    21829 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/databricks/marketplace_offering.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12197 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/docker/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/docker/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       84 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/docker/docker_template.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13516 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/docker/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/emr/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/emr/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      376 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/emr/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11474 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/emr/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1850 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/emr/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4164 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/emr/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/glue/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/glue/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2809 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/glue/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3191 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/glue/utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/benchmark_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6100 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/endpoint_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      690 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/generate_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      832 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      317 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/load_predict_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      908 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2124 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20668 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11364 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3192 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/offline_install.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/snowflake/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/snowflake/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11410 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/snowflake/work_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5673 2024-05-17 08:34:59.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/finance.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/frameworks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/frameworks/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.160007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/frameworks/embedding_retrieval/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      547 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/frameworks/embedding_retrieval/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    18435 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    14001 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6757 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/frameworks/embedding_retrieval/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5614 2024-05-17 08:34:59.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       56 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/llm.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5630 2024-05-17 08:34:59.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1849 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.164007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4945 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    34057 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      121 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/serve.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2935 2024-05-17 08:34:59.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.164007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      997 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/boto_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6668 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4845 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3221 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10596 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4423 2024-05-17 08:34:59.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3109 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/s3_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8495 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.164007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3465 2024-05-17 08:34:59.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2024-05-17 08:34:35.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/viz.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5614 2024-05-21 15:47:39.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       56 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/llm.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5630 2024-05-21 15:47:39.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1849 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.164007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4945 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    34057 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      121 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/serve.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2951 2024-05-21 22:45:18.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.164007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      997 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/boto_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6668 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4715 2024-05-21 22:45:10.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3221 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10596 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4511 2024-05-21 15:47:39.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3109 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/s3_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8495 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.164007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3465 2024-05-21 15:47:39.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-21 22:46:27.164007 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs_for_databricks.egg-info/
+-rw-r--r--   0 ckl       (1000) ckl       (1000)     9572 2024-05-21 22:46:27.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs_for_databricks.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8669 2024-05-21 22:46:27.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs_for_databricks.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-21 22:46:27.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs_for_databricks.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2024-05-21 22:46:27.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs_for_databricks.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2024-05-21 22:46:27.000000 johnsnowlabs_for_databricks-5.3.6/johnsnowlabs_for_databricks.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2024-05-21 22:46:27.168007 johnsnowlabs_for_databricks-5.3.6/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2028 2024-05-17 08:39:17.000000 johnsnowlabs_for_databricks-5.3.6/setup_johnsnowlabs_for_databricks.py
```

### Comparing `johnsnowlabs_for_databricks-5.3.5/LICENSE` & `johnsnowlabs_for_databricks-5.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/PKG-INFO` & `johnsnowlabs_for_databricks-5.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs_for_databricks
-Version: 5.3.5
+Version: 5.3.6
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spark-nlp==5.3.2
-Requires-Dist: nlu==5.3.1
+Requires-Dist: nlu==5.3.2
 Requires-Dist: spark-nlp-display==5.0
 Requires-Dist: numpy
 Requires-Dist: dataclasses
 Requires-Dist: requests
 Requires-Dist: databricks-api
 Requires-Dist: pydantic==1.10.11
 Requires-Dist: colorama
```

### Comparing `johnsnowlabs_for_databricks-5.3.5/README.md` & `johnsnowlabs_for_databricks-5.3.6/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/__init__.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/endpoints.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/endpoints.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/marketplace.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/marketplace.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/marketplace_offering.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/marketplace_offering.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/docker/work_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/docker/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/emr/install_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/emr/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/emr/utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/emr/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/emr/work_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/emr/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/glue/install_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/glue/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/glue/utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/glue/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/endpoint_test.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/endpoint_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/generate_test.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/generate_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/snowflake/work_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/snowflake/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/finance.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/finance.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/__init__.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/embedding_retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/frameworks/embedding_retrieval/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/legal.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/legal.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/medical.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/medical.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/nlp.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/settings.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/boto_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/boto_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/enums.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/functional.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/py_process.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/s3_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs/visual.py` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.5/johnsnowlabs_for_databricks.egg-info/PKG-INFO` & `johnsnowlabs_for_databricks-5.3.6/johnsnowlabs_for_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs-for-databricks
-Version: 5.3.5
+Version: 5.3.6
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spark-nlp==5.3.2
-Requires-Dist: nlu==5.3.1
+Requires-Dist: nlu==5.3.2
 Requires-Dist: spark-nlp-display==5.0
 Requires-Dist: numpy
 Requires-Dist: dataclasses
 Requires-Dist: requests
 Requires-Dist: databricks-api
 Requires-Dist: pydantic==1.10.11
 Requires-Dist: colorama
```

### Comparing `johnsnowlabs_for_databricks-5.3.5/setup_johnsnowlabs_for_databricks.py` & `johnsnowlabs_for_databricks-5.3.6/setup_johnsnowlabs_for_databricks.py`

 * *Files identical despite different names*

