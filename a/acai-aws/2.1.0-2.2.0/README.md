# Comparing `tmp/acai_aws-2.1.0.tar.gz` & `tmp/acai_aws-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acai_aws-2.1.0.tar", last modified: Thu May  2 01:01:28 2024, max compression
+gzip compressed data, was "acai_aws-2.2.0.tar", last modified: Wed May 22 18:57:13 2024, max compression
```

## Comparing `acai_aws-2.1.0.tar` & `acai_aws-2.2.0.tar`

### file list

```diff
@@ -1,192 +1,207 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.726246 acai_aws-2.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-02 01:01:09.000000 acai_aws-2.1.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3589 2024-05-02 01:01:28.726246 acai_aws-2.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-02 01:01:09.000000 acai_aws-2.1.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.694246 acai_aws-2.1.0/acai_aws/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.694246 acai_aws-2.1.0/acai_aws/apigateway/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1826 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/config_validator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/endpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/exception.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5236 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.694246 acai_aws-2.1.0/acai_aws/apigateway/resolver/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5046 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1117 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3765 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/importer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1782 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3026 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3099 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/mapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2701 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4058 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5305 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/router.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/base/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2729 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/no_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/placeholder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      472 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/record.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      530 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/json_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/common/logger/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/logger/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1974 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/logger/common_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      749 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/logger/decorator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/common/records/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/exception.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/requirements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3524 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/schema.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6486 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/documentdb/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/documentdb/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/documentdb/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2387 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/documentdb/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/documentdb/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/dynamodb/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/dynamodb/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      269 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/dynamodb/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/dynamodb/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/dynamodb/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/firehose/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/firehose/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/firehose/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/firehose/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/firehose/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/generic/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/generic/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/generic/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/generic/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/kinesis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/kinesis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/kinesis/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2141 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/kinesis/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/kinesis/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/mq/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/mq/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/mq/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2415 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/mq/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/mq/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/acai_aws/msk/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/msk/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/msk/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/msk/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/msk/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/acai_aws/s3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/s3/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1398 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/s3/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2326 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/s3/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/s3/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/acai_aws/sns/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sns/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sns/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2629 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sns/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sns/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/acai_aws/sqs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sqs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sqs/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sqs/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sqs/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.726246 acai_aws-2.1.0/acai_aws.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3589 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5245 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2024-05-02 01:01:28.726246 acai_aws-2.1.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1413 2024-05-02 01:01:09.000000 acai_aws-2.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/tests/acai_aws/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/tests/acai_aws/apigateway/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.710246 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.710246 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6532 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_mapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6020 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6695 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_cacher.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4685 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_importer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3277 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_init.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.710246 acai_aws-2.1.0/tests/acai_aws/apigateway/router/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27945 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_directory_router.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23227 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_mapping_router.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23394 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_pattern_router.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2570 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_timeout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5015 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_config_validator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4917 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_endpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9556 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3052 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_requirements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3903 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_response.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.714246 acai_aws-2.1.0/tests/acai_aws/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.714246 acai_aws-2.1.0/tests/acai_aws/common/records/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/records/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/records/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/records/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3637 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/records/test_requirements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/test_json_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4655 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/test_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5662 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/test_schema.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5966 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/test_validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.714246 acai_aws-2.1.0/tests/acai_aws/documentdb/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/documentdb/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5554 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/documentdb/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1417 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/documentdb/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/documentdb/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.714246 acai_aws-2.1.0/tests/acai_aws/dynamodb/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/dynamodb/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7744 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/dynamodb/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2860 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/dynamodb/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1549 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/dynamodb/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.718246 acai_aws-2.1.0/tests/acai_aws/firehose/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/firehose/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5174 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/firehose/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1579 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/firehose/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/firehose/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.718246 acai_aws-2.1.0/tests/acai_aws/generic/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/generic/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/generic/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/generic/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.718246 acai_aws-2.1.0/tests/acai_aws/kinesis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/kinesis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5163 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/kinesis/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/kinesis/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/kinesis/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.718246 acai_aws-2.1.0/tests/acai_aws/mq/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/mq/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5104 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/mq/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1891 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/mq/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      894 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/mq/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.722246 acai_aws-2.1.0/tests/acai_aws/msk/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/msk/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5231 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/msk/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/msk/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      908 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/msk/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.722246 acai_aws-2.1.0/tests/acai_aws/s3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/s3/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6700 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/s3/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2565 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/s3/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1499 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/s3/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.722246 acai_aws-2.1.0/tests/acai_aws/sns/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sns/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sns/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2027 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sns/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      904 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sns/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.722246 acai_aws-2.1.0/tests/acai_aws/sqs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sqs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sqs/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1602 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sqs/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      904 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sqs/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.726246 acai_aws-2.1.0/tests/mocks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/mocks/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.700076 acai_aws-2.2.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-22 18:56:57.000000 acai_aws-2.2.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3652 2024-05-22 18:57:13.700076 acai_aws-2.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2443 2024-05-22 18:56:57.000000 acai_aws-2.2.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.680076 acai_aws-2.2.0/acai_aws/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.684075 acai_aws-2.2.0/acai_aws/apigateway/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1595 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1826 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/config_validator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/endpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/exception.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5236 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.684075 acai_aws-2.2.0/acai_aws/apigateway/resolver/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5046 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/resolver/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1117 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/resolver/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3765 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/resolver/importer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.684075 acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1782 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3026 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3099 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/mapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2701 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4058 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5305 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/apigateway/router.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.684075 acai_aws-2.2.0/acai_aws/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/base/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2729 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/base/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/base/no_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/base/placeholder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      472 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/base/record.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.684075 acai_aws-2.2.0/acai_aws/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      530 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/json_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.684075 acai_aws-2.2.0/acai_aws/common/logger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/logger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1974 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/logger/common_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      749 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/logger/decorator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.684075 acai_aws-2.2.0/acai_aws/common/records/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/records/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/records/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/records/exception.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/records/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/records/requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3524 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/schema.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6486 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/common/validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.684075 acai_aws-2.2.0/acai_aws/documentdb/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/documentdb/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/documentdb/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2387 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/documentdb/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/documentdb/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.688076 acai_aws-2.2.0/acai_aws/dynamodb/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      269 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/dynamodb/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/dynamodb/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/dynamodb/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.688076 acai_aws-2.2.0/acai_aws/firehose/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/firehose/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/firehose/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/firehose/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/firehose/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.688076 acai_aws-2.2.0/acai_aws/generic/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/generic/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/generic/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/generic/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.688076 acai_aws-2.2.0/acai_aws/kinesis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/kinesis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/kinesis/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2141 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/kinesis/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/kinesis/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.688076 acai_aws-2.2.0/acai_aws/mq/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/mq/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/mq/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2415 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/mq/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/mq/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.688076 acai_aws-2.2.0/acai_aws/msk/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/msk/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/msk/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/msk/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/msk/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.688076 acai_aws-2.2.0/acai_aws/s3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/s3/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1398 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/s3/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2326 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/s3/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/s3/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.688076 acai_aws-2.2.0/acai_aws/sns/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/sns/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/sns/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2629 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/sns/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/sns/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.692076 acai_aws-2.2.0/acai_aws/sqs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/sqs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/sqs/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/sqs/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-22 18:56:57.000000 acai_aws-2.2.0/acai_aws/sqs/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.700076 acai_aws-2.2.0/acai_aws.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3652 2024-05-22 18:57:13.000000 acai_aws-2.2.0/acai_aws.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5864 2024-05-22 18:57:13.000000 acai_aws-2.2.0/acai_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-22 18:57:13.000000 acai_aws-2.2.0/acai_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-05-22 18:57:13.000000 acai_aws-2.2.0/acai_aws.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2024-05-22 18:57:13.000000 acai_aws-2.2.0/acai_aws.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2024-05-22 18:57:13.704076 acai_aws-2.2.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1433 2024-05-22 18:56:57.000000 acai_aws-2.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.692076 acai_aws-2.2.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.692076 acai_aws-2.2.0/tests/acai_aws/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.692076 acai_aws-2.2.0/tests/acai_aws/apigateway/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.692076 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.692076 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/handler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/handler/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      510 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/handler/test_importer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3518 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/handler/test_module.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      979 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/handler/test_scanner.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.692076 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/input/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/input/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/input/test_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1474 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/input/test_validator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/test_file_writer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5434 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/openapi/test_generator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.692076 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.692076 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/modes/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/modes/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/modes/test_directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6532 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/modes/test_mapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6020 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/modes/test_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6695 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/test_cacher.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4685 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/test_importer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3277 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/test_init.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.696076 acai_aws-2.2.0/tests/acai_aws/apigateway/router/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/router/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27945 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/router/test_directory_router.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23227 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/router/test_mapping_router.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23394 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/router/test_pattern_router.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2570 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/router/test_timeout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5015 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/test_config_validator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4917 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/test_endpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      821 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/test_main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9556 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/test_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3052 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/test_requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3903 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/apigateway/test_response.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.696076 acai_aws-2.2.0/tests/acai_aws/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.696076 acai_aws-2.2.0/tests/acai_aws/common/records/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/common/records/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/common/records/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/common/records/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3637 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/common/records/test_requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/common/test_json_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4655 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/common/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5662 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/common/test_schema.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5966 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/common/test_validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.696076 acai_aws-2.2.0/tests/acai_aws/documentdb/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/documentdb/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5554 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/documentdb/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1417 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/documentdb/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/documentdb/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.696076 acai_aws-2.2.0/tests/acai_aws/dynamodb/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7744 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/dynamodb/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2860 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/dynamodb/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1549 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/dynamodb/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.696076 acai_aws-2.2.0/tests/acai_aws/firehose/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/firehose/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5174 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/firehose/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1579 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/firehose/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/firehose/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.696076 acai_aws-2.2.0/tests/acai_aws/generic/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/generic/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/generic/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/generic/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.700076 acai_aws-2.2.0/tests/acai_aws/kinesis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/kinesis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5163 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/kinesis/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/kinesis/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/kinesis/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.700076 acai_aws-2.2.0/tests/acai_aws/mq/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/mq/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5104 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/mq/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1891 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/mq/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      894 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/mq/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.700076 acai_aws-2.2.0/tests/acai_aws/msk/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/msk/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5231 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/msk/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/msk/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      908 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/msk/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.700076 acai_aws-2.2.0/tests/acai_aws/s3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/s3/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6700 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/s3/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2565 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/s3/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1499 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/s3/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.700076 acai_aws-2.2.0/tests/acai_aws/sns/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/sns/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/sns/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2027 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/sns/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      904 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/sns/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.700076 acai_aws-2.2.0/tests/acai_aws/sqs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/sqs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/sqs/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1602 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/sqs/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      904 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/acai_aws/sqs/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:57:13.700076 acai_aws-2.2.0/tests/mocks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:56:57.000000 acai_aws-2.2.0/tests/mocks/__init__.py
```

### Comparing `acai_aws-2.1.0/LICENSE` & `acai_aws-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/PKG-INFO` & `acai_aws-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acai_aws
-Version: 2.1.0
+Version: 2.2.0
 Summary: DRY, configurable, opinionated, minimalist framework for use with AWS Serverless Lambdas
 Home-page: https://github.com/syngenta/acai-python.git
 Author: Paul Cruse III
 Author-email: paulcruse3@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -22,27 +22,29 @@
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: dynamodb_json
 Requires-Dist: jsonpickle
 Requires-Dist: jsonref
 Requires-Dist: jsonschema
 Requires-Dist: icecream
