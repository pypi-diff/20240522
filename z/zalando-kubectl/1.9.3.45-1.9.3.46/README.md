# Comparing `tmp/zalando-kubectl-1.9.3.45.tar.gz` & `tmp/zalando-kubectl-1.9.3.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zalando-kubectl-1.9.3.45.tar", last modified: Mon Jun 18 12:56:52 2018, max compression
+gzip compressed data, was "dist/zalando-kubectl-1.9.3.46.tar", last modified: Mon Jun 18 13:47:09 2018, max compression
```

## Comparing `zalando-kubectl-1.9.3.45.tar` & `zalando-kubectl-1.9.3.46.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/
--rw-r--r--   0 root         (0) root         (0)       38 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      139 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl.egg-info/
--rw-r--r--   0 root         (0) root         (0)       16 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       56 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1777 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     3709 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2258 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/README.rst
--rw-r--r--   0 root         (0) root         (0)     4500 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/setup.py
--rw-r--r--   0 root         (0) root         (0)     3709 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/
--rw-r--r--   0 root         (0) root         (0)     2202 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/secrets.py
--rw-r--r--   0 root         (0) root         (0)       77 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4221 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templating.py
--rw-r--r--   0 root         (0) root         (0)       76 2018-06-18 12:56:51.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4572 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/traffic.py
--rw-r--r--   0 root         (0) root         (0)     2639 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp/deploy/apply/
--rw-r--r--   0 root         (0) root         (0)      330 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp/deploy/apply/ingress.yaml
--rw-r--r--   0 root         (0) root         (0)      302 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp/deploy/apply/service.yaml
--rw-r--r--   0 root         (0) root         (0)     1357 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp/deploy/apply/deployment.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp/NOTES.txt
--rw-r--r--   0 root         (0) root         (0)      394 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp/delivery.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/deploy/apply/
--rw-r--r--   0 root         (0) root         (0)      278 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/deploy/apply/ingress-template.yaml
--rw-r--r--   0 root         (0) root         (0)      345 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/deploy/apply/service.yaml
--rw-r--r--   0 root         (0) root         (0)     1623 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/deploy/apply/deployment.yaml
--rw-r--r--   0 root         (0) root         (0)      417 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/NOTES.txt
--rw-r--r--   0 root         (0) root         (0)      712 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/delivery.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/deploy/apply/
--rw-r--r--   0 root         (0) root         (0)     1010 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/deploy/apply/credentials.yaml
--rw-r--r--   0 root         (0) root         (0)      299 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/deploy/apply/ingress.yaml
--rw-r--r--   0 root         (0) root         (0)      303 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/deploy/apply/service.yaml
--rw-r--r--   0 root         (0) root         (0)     1890 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/deploy/apply/deployment.yaml
--rw-r--r--   0 root         (0) root         (0)      462 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/NOTES.txt
--rw-r--r--   0 root         (0) root         (0)      334 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/delivery.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp_appdynamics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp_appdynamics/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 12:56:52.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/
--rw-r--r--   0 root         (0) root         (0)      330 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/ingress.yaml
--rw-r--r--   0 root         (0) root         (0)      302 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/service.yaml
--rw-r--r--   0 root         (0) root         (0)     2195 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/deployment.yaml
--rw-r--r--   0 root         (0) root         (0)      228 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp_appdynamics/NOTES.txt
--rw-r--r--   0 root         (0) root         (0)      394 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp_appdynamics/delivery.yaml
--rwxr-xr-x   0 root         (0) root         (0)    26219 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/main.py
--rw-r--r--   0 root         (0) root         (0)     2954 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/kube_config.py
--rw-r--r--   0 root         (0) root         (0)      335 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/utils.py
--rw-r--r--   0 root         (0) root         (0)     3022 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/zalando_kubectl/access_request.py
--rw-r--r--   0 root         (0) root         (0)      148 2018-06-18 12:56:15.000000 zalando-kubectl-1.9.3.45/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/
+-rw-r--r--   0 root         (0) root         (0)       38 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      139 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       16 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1777 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     3709 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2258 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4500 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/
+-rw-r--r--   0 root         (0) root         (0)     2202 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/secrets.py
+-rw-r--r--   0 root         (0) root         (0)       77 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4221 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templating.py
+-rw-r--r--   0 root         (0) root         (0)       76 2018-06-18 13:47:08.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4572 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/traffic.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp/deploy/apply/
+-rw-r--r--   0 root         (0) root         (0)      330 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp/deploy/apply/ingress.yaml
+-rw-r--r--   0 root         (0) root         (0)      302 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp/deploy/apply/service.yaml
+-rw-r--r--   0 root         (0) root         (0)     1357 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp/deploy/apply/deployment.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp/NOTES.txt
+-rw-r--r--   0 root         (0) root         (0)      394 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp/delivery.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/deploy/apply/
+-rw-r--r--   0 root         (0) root         (0)      278 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/deploy/apply/ingress-template.yaml
+-rw-r--r--   0 root         (0) root         (0)      345 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/deploy/apply/service.yaml
+-rw-r--r--   0 root         (0) root         (0)     1623 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/deploy/apply/deployment.yaml
+-rw-r--r--   0 root         (0) root         (0)      417 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/NOTES.txt
+-rw-r--r--   0 root         (0) root         (0)      712 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/delivery.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/deploy/apply/
+-rw-r--r--   0 root         (0) root         (0)     1010 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/deploy/apply/credentials.yaml
+-rw-r--r--   0 root         (0) root         (0)      299 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/deploy/apply/ingress.yaml
+-rw-r--r--   0 root         (0) root         (0)      303 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/deploy/apply/service.yaml
+-rw-r--r--   0 root         (0) root         (0)     1890 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/deploy/apply/deployment.yaml
+-rw-r--r--   0 root         (0) root         (0)      462 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/NOTES.txt
+-rw-r--r--   0 root         (0) root         (0)      334 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/delivery.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp_appdynamics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp_appdynamics/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-18 13:47:09.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/
+-rw-r--r--   0 root         (0) root         (0)      330 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/ingress.yaml
+-rw-r--r--   0 root         (0) root         (0)      302 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/service.yaml
+-rw-r--r--   0 root         (0) root         (0)     2195 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/deployment.yaml
+-rw-r--r--   0 root         (0) root         (0)      228 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp_appdynamics/NOTES.txt
+-rw-r--r--   0 root         (0) root         (0)      394 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp_appdynamics/delivery.yaml
+-rwxr-xr-x   0 root         (0) root         (0)    26758 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/main.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/kube_config.py
+-rw-r--r--   0 root         (0) root         (0)      335 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/zalando_kubectl/access_request.py
+-rw-r--r--   0 root         (0) root         (0)      148 2018-06-18 13:46:31.000000 zalando-kubectl-1.9.3.46/MANIFEST.in
```

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl.egg-info/SOURCES.txt` & `zalando-kubectl-1.9.3.46/zalando_kubectl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl.egg-info/PKG-INFO` & `zalando-kubectl-1.9.3.46/zalando_kubectl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zalando-kubectl
-Version: 1.9.3.45
+Version: 1.9.3.46
 Summary: Kubectl wrapper in Python with OAuth token auth
 Home-page: https://github.com/zalando-incubator/zalando-kubectl
 Author: Henning Jacobs
 Author-email: henning.jacobs@zalando.de
 License: Apache License 2.0
 Description: ===============
         Zalando Kubectl
```

