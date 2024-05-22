# Comparing `tmp/phidata-2.4.8.tar.gz` & `tmp/phidata-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-2.4.8.tar", last modified: Tue May 14 07:47:51 2024, max compression
+gzip compressed data, was "phidata-2.4.9.tar", last modified: Wed May 15 16:57:21 2024, max compression
```

## Comparing `phidata-2.4.8.tar` & `phidata-2.4.9.tar`

### file list

```diff
@@ -1,637 +1,637 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.939035 phidata-2.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-05-14 07:47:39.000000 phidata-2.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-14 07:47:51.939035 phidata-2.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-14 07:47:39.000000 phidata-2.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.855034 phidata-2.4.8/phi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.855034 phidata-2.4.8/phi/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.855034 phidata-2.4.8/phi/api/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/schemas/ai.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/schemas/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/schemas/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/schemas/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/schemas/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.859034 phidata-2.4.8/phi/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/app/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/app/db_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.859034 phidata-2.4.8/phi/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.859034 phidata-2.4.8/phi/assistant/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.859034 phidata-2.4.8/phi/assistant/openai/file/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/file/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/file/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/file/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/row.py
--rw-r--r--   0 runner    (1001) docker     (127)    15218 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/assistant/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.859034 phidata-2.4.8/phi/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.863035 phidata-2.4.8/phi/aws/app/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34343 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.863035 phidata-2.4.8/phi/aws/app/django/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/django/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.863035 phidata-2.4.8/phi/aws/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.863035 phidata-2.4.8/phi/aws/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.863035 phidata-2.4.8/phi/aws/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.863035 phidata-2.4.8/phi/aws/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.863035 phidata-2.4.8/phi/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.863035 phidata-2.4.8/phi/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/acm/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.863035 phidata-2.4.8/phi/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.867035 phidata-2.4.8/phi/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25483 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ec2/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.867035 phidata-2.4.8/phi/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    23497 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.867035 phidata-2.4.8/phi/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (127)    31036 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    23482 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.867035 phidata-2.4.8/phi/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22631 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.867035 phidata-2.4.8/phi/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.867035 phidata-2.4.8/phi/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.871034 phidata-2.4.8/phi/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/glue/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.871034 phidata-2.4.8/phi/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.871034 phidata-2.4.8/phi/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    36601 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/rds/db_subnet_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.871034 phidata-2.4.8/phi/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/s3/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/s3/object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.871034 phidata-2.4.8/phi/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/secret/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    31475 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/aws/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.871034 phidata-2.4.8/phi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/auth_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.871034 phidata-2.4.8/phi/cli/k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/k/k_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.875035 phidata-2.4.8/phi/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/cli/ws/ws_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.875035 phidata-2.4.8/phi/docker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.875035 phidata-2.4.8/phi/docker/app/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.875035 phidata-2.4.8/phi/docker/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/airflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/airflow/flower.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/airflow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/airflow/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/airflow/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.875035 phidata-2.4.8/phi/docker/app/django/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/django/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.875035 phidata-2.4.8/phi/docker/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.875035 phidata-2.4.8/phi/docker/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.875035 phidata-2.4.8/phi/docker/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/mysql/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.875035 phidata-2.4.8/phi/docker/app/ollama/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/ollama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/ollama/ollama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.879035 phidata-2.4.8/phi/docker/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/postgres/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.879035 phidata-2.4.8/phi/docker/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.879035 phidata-2.4.8/phi/docker/app/redis/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.879035 phidata-2.4.8/phi/docker/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.879035 phidata-2.4.8/phi/docker/app/superset/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/superset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/superset/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/superset/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/superset/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/superset/worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.879035 phidata-2.4.8/phi/docker/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.879035 phidata-2.4.8/phi/docker/app/whoami/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/whoami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/app/whoami/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.883035 phidata-2.4.8/phi/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/resource/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/docker/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.883035 phidata-2.4.8/phi/document/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.883035 phidata-2.4.8/phi/document/reader/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/firecrawl_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.883035 phidata-2.4.8/phi/document/reader/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/s3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/s3/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/document/reader/website.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.887035 phidata-2.4.8/phi/embedder/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/embedder/anyscale.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/embedder/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/embedder/fireworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/embedder/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/embedder/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/embedder/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/embedder/together.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/embedder/voyageai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.887035 phidata-2.4.8/phi/file/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.887035 phidata-2.4.8/phi/file/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/file/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/file/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/file/local/txt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.887035 phidata-2.4.8/phi/infra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/infra/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/infra/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.887035 phidata-2.4.8/phi/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.887035 phidata-2.4.8/phi/k8s/app/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.887035 phidata-2.4.8/phi/k8s/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/airflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/airflow/flower.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/airflow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/airflow/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/airflow/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.891035 phidata-2.4.8/phi/k8s/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.891035 phidata-2.4.8/phi/k8s/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.891035 phidata-2.4.8/phi/k8s/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/postgres/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.891035 phidata-2.4.8/phi/k8s/app/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.891035 phidata-2.4.8/phi/k8s/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.891035 phidata-2.4.8/phi/k8s/app/superset/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/superset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/superset/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/superset/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/superset/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/superset/worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.891035 phidata-2.4.8/phi/k8s/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   115745 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/app/traefik/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.891035 phidata-2.4.8/phi/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.891035 phidata-2.4.8/phi/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.895035 phidata-2.4.8/phi/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.895035 phidata-2.4.8/phi/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.895035 phidata-2.4.8/phi/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.895035 phidata-2.4.8/phi/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.895035 phidata-2.4.8/phi/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.895035 phidata-2.4.8/phi/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.895035 phidata-2.4.8/phi/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/crb/eks_admin_crb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.895035 phidata-2.4.8/phi/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.895035 phidata-2.4.8/phi/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.899035 phidata-2.4.8/phi/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.899035 phidata-2.4.8/phi/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.899035 phidata-2.4.8/phi/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.899035 phidata-2.4.8/phi/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.899035 phidata-2.4.8/phi/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/enums/volume_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.899035 phidata-2.4.8/phi/k8s/helm/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/helm/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/helm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.903035 phidata-2.4.8/phi/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.903035 phidata-2.4.8/phi/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.903035 phidata-2.4.8/phi/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.903035 phidata-2.4.8/phi/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.903035 phidata-2.4.8/phi/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10016 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.903035 phidata-2.4.8/phi/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.907035 phidata-2.4.8/phi/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    18798 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.907035 phidata-2.4.8/phi/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.907035 phidata-2.4.8/phi/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.907035 phidata-2.4.8/phi/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.907035 phidata-2.4.8/phi/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.907035 phidata-2.4.8/phi/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.907035 phidata-2.4.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.907035 phidata-2.4.8/phi/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.907035 phidata-2.4.8/phi/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resource/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    46880 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.911035 phidata-2.4.8/phi/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/llamaindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.911035 phidata-2.4.8/phi/knowledge/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/s3/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/s3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/s3/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/website.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/knowledge/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.911035 phidata-2.4.8/phi/llm/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.915035 phidata-2.4.8/phi/llm/anthropic/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/anthropic/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.915035 phidata-2.4.8/phi/llm/anyscale/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/anyscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/anyscale/anyscale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.915035 phidata-2.4.8/phi/llm/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/aws/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/aws/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.915035 phidata-2.4.8/phi/llm/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/azure/openai_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.915035 phidata-2.4.8/phi/llm/cohere/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/cohere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/cohere/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.915035 phidata-2.4.8/phi/llm/fireworks/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/fireworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/fireworks/fireworks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.915035 phidata-2.4.8/phi/llm/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/gemini/gemini.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.915035 phidata-2.4.8/phi/llm/groq/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/groq/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.915035 phidata-2.4.8/phi/llm/mistral/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/mistral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/mistral/mistral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/llm/ollama/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/ollama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20162 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/ollama/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    22661 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/ollama/hermes.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/ollama/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/ollama/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/llm/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54253 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/openai/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/openai/like.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/llm/openrouter/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/openrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/openrouter/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/llm/together/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/together/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/llm/together/together.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/memory/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/prompt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/prompt/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/prompt/template.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/storage/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/storage/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/storage/assistant/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/storage/assistant/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/storage/assistant/singlestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/storage/assistant/sqllite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.919035 phidata-2.4.8/phi/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.923035 phidata-2.4.8/phi/table/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/table/sql/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.923035 phidata-2.4.8/phi/task/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.927035 phidata-2.4.8/phi/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/apify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/arxiv_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/csv_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14650 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/exa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.927035 phidata-2.4.8/phi/tools/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/fastapi/playground.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/hackernews.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/newspaper4k.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/newspaper_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/openbb_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/phi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/pubmed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/resend_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/searxng.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/serpapi_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.927035 phidata-2.4.8/phi/tools/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/streamlit/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/tavily.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/tool_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/yfinance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/youtube_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/tools/zendesk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.931035 phidata-2.4.8/phi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/format_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/json_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/merge_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/py_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/response_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/utils/yaml_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.931035 phidata-2.4.8/phi/vectordb/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/distance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.935035 phidata-2.4.8/phi/vectordb/lancedb/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/lancedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/lancedb/lancedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.935035 phidata-2.4.8/phi/vectordb/pgvector/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/pgvector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/pgvector/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    13562 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/pgvector/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/pgvector/pgvector2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.935035 phidata-2.4.8/phi/vectordb/pineconedb/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/pineconedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/pineconedb/pineconedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.935035 phidata-2.4.8/phi/vectordb/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.935035 phidata-2.4.8/phi/vectordb/singlestore/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/singlestore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/singlestore/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/vectordb/singlestore/s2vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.935035 phidata-2.4.8/phi/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.935035 phidata-2.4.8/phi/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/workspace/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/workspace/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    31881 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/workspace/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-14 07:47:39.000000 phidata-2.4.8/phi/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.939035 phidata-2.4.8/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-14 07:47:51.000000 phidata-2.4.8/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14910 2024-05-14 07:47:51.000000 phidata-2.4.8/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:47:51.000000 phidata-2.4.8/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 07:47:51.000000 phidata-2.4.8/phidata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-14 07:47:51.000000 phidata-2.4.8/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 07:47:51.000000 phidata-2.4.8/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-14 07:47:39.000000 phidata-2.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:47:51.939035 phidata-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 07:47:39.000000 phidata-2.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:47:51.939035 phidata-2.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 07:47:39.000000 phidata-2.4.8/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.066907 phidata-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-05-15 16:57:08.000000 phidata-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-05-15 16:57:21.066907 phidata-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12554 2024-05-15 16:57:08.000000 phidata-2.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.990905 phidata-2.4.9/phi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.990905 phidata-2.4.9/phi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.994905 phidata-2.4.9/phi/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/schemas/ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/schemas/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/schemas/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/schemas/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/schemas/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.994905 phidata-2.4.9/phi/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/app/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/app/db_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.994905 phidata-2.4.9/phi/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.994905 phidata-2.4.9/phi/assistant/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.994905 phidata-2.4.9/phi/assistant/openai/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/file/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/file/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/file/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15218 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/assistant/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34343 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/app/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/django/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/acm/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:20.998905 phidata-2.4.9/phi/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.002905 phidata-2.4.9/phi/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25483 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ec2/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.002905 phidata-2.4.9/phi/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23497 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.002905 phidata-2.4.9/phi/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31036 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23482 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.002905 phidata-2.4.9/phi/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22631 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.002905 phidata-2.4.9/phi/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.002905 phidata-2.4.9/phi/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.002905 phidata-2.4.9/phi/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/glue/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.006905 phidata-2.4.9/phi/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.006905 phidata-2.4.9/phi/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36601 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/rds/db_subnet_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.006905 phidata-2.4.9/phi/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/s3/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/s3/object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.006905 phidata-2.4.9/phi/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/secret/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31475 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/aws/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.006905 phidata-2.4.9/phi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.006905 phidata-2.4.9/phi/cli/k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/k/k_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.006905 phidata-2.4.9/phi/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/cli/ws/ws_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/airflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/airflow/flower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/airflow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/airflow/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/airflow/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/django/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/mysql/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/ollama/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/ollama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/ollama/ollama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/postgres/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.010906 phidata-2.4.9/phi/docker/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.014906 phidata-2.4.9/phi/docker/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.014906 phidata-2.4.9/phi/docker/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/superset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/superset/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/superset/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/superset/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/superset/worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.014906 phidata-2.4.9/phi/docker/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.014906 phidata-2.4.9/phi/docker/app/whoami/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/whoami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/app/whoami/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.014906 phidata-2.4.9/phi/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/resource/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/docker/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.014906 phidata-2.4.9/phi/document/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.018906 phidata-2.4.9/phi/document/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/firecrawl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.018906 phidata-2.4.9/phi/document/reader/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/s3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/s3/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/document/reader/website.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.018906 phidata-2.4.9/phi/embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/embedder/anyscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/embedder/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/embedder/fireworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/embedder/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/embedder/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/embedder/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/embedder/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/embedder/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.018906 phidata-2.4.9/phi/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.018906 phidata-2.4.9/phi/file/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/file/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/file/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/file/local/txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.018906 phidata-2.4.9/phi/infra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/infra/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/infra/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.018906 phidata-2.4.9/phi/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.022906 phidata-2.4.9/phi/k8s/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.022906 phidata-2.4.9/phi/k8s/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/airflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/airflow/flower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/airflow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/airflow/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/airflow/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.022906 phidata-2.4.9/phi/k8s/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.022906 phidata-2.4.9/phi/k8s/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.022906 phidata-2.4.9/phi/k8s/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/postgres/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.022906 phidata-2.4.9/phi/k8s/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.022906 phidata-2.4.9/phi/k8s/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.022906 phidata-2.4.9/phi/k8s/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/superset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/superset/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/superset/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/superset/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/superset/worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115745 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/app/traefik/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.026906 phidata-2.4.9/phi/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/crb/eks_admin_crb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.030906 phidata-2.4.9/phi/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.030906 phidata-2.4.9/phi/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.030906 phidata-2.4.9/phi/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.030906 phidata-2.4.9/phi/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.030906 phidata-2.4.9/phi/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.030906 phidata-2.4.9/phi/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.030906 phidata-2.4.9/phi/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/enums/volume_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.030906 phidata-2.4.9/phi/k8s/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/helm/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/helm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.034906 phidata-2.4.9/phi/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.034906 phidata-2.4.9/phi/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.034906 phidata-2.4.9/phi/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.034906 phidata-2.4.9/phi/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.034906 phidata-2.4.9/phi/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10016 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.034906 phidata-2.4.9/phi/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.038906 phidata-2.4.9/phi/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18798 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.038906 phidata-2.4.9/phi/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.038906 phidata-2.4.9/phi/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.038906 phidata-2.4.9/phi/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.038906 phidata-2.4.9/phi/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.038906 phidata-2.4.9/phi/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.038906 phidata-2.4.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.038906 phidata-2.4.9/phi/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.038906 phidata-2.4.9/phi/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resource/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46880 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.042906 phidata-2.4.9/phi/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/llamaindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.042906 phidata-2.4.9/phi/knowledge/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/s3/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/s3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/s3/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/knowledge/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.042906 phidata-2.4.9/phi/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.042906 phidata-2.4.9/phi/llm/anthropic/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/anthropic/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.042906 phidata-2.4.9/phi/llm/anyscale/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/anyscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/anyscale/anyscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.042906 phidata-2.4.9/phi/llm/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/aws/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/aws/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.042906 phidata-2.4.9/phi/llm/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/azure/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.042906 phidata-2.4.9/phi/llm/cohere/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/cohere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/cohere/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.042906 phidata-2.4.9/phi/llm/fireworks/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/fireworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/fireworks/fireworks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.046906 phidata-2.4.9/phi/llm/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/gemini/gemini.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.046906 phidata-2.4.9/phi/llm/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/groq/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.046906 phidata-2.4.9/phi/llm/mistral/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/mistral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/mistral/mistral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.046906 phidata-2.4.9/phi/llm/ollama/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/ollama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20162 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/ollama/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22661 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/ollama/hermes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/ollama/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/ollama/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.046906 phidata-2.4.9/phi/llm/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54248 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/openai/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/openai/like.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.046906 phidata-2.4.9/phi/llm/openrouter/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/openrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/openrouter/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.046906 phidata-2.4.9/phi/llm/together/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/together/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/llm/together/together.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.046906 phidata-2.4.9/phi/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/memory/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.046906 phidata-2.4.9/phi/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/prompt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/prompt/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/prompt/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.050906 phidata-2.4.9/phi/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.050906 phidata-2.4.9/phi/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.050906 phidata-2.4.9/phi/storage/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/storage/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/storage/assistant/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/storage/assistant/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/storage/assistant/singlestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/storage/assistant/sqllite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.050906 phidata-2.4.9/phi/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.050906 phidata-2.4.9/phi/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/table/sql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.050906 phidata-2.4.9/phi/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.054906 phidata-2.4.9/phi/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/apify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/arxiv_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/csv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14650 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/exa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.054906 phidata-2.4.9/phi/tools/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/fastapi/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/hackernews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/newspaper4k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/newspaper_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/openbb_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/phi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/resend_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/searxng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/serpapi_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.054906 phidata-2.4.9/phi/tools/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/streamlit/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/tavily.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/tool_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/yfinance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/youtube_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/tools/zendesk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.058906 phidata-2.4.9/phi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/format_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/merge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/py_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/response_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/utils/yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.058906 phidata-2.4.9/phi/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/distance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.058906 phidata-2.4.9/phi/vectordb/lancedb/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/lancedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/lancedb/lancedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.062907 phidata-2.4.9/phi/vectordb/pgvector/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/pgvector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/pgvector/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13562 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/pgvector/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/pgvector/pgvector2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.062907 phidata-2.4.9/phi/vectordb/pineconedb/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/pineconedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/pineconedb/pineconedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.062907 phidata-2.4.9/phi/vectordb/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.062907 phidata-2.4.9/phi/vectordb/singlestore/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/singlestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/singlestore/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/vectordb/singlestore/s2vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.062907 phidata-2.4.9/phi/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.062907 phidata-2.4.9/phi/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/workspace/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/workspace/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31881 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/workspace/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-15 16:57:08.000000 phidata-2.4.9/phi/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.066907 phidata-2.4.9/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-05-15 16:57:20.000000 phidata-2.4.9/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14910 2024-05-15 16:57:20.000000 phidata-2.4.9/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:57:20.000000 phidata-2.4.9/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 16:57:20.000000 phidata-2.4.9/phidata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-15 16:57:20.000000 phidata-2.4.9/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 16:57:20.000000 phidata-2.4.9/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-15 16:57:08.000000 phidata-2.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:57:21.066907 phidata-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 16:57:08.000000 phidata-2.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:57:21.066907 phidata-2.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 16:57:08.000000 phidata-2.4.9/tests/test_placeholder.py
```

### Comparing `phidata-2.4.8/LICENSE` & `phidata-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/PKG-INFO` & `phidata-2.4.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.4.8
+Version: 2.4.9
 Summary: Memory, knowledge and tools for LLMs.
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -33,29 +33,30 @@
 Requires-Dist: kubernetes; extra == "k8s"
 
 <h1 align="center">
   phidata
 </h1>
 
 <h3 align="center">
