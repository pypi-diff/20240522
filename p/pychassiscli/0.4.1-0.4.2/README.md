# Comparing `tmp/pychassiscli-0.4.1.tar.gz` & `tmp/pychassiscli-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychassiscli-0.4.1.tar", last modified: Fri Feb 16 14:46:48 2024, max compression
+gzip compressed data, was "pychassiscli-0.4.2.tar", last modified: Wed May 22 03:23:01 2024, max compression
```

## Comparing `pychassiscli-0.4.1.tar` & `pychassiscli-0.4.2.tar`

### file list

```diff
@@ -1,52 +1,56 @@
--rw-r--r--   0        0        0      297 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/README.md
--rw-r--r--   0        0        0     1043 2024-02-16 14:46:48.288280 pychassiscli-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/__init__.py
--rw-r--r--   0        0        0     4554 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/cli.py
--rw-r--r--   0        0        0      127 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/.apiflaskenv
--rw-r--r--   0        0        0       60 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/.dockerignore
--rw-r--r--   0        0        0     3106 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/.gitignore
--rw-r--r--   0        0        0      290 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/Dockerfile
--rw-r--r--   0        0        0       13 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/README.md
--rw-r--r--   0        0        0     2521 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/__init__.py
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/api/__init__.py
--rw-r--r--   0        0        0      203 2024-02-16 14:46:35.884208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/api/v1/__init__.py
--rw-r--r--   0        0        0       72 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/api/v1/api.py
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/api/v1/exception/__init__.py
--rw-r--r--   0        0        0      420 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/api/v1/exception/api.py
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/api/v1/schema/__init__.py
--rw-r--r--   0        0        0      470 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/api/v1/schema/api.py
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/config/__init__.py
--rw-r--r--   0        0        0      152 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/config/config.py
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/util/__init__.py
--rw-r--r--   0        0        0      325 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/app/util/common.py
--rw-r--r--   0        0        0      173 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/docker-compose-build.yml
--rw-r--r--   0        0        0      858 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/docker-compose-run.yml
--rw-r--r--   0        0        0       40 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/docker-deploy.sh
--rw-r--r--   0        0        0      481 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/gunicorn.conf.py
--rw-r--r--   0        0        0       36 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/requirements.txt
--rw-r--r--   0        0        0      258 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/starter.py
--rw-r--r--   0        0        0     3256 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/grafana.json.mako
--rw-r--r--   0        0        0    27021 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/grafana_conf/config/grafana.ini
--rw-r--r--   0        0        0      958 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/grafana_conf/provisioning/dashboards/all.yaml
--rw-r--r--   0        0        0      955 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/grafana_conf/provisioning/datasources/all.yaml
--rw-r--r--   0        0        0     1618 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/prometheus_conf/prometheus.yml
--rw-r--r--   0        0        0      170 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/statsd_config.js
--rw-r--r--   0        0        0      563 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/statsd_mapping.yml.mako
--rw-r--r--   0        0        0       60 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/.dockerignore
--rw-r--r--   0        0        0     3114 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/.gitignore
--rw-r--r--   0        0        0      327 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/Dockerfile
--rw-r--r--   0        0        0       20 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/README.md
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/all_demo/__init__.py
--rw-r--r--   0        0        0     3983 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/all_demo/all_demo.py
--rw-r--r--   0        0        0      888 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/all_demo/config.yml
--rw-r--r--   0        0        0      197 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/docker-compose-build.yml
--rw-r--r--   0        0        0      761 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/docker-compose-run.yml
--rw-r--r--   0        0        0       41 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/docker-deploy.sh
--rw-r--r--   0        0        0       45 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/nameko/requirements.txt
--rw-r--r--   0        0        0      562 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/templates/rabbitmq/docker-compose-rabbitmq.yml
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/tests/unit/__init__.py
--rw-r--r--   0        0        0      822 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/tests/unit/test_service.py
--rw-r--r--   0        0        0    11314 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/src/pychassiscli/utils.py
--rw-r--r--   0        0        0        0 2024-02-16 14:46:35.888208 pychassiscli-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 pychassiscli-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      297 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/README.md
+-rw-r--r--   0        0        0     1043 2024-05-22 03:23:01.039317 pychassiscli-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/__init__.py
+-rw-r--r--   0        0        0     4554 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/cli.py
+-rw-r--r--   0        0        0      127 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/.apiflaskenv
+-rw-r--r--   0        0        0       60 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/.dockerignore
+-rw-r--r--   0        0        0      981 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/.drone.yml
+-rw-r--r--   0        0        0     3106 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/.gitignore
+-rw-r--r--   0        0        0      290 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/Dockerfile
+-rw-r--r--   0        0        0       13 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/README.md
+-rw-r--r--   0        0        0     1168 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/APIDesc.md
+-rw-r--r--   0        0        0     3619 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/api/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/api/v1/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/api/v1/api.py
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/api/v1/exception/__init__.py
+-rw-r--r--   0        0        0      420 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/api/v1/exception/api.py
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/api/v1/schema/__init__.py
+-rw-r--r--   0        0        0      470 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/api/v1/schema/api.py
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/config/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/config/config.py
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/util/__init__.py
+-rw-r--r--   0        0        0     2216 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/util/auth.py
+-rw-r--r--   0        0        0      325 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/util/common.py
+-rw-r--r--   0        0        0      212 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/app/util/exception.py
+-rw-r--r--   0        0        0      173 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/docker-compose-build.yml
+-rw-r--r--   0        0        0      858 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/docker-compose-run.yml
+-rw-r--r--   0        0        0       40 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/docker-deploy.sh
+-rw-r--r--   0        0        0      499 2024-05-22 03:22:48.135293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/gunicorn.conf.py
+-rw-r--r--   0        0        0       36 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/requirements.txt
+-rw-r--r--   0        0        0      258 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/starter.py
+-rw-r--r--   0        0        0     3256 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/grafana.json.mako
+-rw-r--r--   0        0        0    27021 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/grafana_conf/config/grafana.ini
+-rw-r--r--   0        0        0      958 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/grafana_conf/provisioning/dashboards/all.yaml
+-rw-r--r--   0        0        0      955 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/grafana_conf/provisioning/datasources/all.yaml
+-rw-r--r--   0        0        0     1618 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/prometheus_conf/prometheus.yml
+-rw-r--r--   0        0        0      170 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/statsd_config.js
+-rw-r--r--   0        0        0      563 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/statsd_mapping.yml.mako
+-rw-r--r--   0        0        0       60 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/.dockerignore
+-rw-r--r--   0        0        0     3114 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/.gitignore
+-rw-r--r--   0        0        0      327 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/Dockerfile
+-rw-r--r--   0        0        0       20 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/all_demo/__init__.py
+-rw-r--r--   0        0        0     3983 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/all_demo/all_demo.py
+-rw-r--r--   0        0        0      888 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/all_demo/config.yml
+-rw-r--r--   0        0        0      197 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/docker-compose-build.yml
+-rw-r--r--   0        0        0      761 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/docker-compose-run.yml
+-rw-r--r--   0        0        0       41 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/docker-deploy.sh
+-rw-r--r--   0        0        0       45 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/nameko/requirements.txt
+-rw-r--r--   0        0        0      562 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/templates/rabbitmq/docker-compose-rabbitmq.yml
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/tests/unit/__init__.py
+-rw-r--r--   0        0        0      822 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/tests/unit/test_service.py
+-rw-r--r--   0        0        0    11314 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/src/pychassiscli/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 03:22:48.139293 pychassiscli-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 pychassiscli-0.4.2/PKG-INFO
```

### Comparing `pychassiscli-0.4.1/pyproject.toml` & `pychassiscli-0.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pychassiscli"
-version = "0.4.1"
+version = "0.4.2"
 description = "A lightweight Python distributed microservice command line tool"
 authors = [
     { name = "BryantHe", email = "bryantsisu@qq.com" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
```

### Comparing `pychassiscli-0.4.1/src/pychassiscli/cli.py` & `pychassiscli-0.4.2/src/pychassiscli/cli.py`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/apiflask/.gitignore` & `pychassiscli-0.4.2/src/pychassiscli/templates/apiflask/.gitignore`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/grafana.json.mako` & `pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/grafana.json.mako`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/grafana_conf/config/grafana.ini` & `pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/grafana_conf/config/grafana.ini`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/grafana_conf/provisioning/dashboards/all.yaml` & `pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/grafana_conf/provisioning/dashboards/all.yaml`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/grafana_conf/provisioning/datasources/all.yaml` & `pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/grafana_conf/provisioning/datasources/all.yaml`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/prometheus_conf/prometheus.yml` & `pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/prometheus_conf/prometheus.yml`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/metric-configs/statsd_mapping.yml.mako` & `pychassiscli-0.4.2/src/pychassiscli/templates/metric-configs/statsd_mapping.yml.mako`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/nameko/.gitignore` & `pychassiscli-0.4.2/src/pychassiscli/templates/nameko/.gitignore`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/nameko/all_demo/all_demo.py` & `pychassiscli-0.4.2/src/pychassiscli/templates/nameko/all_demo/all_demo.py`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/nameko/all_demo/config.yml` & `pychassiscli-0.4.2/src/pychassiscli/templates/nameko/all_demo/config.yml`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/nameko/docker-compose-run.yml` & `pychassiscli-0.4.2/src/pychassiscli/templates/nameko/docker-compose-run.yml`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/templates/rabbitmq/docker-compose-rabbitmq.yml` & `pychassiscli-0.4.2/src/pychassiscli/templates/rabbitmq/docker-compose-rabbitmq.yml`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/tests/unit/test_service.py` & `pychassiscli-0.4.2/src/pychassiscli/tests/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/src/pychassiscli/utils.py` & `pychassiscli-0.4.2/src/pychassiscli/utils.py`

 * *Files identical despite different names*

### Comparing `pychassiscli-0.4.1/PKG-INFO` & `pychassiscli-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychassiscli
-Version: 0.4.1
+Version: 0.4.2
 Summary: A lightweight Python distributed microservice command line tool
 Author-Email: BryantHe <bryantsisu@qq.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