### Comparing `zalando-kubectl-1.9.3.45/README.rst` & `zalando-kubectl-1.9.3.46/README.rst`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/setup.py` & `zalando-kubectl-1.9.3.46/setup.py`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/PKG-INFO` & `zalando-kubectl-1.9.3.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zalando-kubectl
-Version: 1.9.3.45
+Version: 1.9.3.46
 Summary: Kubectl wrapper in Python with OAuth token auth
 Home-page: https://github.com/zalando-incubator/zalando-kubectl
 Author: Henning Jacobs
 Author-email: henning.jacobs@zalando.de
 License: Apache License 2.0
 Description: ===============
         Zalando Kubectl
```

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/secrets.py` & `zalando-kubectl-1.9.3.46/zalando_kubectl/secrets.py`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/templating.py` & `zalando-kubectl-1.9.3.46/zalando_kubectl/templating.py`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/traffic.py` & `zalando-kubectl-1.9.3.46/zalando_kubectl/traffic.py`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/registry.py` & `zalando-kubectl-1.9.3.46/zalando_kubectl/registry.py`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp/deploy/apply/deployment.yaml` & `zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp/deploy/apply/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/deploy/apply/deployment.yaml` & `zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/deploy/apply/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/templates/traffic/delivery.yaml` & `zalando-kubectl-1.9.3.46/zalando_kubectl/templates/traffic/delivery.yaml`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/deploy/apply/credentials.yaml` & `zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/deploy/apply/credentials.yaml`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/templates/senza/deploy/apply/deployment.yaml` & `zalando-kubectl-1.9.3.46/zalando_kubectl/templates/senza/deploy/apply/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/deployment.yaml` & `zalando-kubectl-1.9.3.46/zalando_kubectl/templates/webapp_appdynamics/deploy/apply/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/main.py` & `zalando-kubectl-1.9.3.46/zalando_kubectl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -525,15 +525,29 @@
               help='Use a custom template (default: webapp)',
               metavar='TEMPLATE_ID', default='webapp')
 @click.option('--from-senza', help='Convert Senza definition',
               type=click.File('r'), metavar='SENZA_FILE')
 @click.option('--kubernetes-cluster')
 @click.pass_obj
 def init(config, directory, template, from_senza, kubernetes_cluster):
-    '''Initialize a new deploy folder with Kubernetes manifests'''
+    '''Initializes a new deploy folder with default Kubernetes manifests and
+    CDP configuration.
+
+    You can choose a different template using the '-t' option and specifying
+    one of the following templates:
+
+    webapp  - Default template with a simple public facing web application
+              configured with rolling updates through CDP;
+
+    traffic - Public facing web application configured for blue/green
+              deployments, enabling manual traffic switching;
+
+    senza   - Used for migrating a Senza definition file. You can use
+              --from-senza directly instead.
+    '''
     if directory:
         path = Path(directory[0])
     else:
         path = Path('.')
 
     if from_senza:
         variables = read_senza_variables(from_senza)
```

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/kube_config.py` & `zalando-kubectl-1.9.3.46/zalando_kubectl/kube_config.py`

 * *Files identical despite different names*

### Comparing `zalando-kubectl-1.9.3.45/zalando_kubectl/access_request.py` & `zalando-kubectl-1.9.3.46/zalando_kubectl/access_request.py`

 * *Files identical despite different names*

