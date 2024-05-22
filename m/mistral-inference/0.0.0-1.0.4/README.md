# Comparing `tmp/mistral_inference-0.0.0.tar.gz` & `tmp/mistral_inference-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistral_inference-0.0.0.tar", last modified: Tue May 14 14:33:32 2024, max compression
+gzip compressed data, was "mistral_inference-1.0.4.tar", max compression
```

## Comparing `mistral_inference-0.0.0.tar` & `mistral_inference-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,11 @@
-drwxr-xr-x   0 patrickvonplaten   (501) staff       (20)        0 2024-05-14 14:33:32.378364 mistral_inference-0.0.0/
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)   456384 2024-05-14 14:28:42.000000 mistral_inference-0.0.0/LICENSE
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)       83 2024-05-14 14:33:32.378037 mistral_inference-0.0.0/PKG-INFO
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)       14 2024-05-14 14:28:42.000000 mistral_inference-0.0.0/README.md
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)      198 2024-05-14 14:32:39.000000 mistral_inference-0.0.0/pyproject.toml
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)       38 2024-05-14 14:33:32.378414 mistral_inference-0.0.0/setup.cfg
-drwxr-xr-x   0 patrickvonplaten   (501) staff       (20)        0 2024-05-14 14:33:32.373476 mistral_inference-0.0.0/src/
-drwxr-xr-x   0 patrickvonplaten   (501) staff       (20)        0 2024-05-14 14:33:32.376058 mistral_inference-0.0.0/src/mistral_inference/
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)       31 2024-05-14 14:32:37.000000 mistral_inference-0.0.0/src/mistral_inference/__init__.py
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)       23 2024-05-14 14:28:42.000000 mistral_inference-0.0.0/src/mistral_inference/hello.py
-drwxr-xr-x   0 patrickvonplaten   (501) staff       (20)        0 2024-05-14 14:33:32.377792 mistral_inference-0.0.0/src/mistral_inference.egg-info/
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)       83 2024-05-14 14:33:32.000000 mistral_inference-0.0.0/src/mistral_inference.egg-info/PKG-INFO
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)      277 2024-05-14 14:33:32.000000 mistral_inference-0.0.0/src/mistral_inference.egg-info/SOURCES.txt
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)        1 2024-05-14 14:33:32.000000 mistral_inference-0.0.0/src/mistral_inference.egg-info/dependency_links.txt
--rw-r--r--   0 patrickvonplaten   (501) staff       (20)       18 2024-05-14 14:33:32.000000 mistral_inference-0.0.0/src/mistral_inference.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11357 2024-05-13 15:10:07.471001 mistral_inference-1.0.4/LICENSE
+-rw-r--r--   0        0        0     7760 2024-05-22 14:58:05.363410 mistral_inference-1.0.4/README.md
+-rw-r--r--   0        0        0     1139 2024-05-22 09:55:48.049936 mistral_inference-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-22 09:55:18.014799 mistral_inference-1.0.4/src/mistral_inference/__init__.py
+-rw-r--r--   0        0        0     7441 2024-05-22 15:25:31.252665 mistral_inference-1.0.4/src/mistral_inference/cache.py
+-rw-r--r--   0        0        0     4262 2024-05-22 15:25:31.307427 mistral_inference-1.0.4/src/mistral_inference/generate.py
+-rw-r--r--   0        0        0     5358 2024-05-20 16:49:26.556866 mistral_inference-1.0.4/src/mistral_inference/main.py
+-rw-r--r--   0        0        0    14527 2024-05-22 15:25:31.311908 mistral_inference-1.0.4/src/mistral_inference/model.py
+-rw-r--r--   0        0        0     1147 2024-05-20 16:41:20.124394 mistral_inference-1.0.4/src/mistral_inference/moe.py
+-rw-r--r--   0        0        0      851 2024-05-20 16:41:20.128114 mistral_inference-1.0.4/src/mistral_inference/rope.py
+-rw-r--r--   0        0        0     8341 1970-01-01 00:00:00.000000 mistral_inference-1.0.4/PKG-INFO
```