+Requires-Dist: pydantic
 Requires-Dist: pyyaml
 Requires-Dist: simplejson
 Requires-Dist: xmltodict
 
 [![CircleCI](https://circleci.com/gh/syngenta/acai-python.svg?style=shield)](https://circleci.com/gh/syngenta/acai-python)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=syngenta_acai-python&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=syngenta_acai-python)
 
 # Acai AWS
 DRY, configurable, declarative node library for working with Amazon Web Service Lambdas.
 
 ## Features
 * Highly configurable apigateway internal router
 * Openapi schema adherence for all event types
+* Generate OpenAPI docs from code base
 * Extensible and customizable middleware for validation and other tasks
 * DRY coding interfaces without the need of boilerplate
 * Ease-of-use with the [serverless framework](https://www.serverless.com/)
 * Local Development support
 * Happy Path Programming (See Philosophy below)
 
 ## Philosophy
```

### Comparing `acai_aws-2.1.0/README.md` & `acai_aws-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # Acai AWS
 DRY, configurable, declarative node library for working with Amazon Web Service Lambdas.
 
 ## Features
 * Highly configurable apigateway internal router
 * Openapi schema adherence for all event types
+* Generate OpenAPI docs from code base
 * Extensible and customizable middleware for validation and other tasks
 * DRY coding interfaces without the need of boilerplate
 * Ease-of-use with the [serverless framework](https://www.serverless.com/)
 * Local Development support
 * Happy Path Programming (See Philosophy below)
 
 ## Philosophy
```

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/config_validator.py` & `acai_aws-2.2.0/acai_aws/apigateway/config_validator.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/endpoint.py` & `acai_aws-2.2.0/acai_aws/apigateway/endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 class Endpoint:
-
     def __init__(self, module, method):
         self.__method = getattr(module, method)
         self.__requirements = getattr(self.__method, 'requirements', {})
 
     @property
     def has_requirements(self):
         return bool(self.__requirements)
 
     @property
     def requirements(self):
         return self.__requirements
 
     @property
     def requires_auth(self):
-        return self.__requirements.get('auth_required', False)
+        return self.__requirements.get('auth_required')
 
     @property
     def has_required_response(self):
-        return self.__requirements.get('required_response', False)
+        return bool(self.__requirements.get('required_response'))
 
     @property
     def has_required_route(self):
         return bool(self.__requirements.get('required_route'))
 
     @property
     def required_route(self):
```

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/exception.py` & `acai_aws-2.2.0/acai_aws/apigateway/exception.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/request.py` & `acai_aws-2.2.0/acai_aws/apigateway/request.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/requirements.py` & `acai_aws-2.2.0/acai_aws/apigateway/requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/resolver/__init__.py` & `acai_aws-2.2.0/acai_aws/apigateway/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/resolver/cache.py` & `acai_aws-2.2.0/acai_aws/apigateway/resolver/cache.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/resolver/importer.py` & `acai_aws-2.2.0/acai_aws/apigateway/resolver/importer.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/base.py` & `acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/base.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/directory.py` & `acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/directory.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/mapping.py` & `acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/mapping.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/pattern.py` & `acai_aws-2.2.0/acai_aws/apigateway/resolver/modes/pattern.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/response.py` & `acai_aws-2.2.0/acai_aws/apigateway/response.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/apigateway/router.py` & `acai_aws-2.2.0/acai_aws/apigateway/router.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/base/event.py` & `acai_aws-2.2.0/acai_aws/base/event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/common/json_helper.py` & `acai_aws-2.2.0/acai_aws/common/json_helper.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/common/logger/common_logger.py` & `acai_aws-2.2.0/acai_aws/common/logger/common_logger.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/common/logger/decorator.py` & `acai_aws-2.2.0/acai_aws/common/logger/decorator.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/common/records/event.py` & `acai_aws-2.2.0/acai_aws/common/records/event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/common/records/exception.py` & `acai_aws-2.2.0/acai_aws/common/records/exception.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/common/records/requirements.py` & `acai_aws-2.2.0/acai_aws/common/records/requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/common/schema.py` & `acai_aws-2.2.0/acai_aws/common/schema.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/common/validator.py` & `acai_aws-2.2.0/acai_aws/common/validator.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/documentdb/record.py` & `acai_aws-2.2.0/acai_aws/documentdb/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/dynamodb/record.py` & `acai_aws-2.2.0/acai_aws/dynamodb/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/firehose/record.py` & `acai_aws-2.2.0/acai_aws/firehose/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/generic/requirements.py` & `acai_aws-2.2.0/acai_aws/generic/requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/kinesis/record.py` & `acai_aws-2.2.0/acai_aws/kinesis/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/mq/record.py` & `acai_aws-2.2.0/acai_aws/mq/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/msk/event.py` & `acai_aws-2.2.0/acai_aws/msk/event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/msk/record.py` & `acai_aws-2.2.0/acai_aws/msk/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/s3/event.py` & `acai_aws-2.2.0/acai_aws/s3/event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/s3/record.py` & `acai_aws-2.2.0/acai_aws/s3/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/sns/record.py` & `acai_aws-2.2.0/acai_aws/sns/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws/sqs/record.py` & `acai_aws-2.2.0/acai_aws/sqs/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/acai_aws.egg-info/PKG-INFO` & `acai_aws-2.2.0/acai_aws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acai_aws
-Version: 2.1.0
+Version: 2.2.0
 Summary: DRY, configurable, opinionated, minimalist framework for use with AWS Serverless Lambdas
 Home-page: https://github.com/syngenta/acai-python.git
 Author: Paul Cruse III
 Author-email: paulcruse3@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -22,27 +22,29 @@
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: dynamodb_json
 Requires-Dist: jsonpickle
 Requires-Dist: jsonref
 Requires-Dist: jsonschema
 Requires-Dist: icecream
+Requires-Dist: pydantic
 Requires-Dist: pyyaml
 Requires-Dist: simplejson
 Requires-Dist: xmltodict
 
 [![CircleCI](https://circleci.com/gh/syngenta/acai-python.svg?style=shield)](https://circleci.com/gh/syngenta/acai-python)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=syngenta_acai-python&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=syngenta_acai-python)
 
 # Acai AWS
 DRY, configurable, declarative node library for working with Amazon Web Service Lambdas.
 
 ## Features
 * Highly configurable apigateway internal router
 * Openapi schema adherence for all event types
+* Generate OpenAPI docs from code base
 * Extensible and customizable middleware for validation and other tasks
 * DRY coding interfaces without the need of boilerplate
 * Ease-of-use with the [serverless framework](https://www.serverless.com/)
 * Local Development support
 * Happy Path Programming (See Philosophy below)
 
 ## Philosophy
```

### Comparing `acai_aws-2.1.0/acai_aws.egg-info/SOURCES.txt` & `acai_aws-2.2.0/acai_aws.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 acai_aws/__init__.py
 acai_aws.egg-info/PKG-INFO
 acai_aws.egg-info/SOURCES.txt
 acai_aws.egg-info/dependency_links.txt
 acai_aws.egg-info/requires.txt
 acai_aws.egg-info/top_level.txt
 acai_aws/apigateway/__init__.py
+acai_aws/apigateway/__main__.py
 acai_aws/apigateway/config_validator.py
 acai_aws/apigateway/endpoint.py
 acai_aws/apigateway/exception.py
 acai_aws/apigateway/request.py
 acai_aws/apigateway/requirements.py
 acai_aws/apigateway/response.py
 acai_aws/apigateway/router.py
@@ -81,17 +82,28 @@
 acai_aws/sqs/record.py
 acai_aws/sqs/requirements.py
 tests/__init__.py
 tests/acai_aws/__init__.py
 tests/acai_aws/apigateway/__init__.py
 tests/acai_aws/apigateway/test_config_validator.py
 tests/acai_aws/apigateway/test_endpoint.py
+tests/acai_aws/apigateway/test_main.py
 tests/acai_aws/apigateway/test_request.py
 tests/acai_aws/apigateway/test_requirements.py
 tests/acai_aws/apigateway/test_response.py
+tests/acai_aws/apigateway/openapi/__init__.py
+tests/acai_aws/apigateway/openapi/test_file_writer.py
+tests/acai_aws/apigateway/openapi/test_generator.py
+tests/acai_aws/apigateway/openapi/handler/__init__.py
+tests/acai_aws/apigateway/openapi/handler/test_importer.py
+tests/acai_aws/apigateway/openapi/handler/test_module.py
+tests/acai_aws/apigateway/openapi/handler/test_scanner.py
+tests/acai_aws/apigateway/openapi/input/__init__.py
+tests/acai_aws/apigateway/openapi/input/test_arguments.py
+tests/acai_aws/apigateway/openapi/input/test_validator.py
 tests/acai_aws/apigateway/resolver/__init__.py
 tests/acai_aws/apigateway/resolver/test_cacher.py
 tests/acai_aws/apigateway/resolver/test_importer.py
 tests/acai_aws/apigateway/resolver/test_init.py
 tests/acai_aws/apigateway/resolver/modes/__init__.py
 tests/acai_aws/apigateway/resolver/modes/test_directory.py
 tests/acai_aws/apigateway/resolver/modes/test_mapping.py
```

### Comparing `acai_aws-2.1.0/setup.py` & `acai_aws-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     install_requires=[
         'boto3',
         'dynamodb_json',
         'jsonpickle',
         'jsonref',
         'jsonschema',
         'icecream',
+        'pydantic',
         'pyyaml',
         'simplejson',
         'xmltodict'
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
```

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_directory.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/modes/test_directory.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_mapping.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/modes/test_mapping.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_pattern.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/modes/test_pattern.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_cacher.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/test_cacher.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_importer.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/test_importer.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_init.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/resolver/test_init.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_directory_router.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/router/test_directory_router.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_mapping_router.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/router/test_mapping_router.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_pattern_router.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/router/test_pattern_router.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_timeout.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/router/test_timeout.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/test_config_validator.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/test_config_validator.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/test_endpoint.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/test_request.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/test_request.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/apigateway/test_response.py` & `acai_aws-2.2.0/tests/acai_aws/apigateway/test_response.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/common/records/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/common/records/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/common/records/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/common/records/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/common/records/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/common/records/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/common/test_json_helper.py` & `acai_aws-2.2.0/tests/acai_aws/common/test_json_helper.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/common/test_logger.py` & `acai_aws-2.2.0/tests/acai_aws/common/test_logger.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/common/test_schema.py` & `acai_aws-2.2.0/tests/acai_aws/common/test_schema.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/common/test_validator.py` & `acai_aws-2.2.0/tests/acai_aws/common/test_validator.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/documentdb/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/documentdb/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/documentdb/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/documentdb/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/documentdb/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/documentdb/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/dynamodb/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/dynamodb/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/dynamodb/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/dynamodb/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/dynamodb/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/dynamodb/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/firehose/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/firehose/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/firehose/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/firehose/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/firehose/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/firehose/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/generic/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/generic/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/kinesis/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/kinesis/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/kinesis/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/kinesis/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/kinesis/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/kinesis/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/mq/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/mq/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/mq/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/mq/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/mq/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/mq/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/msk/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/msk/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/msk/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/msk/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/msk/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/msk/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/s3/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/s3/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/s3/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/s3/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/s3/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/s3/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/sns/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/sns/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/sns/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/sns/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/sns/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/sns/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/sqs/test_event.py` & `acai_aws-2.2.0/tests/acai_aws/sqs/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/sqs/test_record.py` & `acai_aws-2.2.0/tests/acai_aws/sqs/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.1.0/tests/acai_aws/sqs/test_requirements.py` & `acai_aws-2.2.0/tests/acai_aws/sqs/test_requirements.py`

 * *Files identical despite different names*