-Phidata adds memory, knowledge and tools to LLMs
+Build AI Assistants with memory, knowledge and tools
 </h3>
 
 ![image](https://github.com/phidatahq/phidata/assets/22579644/295187f6-ac9d-41e0-abdb-38e3291ad1d1)
 
 ## What is phidata?
 
-Phidata is a framework for adding memory, knowledge and tools to LLMs. <br/> Memory & knowledge make LLMs **smarter** while tools make them **autonomous**.
+**Phidata is a framework for building Autonomous Assistants** (aka Agents) that have long-term memory, contextual knowledge and the ability to take actions using function calling.
 
 ## Why phidata?
 
-**Problem:** LLMs have limited context and cannot take actions.<br />
+**Problem:** LLMs have limited context and cannot take actions.
+
 **Solution:** Add memory, knowledge and tools.
-- **Memory:** Enables LLMs to have long-term conversations by storing **chat history** in a database.
-- **Knowledge:** Provides LLMs with **business context** by storing information in a vector database.
+- **Memory:** Stores **chat history** in a database and enables LLMs to have long-term conversations.
+- **Knowledge:** Stores information in a vector database and provides LLMs with **business context**.
 - **Tools:** Enable LLMs to **take actions** like pulling data from an API, sending emails or querying a database.
 
 ## How it works
 
 - **Step 1:** Create an `Assistant`
 - **Step 2:** Add Tools (functions), Knowledge (vectordb) and Storage (database)
 - **Step 3:** Serve using Streamlit, FastApi or Django to build your AI application
@@ -63,64 +64,50 @@
 
 ## Installation
 
 ```shell
 pip install -U phidata
 ```
 
-## Example: Assistant that can search the web
+## Quickstart: Assistant that can search the web
 
 Create a file `assistant.py`
 
 ```python
 from phi.assistant import Assistant
 from phi.tools.duckduckgo import DuckDuckGo
 
 assistant = Assistant(tools=[DuckDuckGo()], show_tool_calls=True)
 assistant.print_response("Whats happening in France?", markdown=True)
 ```
 
-Install libraries
+Install libraries, export your `OPENAI_API_KEY` and run the `Assistant`
 
 ```shell
 pip install openai duckduckgo-search
-```
-
-Export your OPENAI_API_KEY
 
-```shell
 export OPENAI_API_KEY=sk-xxxx
-```
 
-Run the `Assistant` and let it search the web using `DuckDuckGo`
-
-```shell
 python assistant.py
 ```
 
-## Next Steps
-
-1. Read the <a href="https://docs.phidata.com/basics" target="_blank" rel="noopener noreferrer">basics</a> to learn more about phidata.
-2. Read about <a href="https://docs.phidata.com/assistants/introduction" target="_blank" rel="noopener noreferrer">Assistants</a> and how to customize them.
-3. Checkout the <a href="https://docs.phidata.com/examples/cookbook" target="_blank" rel="noopener noreferrer">cookbook</a> for in-depth examples and code.
+## Documentation and Support
 
-## Documentation
+- Read the docs at <a href="https://docs.phidata.com" target="_blank" rel="noopener noreferrer">docs.phidata.com</a>
+- Chat with us on <a href="https://discord.gg/4MtYHHrgA8" target="_blank" rel="noopener noreferrer">discord</a>
 
-- You can find the full documentation <a href="https://docs.phidata.com" target="_blank" rel="noopener noreferrer">here</a>
-- You can also chat with us on <a href="https://discord.gg/4MtYHHrgA8" target="_blank" rel="noopener noreferrer">discord</a>
+## Examples
 
-## Demos
-
-Checkout the following AI Applications built using phidata:
-
-- <a href="https://pdf.aidev.run/" target="_blank" rel="noopener noreferrer">PDF AI</a> that summarizes and answers questions from PDFs.
-- <a href="https://arxiv.aidev.run/" target="_blank" rel="noopener noreferrer">ArXiv AI</a> that answers questions about ArXiv papers using the ArXiv API.
-- <a href="https://hn.aidev.run/" target="_blank" rel="noopener noreferrer">HackerNews AI</a> summarize stories, users and shares what's new on HackerNews.
-
-## More Examples
+- [LLM OS](https://github.com/phidatahq/phidata/tree/main/cookbook/llm_os): Using LLMs as the CPU for an emerging Operating System.
+- [Autonomous RAG](https://github.com/phidatahq/phidata/tree/main/cookbook/examples/auto_rag): Gives LLMs tools to search its knowledge, web or chat history.
+- [Local RAG](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/ollama/rag): Fully local RAG with Ollama and PgVector.
+- [Investment Researcher](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/investment_researcher): Generate investment reports on stocks using Llama3 and Groq.
+- [News Articles](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/news_articles): Write News Articles using Llama3 and Groq.
+- [Video Summaries](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/video_summary): YouTube video summaries using Llama3 and Groq.
+- [Research Assistant](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/research): Write research reports using Llama3 and Groq.
 
 ### Assistant that can write and run python code
 
 <details>
 
 <summary>Show details</summary>
 
@@ -371,16 +358,32 @@
 python pdf_assistant.py --new
 ```
 
 </details>
 
 ### Checkout the [cookbook](https://github.com/phidatahq/phidata/tree/main/cookbook) for more examples.
 
+## Next Steps
+
+1. Read the <a href="https://docs.phidata.com/basics" target="_blank" rel="noopener noreferrer">basics</a> to learn more about phidata.
+2. Read about <a href="https://docs.phidata.com/assistants/introduction" target="_blank" rel="noopener noreferrer">Assistants</a> and how to customize them.
+3. Checkout the <a href="https://docs.phidata.com/examples/cookbook" target="_blank" rel="noopener noreferrer">cookbook</a> for in-depth examples and code.
+
+## Demos
+
+Checkout the following AI Applications built using phidata:
+
+- <a href="https://pdf.aidev.run/" target="_blank" rel="noopener noreferrer">PDF AI</a> that summarizes and answers questions from PDFs.
+- <a href="https://arxiv.aidev.run/" target="_blank" rel="noopener noreferrer">ArXiv AI</a> that answers questions about ArXiv papers using the ArXiv API.
+- <a href="https://hn.aidev.run/" target="_blank" rel="noopener noreferrer">HackerNews AI</a> summarize stories, users and shares what's new on HackerNews.
+
 ## Tutorials
 
+[![Building the LLM OS with gpt-4o](https://img.youtube.com/vi/6g2KLvwHZlU/0.jpg)](https://www.youtube.com/watch?v=6g2KLvwHZlU "LLM OS")
+
 [![Autonomous RAG](https://img.youtube.com/vi/fkBkNWivq-s/0.jpg)](https://www.youtube.com/watch?v=fkBkNWivq-s "Autonomous RAG")
 
 [![Local RAG with Llama3](https://img.youtube.com/vi/-8NVHaKKNkM/0.jpg)](https://www.youtube.com/watch?v=-8NVHaKKNkM "Local RAG with Llama3")
 
 [![Llama3 Research Assistant powered by Groq](https://img.youtube.com/vi/Iv9dewmcFbs/0.jpg)](https://www.youtube.com/watch?v=Iv9dewmcFbs "Llama3 Research Assistant powered by Groq")
 
 ## Looking to build an AI product?
```

### Comparing `phidata-2.4.8/README.md` & `phidata-2.4.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 <h1 align="center">
   phidata
 </h1>
 
 <h3 align="center">
-Phidata adds memory, knowledge and tools to LLMs
+Build AI Assistants with memory, knowledge and tools
 </h3>
 
 ![image](https://github.com/phidatahq/phidata/assets/22579644/295187f6-ac9d-41e0-abdb-38e3291ad1d1)
 
 ## What is phidata?
 
-Phidata is a framework for adding memory, knowledge and tools to LLMs. <br/> Memory & knowledge make LLMs **smarter** while tools make them **autonomous**.
+**Phidata is a framework for building Autonomous Assistants** (aka Agents) that have long-term memory, contextual knowledge and the ability to take actions using function calling.
 
 ## Why phidata?
 
-**Problem:** LLMs have limited context and cannot take actions.<br />
+**Problem:** LLMs have limited context and cannot take actions.
+
 **Solution:** Add memory, knowledge and tools.
-- **Memory:** Enables LLMs to have long-term conversations by storing **chat history** in a database.
-- **Knowledge:** Provides LLMs with **business context** by storing information in a vector database.
+- **Memory:** Stores **chat history** in a database and enables LLMs to have long-term conversations.
+- **Knowledge:** Stores information in a vector database and provides LLMs with **business context**.
 - **Tools:** Enable LLMs to **take actions** like pulling data from an API, sending emails or querying a database.
 
 ## How it works
 
 - **Step 1:** Create an `Assistant`
 - **Step 2:** Add Tools (functions), Knowledge (vectordb) and Storage (database)
 - **Step 3:** Serve using Streamlit, FastApi or Django to build your AI application
@@ -29,64 +30,50 @@
 
 ## Installation
 
 ```shell
 pip install -U phidata
 ```
 
-## Example: Assistant that can search the web
+## Quickstart: Assistant that can search the web
 
 Create a file `assistant.py`
 
 ```python
 from phi.assistant import Assistant
 from phi.tools.duckduckgo import DuckDuckGo
 
 assistant = Assistant(tools=[DuckDuckGo()], show_tool_calls=True)
 assistant.print_response("Whats happening in France?", markdown=True)
 ```
 
-Install libraries
+Install libraries, export your `OPENAI_API_KEY` and run the `Assistant`
 
 ```shell
 pip install openai duckduckgo-search
-```
-
-Export your OPENAI_API_KEY
 
-```shell
 export OPENAI_API_KEY=sk-xxxx
-```
 
-Run the `Assistant` and let it search the web using `DuckDuckGo`
-
-```shell
 python assistant.py
 ```
 
-## Next Steps
-
-1. Read the <a href="https://docs.phidata.com/basics" target="_blank" rel="noopener noreferrer">basics</a> to learn more about phidata.
-2. Read about <a href="https://docs.phidata.com/assistants/introduction" target="_blank" rel="noopener noreferrer">Assistants</a> and how to customize them.
-3. Checkout the <a href="https://docs.phidata.com/examples/cookbook" target="_blank" rel="noopener noreferrer">cookbook</a> for in-depth examples and code.
+## Documentation and Support
 
-## Documentation
+- Read the docs at <a href="https://docs.phidata.com" target="_blank" rel="noopener noreferrer">docs.phidata.com</a>
+- Chat with us on <a href="https://discord.gg/4MtYHHrgA8" target="_blank" rel="noopener noreferrer">discord</a>
 
-- You can find the full documentation <a href="https://docs.phidata.com" target="_blank" rel="noopener noreferrer">here</a>
-- You can also chat with us on <a href="https://discord.gg/4MtYHHrgA8" target="_blank" rel="noopener noreferrer">discord</a>
+## Examples
 
-## Demos
-
-Checkout the following AI Applications built using phidata:
-
-- <a href="https://pdf.aidev.run/" target="_blank" rel="noopener noreferrer">PDF AI</a> that summarizes and answers questions from PDFs.
-- <a href="https://arxiv.aidev.run/" target="_blank" rel="noopener noreferrer">ArXiv AI</a> that answers questions about ArXiv papers using the ArXiv API.
-- <a href="https://hn.aidev.run/" target="_blank" rel="noopener noreferrer">HackerNews AI</a> summarize stories, users and shares what's new on HackerNews.
-
-## More Examples
+- [LLM OS](https://github.com/phidatahq/phidata/tree/main/cookbook/llm_os): Using LLMs as the CPU for an emerging Operating System.
+- [Autonomous RAG](https://github.com/phidatahq/phidata/tree/main/cookbook/examples/auto_rag): Gives LLMs tools to search its knowledge, web or chat history.
+- [Local RAG](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/ollama/rag): Fully local RAG with Ollama and PgVector.
+- [Investment Researcher](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/investment_researcher): Generate investment reports on stocks using Llama3 and Groq.
+- [News Articles](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/news_articles): Write News Articles using Llama3 and Groq.
+- [Video Summaries](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/video_summary): YouTube video summaries using Llama3 and Groq.
+- [Research Assistant](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/research): Write research reports using Llama3 and Groq.
 
 ### Assistant that can write and run python code
 
 <details>
 
 <summary>Show details</summary>
 
@@ -337,16 +324,32 @@
 python pdf_assistant.py --new
 ```
 
 </details>
 
 ### Checkout the [cookbook](https://github.com/phidatahq/phidata/tree/main/cookbook) for more examples.
 
+## Next Steps
+
+1. Read the <a href="https://docs.phidata.com/basics" target="_blank" rel="noopener noreferrer">basics</a> to learn more about phidata.
+2. Read about <a href="https://docs.phidata.com/assistants/introduction" target="_blank" rel="noopener noreferrer">Assistants</a> and how to customize them.
+3. Checkout the <a href="https://docs.phidata.com/examples/cookbook" target="_blank" rel="noopener noreferrer">cookbook</a> for in-depth examples and code.
+
+## Demos
+
+Checkout the following AI Applications built using phidata:
+
+- <a href="https://pdf.aidev.run/" target="_blank" rel="noopener noreferrer">PDF AI</a> that summarizes and answers questions from PDFs.
+- <a href="https://arxiv.aidev.run/" target="_blank" rel="noopener noreferrer">ArXiv AI</a> that answers questions about ArXiv papers using the ArXiv API.
+- <a href="https://hn.aidev.run/" target="_blank" rel="noopener noreferrer">HackerNews AI</a> summarize stories, users and shares what's new on HackerNews.
+
 ## Tutorials
 
+[![Building the LLM OS with gpt-4o](https://img.youtube.com/vi/6g2KLvwHZlU/0.jpg)](https://www.youtube.com/watch?v=6g2KLvwHZlU "LLM OS")
+
 [![Autonomous RAG](https://img.youtube.com/vi/fkBkNWivq-s/0.jpg)](https://www.youtube.com/watch?v=fkBkNWivq-s "Autonomous RAG")
 
 [![Local RAG with Llama3](https://img.youtube.com/vi/-8NVHaKKNkM/0.jpg)](https://www.youtube.com/watch?v=-8NVHaKKNkM "Local RAG with Llama3")
 
 [![Llama3 Research Assistant powered by Groq](https://img.youtube.com/vi/Iv9dewmcFbs/0.jpg)](https://www.youtube.com/watch?v=Iv9dewmcFbs "Llama3 Research Assistant powered by Groq")
 
 ## Looking to build an AI product?
```

### Comparing `phidata-2.4.8/phi/api/api.py` & `phidata-2.4.9/phi/api/api.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/api/assistant.py` & `phidata-2.4.9/phi/api/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/api/prompt.py` & `phidata-2.4.9/phi/api/prompt.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/api/routes.py` & `phidata-2.4.9/phi/api/routes.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/api/schemas/prompt.py` & `phidata-2.4.9/phi/api/schemas/prompt.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/api/schemas/workspace.py` & `phidata-2.4.9/phi/api/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/api/user.py` & `phidata-2.4.9/phi/api/user.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/api/workspace.py` & `phidata-2.4.9/phi/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/app/base.py` & `phidata-2.4.9/phi/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/app/context.py` & `phidata-2.4.9/phi/app/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/app/db_app.py` & `phidata-2.4.9/phi/app/db_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/app/group.py` & `phidata-2.4.9/phi/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/assistant.py` & `phidata-2.4.9/phi/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/duckdb.py` & `phidata-2.4.9/phi/assistant/duckdb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/openai/assistant.py` & `phidata-2.4.9/phi/assistant/openai/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/openai/file/file.py` & `phidata-2.4.9/phi/assistant/openai/file/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/openai/file/local.py` & `phidata-2.4.9/phi/assistant/openai/file/local.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/openai/file/url.py` & `phidata-2.4.9/phi/assistant/openai/file/url.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/openai/message.py` & `phidata-2.4.9/phi/assistant/openai/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/openai/row.py` & `phidata-2.4.9/phi/assistant/openai/row.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/openai/run.py` & `phidata-2.4.9/phi/assistant/openai/run.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/openai/thread.py` & `phidata-2.4.9/phi/assistant/openai/thread.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/python.py` & `phidata-2.4.9/phi/assistant/python.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/assistant/run.py` & `phidata-2.4.9/phi/assistant/run.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/api_client.py` & `phidata-2.4.9/phi/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/app/base.py` & `phidata-2.4.9/phi/aws/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/app/django/django.py` & `phidata-2.4.9/phi/aws/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/app/fastapi/fastapi.py` & `phidata-2.4.9/phi/aws/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/app/jupyter/jupyter.py` & `phidata-2.4.9/phi/aws/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/app/qdrant/qdrant.py` & `phidata-2.4.9/phi/aws/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/app/streamlit/streamlit.py` & `phidata-2.4.9/phi/aws/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/acm/certificate.py` & `phidata-2.4.9/phi/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/base.py` & `phidata-2.4.9/phi/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/cloudformation/stack.py` & `phidata-2.4.9/phi/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/ec2/security_group.py` & `phidata-2.4.9/phi/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/ec2/subnet.py` & `phidata-2.4.9/phi/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/ec2/volume.py` & `phidata-2.4.9/phi/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/ecs/cluster.py` & `phidata-2.4.9/phi/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/ecs/container.py` & `phidata-2.4.9/phi/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/ecs/service.py` & `phidata-2.4.9/phi/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/ecs/task_definition.py` & `phidata-2.4.9/phi/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/ecs/volume.py` & `phidata-2.4.9/phi/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/eks/addon.py` & `phidata-2.4.9/phi/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/eks/cluster.py` & `phidata-2.4.9/phi/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/eks/fargate_profile.py` & `phidata-2.4.9/phi/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/eks/kubeconfig.py` & `phidata-2.4.9/phi/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/eks/node_group.py` & `phidata-2.4.9/phi/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/elasticache/cluster.py` & `phidata-2.4.9/phi/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/elasticache/subnet_group.py` & `phidata-2.4.9/phi/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/elb/listener.py` & `phidata-2.4.9/phi/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/elb/load_balancer.py` & `phidata-2.4.9/phi/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/elb/target_group.py` & `phidata-2.4.9/phi/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/emr/cluster.py` & `phidata-2.4.9/phi/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/glue/crawler.py` & `phidata-2.4.9/phi/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/iam/policy.py` & `phidata-2.4.9/phi/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/iam/role.py` & `phidata-2.4.9/phi/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/rds/db_cluster.py` & `phidata-2.4.9/phi/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/rds/db_instance.py` & `phidata-2.4.9/phi/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/rds/db_subnet_group.py` & `phidata-2.4.9/phi/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/s3/bucket.py` & `phidata-2.4.9/phi/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/s3/object.py` & `phidata-2.4.9/phi/aws/resource/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/secret/manager.py` & `phidata-2.4.9/phi/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/secret/reader.py` & `phidata-2.4.9/phi/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resource/types.py` & `phidata-2.4.9/phi/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/aws/resources.py` & `phidata-2.4.9/phi/aws/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/base.py` & `phidata-2.4.9/phi/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/cli/auth_server.py` & `phidata-2.4.9/phi/cli/auth_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/cli/config.py` & `phidata-2.4.9/phi/cli/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/cli/console.py` & `phidata-2.4.9/phi/cli/console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/cli/credentials.py` & `phidata-2.4.9/phi/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/cli/entrypoint.py` & `phidata-2.4.9/phi/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/cli/k/k_cli.py` & `phidata-2.4.9/phi/cli/k/k_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/cli/operator.py` & `phidata-2.4.9/phi/cli/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/cli/settings.py` & `phidata-2.4.9/phi/cli/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/cli/ws/ws_cli.py` & `phidata-2.4.9/phi/cli/ws/ws_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/constants.py` & `phidata-2.4.9/phi/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/api_client.py` & `phidata-2.4.9/phi/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/airflow/base.py` & `phidata-2.4.9/phi/docker/app/airflow/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/airflow/worker.py` & `phidata-2.4.9/phi/docker/app/airflow/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/base.py` & `phidata-2.4.9/phi/docker/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/django/django.py` & `phidata-2.4.9/phi/docker/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/fastapi/fastapi.py` & `phidata-2.4.9/phi/docker/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/jupyter/jupyter.py` & `phidata-2.4.9/phi/docker/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/mysql/mysql.py` & `phidata-2.4.9/phi/docker/app/mysql/mysql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/postgres/postgres.py` & `phidata-2.4.9/phi/docker/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/qdrant/qdrant.py` & `phidata-2.4.9/phi/docker/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/redis/redis.py` & `phidata-2.4.9/phi/docker/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/streamlit/streamlit.py` & `phidata-2.4.9/phi/docker/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/superset/base.py` & `phidata-2.4.9/phi/docker/app/superset/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/app/traefik/router.py` & `phidata-2.4.9/phi/docker/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/resource/base.py` & `phidata-2.4.9/phi/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/resource/container.py` & `phidata-2.4.9/phi/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/resource/image.py` & `phidata-2.4.9/phi/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/resource/network.py` & `phidata-2.4.9/phi/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/resource/types.py` & `phidata-2.4.9/phi/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/resource/volume.py` & `phidata-2.4.9/phi/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/docker/resources.py` & `phidata-2.4.9/phi/docker/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/base.py` & `phidata-2.4.9/phi/document/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/arxiv.py` & `phidata-2.4.9/phi/document/reader/arxiv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/base.py` & `phidata-2.4.9/phi/document/reader/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/docx.py` & `phidata-2.4.9/phi/document/reader/docx.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/firecrawl_reader.py` & `phidata-2.4.9/phi/document/reader/firecrawl_reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/json.py` & `phidata-2.4.9/phi/document/reader/json.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/pdf.py` & `phidata-2.4.9/phi/document/reader/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/s3/pdf.py` & `phidata-2.4.9/phi/document/reader/s3/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/s3/text.py` & `phidata-2.4.9/phi/document/reader/s3/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/text.py` & `phidata-2.4.9/phi/document/reader/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/document/reader/website.py` & `phidata-2.4.9/phi/document/reader/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/embedder/mistral.py` & `phidata-2.4.9/phi/embedder/mistral.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/embedder/ollama.py` & `phidata-2.4.9/phi/embedder/ollama.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/embedder/openai.py` & `phidata-2.4.9/phi/embedder/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/embedder/voyageai.py` & `phidata-2.4.9/phi/embedder/voyageai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/file/local/csv.py` & `phidata-2.4.9/phi/file/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/infra/resources.py` & `phidata-2.4.9/phi/infra/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/api_client.py` & `phidata-2.4.9/phi/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/airflow/base.py` & `phidata-2.4.9/phi/k8s/app/airflow/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/airflow/worker.py` & `phidata-2.4.9/phi/k8s/app/airflow/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/base.py` & `phidata-2.4.9/phi/k8s/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/fastapi/fastapi.py` & `phidata-2.4.9/phi/k8s/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/jupyter/jupyter.py` & `phidata-2.4.9/phi/k8s/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/postgres/postgres.py` & `phidata-2.4.9/phi/k8s/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/redis/redis.py` & `phidata-2.4.9/phi/k8s/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/streamlit/streamlit.py` & `phidata-2.4.9/phi/k8s/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/superset/base.py` & `phidata-2.4.9/phi/k8s/app/superset/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/traefik/crds.py` & `phidata-2.4.9/phi/k8s/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/app/traefik/router.py` & `phidata-2.4.9/phi/k8s/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.4.9/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.4.9/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/apps/v1/deployment.py` & `phidata-2.4.9/phi/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/base.py` & `phidata-2.4.9/phi/k8s/create/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/common/port.py` & `phidata-2.4.9/phi/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/core/v1/config_map.py` & `phidata-2.4.9/phi/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/core/v1/container.py` & `phidata-2.4.9/phi/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/core/v1/namespace.py` & `phidata-2.4.9/phi/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/core/v1/persistent_volume.py` & `phidata-2.4.9/phi/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-2.4.9/phi/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/core/v1/secret.py` & `phidata-2.4.9/phi/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/core/v1/service.py` & `phidata-2.4.9/phi/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/core/v1/service_account.py` & `phidata-2.4.9/phi/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/core/v1/volume.py` & `phidata-2.4.9/phi/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/crb/eks_admin_crb.py` & `phidata-2.4.9/phi/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-2.4.9/phi/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.4.9/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.4.9/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-2.4.9/phi/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/enums/api_version.py` & `phidata-2.4.9/phi/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/enums/kind.py` & `phidata-2.4.9/phi/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/enums/pv.py` & `phidata-2.4.9/phi/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/helm/chart.py` & `phidata-2.4.9/phi/k8s/helm/chart.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/helm/cli.py` & `phidata-2.4.9/phi/k8s/helm/cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/operator.py` & `phidata-2.4.9/phi/k8s/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.4.9/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.4.9/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/apps/v1/deployment.py` & `phidata-2.4.9/phi/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-2.4.9/phi/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/base.py` & `phidata-2.4.9/phi/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/config_map.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/container.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/local_object_reference.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/namespace.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/node_selector.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/object_reference.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/persistent_volume.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/pod.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/pod_spec.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/pod_template_spec.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/resource_requirements.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/secret.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/service.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/service_account.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/toleration.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/volume.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/core/v1/volume_source.py` & `phidata-2.4.9/phi/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/kubeconfig.py` & `phidata-2.4.9/phi/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/meta/v1/label_selector.py` & `phidata-2.4.9/phi/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/meta/v1/object_meta.py` & `phidata-2.4.9/phi/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-2.4.9/phi/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.4.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.4.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-2.4.9/phi/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/types.py` & `phidata-2.4.9/phi/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resource/yaml.py` & `phidata-2.4.9/phi/k8s/resource/yaml.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/k8s/resources.py` & `phidata-2.4.9/phi/k8s/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/arxiv.py` & `phidata-2.4.9/phi/knowledge/arxiv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/base.py` & `phidata-2.4.9/phi/knowledge/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/combined.py` & `phidata-2.4.9/phi/knowledge/combined.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/document.py` & `phidata-2.4.9/phi/knowledge/document.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/docx.py` & `phidata-2.4.9/phi/knowledge/docx.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/json.py` & `phidata-2.4.9/phi/knowledge/json.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/langchain.py` & `phidata-2.4.9/phi/knowledge/langchain.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/llamaindex.py` & `phidata-2.4.9/phi/knowledge/llamaindex.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/pdf.py` & `phidata-2.4.9/phi/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/s3/base.py` & `phidata-2.4.9/phi/knowledge/s3/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/s3/pdf.py` & `phidata-2.4.9/phi/knowledge/s3/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/s3/text.py` & `phidata-2.4.9/phi/knowledge/s3/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/text.py` & `phidata-2.4.9/phi/knowledge/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/website.py` & `phidata-2.4.9/phi/knowledge/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/knowledge/wikipedia.py` & `phidata-2.4.9/phi/knowledge/wikipedia.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/anthropic/claude.py` & `phidata-2.4.9/phi/llm/anthropic/claude.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/aws/bedrock.py` & `phidata-2.4.9/phi/llm/aws/bedrock.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/aws/claude.py` & `phidata-2.4.9/phi/llm/aws/claude.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/azure/openai_chat.py` & `phidata-2.4.9/phi/llm/azure/openai_chat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/base.py` & `phidata-2.4.9/phi/llm/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/cohere/chat.py` & `phidata-2.4.9/phi/llm/cohere/chat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/gemini/gemini.py` & `phidata-2.4.9/phi/llm/gemini/gemini.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/groq/groq.py` & `phidata-2.4.9/phi/llm/groq/groq.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 except ImportError:
     logger.error("`groq` not installed")
     raise
 
 
 class Groq(LLM):
     name: str = "Groq"
-    model: str = "mixtral-8x7b-32768"
+    model: str = "llama3-70b-8192"
     # -*- Request parameters
     frequency_penalty: Optional[float] = None
     logit_bias: Optional[Any] = None
     logprobs: Optional[bool] = None
     max_tokens: Optional[int] = None
     presence_penalty: Optional[float] = None
     response_format: Optional[Dict[str, Any]] = None
```

### Comparing `phidata-2.4.8/phi/llm/message.py` & `phidata-2.4.9/phi/llm/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/mistral/mistral.py` & `phidata-2.4.9/phi/llm/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/ollama/chat.py` & `phidata-2.4.9/phi/llm/ollama/chat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/ollama/hermes.py` & `phidata-2.4.9/phi/llm/ollama/hermes.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/ollama/tools.py` & `phidata-2.4.9/phi/llm/ollama/tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/llm/openai/chat.py` & `phidata-2.4.9/phi/llm/openai/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     logger.error("`openai` not installed")
     raise
 
 
 class OpenAIChat(LLM):
     name: str = "OpenAIChat"
-    model: str = "gpt-4-turbo"
+    model: str = "gpt-4o"
     # -*- Request parameters
     frequency_penalty: Optional[float] = None
     logit_bias: Optional[Any] = None
     logprobs: Optional[bool] = None
     max_tokens: Optional[int] = None
     presence_penalty: Optional[float] = None
     response_format: Optional[Dict[str, Any]] = None
```

### Comparing `phidata-2.4.8/phi/llm/together/together.py` & `phidata-2.4.9/phi/llm/together/together.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/memory/assistant.py` & `phidata-2.4.9/phi/memory/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/prompt/registry.py` & `phidata-2.4.9/phi/prompt/registry.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/prompt/template.py` & `phidata-2.4.9/phi/prompt/template.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/resource/base.py` & `phidata-2.4.9/phi/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/resource/group.py` & `phidata-2.4.9/phi/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/storage/assistant/base.py` & `phidata-2.4.9/phi/storage/assistant/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/storage/assistant/postgres.py` & `phidata-2.4.9/phi/storage/assistant/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/storage/assistant/singlestore.py` & `phidata-2.4.9/phi/storage/assistant/singlestore.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/storage/assistant/sqllite.py` & `phidata-2.4.9/phi/storage/assistant/sqllite.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/task/task.py` & `phidata-2.4.9/phi/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/airflow.py` & `phidata-2.4.9/phi/tools/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/apify.py` & `phidata-2.4.9/phi/tools/apify.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/arxiv_toolkit.py` & `phidata-2.4.9/phi/tools/arxiv_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/calculator.py` & `phidata-2.4.9/phi/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/csv_tools.py` & `phidata-2.4.9/phi/tools/csv_tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/duckdb.py` & `phidata-2.4.9/phi/tools/duckdb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/duckduckgo.py` & `phidata-2.4.9/phi/tools/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/email.py` & `phidata-2.4.9/phi/tools/email.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/exa.py` & `phidata-2.4.9/phi/tools/exa.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/file.py` & `phidata-2.4.9/phi/tools/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/function.py` & `phidata-2.4.9/phi/tools/function.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/google.py` & `phidata-2.4.9/phi/tools/google.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/hackernews.py` & `phidata-2.4.9/phi/tools/hackernews.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/newspaper4k.py` & `phidata-2.4.9/phi/tools/newspaper4k.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/newspaper_toolkit.py` & `phidata-2.4.9/phi/tools/newspaper_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/openbb_tools.py` & `phidata-2.4.9/phi/tools/openbb_tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/pandas.py` & `phidata-2.4.9/phi/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/phi.py` & `phidata-2.4.9/phi/tools/phi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/pubmed.py` & `phidata-2.4.9/phi/tools/pubmed.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/python.py` & `phidata-2.4.9/phi/tools/python.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/resend_tools.py` & `phidata-2.4.9/phi/tools/resend_tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/searxng.py` & `phidata-2.4.9/phi/tools/searxng.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/serpapi_tools.py` & `phidata-2.4.9/phi/tools/serpapi_tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/shell.py` & `phidata-2.4.9/phi/tools/shell.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/sql.py` & `phidata-2.4.9/phi/tools/sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/streamlit/components.py` & `phidata-2.4.9/phi/tools/streamlit/components.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/tavily.py` & `phidata-2.4.9/phi/tools/tavily.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/toolkit.py` & `phidata-2.4.9/phi/tools/toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/website.py` & `phidata-2.4.9/phi/tools/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/wikipedia.py` & `phidata-2.4.9/phi/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/yfinance.py` & `phidata-2.4.9/phi/tools/yfinance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/youtube_tools.py` & `phidata-2.4.9/phi/tools/youtube_tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/tools/zendesk.py` & `phidata-2.4.9/phi/tools/zendesk.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/common.py` & `phidata-2.4.9/phi/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/defaults.py` & `phidata-2.4.9/phi/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/enum.py` & `phidata-2.4.9/phi/utils/enum.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/filesystem.py` & `phidata-2.4.9/phi/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/functions.py` & `phidata-2.4.9/phi/utils/functions.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/git.py` & `phidata-2.4.9/phi/utils/git.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/json_io.py` & `phidata-2.4.9/phi/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/json_schema.py` & `phidata-2.4.9/phi/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/load_env.py` & `phidata-2.4.9/phi/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/log.py` & `phidata-2.4.9/phi/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/merge_dict.py` & `phidata-2.4.9/phi/utils/merge_dict.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/message.py` & `phidata-2.4.9/phi/utils/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/pickle.py` & `phidata-2.4.9/phi/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/py_io.py` & `phidata-2.4.9/phi/utils/py_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/pyproject.py` & `phidata-2.4.9/phi/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/resource_filter.py` & `phidata-2.4.9/phi/utils/resource_filter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/shell.py` & `phidata-2.4.9/phi/utils/shell.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/timer.py` & `phidata-2.4.9/phi/utils/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/tools.py` & `phidata-2.4.9/phi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/utils/yaml_io.py` & `phidata-2.4.9/phi/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/vectordb/base.py` & `phidata-2.4.9/phi/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/vectordb/lancedb/lancedb.py` & `phidata-2.4.9/phi/vectordb/lancedb/lancedb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/vectordb/pgvector/pgvector.py` & `phidata-2.4.9/phi/vectordb/pgvector/pgvector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/vectordb/pgvector/pgvector2.py` & `phidata-2.4.9/phi/vectordb/pgvector/pgvector2.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/vectordb/pineconedb/pineconedb.py` & `phidata-2.4.9/phi/vectordb/pineconedb/pineconedb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/vectordb/qdrant/qdrant.py` & `phidata-2.4.9/phi/vectordb/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/vectordb/singlestore/index.py` & `phidata-2.4.9/phi/vectordb/singlestore/index.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/vectordb/singlestore/s2vectordb.py` & `phidata-2.4.9/phi/vectordb/singlestore/s2vectordb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/workflow/workflow.py` & `phidata-2.4.9/phi/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/workspace/config.py` & `phidata-2.4.9/phi/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/workspace/helpers.py` & `phidata-2.4.9/phi/workspace/helpers.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/workspace/operator.py` & `phidata-2.4.9/phi/workspace/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phi/workspace/settings.py` & `phidata-2.4.9/phi/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/phidata.egg-info/PKG-INFO` & `phidata-2.4.9/phidata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.4.8
+Version: 2.4.9
 Summary: Memory, knowledge and tools for LLMs.
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -33,29 +33,30 @@
 Requires-Dist: kubernetes; extra == "k8s"
 
 <h1 align="center">
   phidata
 </h1>
 
 <h3 align="center">
-Phidata adds memory, knowledge and tools to LLMs
+Build AI Assistants with memory, knowledge and tools
 </h3>
 
 ![image](https://github.com/phidatahq/phidata/assets/22579644/295187f6-ac9d-41e0-abdb-38e3291ad1d1)
 
 ## What is phidata?
 
-Phidata is a framework for adding memory, knowledge and tools to LLMs. <br/> Memory & knowledge make LLMs **smarter** while tools make them **autonomous**.
+**Phidata is a framework for building Autonomous Assistants** (aka Agents) that have long-term memory, contextual knowledge and the ability to take actions using function calling.
 
 ## Why phidata?
 
-**Problem:** LLMs have limited context and cannot take actions.<br />
+**Problem:** LLMs have limited context and cannot take actions.
+
 **Solution:** Add memory, knowledge and tools.
-- **Memory:** Enables LLMs to have long-term conversations by storing **chat history** in a database.
-- **Knowledge:** Provides LLMs with **business context** by storing information in a vector database.
+- **Memory:** Stores **chat history** in a database and enables LLMs to have long-term conversations.
+- **Knowledge:** Stores information in a vector database and provides LLMs with **business context**.
 - **Tools:** Enable LLMs to **take actions** like pulling data from an API, sending emails or querying a database.
 
 ## How it works
 
 - **Step 1:** Create an `Assistant`
 - **Step 2:** Add Tools (functions), Knowledge (vectordb) and Storage (database)
 - **Step 3:** Serve using Streamlit, FastApi or Django to build your AI application
@@ -63,64 +64,50 @@
 
 ## Installation
 
 ```shell
 pip install -U phidata
 ```
 
-## Example: Assistant that can search the web
+## Quickstart: Assistant that can search the web
 
 Create a file `assistant.py`
 
 ```python
 from phi.assistant import Assistant
 from phi.tools.duckduckgo import DuckDuckGo
 
 assistant = Assistant(tools=[DuckDuckGo()], show_tool_calls=True)
 assistant.print_response("Whats happening in France?", markdown=True)
 ```
 
-Install libraries
+Install libraries, export your `OPENAI_API_KEY` and run the `Assistant`
 
 ```shell
 pip install openai duckduckgo-search
-```
-
-Export your OPENAI_API_KEY
 
-```shell
 export OPENAI_API_KEY=sk-xxxx
-```
 
-Run the `Assistant` and let it search the web using `DuckDuckGo`
-
-```shell
 python assistant.py
 ```
 
-## Next Steps
-
-1. Read the <a href="https://docs.phidata.com/basics" target="_blank" rel="noopener noreferrer">basics</a> to learn more about phidata.
-2. Read about <a href="https://docs.phidata.com/assistants/introduction" target="_blank" rel="noopener noreferrer">Assistants</a> and how to customize them.
-3. Checkout the <a href="https://docs.phidata.com/examples/cookbook" target="_blank" rel="noopener noreferrer">cookbook</a> for in-depth examples and code.
+## Documentation and Support
 
-## Documentation
+- Read the docs at <a href="https://docs.phidata.com" target="_blank" rel="noopener noreferrer">docs.phidata.com</a>
+- Chat with us on <a href="https://discord.gg/4MtYHHrgA8" target="_blank" rel="noopener noreferrer">discord</a>
 
-- You can find the full documentation <a href="https://docs.phidata.com" target="_blank" rel="noopener noreferrer">here</a>
-- You can also chat with us on <a href="https://discord.gg/4MtYHHrgA8" target="_blank" rel="noopener noreferrer">discord</a>
+## Examples
 
-## Demos
-
-Checkout the following AI Applications built using phidata:
-
-- <a href="https://pdf.aidev.run/" target="_blank" rel="noopener noreferrer">PDF AI</a> that summarizes and answers questions from PDFs.
-- <a href="https://arxiv.aidev.run/" target="_blank" rel="noopener noreferrer">ArXiv AI</a> that answers questions about ArXiv papers using the ArXiv API.
-- <a href="https://hn.aidev.run/" target="_blank" rel="noopener noreferrer">HackerNews AI</a> summarize stories, users and shares what's new on HackerNews.
-
-## More Examples
+- [LLM OS](https://github.com/phidatahq/phidata/tree/main/cookbook/llm_os): Using LLMs as the CPU for an emerging Operating System.
+- [Autonomous RAG](https://github.com/phidatahq/phidata/tree/main/cookbook/examples/auto_rag): Gives LLMs tools to search its knowledge, web or chat history.
+- [Local RAG](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/ollama/rag): Fully local RAG with Ollama and PgVector.
+- [Investment Researcher](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/investment_researcher): Generate investment reports on stocks using Llama3 and Groq.
+- [News Articles](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/news_articles): Write News Articles using Llama3 and Groq.
+- [Video Summaries](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/video_summary): YouTube video summaries using Llama3 and Groq.
+- [Research Assistant](https://github.com/phidatahq/phidata/tree/main/cookbook/llms/groq/research): Write research reports using Llama3 and Groq.
 
 ### Assistant that can write and run python code
 
 <details>
 
 <summary>Show details</summary>
 
@@ -371,16 +358,32 @@
 python pdf_assistant.py --new
 ```
 
 </details>
 
 ### Checkout the [cookbook](https://github.com/phidatahq/phidata/tree/main/cookbook) for more examples.
 
+## Next Steps
+
+1. Read the <a href="https://docs.phidata.com/basics" target="_blank" rel="noopener noreferrer">basics</a> to learn more about phidata.
+2. Read about <a href="https://docs.phidata.com/assistants/introduction" target="_blank" rel="noopener noreferrer">Assistants</a> and how to customize them.
+3. Checkout the <a href="https://docs.phidata.com/examples/cookbook" target="_blank" rel="noopener noreferrer">cookbook</a> for in-depth examples and code.
+
+## Demos
+
+Checkout the following AI Applications built using phidata:
+
+- <a href="https://pdf.aidev.run/" target="_blank" rel="noopener noreferrer">PDF AI</a> that summarizes and answers questions from PDFs.
+- <a href="https://arxiv.aidev.run/" target="_blank" rel="noopener noreferrer">ArXiv AI</a> that answers questions about ArXiv papers using the ArXiv API.
+- <a href="https://hn.aidev.run/" target="_blank" rel="noopener noreferrer">HackerNews AI</a> summarize stories, users and shares what's new on HackerNews.
+
 ## Tutorials
 
+[![Building the LLM OS with gpt-4o](https://img.youtube.com/vi/6g2KLvwHZlU/0.jpg)](https://www.youtube.com/watch?v=6g2KLvwHZlU "LLM OS")
+
 [![Autonomous RAG](https://img.youtube.com/vi/fkBkNWivq-s/0.jpg)](https://www.youtube.com/watch?v=fkBkNWivq-s "Autonomous RAG")
 
 [![Local RAG with Llama3](https://img.youtube.com/vi/-8NVHaKKNkM/0.jpg)](https://www.youtube.com/watch?v=-8NVHaKKNkM "Local RAG with Llama3")
 
 [![Llama3 Research Assistant powered by Groq](https://img.youtube.com/vi/Iv9dewmcFbs/0.jpg)](https://www.youtube.com/watch?v=Iv9dewmcFbs "Llama3 Research Assistant powered by Groq")
 
 ## Looking to build an AI product?
```

### Comparing `phidata-2.4.8/phidata.egg-info/SOURCES.txt` & `phidata-2.4.9/phidata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phidata-2.4.8/pyproject.toml` & `phidata-2.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phidata"
-version = "2.4.8"
+version = "2.4.9"
 description = "Memory, knowledge and tools for LLMs."
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
```

