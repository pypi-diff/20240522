# Comparing `tmp/inciweb-wildfires-1.0.0.tar.gz` & `tmp/inciweb-wildfires-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inciweb-wildfires-1.0.0.tar", last modified: Fri Apr 12 10:19:37 2024, max compression
+gzip compressed data, was "inciweb-wildfires-1.1.0.tar", last modified: Wed May 22 00:49:41 2024, max compression
```

## Comparing `inciweb-wildfires-1.0.0.tar` & `inciweb-wildfires-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.138078 inciweb-wildfires-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.130078 inciweb-wildfires-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.github/workflows/scrape.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-12 10:19:37.138078 inciweb-wildfires-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    52150 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/data/
--rw-r--r--   0 runner    (1001) docker     (127)   110262 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/data/incidents.json
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/data/timestamp.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.130078 inciweb-wildfires-1.0.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/_templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/inciweb_wildfires/
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/inciweb_wildfires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/inciweb_wildfires/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.138078 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 10:19:37.138078 inciweb-wildfires-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:49:41.318547 inciweb-wildfires-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:49:41.314547 inciweb-wildfires-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:49:41.318547 inciweb-wildfires-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/.github/workflows/scrape.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-22 00:49:41.318547 inciweb-wildfires-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    53128 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:49:41.318547 inciweb-wildfires-1.1.0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   184720 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/data/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/data/timestamp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:49:41.318547 inciweb-wildfires-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:49:41.318547 inciweb-wildfires-1.1.0/inciweb_wildfires/
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/inciweb_wildfires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/inciweb_wildfires/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:49:41.318547 inciweb-wildfires-1.1.0/inciweb_wildfires.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-22 00:49:41.000000 inciweb-wildfires-1.1.0/inciweb_wildfires.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-22 00:49:41.000000 inciweb-wildfires-1.1.0/inciweb_wildfires.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:49:41.000000 inciweb-wildfires-1.1.0/inciweb_wildfires.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 00:49:41.000000 inciweb-wildfires-1.1.0/inciweb_wildfires.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 00:49:41.000000 inciweb-wildfires-1.1.0/inciweb_wildfires.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 00:49:41.000000 inciweb-wildfires-1.1.0/inciweb_wildfires.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 00:49:41.318547 inciweb-wildfires-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-22 00:49:16.000000 inciweb-wildfires-1.1.0/test.py
```

### Comparing `inciweb-wildfires-1.0.0/.github/workflows/continuous-deployment.yml` & `inciweb-wildfires-1.1.0/.github/workflows/continuous-deployment.yml`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-1.0.0/.github/workflows/scrape.yml` & `inciweb-wildfires-1.1.0/.github/workflows/scrape.yml`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-1.0.0/.gitignore` & `inciweb-wildfires-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-1.0.0/.pre-commit-config.yaml` & `inciweb-wildfires-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-1.0.0/CODE_OF_CONDUCT.md` & `inciweb-wildfires-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-1.0.0/LICENSE` & `inciweb-wildfires-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-1.0.0/PKG-INFO` & `inciweb-wildfires-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inciweb-wildfires
-Version: 1.0.0
+Version: 1.1.0
 Summary: Download wildfire incidents data from InciWeb
 Home-page: http://www.github.com/datadesk/inciweb-wildfires
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/inciweb-wildfires
```

### Comparing `inciweb-wildfires-1.0.0/Pipfile.lock` & `inciweb-wildfires-1.1.0/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807035519125683%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'5ce0d53eeccf59bab144b465da5ed79a36a53bfd182b280ce988f7d74b47e866'}}",*

 * * "'develop'": "{'jinja2': {'hashes': "*

 * *              "['sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369', "*

 * *              "'sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d'], "*

 * *              "'version': '==3.1.4', 'index': 'pypi'}, 'mdit-py-plugins': OrderedDict([('hashes', "*

 * *              "['sha256:b51b3bb70691f57f974e257e367107857a93b36f322a […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "bccbc7eabc4a929b5563f4449b4afb86f460b30561e6ed0397c59eff69c00e31"
+            "sha256": "5ce0d53eeccf59bab144b465da5ed79a36a53bfd182b280ce988f7d74b47e866"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.10"
         },
         "sources": [
             {
@@ -387,19 +387,20 @@
                 "sha256:daf276ddf234bea897ef14f43c4e1bf9eefeac7b7a82a4dd69228ac20acff68d"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==4.0.0"
         },
         "jinja2": {
             "hashes": [
-                "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
-                "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
+                "sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369",
+                "sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d"
             ],
+            "index": "pypi",
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.3"
+            "version": "==3.1.4"
         },
         "keyring": {
             "hashes": [
                 "sha256:26fc12e6a329d61d24aa47b22a7c5c3f35753df7d8f2860973cf94f4e1fb3427",
                 "sha256:7230ea690525133f6ad536a9b5def74a4bd52642abe594761028fc044d7c7893"
             ],
             "markers": "python_version >= '3.8'",
@@ -483,14 +484,22 @@
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
+        "mdit-py-plugins": {
+            "hashes": [
+                "sha256:b51b3bb70691f57f974e257e367107857a93b36f322a9e6d44ca5bf28ec2def9",
+                "sha256:d8ab27e9aed6c38aa716819fedfde15ca275715955f8a185a8e1cf90fb1d2c1b"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==0.4.0"
+        },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
@@ -541,14 +550,23 @@
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
+        "myst-parser": {
+            "hashes": [
+                "sha256:7c36344ae39c8e740dad7fdabf5aa6fc4897a813083c6cc9990044eb93656b14",
+                "sha256:ea929a67a6a0b1683cdbe19b8d2e724cd7643f8aa3e7bb18dd65beac3483bead"
+            ],
+            "index": "pypi",
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.0"
+        },
         "nh3": {
             "hashes": [
                 "sha256:0316c25b76289cf23be6b66c77d3608a4fdf537b35426280032f432f14291b9a",
                 "sha256:1a814dd7bba1cb0aba5bcb9bebcc88fd801b63e21e2450ae6c52d3b3336bc911",
                 "sha256:1aa52a7def528297f256de0844e8dd680ee279e79583c76d6fa73a978186ddfb",
                 "sha256:22c26e20acbb253a5bdd33d432a326d18508a910e4dcf9a3316179860d53345a",
                 "sha256:40015514022af31975c0b3bca4014634fa13cb5dc4dbcbc00570acc781316dcc",
@@ -758,14 +776,21 @@
                 "sha256:1e09160a40b956dc623c910118fa636da93bd3ca0b9876a7b3df90f07d691560",
                 "sha256:9a5160e1ea90688d5963ba09a2dcd8bdd526620edbb65c328728f1b2228d5ab5"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.9'",
             "version": "==7.2.6"
         },
+        "sphinx-palewire-theme": {
+            "hashes": [
+                "sha256:f009e70d388f314c42c9a5cab9e5c7d8f8ea90ffe9acc10932cbcd6986ed105b"
+            ],
+            "index": "pypi",
+            "version": "==0.0.18"
+        },
         "sphinxcontrib-applehelp": {
             "hashes": [
                 "sha256:c40a4f96f3776c4393d933412053962fac2b84f4c99a7982ba42e09576a70619",
                 "sha256:cb61eb0ec1b61f349e5cc36b2028e9e7ca765be05e49641c97241274753067b4"
             ],
             "markers": "python_version >= '3.9'",
             "version": "==1.0.8"
```

### Comparing `inciweb-wildfires-1.0.0/data/incidents.json` & `inciweb-wildfires-1.1.0/data/incidents.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8668079096045198%*

 * *Differences: {"'features'": "{0: {'geometry': {'coordinates': [-107.871944, 37.323333]}, 'properties': "*

 * *               "{'changed': '6 days 5 hours ago', 'created': '<time "*

 * *               'datetime="2021-07-18T13:48:57-04:00">2021-07-18</time>\\n\', '*

 * *               "'field_incident_overview': '<p>On May 8, 2023, conditions were good for ignitions "*

 * *               'to start on the Animas City Mountain. The project took the whole week to make sure '*

 * *               'the prescribed fire was an success. Ignitions were com […]*

```diff
@@ -1,55 +1,55 @@
 {
     "features": [
         {
             "geometry": {
                 "coordinates": [
-                    -105.086111,
-                    40.558889
+                    -107.871944,
+                    37.323333
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 day 6 hours ago",
-                "created": "<time datetime=\"2015-11-05T09:08:58-05:00\">2015-11-05</time>\n",
+                "changed": "6 days 5 hours ago",
+                "created": "<time datetime=\"2021-07-18T13:48:57-04:00\">2021-07-18</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p><span><strong>Pile Burning for 2023-2024:</strong></span></p><p><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001GivvFcc-tevUzDYrb0Gg4UpVPrfqSVl4JAAusVwHGRLqUMVRAXqh61IB-4CKDgb8PgEM2lDZDpwfVEFnWFNRcjKigIgrDFwwR8QpaLeaxmhfBaSN-FaMc_U0P6HKTv9kzhAF5p5Y2GKaRPetAPbeeEfbVrjJLfMgFuq3qSqebfcNcxLebe6j9mBCiWcDKtPjm-jc8pb1-cik0JvLa7-dA4Xx6F5VbyTbBWLLlaLP55UhN_zdoDgu-I86tdLpZBZy1xtVFQDiA3liPWb5zl_FBB9bkHChexVIy4LoMCqYm3ttCabjN-qlyncaj46VmvrZOCrJLW4O9xRlrm_ggTQMkGBHYHJjWl0GzkVo2pZEW3NUA2nh_UC_mf9GTHnEv8eRUDqum0lGuAZuLGomJGGMR8kQxin6COln%26c%3Dp9KqBFwz5AmuJUEREBmnKB7Uubc2Apvfey7W_5_-v6jwmIxlSQc7xg%3D%3D%26ch%3Dcp3EVjrm9p78Ut1VlhMYW2acMfEeS6DsVCfX1tHbtHhsUi5EMFpE8Q%3D%3D&amp;data=05%7C01%7Cvictoria.ibarra%40usda.gov%7C93a28af96c9c49c0ace308dbe172625f%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C1%7C0%7C638351653617355410%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=DHK740qbPk7vfkQeM3d09VrzerI7QbfIxfQgpYokyvY%3D&amp;reserved=0\"><span><strong>Sign up to receive a weekly email</strong></span></a><span><strong>\u00a0</strong>newsletter about\u00a0pile burning projects in your area (select Forest Health and Fire for your zone).\u00a0 Have questions? See our </span><a href=\"https://www.fs.usda.gov/detail/arp/fire/?cid=fsm91_058291\"><span>Pile Burning FAQ</span></a><span> or email </span><a href=\"mailto:ARPFireInfo@usda.gov\"><span>ARPFireInfo@usda.gov</span></a><span>.</span></p><p><span>Regular burning activity notifications will be posted on this Inciweb page under \"Announcements.\"\u00a0</span></p><p><span><strong>What is pile burning?</strong></span></p><p><span>Pile burning is a type of prescribed fire that helps remove woody debris from the forests, reducing the potential of more impactful, unplanned fire activity at other times of the year. Pile burning helps eliminate branches, limbs, twigs and small logs that can't easily be removed through other means due to topography, access or cost feasibility. Pile burning typically follows forest thinning projects in overgrown forests. If heavy machinery was used to conduct the thinning, the piles may be much larger than if thinning and piling was completed by hand using chainsaws.\u00a0</span></p><p><span>Before burning piles, fire managers track hyper-localized weather forecasts to check temperatures, snowpack conditions and wind. Snow and cooler temperatures are key tools in helping contain fire behavior while wind is an important factor in aiding smoke dispersal. Firefighters use air quality monitoring stations in areas where they plan on burning.</span></p><p><span>Smoke, flames, and glowing embers are often visible, and are a normal part of pile burning operations. Mild fire behavior between piles is expected and is also beneficial for future wildfire risk reduction. This can include forest litter between piles and lower limbs of trees. \u00a0Once burning has begun, firefighters patrol and monitor burned piles until there is no longer any heat emitted.\u00a0</span></p><p><span>This work is part of the\u00a0</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001GivvFcc-tevUzDYrb0Gg4UpVPrfqSVl4JAAusVwHGRLqUMVRAXqh62er91EqRMexV5h4aIUoB0Yk5CJIEi6z9lLwq-Ydxeub9V334nOSX2nXnq5BrpHeyR0ofshlyQREJm_TLpC4h3eaGamv4e1tGQvPi1Y0ykgD-tOJyaYFUreY6cGA2KIlUYDeTwnG6NhA%26c%3Dp9KqBFwz5AmuJUEREBmnKB7Uubc2Apvfey7W_5_-v6jwmIxlSQc7xg%3D%3D%26ch%3Dcp3EVjrm9p78Ut1VlhMYW2acMfEeS6DsVCfX1tHbtHhsUi5EMFpE8Q%3D%3D&amp;data=05%7C01%7Cvictoria.ibarra%40usda.gov%7C93a28af96c9c49c0ace308dbe172625f%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C1%7C0%7C638351653617355410%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=WBQ7IgL6IwVgqu%2FkJCbEQK%2BlJFwhO1iMxUXqgxiAgpg%3D&amp;reserved=0\"><span><strong>National Wildfire Crisis Strategy</strong></span></a><span>\u00a0effort to reduce the impacts of unplanned, large-scale fires on watersheds, wildlife habitat, recreation and communities. Fire is a natural and important part of a healthy Colorado ecosystem. With help from the\u00a0</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001GivvFcc-tevUzDYrb0Gg4UpVPrfqSVl4JAAusVwHGRLqUMVRAXqh65eytHHLyY6_O4z26QjK4B-vaBmW65xtGOgeIliQhShzDwr_IXrEosOglMhQ0SBa-jSOEr4JDIinMocx_MzjP6LH2FhoMwgUTg%3D%3D%26c%3Dp9KqBFwz5AmuJUEREBmnKB7Uubc2Apvfey7W_5_-v6jwmIxlSQc7xg%3D%3D%26ch%3Dcp3EVjrm9p78Ut1VlhMYW2acMfEeS6DsVCfX1tHbtHhsUi5EMFpE8Q%3D%3D&amp;data=05%7C01%7Cvictoria.ibarra%40usda.gov%7C93a28af96c9c49c0ace308dbe172625f%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C1%7C0%7C638351653617355410%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=dLo6YHDYA9A5h9%2B%2Fe91ZNz3sk5dGjcLOpThE%2BtYQjDQ%3D&amp;reserved=0\"><span><strong>Northern Colorado Fireshed Collaborative</strong></span></a><span>\u00a0and our community partners, prescribed fire on the Arapaho and Roosevelt National Forests and adjacent public and private lands is helping prepare our forests for unplanned fire when it happens.\u00a0</span></p><p><strong>Learn more:</strong></p><p><span>To view all prescribed fire projects across the Arapaho and Roosevelt National Forests, check out our </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a\"><span>new interactive map</span></a><span>. Zoom into the location you are interested in, click on a prescribed burn unit and learn more about its status.\u00a0</span></p><p><span>Fire managers work with the Colorado Air Pollution Control Division to reduce the impacts of smoke on the public. For more information on how fire smoke may affect your health, see the\u00a0</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001GivvFcc-tevUzDYrb0Gg4UpVPrfqSVl4JAAusVwHGRLqUMVRAXqh65inXleRY-_ixKOA7ScyP3ihg4YroOYFTMsnjZlI_a4dWKMIwrAAYs-yfKpKtBKKreYdyyWA9PrN7FTw3zS-JxxHYy1Z24pttcpMqjalnJPR--zHrEwQWL7RfzvCIsb-_E-w-aXAsMYQMhsiyJX61nE%3D%26c%3Dp9KqBFwz5AmuJUEREBmnKB7Uubc2Apvfey7W_5_-v6jwmIxlSQc7xg%3D%3D%26ch%3Dcp3EVjrm9p78Ut1VlhMYW2acMfEeS6DsVCfX1tHbtHhsUi5EMFpE8Q%3D%3D&amp;data=05%7C01%7Cvictoria.ibarra%40usda.gov%7C93a28af96c9c49c0ace308dbe172625f%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C1%7C0%7C638351653617355410%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=r%2BnI9hMry8rlUzyZww6SIzd7O2kY%2BKzUzM3gLLO1OW0%3D&amp;reserved=0\"><span><strong>Colorado Department of Public Health &amp; Environment</strong></span></a><span>.\u00a0</span><br /><span><strong>\u00a0</strong></span><br /><span><strong>Areas on the Sulphur Ranger District (Grand County) with hand and machine piles ready for burning:\u00a0</strong></span></p><ul><li><span>Near Fair Tracts, east of Tabernash\u00a0along Water Board Rd (FSR 128): </span><a href=\"https://tinyurl.com/3ns7ph5n\"><span>Map</span></a></li><li><span>West of Snow Mountain Ranch: </span><a href=\"https://tinyurl.com/ynef7nns\"><span>Map</span></a></li><li><span>6 miles east of Granby: </span><a href=\"https://tinyurl.com/yd6kce38\"><span>Map</span></a></li><li><span>South of County Road 55 along the top of Blue Ridge: </span><a href=\"https://tinyurl.com/3muhbfxf\"><span>Map</span></a></li><li><span>West of County Road 50 at the Horseshoe Trailhead: </span><a href=\"https://tinyurl.com/ythvbmym\"><span>Map</span></a><span>\u00a0</span></li><li><span>Between Vasquez and East Elk Creeks on FSR 159, West of Winter Park Resort: </span><a href=\"https://tinyurl.com/mpapas4b\"><span>Map</span></a></li><li><span>Bottle Pass between Ptarmigan and Bottle Peak: </span><a href=\"https://tinyurl.com/2p97y9ck\"><span>Map</span></a></li></ul><p><span><strong>Areas on the Clear Creek Ranger District (Clear Creek, Gilpin, and Jefferson County) with hand piles ready for burning:\u00a0</strong></span></p><ul><li>Yankee Hill Area <a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.52,39.83&amp;level=13\"><span>Map</span></a><ul><li><em><span>Intersection of<strong>\u00a0</strong>HWY 119 and HWY 46, East of HWY 119, and South of HWY 46 (completed)</span></em></li><li><span>1 mile north of Gilpin County School, at the end of FS Trail 732</span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.52,39.83&amp;level=13\"><span> </span></a><em><span>(completed)</span></em></li><li><span>2 miles west of Central City, west of the intersection of Bald Mountain Road and FS Road 273.2 </span><em><span>(completed)</span></em></li></ul></li><li><span>Cub Creek Trailhead, 5 miles SW of Evergreen </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.38,39.565&amp;level=16\"><span>Map</span></a></li></ul><p><span><strong>Areas on the Boulder Ranger District (Gilpin and Boulder Counties) with hand and machine piles ready for burning:\u00a0</strong></span></p><ul><li><span>Lump Gulch Area (Gilpin County) </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.48,39.91&amp;level=14\"><span>Map</span></a><ul><li><em><span>Half-mile north of\u00a0Rollinsville\u00a0on Westside of Highway 119 (Peak to Peak) (completed)</span></em></li><li><span>West side of Lump Gulch Road, 1.5 miles south of Rollinsville on west side of Highway 119 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.5,39.895&amp;level=16\"><span>Map</span></a></li><li><span>Gilpin County south and north sides of Gilpin Road, 3 miles south of Rollinsville on west side of Highway 119 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.48,39.89&amp;level=15\"><span>Map</span></a><span> </span><em><span>(completed)</span></em></li><li><span>Off of South Beaver Rd (South Side) mile east of Highway 119</span></li></ul></li><li><span>James Creek Area </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.44,40.10&amp;level=13\"><span>Map</span></a><ul><li><span>1.5 miles northwest of Jamestown, west of\u00a0County Road 87</span></li><li><span>Half mile south of Jamestown or quarter mile east of Bar K Ranch</span></li><li><span>2 miles east of Peak-to-Peak Highway on County Road 52</span></li><li><span>Half-mile north of Cal-Wood Education Center</span></li></ul></li><li><span>St.\u00a0Vrain Area \u00a0</span><ul><li><span>In Meeker Park </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.53,40.24&amp;level=15\"><span>Map</span></a></li><li><span>5 miles west of Lyons, north side of Ralph Price Reservoir (Button Rock) </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.37,40.23&amp;level=15\"><span>Map</span></a></li></ul></li><li><span>Forsythe Area </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.413,39.94&amp;level=13\"><span>Map</span></a><ul><li><span>2 miles east of Nederland, north of Magnolia Road, adjacent to FS Trail 606 and near the intersection of Magnolia Road and Lazy Z Road </span><em><span>(completed)</span></em></li><li><span>1 mile northeast of Rollinsville, just north of Shoshone Road </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.48,39.93&amp;level=16\"><span>Map</span></a><span> </span><em><span>(completed)</span></em></li><li><span>Approximately mile maker 4.5 of Magnolia Road, north and south of Magnolia Road off FS Road 321 and 302 </span><em><span>(completed)</span></em></li><li><span>1.5 miles northwest of Wondervu, west side of Gross Reservoir</span></li><li><span>2 miles southwest of Pinecliffe, east of South Beaver Road off </span><em><span>Emory Road ,</span></em><span> La Chula Road, and Wedgewood Road </span><em><span>(completed)</span></em></li></ul></li></ul><p><span><strong>Areas on the Canyon Lakes Ranger District (Larimer County) with hand and machine piles ready for burning:\u00a0\u00a0</strong></span></p><ul><li><span>Cedar Park 1 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.304,40.443&amp;level=14\"><span>Map</span></a>: (hand piles) 1 mile northeast of Drake from the intersection of US34 and CR43</li><li><span>Cedar Park 2 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.347,40.458&amp;level=14\"><span>Map</span></a>: (hand piles) 1 mile north of Drake from the intersection of US34 and CR43</li><li><span>Cedar Park 3 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.278,40.457&amp;level=14\"><span>Map</span></a><span>: (hand piles) 3 miles east of Drake and north of US34 at Cedar Cove</span></li><li><span>Glen Haven 2 &amp; 3 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.465,40.45&amp;level=14\"><span>Map</span></a>: (hand piles) adjacent to Glen Haven on both sides of CR43</li><li><span>Glen Haven 4 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.437,40.404&amp;level=14\"><span>Map</span></a>: (hand piles) 3 miles east of Estes Park at the intersection of US34 and FSR117, north of Glen Comfort</li><li><span>Thompson River 4 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.371,40.355&amp;level=14\"><span>Map</span></a><span>: (hand piles) 6 miles east of Estes Park, along FSR122 (Pole Hill Road)</span></li><li><span>Thompson River 5 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.41,40.33&amp;level=14\"><span>Map</span></a>: (hand piles) 4 miles southeast of Estes Park, at the intersection of US36 and FSR124</li><li><span>Magic Sky 4 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.457,40.776&amp;level=14\"><span>Map</span></a>: (hand piles) 5 miles southeast of Red Feather Lakes and north of CR74E near Red Feather Highlands/DU Mountain Campus</li><li><span>Red Feather 5 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.483,40.859&amp;level=13\"><span>Map</span></a>: (hand piles) 4 miles northeast of Red Feather Lakes, along CR67J (Prairie Divide Road)</li><li><span>Cameron Peak </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.629,40.824&amp;level=14\"><span>Map</span></a>: (machine piles) along roads west of Crystal Lakes subdivision and near the Killpecker repeater site at CR86 (Deadman Road) and FSR300</li><li><span>Elkhorn 3 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.654,40.759&amp;level=14\"><span>Map</span></a>: (machine piles) 3 miles southwest of Red Feather Lakes and west along FSR517 (Bald Mountain Road)</li><li><span>Elkhorn 2019 </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.617,40.745&amp;level=14\"><span>Map</span></a>: (machine piles) 2 miles southwest of Red Feather Lakes and west along CR69 (Manhattan Road)</li><li><span>Roach </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-106.177,40.987&amp;level=14\"><span>Map</span></a>: (machine piles) 1 mile south of Mountain Home, WY, along FSR516</li><li><span>Tower Timber Sale </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.77,40.819&amp;level=14\"><span>Map</span></a><span>: (machine piles) 5 miles southwest of Crystal Lakes subdivision at the intersection of CR86 (Deadman Road) and FSR170 (Deadman Lookout Road)\u00a0</span></li><li><span>Cow Creek </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.752,40.885&amp;level=14\"><span>Map</span></a><span>: (machine piles) 4 miles west of Crystal Lakes subdivision at the intersection of FSR169 (Pearl Beaver Road) and FSR 199\u00a0</span></li><li><span>Lonesome Timber Sale </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.677,40.789&amp;level=14\"><span>Map</span></a><span>: (machine piles) 3 miles south of Crystal Lakes subdivision at the intersection of CR86 (Deadman Road) and FSR300</span></li><li><span>Diamond View </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.525,40.967&amp;level=14\"><span>Map</span></a><span>: (machine piles) 11 miles northeast of Red Feather Lakes, along CR59 and FSR184 (adjacent to the Mill Creek subdivision)</span></li><li><span>Devils Creek </span><a href=\"https://usfs.maps.arcgis.com/apps/webappviewer/index.html?id=abefa61010ee43418aa942f949d2cf5a&amp;center=-105.568,40.936&amp;level=14\"><span>Map</span></a><span>: (machine piles) 5 miles north of Crystal Lakes Subdivision; at the intersection of CR80C and FSR182</span></li></ul><p>\u00a0</p>",
+                "field_incident_overview": "<p>On May 8, 2023, conditions were good for ignitions to start on the Animas City Mountain. The project took the whole week to make sure the prescribed fire was an success. Ignitions were completed on Friday, May 12th, for a total of 495 acres treated. Firefighters patrolled and secured the edges for weeks after until moisture came into the area. Check out this YouTube video about the project&nbsp;<a href=\"https://youtu.be/x78BLZyVvKA?si=g_B8r3rP_llqVZsv\">https://youtu.be/x78BLZyVvKA?si=g_B8r3rP_llqVZsv</a>.&nbsp;</p>\n\n<p>In order to reduce the risk of high-intensity wildfire, improve forest health and wildlife habitat, the Bureau of Land Management Tres Rios Field Office has planned a prescribed fire treatment for up to 652 acres on Animas City Mountain in Durango, Colorado. Dependent on weather and the availability of firefighters to conduct the operation, the prescribed burns could take place in spring and fall months. An Environmental Assessment which covers this, as well as other treatment areas in La Plata County, has been completed and is available here:&nbsp;<a href=\"https://eplanning.blm.gov/eplanning-ui/project/1505044/510\">Final Environmental Assessment</a>.</p>\n\n<p>Prescribed fires require a comprehensive plan consisting of 21 elements. The plan outlines the methodical process from inception to completion. The Animas City Mountain project is expected to take 2-3 days for ignitions, with additional time to patrol the area and extinguish hot spots. The mountain has been divided into seven units or compartments. Crews are expected to begin burning on the top of the mountain by slowly lighting an edge that has already been thinned with chainsaws. Once a secure edge or \u201cblack line\u201d has been established, firefighters ignite the interior of each unit, one unit at a time. The fire then burns back toward the secured, black edge. This methodical approach allows firefighters opportunities to halt ignitions if burning conditions become undesirable. Examples of undesirable conditions are fire behavior that is too active/not active enough, and poor smoke dispersion. Firefighters will also have water on hand to cool things down if fire activity grows beyond a desirable level.</p>\n\n<p>Prescribed fires are watched carefully by firefighters around the burn, lookouts at more distant locations, aerially (helicopters, planes, drones), and with calibrated smoke monitors. These monitors will be placed at locations around the burn to track smoke impacts in real time. The BLM and Colorado Department of Public Health and Environment Air Quality (CPDHE) have been working since 2018 to develop a permit that accomplishes the burn while minimizing smoke impacts to the surrounding area. Prescribed fire smoke may affect your health. For more information, visit&nbsp;<a href=\"https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health\">https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health</a>. Prescribed fires are a tool to minimize smoke impacts to communities by careful selection of when fires burn and when they stop. Firefighters utilize compartments to halt the fire from spreading overnight, whereas wildfire continue to burn overnight when smoke is likely to settle into low lying areas where communities are located. Residual smoke from the interior areas of the compartments is anticipated, but the goal is to start early in the day and stop early in the evening to give material as much time as possible to be consumed before night-time cooling occurs and smoke sinks into the valley.</p>\n\n<p>Ideal timing (windows) for the project occurs during the Spring and Fall when conditions are more favorable for low-intensity fire. Fuel (vegetation) and weather conditions must fall within a predetermined \u201cprescription\u201d that is known to yield desirable results while still being controllable by the fire personnel conducting the burn. Dissipation of smoke is also part of the prescription. Prescription development has been done by local fire experts who utilize fire behavior computer modeling software combined with decades of experience conducting prescribed burn in southwest Colorado.</p>\n\n<p>This project is a coordinated effort between the federal/county/local government, NGOs, emergency managers, fire departments, public health officials, state smoke regulators and nearby residents. The burn is planned to take place over the course of 2-3 days. Brief closure of Animas City Mountain during the ignitions will occur for public and firefighter safety. The containment lines used for the project will consist of BLM designated trails. The units will be ignited using a combination of ground and aerial resources and will be patrolled/mopped up until out.</p>\n\n<p>The project is part of the BLM\u2019s ongoing commitment to protecting human health and safety while maintaining or enhancing forest and woodland health and functionality. The Animas City Mountain area was previously masticated in 2010 which altered the vertical structure of the forest stand to reduce the risk of catastrophic fire. Mastication is a treatment method where the understory is mowed and mulched with a large machine. The mulched material slowly decomposes, while the understory regrows. Mastication and prescribed fire are effective in preventing fires from leaving the ground and becoming \u201ccrown\u201d fires where the entire trees or stand of trees burn. Treatments thin and remove some of the large dense understory or \u201cladder fuels\u201d.</p>\n\n<p>Vegetation, however, grows back and requires maintenance. Prescribed fire is the best treatment option for this forest type, if possible, after the initial mechanical treatment. While consuming some of the standing vegetation; prescribed fire also eliminates material left on the ground from both mastication and the natural shedding of leaves, needles, etc. Fire is the only natural process used as a treatment method and produces the most effective results for hazardous fuel reduction while enhancing woodland health. Ponderosa pine woodlands are a drought resistant species that have evolved with a natural cycle of frequent, low-intensity fire.</p>\n\n<p>Prescribed fire mimics this natural process and improves forage for wildlife, as well as increasing plant diversity by creating breaks in the understory where grasses and flowers can thrive.</p>\n\n<p>Every year the west is impacted by large catastrophic wildfires. Prescribed fires and other treatment methods lessen the impacts of future fires and increase the likelihood firefighters can work safely and be effective at stopping fires in and near treated areas.</p>\n\n<p>&nbsp;</p>",
                 "field_percent_of_perimeter": "0",
-                "field_title_and_unit": "COARF Arapaho Roosevelt National Forests Pile Burning",
-                "field_unit_code": "COARF",
-                "id": "291567",
-                "lat_deg": "40",
-                "lat_min": "33",
-                "lat_sec": "32",
-                "long_deg": "105",
-                "long_min": "5",
-                "long_sec": "10",
+                "field_title_and_unit": "COSJD Animas City Mountain Prescribed Burn",
+                "field_unit_code": "COSJD",
+                "id": "291575",
+                "lat_deg": "37",
+                "lat_min": "19",
+                "lat_sec": "24",
+                "long_deg": "107",
+                "long_min": "52",
+                "long_sec": "19",
                 "measurement_type": "Acres",
                 "size": "",
-                "title": "Arapaho &amp; Roosevelt National Forests Pile Burning",
+                "title": "Animas City Mountain Prescribed Burn",
                 "type": "Prescribed Fire",
-                "urlPath": "/coarf-arapaho-roosevelt-national-forests-pile-burning"
+                "urlPath": "/cosjd-animas-city-mountain-prescribed-burn"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
                     -108.825556,
                     37.9025
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 3 days ago",
+                "changed": "6 days 5 hours ago",
                 "created": "<time datetime=\"2021-09-23T08:43:22-04:00\">2021-09-23</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p>The Bureau of Land Management Southwest District plans to conduct several prescribed burns beginning early October or as conditions allow. The prescribed burn projects will be on the Gunnison, Tres Rios and Uncompahgre Field Offices. The planned burns are part of larger projects to reduce hazardous fuels; protect wildland-urban interface communities; improve big game habitat, sage grouse habitat, and range conditions; and reintroduce fire to a fire-adapted ecosystem to restore healthy forests and species diversity. \u00a0<br /><br />\nWhile no road closures are expected during the projects, camping near the units is discouraged due to increased traffic and likelihood of smoke in the area, particularly at night. Multiple days of burning may occur throughout the fall into the winter, as fuel conditions and weather permit. Project areas will be monitored once completed to ensure public safety. While smoke may be visible in the burn area at times, most of the smoke will lift and dissipate during the warmest parts of the day. Expect visible smoke in the area for several days after each burn is completed as vegetation in the interior continues to smolder.\u00a0<br /><br />\nThe BLM obtained smoke permits from the Colorado State Air Pollution Control Division, which identify atmospheric conditions under which the burns can be implemented. Prescribed fire smoke may affect your health.\u00a0For more information, visit <a href=\"https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health\">https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health</a>.<br />\n\u00a0</p>\n\n<p>Specific information on upcoming prescribed burn projects can be found in the News section.</p>",
+                "field_incident_overview": "<p>The Bureau of Land Management Southwest District plans to conduct several prescribed burns beginning early October or as conditions allow. The prescribed burn projects will be on the Gunnison, Tres Rios and Uncompahgre Field Offices. The planned burns are part of larger projects to reduce hazardous fuels; protect wildland-urban interface communities; improve big game habitat, sage grouse habitat, and range conditions; and reintroduce fire to a fire-adapted ecosystem to restore healthy forests and species diversity. &nbsp;<br>\n<br>\nWhile no road closures are expected during the projects, camping near the units is discouraged due to increased traffic and likelihood of smoke in the area, particularly at night. Multiple days of burning may occur throughout the fall into the winter, as fuel conditions and weather permit. Project areas will be monitored once completed to ensure public safety. While smoke may be visible in the burn area at times, most of the smoke will lift and dissipate during the warmest parts of the day. Expect visible smoke in the area for several days after each burn is completed as vegetation in the interior continues to smolder.&nbsp;<br>\n<br>\nThe BLM obtained smoke permits from the Colorado State Air Pollution Control Division, which identify atmospheric conditions under which the burns can be implemented. Prescribed fire smoke may affect your health.&nbsp;For more information, visit <a href=\"https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health\">https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health</a>.<br>\n&nbsp;</p>\n\n<p>Specific information on upcoming prescribed burn projects can be found in the News section.</p>",
                 "field_percent_of_perimeter": "0",
                 "field_title_and_unit": "COSJD Southwest District BLM Prescribed Fire",
                 "field_unit_code": "COSJD",
                 "id": "291580",
                 "lat_deg": "37",
                 "lat_min": "54",
                 "lat_sec": "9",
@@ -69,19 +69,19 @@
                 "coordinates": [
                     -107.893023,
                     37.273411
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "2 days 3 hours ago",
+                "changed": "1 week ago",
                 "created": "<time datetime=\"2022-11-02T15:33:16-04:00\">2022-11-02</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p><span>The San Juan National Forest has wrapped up winter pile burning and is planning the 2024 broadcast prescribed fire season. Fire Officials will begin performing prescribed fires as weather, fuel, and fire resources permit.\u00a0</span></p><p><a><span>The forests in Southwest Colorado are part of a fire-adapted ecosystem, which historically experienced frequent, low intensity fires on a large scale. </span></a><span>Prescribed fire replicates that fire regime and increases the area on our landscape that has been burned at low and moderate conditions.</span></p><p><span>Reintroduction of prescribed fire is necessary to improve and restore vegetative conditions. This effort will reduce hazardous ground fuels, lessen the risk of unplanned large-scale wildfire, help restore ponderosa pine ecosystems, and improve wildlife habitat. Prescribed fire also reduces the ladder fuels that can carry fire into the canopy, killing mature trees.</span></p><h3>2024 Broadcast Prescribed Fire Plans:</h3><p><strong>DOLORES RANGER DISTRICT:</strong></p><ul><li>Haycamp Mesa 4,583 Acres</li><li>Salter 2,943 Acres</li><li>Boggy Draw 7,615 Acres (<a href=\"https://inciweb.nwcg.gov/incident-publication/cosjf-2024-san-juan-national-forest-prescribed-fire-program/san-juan-national-forest-issues-trail,-road-closures-for-boggy-draw-area-prescribed-fire-operations-04-08-2024\">see news release</a>)</li></ul><p><strong>COLUMBINE RANGER DISTRICT (</strong><a href=\"https://inciweb.nwcg.gov/incident-publication/cosjf-2024-san-juan-national-forest-prescribed-fire-program/prescribed-fires-planned-for-the-columbine-ranger-district-03-12-2024\"><strong>see news release for details</strong></a><strong>):</strong></p><ul><li>Vallecito Piedra 1,135 Acres<ul><li>A small 22-acre burning operation is planned for April 10th within the Wickinson burn unit. Snow remains on the north side of the unit, delaying additional burning operations.</li></ul></li><li>Sauls Creek 1,640 Acres</li></ul><p><strong>PAGOSA RANGER DISTRICT:</strong></p><ul><li>Brockover-Devil Creek 2,100 Acres</li></ul><p>\u00a0</p><p>_____________</p><h3><strong>2023/24 Winter Pile Burning Accomplishments:\u00a0</strong></h3><p><strong>DOLORES RANGER DISTRICT:</strong></p><p><span>Smoke may be visible from State Highway 184, State Highway 145, and U.S. Route 491.</span></p><ul><li><span>Haycamp Mesa area (427 acres, 750 piles) near FSRs 556 and 492, south of Beef Pasture Reservoir</span></li><li><span>Taylor Mesa area (145 acres, 44 piles) near FSRs 545 and 692</span></li><li><span>Salter area (321 acres, 267 piles) near FSRs 514, 504, 519 and 293, northwest of Salter Y</span></li><li><span>Lake Canyon area (518 acres, 336 piles) near FSRs 506, 504, 508, 514, 215, and 216 near Cow Canyon\u00a0</span></li></ul><p><strong>COLUMBINE RANGER DISTRICT:</strong></p><ul><li><span>Sauls Creek (110 acres, 1800 piles) near FS roads 755, 755.A, 131, and 131.C\u00a0</span></li><li><span>Junction Creek (90 acres, 75 piles) near FS road 171, in the Log Chutes trail area\u00a0</span></li><li><span>Fossett Gulch (40 acres, 100 piles) near FS roads 613 and 841</span></li><li><span>Baldy Mountain (623 acres, 60 slash piles) off of Beaver Meadows Road\u00a0</span></li></ul><p><strong>PAGOSA RANGER DISTRICT:</strong></p><ul><li><span>Lower portion of Turkey springs Road (FSR 629) near the powerlines</span></li><li><span>Turkey Springs Road near the Turkey Springs Guard Station\u00a0</span></li><li><span>Brockover Road (FSR 919), Buckles Lake Road (FSR 633)</span></li><li><span>Huerto Creek timber sale between Piedra Road (FSR 621) and Poison Park Road (FSR 644)\u00a0</span></li></ul>",
+                "field_incident_overview": "<p><span>The San Juan National Forest has wrapped up winter pile burning and the 2024 broadcast prescribed fire season is underway. Fire personnel have been performing prescribed fires as weather, fuel, and the availability of fire resources permit.&nbsp;</span></p><p><a><span>The forests in Southwest Colorado are part of a fire-adapted ecosystem, which historically experienced frequent, low intensity fires on a large scale. </span></a><span>Prescribed fire replicates that fire regime and increases the area on our landscape that has been burned at low and moderate conditions.</span></p><p><span>Reintroduction of prescribed fire is necessary to improve and restore vegetative conditions. This effort will reduce hazardous ground fuels, lessen the risk of unplanned large-scale wildfire, help restore ponderosa pine ecosystems, and improve wildlife habitat. Prescribed fire also reduces the ladder fuels that can carry fire into the canopy, killing mature trees.</span></p><h3>2024 Broadcast Prescribed Fire Plans:</h3><p><strong>DOLORES RANGER DISTRICT:</strong></p><ul><li>Haycamp Mesa 4,583 Acres<ul><li>May-June Unit 9, a 700 acre area is tentatively planned for burning if conditions permit.</li></ul></li><li>Salter 2,943 Acres</li><li>Boggy Draw 7,615 Acres (<a href=\"https://inciweb.nwcg.gov/incident-publication/cosjf-2024-san-juan-national-forest-prescribed-fire-program/san-juan-national-forest-issues-trail,-road-closures-for-boggy-draw-area-prescribed-fire-operations-04-08-2024\">see news release</a>) (<a href=\"https://inciweb.wildfire.gov/incident-publication/cosjf-2024-san-juan-national-forest-prescribed-fire-program/boggy-draw-prescribed-fire-closure-order-04-08-2024\">closure order</a>)<ul><li>May 9: Fire personnel burned approximately 1133 acres in Boggy Draw - Unit 20 (Butler's Corner) and Units 17 and 18 (Boggy Draw Trailhead) (<a href=\"https://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-04/FY24%20DOL%20Rx%20fire%20Overview_20240318_8.5x11_0.pdf?VersionId=sOL6HWKH1TkSGpdGaP2jfzxNQwjVTN5c\">see map</a>). Roads are open but an area closure is in place which will impact the Boggy Draw Trail system for some time. Follow this site or the San Juan National Forest on Facebook for updated information.</li></ul></li></ul><p><strong>COLUMBINE RANGER DISTRICT (</strong><a href=\"https://inciweb.nwcg.gov/incident-publication/cosjf-2024-san-juan-national-forest-prescribed-fire-program/prescribed-fires-planned-for-the-columbine-ranger-district-03-12-2024\"><strong>see news release for details</strong></a><strong>):</strong></p><ul><li>Vallecito Piedra 1,135 Acres<ul><li>April 21: Firefighters have completed 235 acres in the Wickenson East unit of the Vallecito-Piedra Project.</li></ul></li><li>Sauls Creek 1,640 Acres<ul><li>April 23: Firefighters completed 1,330 acres in Sauls Creek on April 22 and 23.&nbsp;</li></ul></li></ul><p><strong>PAGOSA RANGER DISTRICT</strong></p><ul><li>Brockover-Devil Creek 2,100 Acres</li></ul><p>&nbsp;</p><p>_____________</p><h3><strong>2023/24 Winter Pile Burning Accomplishments:&nbsp;</strong></h3><p><strong>DOLORES RANGER DISTRICT:</strong></p><p><span>Smoke may be visible from State Highway 184, State Highway 145, and U.S. Route 491.</span></p><ul><li><span>Haycamp Mesa area (427 acres, 750 piles) near FSRs 556 and 492, south of Beef Pasture Reservoir</span></li><li><span>Taylor Mesa area (145 acres, 44 piles) near FSRs 545 and 692</span></li><li><span>Salter area (321 acres, 267 piles) near FSRs 514, 504, 519 and 293, northwest of Salter Y</span></li><li><span>Lake Canyon area (518 acres, 336 piles) near FSRs 506, 504, 508, 514, 215, and 216 near Cow Canyon&nbsp;</span></li></ul><p><strong>COLUMBINE RANGER DISTRICT:</strong></p><ul><li><span>Sauls Creek (110 acres, 1800 piles) near FS roads 755, 755.A, 131, and 131.C&nbsp;</span></li><li><span>Junction Creek (90 acres, 75 piles) near FS road 171, in the Log Chutes trail area&nbsp;</span></li><li><span>Fossett Gulch (40 acres, 100 piles) near FS roads 613 and 841</span></li><li><span>Baldy Mountain (623 acres, 60 slash piles) off of Beaver Meadows Road&nbsp;</span></li></ul><p><strong>PAGOSA RANGER DISTRICT:</strong></p><ul><li><span>Lower portion of Turkey springs Road (FSR 629) near the powerlines</span></li><li><span>Turkey Springs Road near the Turkey Springs Guard Station&nbsp;</span></li><li><span>Brockover Road (FSR 919), Buckles Lake Road (FSR 633)</span></li><li><span>Huerto Creek timber sale between Piedra Road (FSR 621) and Poison Park Road (FSR 644)&nbsp;</span></li></ul>",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "COSJF 2024 San Juan National Forest Prescribed Fire Program",
                 "field_unit_code": "COSJF",
                 "id": "312546",
                 "lat_deg": "37",
                 "lat_min": "16",
                 "lat_sec": "24.2796",
@@ -101,19 +101,19 @@
                 "coordinates": [
                     -105.53797,
                     40.779597
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 1 day ago",
+                "changed": "3 weeks 3 days ago",
                 "created": "<time datetime=\"2022-11-08T12:02:21-05:00\">2022-11-08</time>\n",
                 "field_active": "1",
                 "field_incident_description": "The entire project area is 6,329 acres. In early October, firefighters successfully burned 470 acres. 553 acres have previously been burned in July 2023. ",
-                "field_incident_overview": "<p><strong>UPDATE (4/3/24)</strong><span> \u2013 If conditions allow, burning could begin as soon as mid-April 2024 on the Magic Feather Prescribed Burn. Firefighters are closely monitoring snow conditions in the area. Burning could begin when south-facing slopes dry and snow remains on north-facing slopes.\u00a0</span></p><p><span>-----------------------------------------------------------</span></p><p><span>The burn is located east and southeast of Red Feather Lakes. Firefighters successfully burned 775 acres in 2023. Appropriate, localized conditions must be met before ignitions can take place. Fire managers have been carefully monitoring these conditions, including favorable weather forecast (temperature, wind, precipitation, relative humidity), fuel moisture, smoke dispersal and staffing. Weather is monitored throughout the burn and burning is halted if conditions fall outside of the required conditions.</span></p><p><span>People in the surrounding area should expect to see smoke west of Livermore and Glacier View when operations are taking place. Smoke may also impact those using the Dowdy Lake Campgrounds and Day-Use Area. Prescribed fire smoke may affect your health. For more information about the potential health impacts of smoke, visit </span><a href=\"https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health\"><strong>Colorado Department of Public Health and Environment</strong></a><span>.\u00a0</span></p><p><span>This prescribed burn is part of the overall strategy on the Arapaho and Roosevelt National Forests to confront the </span><a href=\"https://www.fs.usda.gov/managing-land/wildfire-crisis\"><strong>Wildfire Crisis</strong></a><span>. Prescribed fire is one of the most efficient ways of reducing wildfire risk. Regularly conducting prescribed fires, which mimic nature, reduces the buildup of flammable vegetation and overgrowth. Even with the most thorough planning and preparation, the use of prescribed fire carries an innate level of risk that cannot be eliminated entirely. However, prescribed fire is one of the most efficient ways of reducing wildfire risk. Regularly conducting prescribed fires, which mimic nature, reduces the buildup of flammable vegetation and overgrowth.</span></p><p><span>\ufeff\ufeffTo receive updates, follow us on </span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001_4jQevMBOHm3ij4X-dPiBcWzTzhBlKNG7Ak20ATiL5hV8dbH0ztFvQihs44UwsWlSe5bGkI176N1h-l5TyqtuEYfaE-_LANcpc9obrtT3nKEAqFO18PTR_dqaAf8xPtNcyHOtfrqyMKc1KJyLkHLe0bNKsbpmaxc%26c%3Dtu6-bHUBD7B_o7CiWT7VjbjY3EQ2RGUdJBnV-2-5PJc7kz6ezD4ikQ%3D%3D%26ch%3DKkBmbkI9Pj8Pw596zy9vJ8hEwx5R_V70FL4MGPZT38jjcVXICPoHrQ%3D%3D&amp;data=05%7C01%7C%7C8d7f5e8910d04f77a0d108db467312f9%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638181304112273720%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=P1Ou3zBgeWBfIK4j%2BLeuEVKv5zx3UIfq4QcPlVYZJFY%3D&amp;reserved=0\"><strong>Facebook</strong></a><span> and </span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001_4jQevMBOHm3ij4X-dPiBcWzTzhBlKNG7Ak20ATiL5hV8dbH0ztFvQihs44UwsWlvNfg4L24yNGmpu9fPnYBAJtkHFFkIvXBbTSaxVAht5IWVcU3hkHisQptxY3jQ5vxqilRu7y7KVtWlVz_jX-eqQ%3D%3D%26c%3Dtu6-bHUBD7B_o7CiWT7VjbjY3EQ2RGUdJBnV-2-5PJc7kz6ezD4ikQ%3D%3D%26ch%3DKkBmbkI9Pj8Pw596zy9vJ8hEwx5R_V70FL4MGPZT38jjcVXICPoHrQ%3D%3D&amp;data=05%7C01%7C%7C8d7f5e8910d04f77a0d108db467312f9%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638181304112273720%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=xYh6uQsYifWyNPeUQOlhzbPuxGpy9a2r5%2FcjrVk80B0%3D&amp;reserved=0\"><strong>X</strong></a><span> and </span><a href=\"https://visitor.r20.constantcontact.com/manage/optin?v=001IYrlh1STq1nQ4D8XRO5B4Tvbd__skb5DEaSNzAHXRTWsJ95wGZldZ7zrkXvzVXksf3R6x_FiGGtTmBpzdxMnTnede0kaBf28EWf6JhMvjtJ1G2BxcsTGuuXwUui3wHLgc8u79l49Wyo2SYfQARrvjWhWttAZTbd2\"><span><strong>join our email list through Constant Contact</strong></span></a><span> and select list \"Forest Health &amp; Fire: North of Hwy 14 to Wyoming Border (Red Feather Lakes).\"</span></p>",
+                "field_incident_overview": "<p><strong>(4/24/24)</strong><span> \u2013 Test fire was unsuccessful due to fuel moisture. Crews are securing the test fire and beginning mop up. The area received additional rain this afternoon, so it will be too wet to burn tomorrow.</span></p><p><strong>(4/23/24)</strong><span> \u2013 If conditions allow, burning could begin April 24, 2024, on the Magic Feather Prescribed Burn located near Red Feather Lakes. Firefighters are closely monitoring snow conditions in the area and upcoming forecasts. Burning could begin when south-facing slopes are dry and snow remains on north-facing slopes.&nbsp;</span></p><p><span>A public field trip is planned for April 24. Sign up </span><a href=\"https://poudrewatershed.networkforgood.com/events/70939-live-prescribed-fire-visit-magic-feather-broadcast-burn-area?fbclid=IwZXh0bgNhZW0CMTEAAR3XwvAq9tcXLdAPp-_fZsikaS7AuK5ZTEKaKVXCf38p7LcpgLQQ5b2Xvvw_aem_Ac0R_6tUz7nxDUgoDA04bv8cDkvywYeibzNVK4H0cMw0tvV3OB8vMba9yfDRCUIO0q_p9RG35MFchHf_XKi0PrBb\"><span>here</span></a><span>.&nbsp;</span></p><p><span>-----------------------------------------------------------</span></p><p><span>The burn is located east and southeast of Red Feather Lakes. Firefighters successfully burned 775 acres in 2023. Appropriate, localized conditions must be met before ignitions can take place. Fire managers have been carefully monitoring these conditions, including favorable weather forecast (temperature, wind, precipitation, relative humidity), fuel moisture, smoke dispersal and staffing. Weather is monitored throughout the burn and burning is halted if conditions fall outside of the required conditions.</span></p><p><span>People in the surrounding area should expect to see smoke west of Livermore and Glacier View when operations are taking place. Smoke may also impact those using the Dowdy Lake Campgrounds and Day-Use Area. Prescribed fire smoke may affect your health. For more information about the potential health impacts of smoke, visit </span><a href=\"https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health\"><strong>Colorado Department of Public Health and Environment</strong></a><span>.&nbsp;</span></p><p><span>This prescribed burn is part of the overall strategy on the Arapaho and Roosevelt National Forests to confront the </span><a href=\"https://www.fs.usda.gov/managing-land/wildfire-crisis\"><strong>Wildfire Crisis</strong></a><span>. Prescribed fire is one of the most efficient ways of reducing wildfire risk. Regularly conducting prescribed fires, which mimic nature, reduces the buildup of flammable vegetation and overgrowth. Even with the most thorough planning and preparation, the use of prescribed fire carries an innate level of risk that cannot be eliminated entirely. However, prescribed fire is one of the most efficient ways of reducing wildfire risk. Regularly conducting prescribed fires, which mimic nature, reduces the buildup of flammable vegetation and overgrowth.</span></p><p><span>\ufeff\ufeffTo receive updates, follow us on </span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001_4jQevMBOHm3ij4X-dPiBcWzTzhBlKNG7Ak20ATiL5hV8dbH0ztFvQihs44UwsWlSe5bGkI176N1h-l5TyqtuEYfaE-_LANcpc9obrtT3nKEAqFO18PTR_dqaAf8xPtNcyHOtfrqyMKc1KJyLkHLe0bNKsbpmaxc%26c%3Dtu6-bHUBD7B_o7CiWT7VjbjY3EQ2RGUdJBnV-2-5PJc7kz6ezD4ikQ%3D%3D%26ch%3DKkBmbkI9Pj8Pw596zy9vJ8hEwx5R_V70FL4MGPZT38jjcVXICPoHrQ%3D%3D&amp;data=05%7C01%7C%7C8d7f5e8910d04f77a0d108db467312f9%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638181304112273720%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=P1Ou3zBgeWBfIK4j%2BLeuEVKv5zx3UIfq4QcPlVYZJFY%3D&amp;reserved=0\"><strong>Facebook</strong></a><span> and </span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001_4jQevMBOHm3ij4X-dPiBcWzTzhBlKNG7Ak20ATiL5hV8dbH0ztFvQihs44UwsWlvNfg4L24yNGmpu9fPnYBAJtkHFFkIvXBbTSaxVAht5IWVcU3hkHisQptxY3jQ5vxqilRu7y7KVtWlVz_jX-eqQ%3D%3D%26c%3Dtu6-bHUBD7B_o7CiWT7VjbjY3EQ2RGUdJBnV-2-5PJc7kz6ezD4ikQ%3D%3D%26ch%3DKkBmbkI9Pj8Pw596zy9vJ8hEwx5R_V70FL4MGPZT38jjcVXICPoHrQ%3D%3D&amp;data=05%7C01%7C%7C8d7f5e8910d04f77a0d108db467312f9%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638181304112273720%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=xYh6uQsYifWyNPeUQOlhzbPuxGpy9a2r5%2FcjrVk80B0%3D&amp;reserved=0\"><strong>X</strong></a><span> and </span><a href=\"https://visitor.r20.constantcontact.com/manage/optin?v=001IYrlh1STq1nQ4D8XRO5B4Tvbd__skb5DEaSNzAHXRTWsJ95wGZldZ7zrkXvzVXksf3R6x_FiGGtTmBpzdxMnTnede0kaBf28EWf6JhMvjtJ1G2BxcsTGuuXwUui3wHLgc8u79l49Wyo2SYfQARrvjWhWttAZTbd2\"><span><strong>join our email list through Constant Contact</strong></span></a><span> and select list \"Forest Health &amp; Fire: North of Hwy 14 to Wyoming Border (Red Feather Lakes).\"</span></p>",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "COARF Magic Feather Prescribed Burn",
                 "field_unit_code": "COARF",
                 "id": "312554",
                 "lat_deg": "40",
                 "lat_min": "46",
                 "lat_sec": "46.5492",
@@ -133,19 +133,19 @@
                 "coordinates": [
                     -105.368056,
                     39.95
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "2 days ago",
+                "changed": "5 hours 50 minutes ago",
                 "created": "<time datetime=\"2023-03-16T10:02:56-04:00\">2023-03-16</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p><strong>UPDATE (4/8/24)</strong><span> \u2013 Firefighters on the Boulder Ranger District of the Roosevelt National Forest are once again monitoring conditions to begin operations on the Forsythe II Prescribed Burn area, located 7 miles southwest of Boulder and 5.5 miles east of Nederland, as soon as April 15, 2024. This will be the second year of operations for this project after successfully treating 307 acres in April of 2023.\u00a0</span></p><p><span>________________________</span></p><p>The Forsythe II Project is part of the Forest Service\u2019s on-going effort to improve forest health conditions on the Boulder Ranger District. The project area is located near Gross Reservoir and Winiger Ridge in Boulder County, Colo. The entire project area encompasses 18,954 acres; 9,940 of those acres are National Forest System lands, 1,892 acres are Boulder County Parks and Open Space lands, and 7,122 acres are private lands. Elevation ranges from 6,082 to 8,945 feet. The project is generally located east of Nederland, CO and west of Gross Reservoir.\u00a0\u00a0</p><p>The broadcast burn units from the Forsythe II Decision are located 7 miles southwest of Boulder and 5.5 miles east of Nederland and total 931 acres. Forest thinning and pile burning treatments for areas near the planned prescribed burn area are mostly complete. The area has two main burn units that are subdivided into multiple sub-units that vary in size from 18 acres to 130 acres to provide a variety of options for control using existing roads, water, natural features and control lines, up to 340 acres per year. The prescribed burning treatments will be implemented over several years, with the amount treated per year dependent on weather, ground conditions, and available resources.\u00a0\u00a0</p><p>All burning will be implemented in close coordination and with assistance from local cooperating agencies and partners, including Boulder Watershed Collective, Boulder County Fireshed, state and county public health agencies, and multiple local agency fire cooperators.</p><p><span>Smoke will be in the air, and fire managers work closely with experts to minimize the impacts to the extent possible. Air quality is carefully monitored before and during a prescribed fire and all prescribed burns comply with state air quality regulations to minimize impacts to communities. To learn more about the potential health impacts of smoke visit </span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=http%3A%2F%2Fwww.colorado.gov%2Fpacific%2Fcdphe%2Fwood-smoke-and-health&amp;data=05%7C01%7C%7C8b18517df1f44aaec36f08db314bfac3%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638157974616252064%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=xazvkJjr3gmpTxXj%2FveiaJGxnj%2FnMmUlBLT378zSLO0%3D&amp;reserved=0\"><span>www.colorado.gov/pacific/cdphe/wood-smoke-and-health</span></a><span>.</span></p><p>To receive updates,\u00a0<a href=\"https://visitor.r20.constantcontact.com/manage/optin?v=001IYrlh1STq1nQ4D8XRO5B4Tvbd__skb5DEaSNzAHXRTWsJ95wGZldZ7zrkXvzVXksf3R6x_FiGGtTmBpzdxMnTnede0kaBf28EWf6JhMvjtJ1G2BxcsTGuuXwUui3wHLgc8u79l49Wyo2SYfQARrvjWhWttAZTbd2\">join our email list</a>\u00a0and select list \"Forest Health &amp; Fire: North of Hwy 72 (Coal Creek Canyon) to Hwy 119 Boulder Canyon (Nederland and Magnolia areas)\".\u00a0Have questions? Email\u00a0ARPFireInfo@usda.gov.</p><p>\u00a0</p><div class=\"highligh-media-item\">\n  <div class=\"ibox-media\">\n\n      \n      <a href=\"#&#10;&#10;&#9;&#9;&#9;&#9;&#9;&#9;forsythe-ii-rx-burn-public-map-2024&#10;&#9;&#9;&#9;\" aria-controls=\"&#10;&#10;&#9;&#9;&#9;&#9;&#9;&#9;forsythe-ii-rx-burn-public-map-2024&#10;&#9;&#9;&#9;\" data-open-modal=\"\">\n        <div class=\"media-name\">\n         \n\n\t\t\t\t\t\tForsythe II Rx Burn Public Map 2024\n\t\t\t\n        </div>\n\n        <div class=\"modal-image-container\">\n\n                          <img src=\"&#10;&#10;&#9;&#9;&#9;&#9;&#9;&#9;https://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-04/ForsytheIIRxBurn_PublicMap_20240402.jpg?VersionId=ieObdWtYdXjTtv6uuPIJ6CpNodrQ7z4E&#10;&#9;&#9;&#9;\" alt=\"&#10;&#10;&#9;&#9;&#9;&#9;&#9;&#9;Forsythe II Rx Burn Public Map 2024&#10;&#9;&#9;&#9;\" /></div>\n\n        <div class=\"date\">\n          \n\n\t\t\t\t\t\tMon, 04/08/2024 - 16:18\n\n\t\t\t\n        </div>\n      </a>\n\n      \n  </div>  \n\n  <div class=\"usa-modal\" id=\"&#10;&#10;&#9;&#9;&#9;&#9;&#9;&#9;forsythe-ii-rx-burn-public-map-2024&#10;&#9;&#9;&#9;\" aria-labelledby=\"&#10;&#10;&#9;&#9;&#9;&#9;&#9;&#9;forsythe-ii-rx-burn-public-map-2024&#10;&#9;&#9;&#9;\" aria-describedby=\"&#10;&#10;&#9;&#9;&#9;&#9;&#9;&#9;forsythe-ii-rx-burn-public-map-2024&#10;&#9;&#9;&#9;\">\n      <div class=\"usa-modal__content\">\n\n        <button class=\"usa-button usa-modal__close\" aria-label=\"Close this window\" data-close-modal=\"\">\n          <i class=\"fas fa-times\"></i>\n        </button>\n\n        <div class=\"usa-modal__main\">\n\n                \n\n        <hr style=\"margin: 15px 0 5px;\" /><div class=\"modal-image\">\n                          <img src=\"&#10;&#10;&#9;&#9;&#9;&#9;&#9;&#9;https://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-04/ForsytheIIRxBurn_PublicMap_20240402.jpg?VersionId=ieObdWtYdXjTtv6uuPIJ6CpNodrQ7z4E&#10;&#9;&#9;&#9;\" alt=\"&#10;&#10;&#9;&#9;&#9;&#9;&#9;&#9;Forsythe II Rx Burn Public Map 2024&#10;&#9;&#9;&#9;\" /></div>\n\n        <div class=\"usa-modal__footer\">\n          <div class=\"media-name\">\n            \n\n\t\t\t\t\t\tForsythe II Rx Burn Public Map 2024\n\t\t\t\n          </div>\n        </div>\n\n        <div class=\"media-caption\">\n          \n        </div>\n\n        </div>\n\n      </div>\n    </div>\n</div>\n\n",
+                "field_incident_overview": "<p><strong>Spring 2024 Update</strong><span> \u2013 </span>Fire managers began ignitions on the Forsythe II Prescribed Burn area, just west of Gross Reservoir, on Monday, April 15th. Ignitions are contingent on appropriate weather conditions and may not occur every day. Fire managers watch for weather that aligns appropriately for a planned burn, sufficiently dry fuels, and enough wind for smoke dispersal.</p><p>The immediate area around Forsythe Canyon and Winiger Ridge is currently closed to recreation and will remain closed while prescribed burn operations are active.</p><p>Residents and visitors in the area should expect to see smoke and flames when operations are underway, particularly in the following areas: Lakeshore subdivision, Crescent Village, Crescent Meadows, Gross Reservoir, Walker Park Ranch, Miramonte, Wondervu, Eldorado Canyon State Park, and parts of east Boulder County.&nbsp;</p><p>Email notifications are being sent out periodically during ignition periods. To receive these updates, join <a href=\"https://visitor.r20.constantcontact.com/manage/optin?v=001IYrlh1STq1nQ4D8XRO5B4Tvbd__skb5DEaSNzAHXRTWsJ95wGZldZ7zrkXvzVXksf3R6x_FiGGtTmBpzdxMnTnede0kaBf28EWf6JhMvjtJ1G2BxcsTGuuXwUui3wHLgc8u79l49Wyo2SYfQARrvjWhWttAZTbd2\">our email list</a> and select list \"Forest Health &amp; Fire: North of Hwy 72 (Coal Creek Canyon) to Hwy 119 Boulder Canyon (Nederland and Magnolia areas)\". Additional questions can be sent to <a href=\"mailto:ARPFireInfo@usda.gov\">ARPFireInfo@usda.gov</a>.</p><p><span>________________________</span></p><p><strong>General Information about the Project</strong>:</p><p>The Forsythe II Project is part of the Forest Service\u2019s on-going effort to improve forest health conditions on the Boulder Ranger District. The project area is located near Gross Reservoir and Winiger Ridge in Boulder County, Colo. The entire project area encompasses 18,954 acres; 9,940 of those acres are National Forest System lands, 1,892 acres are Boulder County Parks and Open Space lands, and 7,122 acres are private lands. Elevation ranges from 6,082 to 8,945 feet. The project is generally located east of Nederland, CO and west of Gross Reservoir.&nbsp;&nbsp;</p><p>The broadcast burn units from the Forsythe II Decision are located 7 miles southwest of Boulder and 5.5 miles east of Nederland and total 931 acres. Forest thinning and pile burning treatments for areas near the planned prescribed burn area are mostly complete. The area has two main burn units that are subdivided into multiple sub-units that vary in size from 18 acres to 130 acres to provide a variety of options for control using existing roads, water, natural features and control lines, up to 340 acres per year. The prescribed burning treatments will be implemented over several years, with the amount treated per year dependent on weather, ground conditions, and available resources.&nbsp;&nbsp;</p><p>All burning will be implemented in close coordination and with assistance from local cooperating agencies and partners, including Boulder Watershed Collective, Boulder County Fireshed, state and county public health agencies, and multiple local agency fire cooperators.</p><p><span>Smoke will be in the air, and fire managers work closely with experts to minimize the impacts to the extent possible. Air quality is carefully monitored before and during a prescribed fire and all prescribed burns comply with state air quality regulations to minimize impacts to communities. To learn more about the potential health impacts of smoke visit </span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=http%3A%2F%2Fwww.colorado.gov%2Fpacific%2Fcdphe%2Fwood-smoke-and-health&amp;data=05%7C01%7C%7C8b18517df1f44aaec36f08db314bfac3%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638157974616252064%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=xazvkJjr3gmpTxXj%2FveiaJGxnj%2FnMmUlBLT378zSLO0%3D&amp;reserved=0\"><span>www.colorado.gov/pacific/cdphe/wood-smoke-and-health</span></a><span>.</span></p><p>To receive updates,&nbsp;<a href=\"https://visitor.r20.constantcontact.com/manage/optin?v=001IYrlh1STq1nQ4D8XRO5B4Tvbd__skb5DEaSNzAHXRTWsJ95wGZldZ7zrkXvzVXksf3R6x_FiGGtTmBpzdxMnTnede0kaBf28EWf6JhMvjtJ1G2BxcsTGuuXwUui3wHLgc8u79l49Wyo2SYfQARrvjWhWttAZTbd2\">join our email list</a>&nbsp;and select list \"Forest Health &amp; Fire: North of Hwy 72 (Coal Creek Canyon) to Hwy 119 Boulder Canyon (Nederland and Magnolia areas)\".&nbsp;Have questions? Email&nbsp;ARPFireInfo@usda.gov.</p><p>&nbsp;</p><div class=\"highligh-media-item\">\n  <div class=\"ibox-media\">\n\n      \n      <a href=\"#\n\n\t\t\t\t\t\tforsythe-ii-rx-burn-public-map-2024\n\t\t\t\" aria-controls=\"\n\n\t\t\t\t\t\tforsythe-ii-rx-burn-public-map-2024\n\t\t\t\" data-open-modal>\n        <div class=\"media-name\">\n         \n\n\t\t\t\t\t\tForsythe II Rx Burn Public Map 2024\n\t\t\t\n        </div>\n\n        <div class=\"modal-image-container\">\n\n                          <img src=\"\n\n\t\t\t\t\t\thttps://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-04/ForsytheIIRxBurn_PublicMap_20240402.jpg?VersionId=ieObdWtYdXjTtv6uuPIJ6CpNodrQ7z4E\n\t\t\t\" alt=\"\n\n\t\t\t\t\t\tForsythe II Rx Burn Public Map 2024\n\t\t\t\"> \n            \n            \n            \n        </div>\n\n        <div class=\"date\">\n          \n\n\t\t\t\t\t\tMon, 04/08/2024 - 16:18\n\n\t\t\t\n        </div>\n      </a>\n\n      \n  </div>  \n\n  <div class=\"usa-modal\" id=\"\n\n\t\t\t\t\t\tforsythe-ii-rx-burn-public-map-2024\n\t\t\t\" aria-labelledby=\"\n\n\t\t\t\t\t\tforsythe-ii-rx-burn-public-map-2024\n\t\t\t\" aria-describedby=\"\n\n\t\t\t\t\t\tforsythe-ii-rx-burn-public-map-2024\n\t\t\t\">\n      <div class=\"usa-modal__content\">\n\n        <button class=\"usa-button usa-modal__close\" aria-label=\"Close this window\" data-close-modal>\n          <i class=\"fas fa-times\"></i>\n        </button>\n\n        <div class=\"usa-modal__main\">\n\n                \n\n        <hr style=\"margin: 15px 0 5px;\">\n\n        <div class=\"modal-image\">\n                          <img src=\"\n\n\t\t\t\t\t\thttps://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-04/ForsytheIIRxBurn_PublicMap_20240402.jpg?VersionId=ieObdWtYdXjTtv6uuPIJ6CpNodrQ7z4E\n\t\t\t\" alt=\"\n\n\t\t\t\t\t\tForsythe II Rx Burn Public Map 2024\n\t\t\t\"> \n                        \n            \n                        \n        </div>\n\n        <div class=\"usa-modal__footer\">\n          <div class=\"media-name\">\n            \n\n\t\t\t\t\t\tForsythe II Rx Burn Public Map 2024\n\t\t\t\n          </div>\n        </div>\n\n        <div class=\"media-caption\">\n          \n        </div>\n\n        </div>\n\n      </div>\n    </div>\n</div>\n\n",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "COARF Forsythe II Prescribed Burn",
                 "field_unit_code": "COARF",
                 "id": "312664",
                 "lat_deg": "39",
                 "lat_min": "57",
                 "lat_sec": "0",
@@ -165,19 +165,19 @@
                 "coordinates": [
                     -117.432658,
                     33.626082
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 day 6 hours ago",
+                "changed": "4 days 12 hours ago",
                 "created": "<time datetime=\"2023-05-03T06:38:36-04:00\">2023-05-03</time>\n",
                 "field_active": "1",
                 "field_incident_description": "For complete information on projects for each Ranger District please go to the 2024 CNF Project page, link is listed above. <br />\r\n<br />\r\nResidents in the area may call:   Battalion Chief: Jamie Rickard 619-445-1042x1044 for further information on the planned projects. ",
-                "field_incident_overview": "<p><a href=\"https://inciweb.wildfire.gov/incident-news/cacnf-2024-cleveland-national-forest-fuel-treatments\"><span>Updates</span></a>\u00a0|<a href=\"https://inciweb.nwcg.gov/incident-photos-gallery/cacnf-2024-cleveland-national-forest-fuel-treatments\"> Photos</a> | <a href=\"https://inciweb.wildfire.gov/incident-publication/cacnf-2024-cleveland-national-forest-fuel-treatments/2024-cnf-projects-01-01-2024\">2024 CNF Projects</a></p><p><span>On January 2022, the Forest Service launched a robust, 10-year strategy to address the wildfire crisis in the places where it poses the most immediate threats to communities. The strategy, called \u201c</span><a href=\"https://www.fs.usda.gov/managing-land/wildfire-crisis\"><span>Confronting the Wildfire Crisis: A Strategy for Protecting Communities and Improving Resilience in America\u2019s Forests</span></a><span>,\u201d combines a historic investment of congressional funding with years of scientific research and planning into a national effort that will dramatically increase the scale and pace of forest health treatments over the next decade. Through the strategy, the agency will work with states, Tribes and other partners to addresses wildfire risks to critical infrastructure, protect communities, and make forests more resilient.</span></p><p><span>In early 2023, the USDA Forest Service added </span><a href=\"https://www.fs.usda.gov/sites/default/files/fs_media/fs_document/WCS-Second-Landscapes.pdf\"><span>11 additional landscapes</span></a><span>. This announcement followed a year of progress in collaborating with partners across 10 initial landscapes to address wildfire risk to infrastructure and communities. One of these 11 additional landscapes is the Cleveland National Forest.\u00a0</span></p><p><span>Cleveland National Forest fire crews are starting to conduct fuel treatment operations. These projects will continue through 2023 and into spring 2024. These fuel treatment operations will include vegetation thinning, cutting and piling, mastication, prescribed fire by burning of piles, and low-intensity understory burning.\u00a0 Fire and mechanical treatments are important tools for the Forest Service\u2019s mission to reduce vegetation loading, and restore natural fire regimes, which in the long-term help communities live more safely in fire prone areas and improve forest health. To view project information for each district please go to projects page: </span><a href=\"https://inciweb.wildfire.gov/incident-publication/cacnf-2024-cleveland-national-forest-fuel-treatments/2024-cnf-projects-01-01-2024\"><span>2024 CNF Projects</span></a></p><p><span>Fire managers follow a risk-management approach when conducting these projects and mitigate impacts to local communities, residences and infrastructure. Fire managers will conduct prescribed fire activities during the safest possible \u201cburn windows\u201d in the coming months. Numerous factors including wind, humidity, air quality, fuel moisture and availability of fire crew personnel must be met before crews are authorized to move forward with burning.</span></p><p><span>The objective of the projects is to reduce the risk of catastrophic wildfire to people and communities, create conditions which offer a safer and more effective wildfire response, foster more resilient ecosystems, and minimize the effects of large wildfires on the landscape. In fiscal year 2023, the Forest's target for fuels reduction is 6,900 acres. 2,400 acres of planned prescribed fire, and 3,500 acres of mechanical treatments which is a combination of mastication, cut and pile with chainsaws.</span></p><p><span>Residents and visitors are asked to avoid areas where prescribed fires are being conducted. Some smoke may be visible. People should not be alarmed as the fires are carefully managed and monitored. Local fire and government authorities are notified prior to burn days and kept informed throughout prescribed fire operations.</span><br /><br /><span>Additional updates on prescribed burning will be shared on this page\u00a0and the forest\u2019s social media on X (formally known as Twitter) at\u00a0</span><a href=\"https://twitter.com/clevelandnf\"><span>https://twitter.com/clevelandnf</span></a><span> and Facebook at </span><a href=\"https://www.facebook.com/clevelandnf\"><span>https://www.facebook.com/clevelandnf</span></a></p>",
+                "field_incident_overview": "<p><a href=\"https://inciweb.wildfire.gov/incident-news/cacnf-2024-cleveland-national-forest-fuel-treatments\"><span>Updates</span></a>&nbsp;|<a href=\"https://inciweb.nwcg.gov/incident-photos-gallery/cacnf-2024-cleveland-national-forest-fuel-treatments\"> Photos</a> | <a href=\"https://inciweb.wildfire.gov/incident-publication/cacnf-2024-cleveland-national-forest-fuel-treatments/2024-cnf-projects-01-01-2024\">2024 CNF Projects</a></p><p><span>On January 2022, the Forest Service launched a robust, 10-year strategy to address the wildfire crisis in the places where it poses the most immediate threats to communities. The strategy, called \u201c</span><a href=\"https://www.fs.usda.gov/managing-land/wildfire-crisis\"><span>Confronting the Wildfire Crisis: A Strategy for Protecting Communities and Improving Resilience in America\u2019s Forests</span></a><span>,\u201d combines a historic investment of congressional funding with years of scientific research and planning into a national effort that will dramatically increase the scale and pace of forest health treatments over the next decade. Through the strategy, the agency will work with states, Tribes and other partners to addresses wildfire risks to critical infrastructure, protect communities, and make forests more resilient.</span></p><p><span>In early 2023, the USDA Forest Service added </span><a href=\"https://www.fs.usda.gov/sites/default/files/fs_media/fs_document/WCS-Second-Landscapes.pdf\"><span>11 additional landscapes</span></a><span>. This announcement followed a year of progress in collaborating with partners across 10 initial landscapes to address wildfire risk to infrastructure and communities. One of these 11 additional landscapes is the Cleveland National Forest.&nbsp;</span></p><p><span>Cleveland National Forest fire crews are starting to conduct fuel treatment operations. These projects will continue through 2023 and into spring 2024. These fuel treatment operations will include vegetation thinning, cutting and piling, mastication, prescribed fire by burning of piles, and low-intensity understory burning.&nbsp; Fire and mechanical treatments are important tools for the Forest Service\u2019s mission to reduce vegetation loading, and restore natural fire regimes, which in the long-term help communities live more safely in fire prone areas and improve forest health. To view project information for each district please go to projects page: </span><a href=\"https://inciweb.wildfire.gov/incident-publication/cacnf-2024-cleveland-national-forest-fuel-treatments/2024-cnf-projects-01-01-2024\"><span>2024 CNF Projects</span></a></p><p><span>Fire managers follow a risk-management approach when conducting these projects and mitigate impacts to local communities, residences and infrastructure. Fire managers will conduct prescribed fire activities during the safest possible \u201cburn windows\u201d in the coming months. Numerous factors including wind, humidity, air quality, fuel moisture and availability of fire crew personnel must be met before crews are authorized to move forward with burning.</span></p><p><span>The objective of the projects is to reduce the risk of catastrophic wildfire to people and communities, create conditions which offer a safer and more effective wildfire response, foster more resilient ecosystems, and minimize the effects of large wildfires on the landscape. In fiscal year 2023, the Forest's target for fuels reduction is 6,900 acres. 2,400 acres of planned prescribed fire, and 3,500 acres of mechanical treatments which is a combination of mastication, cut and pile with chainsaws.</span></p><p><span>Residents and visitors are asked to avoid areas where prescribed fires are being conducted. Some smoke may be visible. People should not be alarmed as the fires are carefully managed and monitored. Local fire and government authorities are notified prior to burn days and kept informed throughout prescribed fire operations.</span><br><br><span>Additional updates on prescribed burning will be shared on this page&nbsp;and the forest\u2019s social media on X (formally known as Twitter) at&nbsp;</span><a href=\"https://twitter.com/clevelandnf\"><span>https://twitter.com/clevelandnf</span></a><span> and Facebook at </span><a href=\"https://www.facebook.com/clevelandnf\"><span>https://www.facebook.com/clevelandnf</span></a></p>",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "CACNF 2024 Cleveland National Forest Forest Health Treatments",
                 "field_unit_code": "CACNF",
                 "id": "312808",
                 "lat_deg": "33",
                 "lat_min": "37",
                 "lat_sec": "33.895",
@@ -191,25 +191,89 @@
                 "urlPath": "/cacnf-2024-cleveland-national-forest-forest-health-treatments"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
+                    -106.193389,
+                    36.994331
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "4 weeks ago",
+                "created": "<time datetime=\"2023-06-19T12:01:10-04:00\">2023-06-19</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><strong>This project is currently in the planning stages for Spring 2024.</strong></p><p>The Rio Grande National Forest (RGNF) in Colorado and Carson National Forest in New Mexico are planning to initiate a broadcast prescribed fire to the south of Mogote, CO and northeast of Chama, NM. Fire managers are currently monitoring conditions, including snowmelt and fuel moistures. A date for planned ignitions is not yet being estimated. Careful consideration of weather, fuels conditions and resource availability in the area will be given, prior to the fire being started.</p><p>Three separate burn units are planned for this 700 to 900-acre prescribed fire which includes 192 acres on the Carson National Forest in New Mexico. Fire managers from both agencies are closely coordinating on this prescribed fire.</p><p>The general location of the prescribed fire is south of Mogote, CO just southeast of RGNF Forest Road 103, along the 103.2B on the west and 125.2B on the east. The south units are bound by Carson NF Road 75 and on the west by the 494 Road. The forest roads will be open to the public, but fire crew traffic may limit access.<span>&nbsp;</span></p><p>The purpose of the Bighorn/Stateline Prescribed Fire, which is within the <a href=\"https://232partnership.org/rio-chama-cflrp/\">Rio Chama Collaborative Forest Landscape Restoration Project</a> boundaries, is to reduce thinning slash that was generated several years ago and to return fire to both the mixed conifer and ponderosa forest settings. This condition more closely resembles its natural state, where frequent and low intensity surface fires burn ground fuels and small trees while maintaining an open stand of larger trees.</p><p>Conejos Canyon Prescribed Fire information will be added at a later date.</p>",
+                "field_percent_of_perimeter": "0",
+                "field_title_and_unit": "CORGF Bighorn Stateline Prescribed Fire",
+                "field_unit_code": "CORGF",
+                "id": "313115",
+                "lat_deg": "36",
+                "lat_min": "59",
+                "lat_sec": "39.59",
+                "long_deg": "106",
+                "long_min": "11",
+                "long_sec": "36.20",
+                "measurement_type": "Acres",
+                "size": "900",
+                "title": "Bighorn / Stateline Prescribed Fire",
+                "type": "Prescribed Fire",
+                "urlPath": "/corgf-bighorn-stateline-prescribed-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -119.719444,
+                    39.523611
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 month ago",
+                "created": "<time datetime=\"2023-07-17T14:51:04-04:00\">2023-07-17</time>\n",
+                "field_active": "1",
+                "field_incident_description": "The Humboldt-Toiyabe NF acknowledges the wildfire suppression and wildfire preparedness efforts for the 2024 fire season. The Forest extends great respect and gratitude towards the active work of firefighters in containing and controlling wildfires through techniques such as removing fuels, suffocating the fire with dirt, and cooling vegetation with targeted water.<br />\r\n<br />\r\nWe wish to emphasize the importance of families and communities taking a hands-on approach to wildfire preparedness, including creating defensible space around homes and buildings, making homes more fire-resistant, and having emergency plans in place. Several Nevadans live in a high-risk fire zone, making these efforts even more crucial.<br />\r\n<br />\r\nThe Forest Service&#039;s 10-year Wildfire Crisis Strategy is of the utmost importance for the HTNF with the announcement of 10 landscape project areas and the addition of 11 more in January 2023. These landscapes represent investments in high-risk fire sheds in the western United States, which are large, forested landscapes and rangelands with a high likelihood of destructive wildfires. The agency treated 3.2 million acres nationally in the previous year, thanks to funding from the Bipartisan Infrastructure Law and Inflation Reduction Act.<br />\r\n<br />\r\nWe encourage Nevadans to access the Living With Fire website, https://www.livingwithfire.com/, which provides local alerts, preparedness checklists, evacuation plans, and other resources.<br />\r\n<br />\r\nFOR UP-TO-DATE INFORMATION ON ALL HTF FIRE INCIDENTS - Please follow us on FACEBOOK https://www.facebook.com/HumboldtToiyabeNF and TWITTER https://twitter.com/HumboldtToiyabe/ <br />\r\n<br />\r\nRemember - Only you can prevent wildfires!",
+                "field_incident_overview": "<p><em><strong>HTNF Initial Attack Incidents less than 10 acres in size will be placed here. All others will have their own page. Exception - Cal Fire Incidents in HTNF Coverage areas</strong></em></p><p><em><strong>&nbsp; &nbsp; &nbsp; &nbsp; DATE/TIME&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; LOCATION&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;NAME&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; LAT/LONG&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; SIZE&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; STATUS&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</strong></em></p><p>1.</p><p>&nbsp;</p>",
+                "field_percent_of_perimeter": "100",
+                "field_title_and_unit": "NVHTF HTNF 2024 Initial Attack",
+                "field_unit_code": "NVHTF",
+                "id": "313492",
+                "lat_deg": "39",
+                "lat_min": "31",
+                "lat_sec": "25",
+                "long_deg": "119",
+                "long_min": "43",
+                "long_sec": "10",
+                "measurement_type": "Acres",
+                "size": "0",
+                "title": "HTNF 2024 Initial Attack ",
+                "type": "Wildfire",
+                "urlPath": "/nvhtf-htnf-2024-initial-attack"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
                     -112.154444,
                     34.619722
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 month 1 week ago",
+                "changed": "2 months 2 weeks ago",
                 "created": "<time datetime=\"2023-07-23T14:00:42-04:00\">2023-07-23</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p>At approximately 4:00 PM on Friday, July 21, 2023, resources from Prescott National Forest responded to a smoke report on the south side of Mingus Mountain, on the Verde Ranger District.\u00a0 \u00a0</p>\n\n<p><strong>Grapevine Fire Area/Road Closure terminated August 2, 2023 @5:00 pm.\u00a0 \u00a0</strong></p>\n\n<p><strong>\u00a0</strong></p>",
+                "field_incident_overview": "<p>At approximately 4:00 PM on Friday, July 21, 2023, resources from Prescott National Forest responded to a smoke report on the south side of Mingus Mountain, on the Verde Ranger District.&nbsp; &nbsp;</p>\n\n<p><strong>Grapevine Fire Area/Road Closure terminated August 2, 2023 @5:00 pm.&nbsp; &nbsp;</strong></p>\n\n<p><strong>&nbsp;</strong></p>",
                 "field_percent_of_perimeter": "100",
                 "field_title_and_unit": "AZPNF 2023 Grapevine Fire",
                 "field_unit_code": "AZPNF",
                 "id": "313588",
                 "lat_deg": "34",
                 "lat_min": "37",
                 "lat_sec": "11",
@@ -223,25 +287,57 @@
                 "urlPath": "/azpnf-2023-grapevine-fire"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
+                    -115.3545,
+                    48.027333
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "3 weeks 6 days ago",
+                "created": "<time datetime=\"2023-08-03T17:20:30-04:00\">2023-08-03</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span><span>The Gravel Pit Fire is burning in heavy fuels on a mix of private and federal land located along Highway 2 near Houghton Creek and McGinnis Meadows Roads. The human-caused fire was discovered on Tuesday, August 1. Firefighters from&nbsp;</span></span>Montana DNRC, USFS and Fisher River Valley Fire Rescue&nbsp;responded quickly after it was reported.<span><span>&nbsp;Fire activity includes spotting, torching and active consumption of heavy fuels.&nbsp;</span></span></p>\n\n<p>The Gravel Pit Fire is a full suppression fire. Firefighters are continuing to construct and improve fuel breaks and containment lines. Additionally, crews have performed structure protection&nbsp;assessments and preparations. Air resources have been used as needed to slow fire spread and cool down areas of heat.</p>\n\n<p>For the safety of firefighters and first responders, avoid traveling through the incident area along Hwy 2 whenever possible. If you must travel, please exercise extreme caution, slow down, and DO NOT STOP&nbsp;along Hwy 2! Due to fire activity and intermittent smoke across the roadway, visibility may be impaired. Watch out for emergency vehicles if you must travel in this area.</p>\n\n<p><span><span><span><span><span>The Western Montana All-Hazards Incident Management Team will transfer command of the Gravel Pit Fire to the Montana Department of Natural Resources and Conservation, Libby Unit at 6:00 a.m. on Sunday, August 20, 2023. This will be the final update the Gravel Pit Fire unless conditions change.</span></span></span></span></span></p>",
+                "field_percent_of_perimeter": "95",
+                "field_title_and_unit": "MTMTS Gravel Pit Fire",
+                "field_unit_code": "MTMTS",
+                "id": "314005",
+                "lat_deg": "48",
+                "lat_min": "1",
+                "lat_sec": "38.3982",
+                "long_deg": "115",
+                "long_min": "21",
+                "long_sec": "16.2",
+                "measurement_type": "Acres",
+                "size": "304",
+                "title": "Gravel Pit Fire",
+                "type": "Wildfire",
+                "urlPath": "/mtmts-gravel-pit-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
                     -124.343611,
                     42.745833
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "2 days 2 hours ago",
+                "changed": "1 month 1 week ago",
                 "created": "<time datetime=\"2023-08-31T23:09:52-04:00\">2023-08-31</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p><strong>The Anvil Fire was discovered on August 25th.</strong> The fire is located 7.5 miles east of Port Orford, OR, on Anvil Mountain. <span>The Forest and Incident Management Team (IMT) are working in close coordination with\u00a0Coos Forest Protective Association, Douglas Forest Protective Association and Curry County Sheriff.\u00a0The IMT's top priority is public and firefighter safety. They are using a full suppression strategy to contain the fire as small as possible, as safely as possible. More information can be found on </span><a href=\"https://www.facebook.com/flatfireoregon2023\"><span>Facebook</span></a><span> and</span><a href=\"twitter.com/RRSNF\"><span> </span></a><a href=\"https://twitter.com/RRSNF\"><span>X (formerly known as Twitter)</span></a></p><p><span><strong>Evacuations: </strong>All evacuation levels have been lifted.</span><a href=\"https://bit.ly/CurryCoEM\"><span lang=\"EN\" xml:lang=\"EN\" xml:lang=\"EN\"><strong>\u00a0</strong></span></a><a href=\"https://bit.ly/CurryCoEM.\"><span lang=\"EN\" xml:lang=\"EN\" xml:lang=\"EN\"><strong>https://bit.ly/CurryCoEM.</strong></span></a></p><p><strong>Area and Road Closures:\u00a0</strong></p><p><span>The Rogue River-Siskiyou National Forest/Powers Ranger District has determined that the Anvil Fire closure, which was scheduled to be in effect through July 1, 2024, is now safe and open for public entry.</span></p><p><span>The Anvil Fire closure included the Grassy Knob Wilderness area; Forest Service Roads 5201 (Sixes River Road) and 5201-90 (Butler Creek Road) and the Grassy Knob Trail #1241</span></p><p><span>\u00a0Please continue to be cautious when driving through the area and maintain situational awareness around any snags in the burned area.</span></p><p><span lang=\"EN\" xml:lang=\"EN\" xml:lang=\"EN\"><strong>Road Conditions: </strong>For specific information on road access, please see the Caltrans QuickMap site</span><a href=\"https://quickmap.dot.ca.gov/\"><span lang=\"EN\" xml:lang=\"EN\" xml:lang=\"EN\"><strong>,\u00a0https://quickmap.dot.ca.gov/\u00a0</strong></span></a><span lang=\"EN\" xml:lang=\"EN\" xml:lang=\"EN\">and Oregon Department of Transportation site,\u00a0</span><a href=\"https://www.tripcheck.com/\"><span lang=\"EN\" xml:lang=\"EN\" xml:lang=\"EN\"><strong>https://www.tripcheck.com/.</strong></span></a><span lang=\"EN\" xml:lang=\"EN\" xml:lang=\"EN\">\u00a0 <strong>Do not use forest roads for alternate routes</strong>.</span></p><p>\u00a0</p>",
+                "field_incident_overview": "<p><strong>The Anvil Fire was discovered on August 25th.</strong> The fire is located 7.5 miles east of Port Orford, OR, on Anvil Mountain. <span>The Forest and Incident Management Team (IMT) are working in close coordination with&nbsp;Coos Forest Protective Association, Douglas Forest Protective Association and Curry County Sheriff.&nbsp;The IMT's top priority is public and firefighter safety. They are using a full suppression strategy to contain the fire as small as possible, as safely as possible. More information can be found on </span><a href=\"https://www.facebook.com/flatfireoregon2023\"><span>Facebook</span></a><span> and</span><a href=\"twitter.com/RRSNF\"><span> </span></a><a href=\"https://twitter.com/RRSNF\"><span>X (formerly known as Twitter)</span></a></p><p><span><strong>Evacuations: </strong>All evacuation levels have been lifted.</span><a href=\"https://bit.ly/CurryCoEM\"><span lang=\"EN\"><strong>&nbsp;</strong></span></a><a href=\"https://bit.ly/CurryCoEM.\"><span lang=\"EN\"><strong>https://bit.ly/CurryCoEM.</strong></span></a></p><p><strong>Area and Road Closures:&nbsp;</strong></p><p><span>The Rogue River-Siskiyou National Forest/Powers Ranger District has determined that the Anvil Fire closure, which was scheduled to be in effect through July 1, 2024, is now safe and open for public entry.</span></p><p><span>The Anvil Fire closure included the Grassy Knob Wilderness area; Forest Service Roads 5201 (Sixes River Road) and 5201-90 (Butler Creek Road) and the Grassy Knob Trail #1241</span></p><p><span>&nbsp;Please continue to be cautious when driving through the area and maintain situational awareness around any snags in the burned area.</span></p><p><span lang=\"EN\"><strong>Road Conditions: </strong>For specific information on road access, please see the Caltrans QuickMap site</span><a href=\"https://quickmap.dot.ca.gov/\"><span lang=\"EN\"><strong>,&nbsp;https://quickmap.dot.ca.gov/&nbsp;</strong></span></a><span lang=\"EN\">and Oregon Department of Transportation site,&nbsp;</span><a href=\"https://www.tripcheck.com/\"><span lang=\"EN\"><strong>https://www.tripcheck.com/.</strong></span></a><span lang=\"EN\">&nbsp; <strong>Do not use forest roads for alternate routes</strong>.</span></p><p>&nbsp;</p>",
                 "field_percent_of_perimeter": "95",
                 "field_title_and_unit": "ORRSF Anvil Fire",
                 "field_unit_code": "ORRSF",
                 "id": "315330",
                 "lat_deg": "42",
                 "lat_min": "44",
                 "lat_sec": "45",
@@ -261,19 +357,19 @@
                 "coordinates": [
                     -113.936944,
                     46.837778
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "5 hours 20 minutes ago",
+                "changed": "5 days 15 hours ago",
                 "created": "<time datetime=\"2023-09-10T09:58:41-04:00\">2023-09-10</time>\n",
                 "field_active": "1",
                 "field_incident_description": "Prescribed fires help reduce hazardous fuels, restore wildlife habitat, and create better protection around communities from future wildfires.",
-                "field_incident_overview": "<p><a href=\"https://inciweb.nwcg.gov/incident-announcement/mtlnf-lolo-national-forest-fall-prescribed-fires\">Announcements</a>\u00a0 \u00a0\u00a0<a href=\"https://inciweb.nwcg.gov/incident-closures/mtlnf-lolo-national-forest-fall-prescribed-fires\">Closures</a>\u00a0 \u00a0<a href=\"https://inciweb.nwcg.gov/incident-news/mtlnf-lolo-national-forest-fall-prescribed-fires\">News</a>\u00a0\u00a0\u00a0\u00a0 <a href=\"https://inciweb.nwcg.gov/incident-photos-gallery/mtlnf-lolo-national-forest-fall-prescribed-fires\">Photographs</a>\u00a0\u00a0 \u00a0<a href=\"https://inciweb.nwcg.gov/incident-maps-gallery/mtlnf-lolo-national-forest-fall-prescribed-fires\">Maps</a></p><p>The Lolo National Forest, along with their interagency partners and neighbors, is preparing to conduct spring prescribed fire projects to reduce hazardous fuels, restore wildlife habitat, and create better protection around communities from future wildfires.\u00a0</p><p>\u201cAs snow melts and opens access to planned burn units, we will take advantage of favorable conditions to start prescribed burning as soon as this week, \u201d said<span>\u00a0</span>Jeff<span>\u00a0</span>Hayes,<span>\u00a0</span>Lolo<span>\u00a0</span>National<span>\u00a0</span>Forest<span>\u00a0</span>Fuels<span>\u00a0</span>Specialist.\u00a0<span> </span>\u201cOver the next two-three months, we will plan burn operations on days which minimize smoke impacts, restore healthy forest conditions and wildlife habitat, and/or meet fuels reduction goals.\u201d</p><p>Prescribed fire operations are a key component of the\u00a0<a href=\"https://www.fs.usda.gov/managing-land/wildfire-crisis\">Wildfire Crisis Strategy\u00a0</a>that works with partners to reduce wildfire risk to communities, critical infrastructure, natural resources and improve the resilience of America\u2019s Forests. Prescribed<span>\u00a0</span>fires<span>\u00a0</span>are<span>\u00a0</span>carefully<span>\u00a0</span>planned<span>\u00a0</span>and<span>\u00a0</span>implemented<span>\u00a0</span>in<span>\u00a0</span>accordance<span>\u00a0</span>with<span>\u00a0</span>a<span>\u00a0</span>written<span>\u00a0</span>burn<span>\u00a0</span>plan. Prior to implementation, local fire managers coordinate with local cooperators, counties, and partners. When prescription criteria are met, firefighters implement, monitor, and patrol each burn to ensure it meets forest health and public safety goals.</p><p>All prescribed fires will be implemented in compliance with Montana air quality standards and coordinated with the Montana Department of Environmental Quality and the appropriate county health departments to minimize<span>\u00a0</span>the impacts of smoke to neighbors, cooperators, and surrounding<span>\u00a0</span>communities.<span>\u00a0</span>Smoke<span>\u00a0</span>may<span>\u00a0</span>settle<span>\u00a0</span>in<span>\u00a0</span>valley<span>\u00a0</span>bottoms<span>\u00a0</span>and<span>\u00a0</span>drainages<span>\u00a0</span>overnight,<span>\u00a0</span>but<span>\u00a0</span>it<span>\u00a0</span>is expected to dissipate within a few days.</p><p>Some<span>\u00a0</span>of<span>\u00a0</span>these<span>\u00a0</span>prescribed<span>\u00a0</span>fires<span>\u00a0</span>are<span>\u00a0</span>supported through<span>\u00a0</span>partnerships<span>\u00a0</span>with<span>\u00a0</span>Montana<span>\u00a0</span>DNRC,<span>\u00a0</span>Nature Conservancy, Missoula and Frenchtown Rural Fire Departments, Bureau of Land Management, Rocky Mountain Elk Foundation, Mule Deer Foundation, National Wild Turkey Federation, and Upland Game Bird Enhancement Group.<span>\u00a0</span></p><p>For<span>\u00a0</span>additional<span>\u00a0</span>information<span>\u00a0</span>about<span>\u00a0</span>these<span>\u00a0</span>burns<span>\u00a0</span>follow<span>\u00a0</span>the<span>\u00a0</span><a href=\"https://www.facebook.com/lolonationalforest\"><span>Lolo\u00a0National\u00a0Forest\u00a0on\u00a0Facebook</span></a><span>\u00a0</span>or visit <a href=\"https://inciweb.nwcg.gov/incident-information/mtlnf-lolo-national-forest-prescribed-fire-operations\"><span>InciWeb</span></a>.</p><p><span><strong>See the </strong></span><a href=\"https://inciweb.nwcg.gov/incident-announcement/mtlnf-lolo-national-forest-fall-prescribed-fires\"><span><strong>'Announcements'</strong></span></a><span><strong> and </strong></span><a href=\"https://inciweb.nwcg.gov/incident-news/mtlnf-lolo-national-forest-fall-prescribed-fires\"><span><strong>'News'</strong></span></a><span><strong> Tabs for the latest information on planned prescribed fires.</strong></span><br /><br />\u00a0</p>",
+                "field_incident_overview": "<p><a href=\"https://inciweb.nwcg.gov/incident-announcement/mtlnf-lolo-national-forest-fall-prescribed-fires\">Announcements</a>&nbsp; &nbsp;&nbsp;<a href=\"https://inciweb.nwcg.gov/incident-closures/mtlnf-lolo-national-forest-fall-prescribed-fires\">Closures</a>&nbsp; &nbsp;<a href=\"https://inciweb.nwcg.gov/incident-news/mtlnf-lolo-national-forest-fall-prescribed-fires\">News</a>&nbsp;&nbsp;&nbsp;&nbsp; <a href=\"https://inciweb.nwcg.gov/incident-photos-gallery/mtlnf-lolo-national-forest-fall-prescribed-fires\">Photographs</a>&nbsp;&nbsp; &nbsp;<a href=\"https://inciweb.nwcg.gov/incident-maps-gallery/mtlnf-lolo-national-forest-fall-prescribed-fires\">Maps</a></p><p>The Lolo National Forest, along with their interagency partners and neighbors, is preparing to conduct spring prescribed fire projects to reduce hazardous fuels, restore wildlife habitat, and create better protection around communities from future wildfires.&nbsp;</p><p>\u201cAs snow melts and opens access to planned burn units, we will take advantage of favorable conditions to start prescribed burning as soon as this week, \u201d said<span>&nbsp;</span>Jeff<span>&nbsp;</span>Hayes,<span>&nbsp;</span>Lolo<span>&nbsp;</span>National<span>&nbsp;</span>Forest<span>&nbsp;</span>Fuels<span>&nbsp;</span>Specialist.&nbsp;<span> </span>\u201cOver the next two-three months, we will plan burn operations on days which minimize smoke impacts, restore healthy forest conditions and wildlife habitat, and/or meet fuels reduction goals.\u201d</p><p>Prescribed fire operations are a key component of the&nbsp;<a href=\"https://www.fs.usda.gov/managing-land/wildfire-crisis\">Wildfire Crisis Strategy&nbsp;</a>that works with partners to reduce wildfire risk to communities, critical infrastructure, natural resources and improve the resilience of America\u2019s Forests. Prescribed<span>&nbsp;</span>fires<span>&nbsp;</span>are<span>&nbsp;</span>carefully<span>&nbsp;</span>planned<span>&nbsp;</span>and<span>&nbsp;</span>implemented<span>&nbsp;</span>in<span>&nbsp;</span>accordance<span>&nbsp;</span>with<span>&nbsp;</span>a<span>&nbsp;</span>written<span>&nbsp;</span>burn<span>&nbsp;</span>plan. Prior to implementation, local fire managers coordinate with local cooperators, counties, and partners. When prescription criteria are met, firefighters implement, monitor, and patrol each burn to ensure it meets forest health and public safety goals.</p><p>All prescribed fires will be implemented in compliance with Montana air quality standards and coordinated with the Montana Department of Environmental Quality and the appropriate county health departments to minimize<span>&nbsp;</span>the impacts of smoke to neighbors, cooperators, and surrounding<span>&nbsp;</span>communities.<span>&nbsp;</span>Smoke<span>&nbsp;</span>may<span>&nbsp;</span>settle<span>&nbsp;</span>in<span>&nbsp;</span>valley<span>&nbsp;</span>bottoms<span>&nbsp;</span>and<span>&nbsp;</span>drainages<span>&nbsp;</span>overnight,<span>&nbsp;</span>but<span>&nbsp;</span>it<span>&nbsp;</span>is expected to dissipate within a few days.</p><p>Some<span>&nbsp;</span>of<span>&nbsp;</span>these<span>&nbsp;</span>prescribed<span>&nbsp;</span>fires<span>&nbsp;</span>are<span>&nbsp;</span>supported through<span>&nbsp;</span>partnerships<span>&nbsp;</span>with<span>&nbsp;</span>Montana<span>&nbsp;</span>DNRC,<span>&nbsp;</span>Nature Conservancy, Missoula and Frenchtown Rural Fire Departments, Bureau of Land Management, Rocky Mountain Elk Foundation, Mule Deer Foundation, National Wild Turkey Federation, and Upland Game Bird Enhancement Group.<span>&nbsp;</span></p><p>For<span>&nbsp;</span>additional<span>&nbsp;</span>information<span>&nbsp;</span>about<span>&nbsp;</span>these<span>&nbsp;</span>burns<span>&nbsp;</span>follow<span>&nbsp;</span>the<span>&nbsp;</span><a href=\"https://www.facebook.com/lolonationalforest\"><span>Lolo&nbsp;National&nbsp;Forest&nbsp;on&nbsp;Facebook</span></a><span>&nbsp;</span>or visit <a href=\"https://inciweb.nwcg.gov/incident-information/mtlnf-lolo-national-forest-prescribed-fire-operations\"><span>InciWeb</span></a>.</p><p><span><strong>See the </strong></span><a href=\"https://inciweb.nwcg.gov/incident-announcement/mtlnf-lolo-national-forest-fall-prescribed-fires\"><span><strong>'Announcements'</strong></span></a><span><strong> and </strong></span><a href=\"https://inciweb.nwcg.gov/incident-news/mtlnf-lolo-national-forest-fall-prescribed-fires\"><span><strong>'News'</strong></span></a><span><strong> Tabs for the latest information on planned prescribed fires.</strong></span><br><br>&nbsp;</p>",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "MTLNF Lolo National Forest Prescribed Fire Operations",
                 "field_unit_code": "MTLNF",
                 "id": "315767",
                 "lat_deg": "46",
                 "lat_min": "49",
                 "lat_sec": "76",
@@ -287,213 +383,149 @@
                 "urlPath": "/mtlnf-lolo-national-forest-prescribed-fire-operations"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -122.21241,
-                    39.53021
+                    -108.823833,
+                    38.681333
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 1 day ago",
-                "created": "<time datetime=\"2023-10-06T14:10:13-04:00\">2023-10-06</time>\n",
-                "field_active": "1",
-                "field_incident_description": "",
-                "field_incident_overview": "<p><a href=\"https://inciweb.wildfire.gov/incident-publication/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects/mnf-planned-projects-fall-2023spring-2024\"><strong>Planned Project</strong></a><a href=\"https://inciweb.wildfire.gov/incident-publication/camnf-mendocino-nf-2023-rx-fire-projects/2023-mnf-planned-projects\"><strong>s</strong></a><span> \u00a0|\u00a0 </span><a href=\"https://inciweb.wildfire.gov/incident-news/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects\"><strong>Updates</strong></a><span> \u00a0|\u00a0 </span><a href=\"https://inciweb.wildfire.gov/incident-maps-gallery/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects\"><strong>Maps</strong></a><span> \u00a0| </span><a href=\"https://inciweb.wildfire.gov/incident-photos-gallery/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects\"><strong>Photos</strong></a></p><p><span>Prescribed fire is a tool that uses fire under planned ignitions to mimic the natural role of fire in the environment. Without fire, hazardous fuels can build up and carry wildfire from the forest floor to tree canopies, creating extreme fire behavior that poses risk to firefighters, surrounding communities and natural resources. Prescribed fire, including vegetation cutting, removal and burning of piles and low-intensity understory burning, is an important tool to meet the Forest Service\u2019s management objectives for ecological restoration, creating habitat for plants and animals and reducing unwanted fuel loading.</span></p><p><span>Fire managers follow a risk-management approach when conducting these projects and mitigate impacts to local communities, residences and infrastructure. Fire managers will conduct prescribed fire activities during the safest possible \u201cburn windows\u201d in the coming months. Numerous factors including wind, humidity, air quality, fuel moisture and availability of fire crew personnel must be met before crews are authorized to move forward with burning.</span></p><p><span>Residents and visitors are asked to avoid areas where prescribed fires are being conducted. Some smoke may be visible. People should not be alarmed as the fires are carefully monitored. Local fire and government authorities are notified prior to burn days and kept informed throughout prescribed fire operations.</span></p><p><span>Additional updates on prescribed burning will be shared on on this page\u00a0and the forest\u2019s social media on Twitter at\u00a0</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001JYSlPa_F885TgbSiqqdjA0ewuCbUct42Eyz2gZbHSv88Dpc0DyK50tPMb3nI47lwI5UW5IX9USXnRvgHLegKQ5IHVZ5BKNwyKUtdLE8CwgYIUO2Mt1i3S3fsv-xo_M5hAulYgdcWnheiIBIphhgAopwFJf7zuJmG%26c%3DDCGRbAkBb1kqn93TfKXMTMfYrVLYRcYvHS_plx8jP8uIxwS-4_9JcQ%3D%3D%26ch%3DyOyu-KUdDkTAM7UdEC4pWnNdwaJ5z9bT6P-Gvbc6zhx-Lb74n6DvPw%3D%3D&amp;data=05%7C01%7C%7Ccb52b817a0d24f78780708daf9a8b8a8%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638096800284324769%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=rOyrj4bdrmvE3sUPGfhsZWBSVmtU207Rc7%2FmHecNanE%3D&amp;reserved=0\"><span><strong>https://twitter.com/MendocinoNF</strong></span></a><span>\u00a0and Facebook\u00a0</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001JYSlPa_F885TgbSiqqdjA0ewuCbUct42Eyz2gZbHSv88Dpc0DyK50tPMb3nI47lwiTwC5K-RFHQry_eaedXPjtasR8A8Aa6p4FFDfOlMyKiVITYWIV93ncx1V9pl4ftl_-oY5zmYTnXu8lWHXNWf6_EN67YKitt0%26c%3DDCGRbAkBb1kqn93TfKXMTMfYrVLYRcYvHS_plx8jP8uIxwS-4_9JcQ%3D%3D%26ch%3DyOyu-KUdDkTAM7UdEC4pWnNdwaJ5z9bT6P-Gvbc6zhx-Lb74n6DvPw%3D%3D&amp;data=05%7C01%7C%7Ccb52b817a0d24f78780708daf9a8b8a8%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638096800284324769%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=0j4mJWsYdg9DxkgTLYi2yHZOZWKjb%2BLdiT69a5P9U%2BU%3D&amp;reserved=0\"><span><strong>https://www.facebook.com/MendocinoNF</strong></span></a><span>.</span></p>",
-                "field_percent_of_perimeter": "",
-                "field_title_and_unit": "CAMNF Mendocino NF Fall 2023Spring 2024 RX Fire Projects",
-                "field_unit_code": "CAMNF",
-                "id": "316511",
-                "lat_deg": "39",
-                "lat_min": "31",
-                "lat_sec": "48.7554",
-                "long_deg": "122",
-                "long_min": "12",
-                "long_sec": "44.676",
-                "measurement_type": "Acres",
-                "size": "",
-                "title": "Mendocino NF Fall 2023/Spring 2024 RX Fire Projects",
-                "type": "Prescribed Fire",
-                "urlPath": "/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects"
-            },
-            "type": "Feature"
-        },
-        {
-            "geometry": {
-                "coordinates": [
-                    -121.017778,
-                    39.269167
-                ],
-                "type": "Point"
-            },
-            "properties": {
-                "changed": "3 weeks ago",
-                "created": "<time datetime=\"2023-11-06T15:58:37-05:00\">2023-11-06</time>\n",
-                "field_active": "1",
-                "field_incident_description": "",
-                "field_incident_overview": "<p>The Yuba River Ranger District will be conducting a variety of planned prescribed pileburns as conditions allow. Project dates, locations, acreage numbers and updates will be posted in the \"Announcements\" tab of this incident page.</p><p>\u00a0</p><p><strong>Why Are We Burning?</strong><br />The goal of this prescribed burn is to decrease the existing fire hazard and to prevent and reduce the impact of future fires in the area. Other benefits include enhancing wildlife habitat and reintroducing fire into a fire-adapted ecosystem.</p><p><br /><strong>Why Now?</strong><br />Current conditions allow for prescribed burning. Each prescribed fire operation follows a prescribed fire burn plan, which considers temperature, humidity, wind, moisture of the vegetation, and conditions for the dispersal of smoke. This information is used to decide when and where to burn. The Tahoe National Forest strives to give as much advance notice as possible before burning, but some operations may be conducted on short notice.</p><p><strong>Smoke</strong><br />Smoke from prescribed fire operations is normal and may continue for several days after an ignition depending on the project size and environmental conditions. Smoke may settle into the valleys in the evening and lift in the morning. The Tahoe National Forest coordinates with state and local county air pollution control districts and monitors weather conditions closely prior to prescribed fire ignition. Crews also conduct test burns before igniting a larger area, to verify how effectively fuels are consumed and how smoke will travel.</p>",
-                "field_percent_of_perimeter": "",
-                "field_title_and_unit": "CATNF TNF Yuba River Pileburn Projects",
-                "field_unit_code": "CATNF",
-                "id": "316737",
-                "lat_deg": "39",
-                "lat_min": "16",
-                "lat_sec": "09",
-                "long_deg": "121",
-                "long_min": "01",
-                "long_sec": "04",
-                "measurement_type": "Acres",
-                "size": "",
-                "title": "TNF Yuba River Pileburn Projects",
-                "type": "Prescribed Fire",
-                "urlPath": "/catnf-tnf-yuba-river-pileburn-projects"
-            },
-            "type": "Feature"
-        },
-        {
-            "geometry": {
-                "coordinates": [
-                    -120.845278,
-                    39.010278
-                ],
-                "type": "Point"
-            },
-            "properties": {
-                "changed": "1 month 3 weeks ago",
-                "created": "<time datetime=\"2023-11-06T16:15:23-05:00\">2023-11-06</time>\n",
+                "changed": "1 month ago",
+                "created": "<time datetime=\"2023-09-18T12:48:20-04:00\">2023-09-18</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p>The American River Ranger District will be conducting a variety of planned prescribed pileburns as conditions allow. Project dates, locations, acreage numbers and updates will be posted in the \"Announcements\" tab of this incident page.</p><p>\u00a0</p><p><strong>Why Are We Burning?</strong><br />The goal of this prescribed burn is to decrease the existing fire hazard and to prevent and reduce the impact of future fires in the area. Other benefits include enhancing wildlife habitat and reintroducing fire into a fire-adapted ecosystem.</p><p><br /><strong>Why Now?</strong><br />Current conditions allow for prescribed burning. Each prescribed fire operation follows a prescribed fire burn plan, which considers temperature, humidity, wind, moisture of the vegetation, and conditions for the dispersal of smoke. This information is used to decide when and where to burn. The Tahoe National Forest strives to give as much advance notice as possible before burning, but some operations may be conducted on short notice.</p><p><strong>Smoke</strong><br />Smoke from prescribed fire operations is normal and may continue for several days after an ignition depending on the project size and environmental conditions. Smoke may settle into the valleys in the evening and lift in the morning. The Tahoe National Forest coordinates with state and local county air pollution control districts and monitors weather conditions closely prior to prescribed fire ignition. Crews also conduct test burns before igniting a larger area, to verify how effectively fuels are consumed and how smoke will travel.</p>",
+                "field_incident_overview": "<p dir=\"ltr\"><strong>Cow Creek Prescribed Burn Plan:&nbsp;</strong></p><p dir=\"ltr\"><em><strong>Up to 15,000 acres targeted for treatment with prescribed fire in Mesa County&nbsp;</strong></em></p><p dir=\"ltr\"><span>Fire Management Officials from the Grand Mesa,&nbsp; Uncompahgre, and Gunnison (GMUG) National Forests\u2019 Grand Valley Ranger District are conducting the Cow&nbsp;Creek Prescribed Burn starting on Sept. 24, with ignition decisions being made on an ongoing basis, depending upon weather and fuel conditions.&nbsp;</span></p><p dir=\"ltr\"><span>The Cow Creek Prescribed Burn project area is approximately 9 miles east of Gateway, Colorado, and 25 miles southwest of Grand Junction, Colorado. If conditions are appropriate, about 7,000 acres with the potential of up to 15,000 acres are planned to be burned over multiple days, reducing the threat of catastrophic wildfire and improving wildlife habitat. The project area includes Cow Creek, Calamity Creek, and Indian Creek. The Cow Creek Prescribed Burn is being accomplished using joint-agency fire resources, utilizing both aerial and hand ignitions, and&nbsp;is being closely monitored to ensure that the burn area remains within the designated boundaries.&nbsp;</span></p><p dir=\"ltr\"><span>Prescribed burning is a tool that re-introduces fire into the ecosystem to promote and regenerate healthy trees and habitat conditions. This type of fire management strategy is important to maintain a fire-adapted ecosystem and is essential for wildfire prevention. Before conducting a prescribed burn, extensive planning takes place to establish proper parameters such as weather, fuel conditions, smoke dispersion, staffing, and other agency coordination. A prescribed fire is a planned fire used to accomplish management objectives. One of the objectives for this burn is to reduce the overgrown and crowded fuels in the area, therefore creating a mosaic landscape that is more resistant to catastrophic wildfire. This prescribed fire is also aiming to enhance productive vegetation in the oak brush and mountain shrub parts of the burn area, in order to increase habitat for wildlife and livestock. &nbsp;</span></p><p dir=\"ltr\"><span>Significant coordinating efforts occur with local landowners, protection partners, and other cooperating agencies to ensure the burn is conducted safely.&nbsp;The safety of firefighters and the public are the most important factors considered when planning prescribed fires.&nbsp;For more information on prescription burning and its use, please visit: </span><a href=\"https://www.fs.usda.gov/managing-land/prescribed-fire\"><span>https://www.fs.usda.gov/managing-land/prescribed-fire</span></a></p><p dir=\"ltr\"><span>Dispersed recreation in the prescribed fire project areas may be impacted. Staff will be making personal contact with recreationists regarding any temporary closures. Signs will be placed on adjacent roads, notifying the public of the project areas as necessary.&nbsp;&nbsp;</span></p><p dir=\"ltr\"><span>Fire managers have obtained smoke permits from the State of Colorado and will comply with&nbsp;Colorado State air quality regulations. Smoke from the prescribed fire is being managed to have minimal impact on neighboring communities. Smoke may be visible in several communities, including Grand Junction, Whitewater, Gateway, Fruita, Delta, Montrose, and Norwood for multiple days. The public is advised not to call 911 for smoke regarding this prescribed burn.&nbsp;</span></p><p dir=\"ltr\"><span>For more information on how prescribed fire smoke may affect your health, please visit&nbsp;</span><a href=\"https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health\"><span>https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health</span></a></p><p dir=\"ltr\"><span>Prescribed burn updates will be posted on the&nbsp;GMUG Fire Info&nbsp;page. For information on prescribed burns, pile burns, wildfires, and fire restrictions on National Forest System lands, visit&nbsp;</span><a href=\"https://www.westslopefireinformation.com\"><span>https://www.westslopefireinformation.com</span></a></p><p dir=\"ltr\"><span>For information and updates on current fire restrictions, conditions, and recreation opportunities on the Grand&nbsp; Mesa, Uncompahgre, and Gunnison (GMUG) National Forests, visit the&nbsp;forest website. Connect with us on social media </span><a href=\"https://twitter.com/gmug_nf\"><span>https://twitter.com/gmug_nf</span></a><span> and </span><a href=\"https://www.facebook.com/GMUG.NF/\"><span>https://www.facebook.com/GMUG.NF/</span></a></p><p dir=\"ltr\">&nbsp;</p>",
                 "field_percent_of_perimeter": "",
-                "field_title_and_unit": "CATNF TNF American River Pileburn Projects",
-                "field_unit_code": "CATNF",
-                "id": "316739",
-                "lat_deg": "39",
-                "lat_min": "00",
-                "lat_sec": "37",
-                "long_deg": "120",
-                "long_min": "50",
-                "long_sec": "43",
+                "field_title_and_unit": "COGMF Cow Creek Prescribed Burn",
+                "field_unit_code": "COGMF",
+                "id": "316082",
+                "lat_deg": "38",
+                "lat_min": "40",
+                "lat_sec": "52.8000",
+                "long_deg": "108",
+                "long_min": "49",
+                "long_sec": "25.8000",
                 "measurement_type": "Acres",
                 "size": "",
-                "title": "TNF American River Pileburn Projects",
+                "title": "Cow Creek Prescribed Burn",
                 "type": "Prescribed Fire",
-                "urlPath": "/catnf-tnf-american-river-pileburn-projects"
+                "urlPath": "/cogmf-cow-creek-prescribed-burn"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -120.215,
-                    39.446111
+                    -122.21241,
+                    39.53021
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 month 3 weeks ago",
-                "created": "<time datetime=\"2023-11-06T16:23:45-05:00\">2023-11-06</time>\n",
+                "changed": "1 month 2 weeks ago",
+                "created": "<time datetime=\"2023-10-06T14:10:13-04:00\">2023-10-06</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p>The Sierraville &amp; Truckee Ranger Districts (eastside of the forest) will be conducting a variety of planned prescribed pileburns as conditions allow. Project dates, locations, acreage numbers and updates will be posted in the \"Announcements\" tab of this incident page.</p><p>\u00a0</p><p><strong>Why Are We Burning?</strong><br />The goal of this prescribed burn is to decrease the existing fire hazard and to prevent and reduce the impact of future fires in the area. Other benefits include enhancing wildlife habitat and reintroducing fire into a fire-adapted ecosystem.</p><p><br /><strong>Why Now?</strong><br />Current conditions allow for prescribed burning. Each prescribed fire operation follows a prescribed fire burn plan, which considers temperature, humidity, wind, moisture of the vegetation, and conditions for the dispersal of smoke. This information is used to decide when and where to burn. The Tahoe National Forest strives to give as much advance notice as possible before burning, but some operations may be conducted on short notice.</p><p><strong>Smoke</strong><br />Smoke from prescribed fire operations is normal and may continue for several days after an ignition depending on the project size and environmental conditions. Smoke may settle into the valleys in the evening and lift in the morning. The Tahoe National Forest coordinates with state and local county air pollution control districts and monitors weather conditions closely prior to prescribed fire ignition. Crews also conduct test burns before igniting a larger area, to verify how effectively fuels are consumed and how smoke will travel.</p><p><br />\u00a0</p>",
+                "field_incident_overview": "<p><a href=\"https://inciweb.wildfire.gov/incident-publication/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects/mnf-planned-projects-fall-2023spring-2024\"><strong>Planned Project</strong></a><a href=\"https://inciweb.wildfire.gov/incident-publication/camnf-mendocino-nf-2023-rx-fire-projects/2023-mnf-planned-projects\"><strong>s</strong></a><span> &nbsp;|&nbsp; </span><a href=\"https://inciweb.wildfire.gov/incident-news/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects\"><strong>Updates</strong></a><span> &nbsp;|&nbsp; </span><a href=\"https://inciweb.wildfire.gov/incident-maps-gallery/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects\"><strong>Maps</strong></a><span> &nbsp;| </span><a href=\"https://inciweb.wildfire.gov/incident-photos-gallery/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects\"><strong>Photos</strong></a></p><p><span>Prescribed fire is a tool that uses fire under planned ignitions to mimic the natural role of fire in the environment. Without fire, hazardous fuels can build up and carry wildfire from the forest floor to tree canopies, creating extreme fire behavior that poses risk to firefighters, surrounding communities and natural resources. Prescribed fire, including vegetation cutting, removal and burning of piles and low-intensity understory burning, is an important tool to meet the Forest Service\u2019s management objectives for ecological restoration, creating habitat for plants and animals and reducing unwanted fuel loading.</span></p><p><span>Fire managers follow a risk-management approach when conducting these projects and mitigate impacts to local communities, residences and infrastructure. Fire managers will conduct prescribed fire activities during the safest possible \u201cburn windows\u201d in the coming months. Numerous factors including wind, humidity, air quality, fuel moisture and availability of fire crew personnel must be met before crews are authorized to move forward with burning.</span></p><p><span>Residents and visitors are asked to avoid areas where prescribed fires are being conducted. Some smoke may be visible. People should not be alarmed as the fires are carefully monitored. Local fire and government authorities are notified prior to burn days and kept informed throughout prescribed fire operations.</span></p><p><span>Additional updates on prescribed burning will be shared on on this page&nbsp;and the forest\u2019s social media on Twitter at&nbsp;</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001JYSlPa_F885TgbSiqqdjA0ewuCbUct42Eyz2gZbHSv88Dpc0DyK50tPMb3nI47lwI5UW5IX9USXnRvgHLegKQ5IHVZ5BKNwyKUtdLE8CwgYIUO2Mt1i3S3fsv-xo_M5hAulYgdcWnheiIBIphhgAopwFJf7zuJmG%26c%3DDCGRbAkBb1kqn93TfKXMTMfYrVLYRcYvHS_plx8jP8uIxwS-4_9JcQ%3D%3D%26ch%3DyOyu-KUdDkTAM7UdEC4pWnNdwaJ5z9bT6P-Gvbc6zhx-Lb74n6DvPw%3D%3D&amp;data=05%7C01%7C%7Ccb52b817a0d24f78780708daf9a8b8a8%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638096800284324769%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=rOyrj4bdrmvE3sUPGfhsZWBSVmtU207Rc7%2FmHecNanE%3D&amp;reserved=0\"><span><strong>https://twitter.com/MendocinoNF</strong></span></a><span>&nbsp;and Facebook&nbsp;</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fr20.rs6.net%2Ftn.jsp%3Ff%3D001JYSlPa_F885TgbSiqqdjA0ewuCbUct42Eyz2gZbHSv88Dpc0DyK50tPMb3nI47lwiTwC5K-RFHQry_eaedXPjtasR8A8Aa6p4FFDfOlMyKiVITYWIV93ncx1V9pl4ftl_-oY5zmYTnXu8lWHXNWf6_EN67YKitt0%26c%3DDCGRbAkBb1kqn93TfKXMTMfYrVLYRcYvHS_plx8jP8uIxwS-4_9JcQ%3D%3D%26ch%3DyOyu-KUdDkTAM7UdEC4pWnNdwaJ5z9bT6P-Gvbc6zhx-Lb74n6DvPw%3D%3D&amp;data=05%7C01%7C%7Ccb52b817a0d24f78780708daf9a8b8a8%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638096800284324769%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=0j4mJWsYdg9DxkgTLYi2yHZOZWKjb%2BLdiT69a5P9U%2BU%3D&amp;reserved=0\"><span><strong>https://www.facebook.com/MendocinoNF</strong></span></a><span>.</span></p>",
                 "field_percent_of_perimeter": "",
-                "field_title_and_unit": "CATNF TNF Eastside Pileburn Projects",
-                "field_unit_code": "CATNF",
-                "id": "316740",
+                "field_title_and_unit": "CAMNF Mendocino NF Fall 2023Spring 2024 RX Fire Projects",
+                "field_unit_code": "CAMNF",
+                "id": "316511",
                 "lat_deg": "39",
-                "lat_min": "26",
-                "lat_sec": "46",
-                "long_deg": "120",
+                "lat_min": "31",
+                "lat_sec": "48.7554",
+                "long_deg": "122",
                 "long_min": "12",
-                "long_sec": "54",
+                "long_sec": "44.676",
                 "measurement_type": "Acres",
                 "size": "",
-                "title": "TNF Eastside Pileburn Projects",
+                "title": "Mendocino NF Fall 2023/Spring 2024 RX Fire Projects",
                 "type": "Prescribed Fire",
-                "urlPath": "/catnf-tnf-eastside-pileburn-projects"
+                "urlPath": "/camnf-mendocino-nf-fall-2023spring-2024-rx-fire-projects"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -111.674056,
-                    35.186169
+                    -117.835536,
+                    34.324381
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "2 days 4 hours ago",
-                "created": "<time datetime=\"2024-01-08T15:10:11-05:00\">2024-01-08</time>\n",
+                "changed": "1 week 3 days ago",
+                "created": "<time datetime=\"2023-11-14T22:03:06-05:00\">2023-11-14</time>\n",
                 "field_active": "1",
-                "field_incident_description": "Prescribed fire projects usually commence during the months of March and April. If you want to sign up to receive news releases about prescribed fire and other projects on Coconino National Forest, please visit https://www.fs.usda.gov/news/coconino/news-events and click on the blue &quot;Sign Up!&quot; icon in the right column.<br />\r\n<br />\r\nPile burns are an important part of forest restoration projects planned in accordance with the Forest Service\u2019s 10-year Wildfire Crisis Strategy.<br />\r\n<br />\r\nPile burns work alongside both prescribed fire and mechanical thinning to remove fuels such as woody debris and logging scraps from the forest floor during times of opportune weather. <br />\r\n<br />\r\nFire managers make every effort to effectively plan and execute burn plans at times when weather allows for smoke impacts to be minimized and transport up and over communities.<br />\r\n<br />\r\nFor more information about prescribed burns and why wildfire is a necessary part of this ecosystem, please visit our website at coconinonationalforest.us.",
-                "field_incident_overview": "<h2>There are no prescribed fire plans for the week of April 8, 2024.</h2>",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span lang=\"EN-US\">The Pine Flats Prescribed Fire is planned for Wednesday, November 15 (morning), if conditions allow, at the Crystal Lake Recreation Area above Azusa, CA.&nbsp;</span></p><p>This planned fire will <span>reduce the risk of unwanted wildfires in nearby communities; help reduce risks for wildland firefighters; protect buildings, campgrounds, and picnic areas; and/or benefit forest health.</span></p>",
                 "field_percent_of_perimeter": "",
-                "field_title_and_unit": "AZCOF Coconino National Forest prescribed fire and pile burns WinterSpring 2024",
-                "field_unit_code": "AZCOF",
-                "id": "316935",
-                "lat_deg": "35",
-                "lat_min": "11",
-                "lat_sec": "10.2078",
-                "long_deg": "111",
-                "long_min": "40",
-                "long_sec": "26.6",
+                "field_title_and_unit": "CAANF Pine Flat Prescribed Fire",
+                "field_unit_code": "CAANF",
+                "id": "316822",
+                "lat_deg": "34.324381350050245",
+                "lat_min": "",
+                "lat_sec": "",
+                "long_deg": "-117.83553559465481",
+                "long_min": "",
+                "long_sec": "",
                 "measurement_type": "Acres",
                 "size": "",
-                "title": "Coconino National Forest prescribed fire and pile burns (Winter/Spring 2024)",
+                "title": "Pine Flat Prescribed Fire",
                 "type": "Prescribed Fire",
-                "urlPath": "/azcof-coconino-national-forest-prescribed-fire-and-pile-burns-winterspring-2024"
+                "urlPath": "/caanf-pine-flat-prescribed-fire"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
                     -116.575278,
                     39.205
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 month ago",
+                "changed": "1 week 3 days ago",
                 "created": "<time datetime=\"2024-01-17T17:01:14-05:00\">2024-01-17</time>\n",
                 "field_active": "1",
                 "field_incident_description": "The Sierra and Elko Fronts, a Wildfire Crisis Landscape Project on the Humboldt-Toiyabe National Forest, was selected to receive a historic investment of $53 million in 2023 to support the USDA Forest Service\u2019s National Wildfire Crisis Strategy. Landscapes were chosen based on the potential for wildfire to affect nearby communities, critical infrastructure, public water sources, and Tribal lands. The Forest was positioned well given current efforts around the Nevada Shared Stewardship Agreement, an interagency collaboration effort that has previously identified wildfire crisis landscapes across the state based on similar threats to public and private land.<br />\r\n<br />\r\nThe wildfire crisis landscape projects are a large-scale effort to reduce the risk of wildfire to protect at-risk communities and critical infrastructure, while also increasing the landscape\u2019s resilience and ability to survive the effects of changing climates and other stressors such as insects, disease, and invasive species. Selected wildfire crisis landscapes will advance the goals of the Wildfire Crisis Strategy by utilizing the best available science and strategic network of hazardous fuels and vegetation treatments to reduce wildfire risk.<br />\r\n<br />\r\nWildfire crisis landscapes, also known as firesheds, are large forested and rangeland areas where communities, infrastructure, and natural resources are at the highest risk to be impacted by wildfire. Examples include critical watersheds and wildlife habitats; utility, energy, and mining facilities; transportation corridors; and recreation areas. Several high-risk fire sheds were identified on the Humboldt-Toiyabe National Forest, including the Sierra and Elko Fronts.<br />\r\n<br />\r\nCombined with the initial ten selected landscapes in 2022, the wildfire crisis landscape projects now span nearly 45 million acres across 137 of the 250 high-risk firesheds in the western United States. More than $930 million will be invested in 21 landscapes across 26.7 million acres. This work will mitigate risk to approximately 200 communities within these selected landscapes.",
-                "field_incident_overview": "<p>Here\u2019s more info on what we have going on!!\u00a0</p><p><a href=\"https://www.facebook.com/hashtag/prescribedfireis?__eep__=6&amp;__cft__[0]=AZWhihRWXoujGsIOKhiF2bzIhq9Dn8qmq4K_Jxfahh8YP11Chq-_D71rY09MMvUjtJf1SdT53Ddk5dNmxrHjPEfIpCIfr2-M-vDiIN-9tX38iDmDJ5qury9FWIksl8nutrG9p_DRWFUPF_4jqoLFXfy8DCuhmr8rAiFjNQYs8cNA9Gu-wDBkuxY5iL0Ycmj_3u4&amp;__tn__=*NK-R\"><span>Prescribed Fire is</span></a> an important tool for decreasing long-term fire risk to communities and restoring our forests, so they are more resilient to natural fire in the future.</p><p>Pile burning is a type of prescribed fire where firefighters pile and burn forest debris to reduce an area\u2019s wildfire risk. These piles are made from the debris cut by hand (<a href=\"https://www.facebook.com/hashtag/chainsaws?__eep__=6&amp;__cft__[0]=AZWhihRWXoujGsIOKhiF2bzIhq9Dn8qmq4K_Jxfahh8YP11Chq-_D71rY09MMvUjtJf1SdT53Ddk5dNmxrHjPEfIpCIfr2-M-vDiIN-9tX38iDmDJ5qury9FWIksl8nutrG9p_DRWFUPF_4jqoLFXfy8DCuhmr8rAiFjNQYs8cNA9Gu-wDBkuxY5iL0Ycmj_3u4&amp;__tn__=*NK-R\"><span>chainsaws</span></a>) and stacked for fuel reduction projects in the forest. Piles are only ignited under certain conditions, including favorable <a href=\"https://www.facebook.com/hashtag/smoke?__eep__=6&amp;__cft__[0]=AZWhihRWXoujGsIOKhiF2bzIhq9Dn8qmq4K_Jxfahh8YP11Chq-_D71rY09MMvUjtJf1SdT53Ddk5dNmxrHjPEfIpCIfr2-M-vDiIN-9tX38iDmDJ5qury9FWIksl8nutrG9p_DRWFUPF_4jqoLFXfy8DCuhmr8rAiFjNQYs8cNA9Gu-wDBkuxY5iL0Ycmj_3u4&amp;__tn__=*NK-R\"><span>smoke</span></a> dispersal and adequate snow cover, which helps contain the piles. These conditions direct firefighters on where within project areas burning can occur due to the localized nature of conditions.</p><p>All of our pile burns are conducted within the requirements of federally established guidelines.</p><p>\u00a0</p><p><em><strong>CURRENT STATUS\u00a0</strong></em></p><ul><li><strong>Sierra Front (Includes Carson and Bridgeport Ranger Districts) - 12 to15 Personnel</strong></li></ul><p>Walker, CA - Mill Canyon RX - <em><strong>NO BURNING TODAY</strong></em></p><p>Reno, NV - Arrowhawk RX - <em><strong>NO BURNING TODAY</strong></em></p><p>Markleeville, CA - Tamarack RX - <em><strong>NO BURNING TODAY</strong></em></p><p>Genoa, NV - Genoa RX - <em><strong>NO BURNING TODAY</strong></em></p><p>\u00a0</p><ul><li><strong>Spring Mountains National Recreation Area - 12 to 15 Personnel</strong></li></ul><p>Southern Nevada - Cole Springs RX - <em><strong>NO BURNING TODAY</strong></em></p><p><em><strong>\u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0 \u00a0\u00a0</strong></em>McFarland RX -<em><strong> NO BURNING TODAY</strong></em></p><p>\u00a0</p><ul><li><strong>Mountain City, Ruby Mountains, Jarbidge Ranger Districts - 12 to15 Personnel</strong></li></ul><p>Ruby Valley, NV - Ruby Lake Estates RX - <em><strong>NO BURNING TODAY</strong></em></p><p>\u00a0</p><p>Please do not call 911. Local Fire Departments are continuously in communication with our <a href=\"https://www.facebook.com/hashtag/firefighters?__eep__=6&amp;__cft__[0]=AZWkb9a9qc1ajg8gw3q-6MwaynRF8OddgbYTmtBlauJhuvI7cvPo7Bnv5fUNDtrh1e2oVaUirEBtbvMvEZykttKtLx_e_1D0QCsiTgMlkj8QmzHkk7crv7NtvtXykKDTTyueTpdRjFqc6YCFEbkpYfvxLL4C4VLQFF4CSrVG6HjU3uirpfqgIxCZanmR-ATvc68&amp;__tn__=*NK-R\"><span>#firefighters</span></a> on the ground.</p><p>\u00a0</p><p>\u00a0</p>",
+                "field_incident_overview": "<p>Here\u2019s more info on what we have going on!!&nbsp;</p><p><a href=\"https://www.facebook.com/hashtag/prescribedfireis?__eep__=6&amp;__cft__[0]=AZWhihRWXoujGsIOKhiF2bzIhq9Dn8qmq4K_Jxfahh8YP11Chq-_D71rY09MMvUjtJf1SdT53Ddk5dNmxrHjPEfIpCIfr2-M-vDiIN-9tX38iDmDJ5qury9FWIksl8nutrG9p_DRWFUPF_4jqoLFXfy8DCuhmr8rAiFjNQYs8cNA9Gu-wDBkuxY5iL0Ycmj_3u4&amp;__tn__=*NK-R\"><span>Prescribed Fire is</span></a> an important tool for decreasing long-term fire risk to communities and restoring our forests, so they are more resilient to natural fire in the future. <span>Prescribed fires, also known as prescribed burns, refer to the controlled application of fire by a team of fire experts under specified weather conditions to restore health to ecosystems that depend on fire.</span></p><p>&nbsp;</p><p><em><strong>CURRENT STATUS&nbsp;</strong></em></p><ul><li><strong>Sierra Front (Includes Carson and Bridgeport Ranger Districts) - l</strong></li></ul><p>Reno, NV - Dog Valley RX (343 Acres) -<em><strong> 302</strong></em> <em><strong>total</strong></em> <em><strong>acres treated&nbsp;</strong></em></p><p>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - Mitchell Canyon RX - <em><strong>91 acres treated&nbsp;</strong></em></p><p>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - White's Creek RX - <em><strong>21 acres treated&nbsp;</strong></em></p><p>Walker, CA - Mill Canyon RX - <em><strong>UPCOMING</strong></em> <em><strong>Burning planned for 4/23/24</strong></em></p><p>&nbsp;</p><p><strong>Spring Mountains National Recreation Area&nbsp;</strong></p><p>Southern Nevada - Cole Springs RX - <em><strong>Burning Complete for Season</strong></em></p><p><em><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;</strong></em>McFarland RX -<em><strong> Burning Complete for Season</strong></em></p><p>&nbsp;</p><p><strong>Mountain City, Ruby Mountains, Jarbidge Ranger Districts&nbsp;</strong></p><p>Ruby Valley, NV - Ruby Lake Estates RX - <em><strong>Burning Complete for Season</strong></em></p><p>&nbsp;</p><p>Please do not call 911. Local Fire Departments are continuously in communication with our <a href=\"https://www.facebook.com/hashtag/firefighters?__eep__=6&amp;__cft__[0]=AZWkb9a9qc1ajg8gw3q-6MwaynRF8OddgbYTmtBlauJhuvI7cvPo7Bnv5fUNDtrh1e2oVaUirEBtbvMvEZykttKtLx_e_1D0QCsiTgMlkj8QmzHkk7crv7NtvtXykKDTTyueTpdRjFqc6YCFEbkpYfvxLL4C4VLQFF4CSrVG6HjU3uirpfqgIxCZanmR-ATvc68&amp;__tn__=*NK-R\"><span>#firefighters</span></a> on the ground.</p><p>&nbsp;</p><p>&nbsp;</p>",
                 "field_percent_of_perimeter": "",
-                "field_title_and_unit": "NVHTF 2024 HTNF FOREST WIDE Winter Pile Burning",
+                "field_title_and_unit": "NVHTF 2024 HTNF FOREST WIDE PRESCRIBED FIRE",
                 "field_unit_code": "NVHTF",
                 "id": "316953",
                 "lat_deg": "39",
                 "lat_min": "12",
                 "lat_sec": "18",
                 "long_deg": "-117",
                 "long_min": "25",
                 "long_sec": "29",
                 "measurement_type": "Acres",
                 "size": "",
-                "title": "2024 HTNF FOREST WIDE Winter Pile Burning",
+                "title": "2024 HTNF FOREST WIDE PRESCRIBED FIRE",
                 "type": "Prescribed Fire",
-                "urlPath": "/nvhtf-2024-htnf-forest-wide-winter-pile-burning"
+                "urlPath": "/nvhtf-2024-htnf-forest-wide-prescribed-fire"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
                     -115.8475,
                     33.466389
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 month 1 week ago",
+                "changed": "2 months 3 weeks ago",
                 "created": "<time datetime=\"2024-02-21T14:37:12-05:00\">2024-02-21</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
                 "field_incident_overview": "<p>The Palmas Fire is now 100% contained. Some trial closures remain in effect. There is no threat to neighboring communities, as the fire was contained within the preserve.</p>",
                 "field_percent_of_perimeter": "100",
                 "field_title_and_unit": "CACDD Palmas Fire",
                 "field_unit_code": "CACDD",
@@ -511,57 +543,25 @@
                 "urlPath": "/cacdd-palmas-fire"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -79.766222,
-                    38.382611
-                ],
-                "type": "Point"
-            },
-            "properties": {
-                "changed": "6 days 3 hours ago",
-                "created": "<time datetime=\"2024-03-19T12:12:31-04:00\">2024-03-19</time>\n",
-                "field_active": "1",
-                "field_incident_description": "",
-                "field_incident_overview": "<p>Monongahela National Forest staff plan to conduct prescribed burns on 3,667 acres in Pocahontas, Greenbrier and Tucker counties from March through June, weather permitting.\u00a0</p><p>Project areas planned for prescribed burns this spring include:</p><ul><li>Guinn Ridge \u2013 1,462 acres (Pocahontas County)</li><li>Ramshorn Ridge \u2013 1,005 acres (Pocahontas County)</li><li>Upper Greenbrier North \u2013 514 acres (Pocahontas County)</li><li><span>Lake Sherwood Piles and Dam \u2013 5 acres (Greenbrier County)</span></li><li><span>Meadow Creek Units 1 &amp; 2 \u2013 243 acres (Greenbrier County)</span></li><li><span>Rucker Gap \u2013 384 acres (Greenbrier County)</span></li><li>Nursery Bottom \u2013 54 acres (Tucker County)\u00a0</li></ul><p><span><strong>Why do we burn?</strong></span></p><p><span>Reintroducing fire into the forest will:\u00a0</span></p><ul type=\"disc\"><li><span>Restore historic fire regimes</span></li><li><span>Improve wildlife habitat</span></li><li><span>Enhance forest structure and age diversity</span></li><li><span>Improve oak regeneration</span></li><li><span>Control tree diseases and insects</span></li><li><span>Reduce hazardous fuel levels</span></li></ul><p><span><strong>How do we manage a prescribed burn?</strong></span></p><p><span>Fire managers prepare a burn plan for each prescribed burn describing the appropriate conditions needed to conduct the burn safely and achieve the desired results. Burn plans consider public safety, protection of private property, staffing and equipment needs, temperature, humidity, wind, moisture of the vegetation, and conditions for the dispersal of smoke. Appropriate conditions must be met before igniting prescribed burns. A control line is established around each burn area before ignition, using hand tools and other equipment, roads, trails, and natural features such as creeks and other water sources.</span></p><p><span><strong>Public Safety</strong></span></p><p><span>Each burn area will be closed to the public on the day of the burn. The area may be closed for several days for public safety. Signs will be posted along the fire line and at entry points into the area. Area residents and travelers may see or smell smoke during fire operations. If you encounter smoke on the highway, slow down, turn on your vehicle\u2019s lights and drive appropriately for the conditions.\u00a0</span></p><p><span><strong>Public Notification</strong></span></p><p><span>The Forest Service will notify local 911 centers and radio stations on the day of the burn. Information, maps and the latest updates are available at\u00a0</span><a href=\"https://inciweb.nwcg.gov/\"><span>inciweb.gov</span></a><span>.</span></p>",
-                "field_percent_of_perimeter": "",
-                "field_title_and_unit": "WVMOF Monongahela National Forest Spring 2024 Prescribed Fire Operations",
-                "field_unit_code": "WVMOF",
-                "id": "317071",
-                "lat_deg": "38",
-                "lat_min": "22",
-                "lat_sec": "57.4",
-                "long_deg": "79",
-                "long_min": "45",
-                "long_sec": "58.4",
-                "measurement_type": "Acres",
-                "size": "",
-                "title": "Monongahela National Forest Spring 2024 Prescribed Fire Operations",
-                "type": "Prescribed Fire",
-                "urlPath": "/wvmof-monongahela-national-forest-spring-2024-prescribed-fire-operations"
-            },
-            "type": "Feature"
-        },
-        {
-            "geometry": {
-                "coordinates": [
                     -78.336389,
                     38.695556
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "2 weeks ago",
+                "changed": "1 month 3 weeks ago",
                 "created": "<time datetime=\"2024-03-21T16:02:08-04:00\">2024-03-21</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p><span lang=\"EN-US\" xml:lang=\"EN-US\" xml:lang=\"EN-US\">After a major wind event early afternoon March 20, 2024, a fire was reported on private land in the Rocky Branch area of Luray, Virginia, just north of Shenandoah National Park Headquarters. Initial responders included Luray Fire Department and National Park Service (NPS) firefighters. The fire progressed into the Park, and NPS firefighters assembled a crew to contain it. On March 23, the Southern Area Incident Management Team assumed command of the fire. At the end of the day on March 27, fire management was returned to Shenandoah National Park. The cause of the fire is undetermined.\u00a0</span><span>\u00a0</span></p>",
+                "field_incident_overview": "<p><span lang=\"EN-US\">After a major wind event early afternoon March 20, 2024, a fire was reported on private land in the Rocky Branch area of Luray, Virginia, just north of Shenandoah National Park Headquarters. Initial responders included Luray Fire Department and National Park Service (NPS) firefighters. The fire progressed into the Park, and NPS firefighters assembled a crew to contain it. On March 23, the Southern Area Incident Management Team assumed command of the fire. At the end of the day on March 27, fire management was returned to Shenandoah National Park. The cause of the fire is undetermined.&nbsp;</span><span>&nbsp;</span></p>",
                 "field_percent_of_perimeter": "80",
                 "field_title_and_unit": "VASHP Rocky Branch Fire",
                 "field_unit_code": "VASHP",
                 "id": "317080",
                 "lat_deg": "38",
                 "lat_min": "41",
                 "lat_sec": "44",
@@ -581,15 +581,15 @@
                 "coordinates": [
                     -78.585833,
                     38.651944
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 3 days ago",
+                "changed": "1 month 2 weeks ago",
                 "created": "<time datetime=\"2024-03-23T14:57:10-04:00\">2024-03-23</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
                 "field_incident_overview": "",
                 "field_percent_of_perimeter": "98",
                 "field_title_and_unit": "VAVAF 2024 Waterfall MountainShenandoah Forest211 Fire North Zone Complex",
                 "field_unit_code": "VAVAF",
@@ -613,15 +613,15 @@
                 "coordinates": [
                     -78.593333,
                     39.040556
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 3 days ago",
+                "changed": "1 month 2 weeks ago",
                 "created": "<time datetime=\"2024-03-23T15:03:22-04:00\">2024-03-23</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
                 "field_incident_overview": "",
                 "field_percent_of_perimeter": "100",
                 "field_title_and_unit": "VAVAF 2024 Waites Run Fire North Zone Complex",
                 "field_unit_code": "VAVAF",
@@ -645,15 +645,15 @@
                 "coordinates": [
                     -78.925278,
                     38.766389
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 3 days ago",
+                "changed": "1 month 2 weeks ago",
                 "created": "<time datetime=\"2024-03-23T15:08:04-04:00\">2024-03-23</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
                 "field_incident_overview": "",
                 "field_percent_of_perimeter": "100",
                 "field_title_and_unit": "VAVAF 2024 CaponBrush Run Fire North Zone Complex",
                 "field_unit_code": "VAVAF",
@@ -677,15 +677,15 @@
                 "coordinates": [
                     -78.506389,
                     38.723056
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 2 days ago",
+                "changed": "1 month 2 weeks ago",
                 "created": "<time datetime=\"2024-03-23T15:10:23-04:00\">2024-03-23</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
                 "field_incident_overview": "",
                 "field_percent_of_perimeter": "100",
                 "field_title_and_unit": "VAVAF 2024 Edith GapSerenity Ridge Fire North Zone Complex",
                 "field_unit_code": "VAVAF",
@@ -709,15 +709,15 @@
                 "coordinates": [
                     -78.845278,
                     38.864167
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 5 days ago",
+                "changed": "1 month 3 weeks ago",
                 "created": "<time datetime=\"2024-03-23T15:13:03-04:00\">2024-03-23</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
                 "field_incident_overview": "",
                 "field_percent_of_perimeter": "100",
                 "field_title_and_unit": "VAVAF 2024 Cove Mountain Fire North Zone Complex",
                 "field_unit_code": "VAVAF",
@@ -741,19 +741,19 @@
                 "coordinates": [
                     -78.621389,
                     38.768889
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 day 8 hours ago",
+                "changed": "1 month 1 week ago",
                 "created": "<time datetime=\"2024-03-23T16:45:37-04:00\">2024-03-23</time>\n",
                 "field_active": "1",
                 "field_incident_description": "Complex",
-                "field_incident_overview": "<p>The North Zone Complex covers five wildfires in the George Washington and Jefferson National Forests and on state and private land in West Virginia and Virginia. They are: <strong>Waterfall Mountain/Shenandoah Forest/211 Fire, Waites Run Fire, Capon/Brush Run Fire, Edith Gap/Serenity Ridge Fire, and Cove Mountain Fire. </strong>Co<span>mmand of the North Zone Complex has been transferred to a local Type 3 Team led by Incident Commander Colten Moor.\u00a0</span></p><p><strong>FINAL Fire Update - Wednesday April 3</strong><span><strong>, 2024</strong></span></p><p><a><span><strong>Current Status:</strong></span></a><span> Command of the North Zone Complex is assigned to a local Type 3 Team led by Incident Commander Colten Moor.\u00a0\u00a0The Team will hand command of the incident back to the local unit on Saturday April 6th.\u00a0 Cove, Edith Gap, Capon, Waterfall Mountain and Waites Run Fires will be monitored and patrolled until declared out. With the increase in moisture and more favorable weather conditions all fires associated with the North Zone Complex have been contained.</span></p><p><span>Closure orders for all areas in the North Zone Complex remain in effect. The local district will continue to assess conditions on the ground and determine when it is safe to re-open the areas to the public. Be aware of areas adjacent to recently burned areas as they are prone to flash flooding and debris flows. Continuation of suppression repair will occur as needs are identified. \u00a0Firefighters continue to remove snags, address other safety concerns, and continue to secure containment lines.\u00a0 Fire and insect weakened trees continue to fall within burned areas. Road conditions have deteriorated due to rainfall and equipment traffic.\u00a0Burn Area Emergency Response (BAER) Team will be working on plans to rehabilitate damage to natural drainages and structures moving forward.</span></p><p><span><strong>Individual Fire Updates: 15,977 total acres 100% contained</strong></span></p><ol><li><span>Waterfall Mountain/Shenandoah Forest/211 West Fire in Shenandoah and Page Counties, VA</span></li></ol><ul><li><span>6,399 acres; <strong>100% contained</strong></span></li></ul><ol><li><span>Waites Run Fire in Hardy County, WV</span><ul><li><span>6,223 acres, <strong>100% contained</strong></span></li></ul></li><li><span>Capon/Brush Run Fire in Rockingham County, VA\u00a0</span><ul><li><span>2,368 acres, <strong>100% contained</strong></span></li></ul></li><li><span>Edith Gap/Serenity Ridge Fire in Shenandoah and Page Counties, VA</span><ul><li><span>832 acres, <strong>100% contained</strong></span></li></ul></li><li><span>Cove Mountain Fire in Hardy County, WV</span><ul><li><span>155 acres, <strong>100% contained</strong></span></li></ul></li></ol><p><span><strong>Resources:\u00a0</strong>5 Type 2 Crews, 1 Type 2IA crew, 1 Type 3 helicopter, 6 engines, 1 dozers and 108 personnel<strong>.\u00a0</strong></span></p><p><span><strong>Date and Cause Reported:\u00a0</strong>The fires were reported on Wednesday, March 20, 2024, and Thursday, March 21, 2024. The causes of the fires are undetermined.\u00a0</span></p><p><span><strong>Weather:\u00a0</strong>Today unsettled weather continues as multiple rounds of showers and storms impact the region. \u00a0A series of cold fronts sweep through the area Wednesday and Thursday, bringing windy conditions that last through the weekend. High pressure builds overhead Sunday into early next week</span><a><span>.</span></a></p><p><span><strong>Closures: </strong>For the protection of public health and safety, and for the protection of resources, <strong>please respect area, road and trail closures.</strong>\u00a0 Check the George Washington and Jefferson website for the full list of closures.\u00a0</span><a href=\"http://www.fs.usda.gov/gwj\"><span>www.fs.usda.gov/gwj</span></a></p><p><span><strong>Advisories:\u00a0</strong>We ask the public to avoid areas with active fire for their own safety and to allow firefighters to work safely. Public and firefighter safety is always our top priority. In addition, <strong>please do not fly drones</strong> near or over a wildfire. Drones and firefighting aircraft are a dangerous mix and could lead to accidents or slow down wildfire suppression. If you fly, we can\u2019t.</span></p><p><span><strong>Smoke and Air Quality:\u00a0</strong>\u00a0Air quality\u00a0information\u00a0is\u00a0available\u00a0at\u00a0</span><a href=\"http://www.airnow.gov\"><span>www.airnow.gov</span></a><span>.\u00a0</span></p><p><span><strong>General Fire Information:\u00a0</strong></span></p><ul><li><span>Homeowners can learn how to make their homes less susceptible to wildfires by visiting:\u00a0 </span><a href=\"http://www.firewise.org\"><span>www.firewise.org</span></a><span>\u00a0</span></li><li><span>Virginia\u2019s 4 p.m. Burning Law remains in effect until April 30, 2024. It bans open-air burning before 4 p.m. if the fire is within 300 feet of the woods or dry grass which could carry fire to the woods. Burning is allowed between 4 p.m. and midnight as long as the burner takes proper precautions and attends the fire at all times. For more information, please visit\u00a0</span><a href=\"https://dof.virginia.gov/wildland-prescribed-fire/fire-laws/4-pm-burning-law\"><span>https://dof.virginia.gov/wildland-prescribed-fire/fire-laws/4-pm-burning-law</span></a><span>.</span></li></ul>",
+                "field_incident_overview": "<p>The North Zone Complex covers five wildfires in the George Washington and Jefferson National Forests and on state and private land in West Virginia and Virginia. They are: <strong>Waterfall Mountain/Shenandoah Forest/211 Fire, Waites Run Fire, Capon/Brush Run Fire, Edith Gap/Serenity Ridge Fire, and Cove Mountain Fire. </strong>Co<span>mmand of the North Zone Complex has been transferred to a local Type 3 Team led by Incident Commander Colten Moor.&nbsp;</span></p><p><strong>FINAL Fire Update - Wednesday April 3</strong><span><strong>, 2024</strong></span></p><p><a><span><strong>Current Status:</strong></span></a><span> Command of the North Zone Complex is assigned to a local Type 3 Team led by Incident Commander Colten Moor.&nbsp;&nbsp;The Team will hand command of the incident back to the local unit on Saturday April 6th.&nbsp; Cove, Edith Gap, Capon, Waterfall Mountain and Waites Run Fires will be monitored and patrolled until declared out. With the increase in moisture and more favorable weather conditions all fires associated with the North Zone Complex have been contained.</span></p><p><span>Closure orders for all areas in the North Zone Complex remain in effect. The local district will continue to assess conditions on the ground and determine when it is safe to re-open the areas to the public. Be aware of areas adjacent to recently burned areas as they are prone to flash flooding and debris flows. Continuation of suppression repair will occur as needs are identified. &nbsp;Firefighters continue to remove snags, address other safety concerns, and continue to secure containment lines.&nbsp; Fire and insect weakened trees continue to fall within burned areas. Road conditions have deteriorated due to rainfall and equipment traffic.&nbsp;Burn Area Emergency Response (BAER) Team will be working on plans to rehabilitate damage to natural drainages and structures moving forward.</span></p><p><span><strong>Individual Fire Updates: 15,977 total acres 100% contained</strong></span></p><ol><li><span>Waterfall Mountain/Shenandoah Forest/211 West Fire in Shenandoah and Page Counties, VA</span></li></ol><ul><li><span>6,399 acres; <strong>100% contained</strong></span></li></ul><ol><li><span>Waites Run Fire in Hardy County, WV</span><ul><li><span>6,223 acres, <strong>100% contained</strong></span></li></ul></li><li><span>Capon/Brush Run Fire in Rockingham County, VA&nbsp;</span><ul><li><span>2,368 acres, <strong>100% contained</strong></span></li></ul></li><li><span>Edith Gap/Serenity Ridge Fire in Shenandoah and Page Counties, VA</span><ul><li><span>832 acres, <strong>100% contained</strong></span></li></ul></li><li><span>Cove Mountain Fire in Hardy County, WV</span><ul><li><span>155 acres, <strong>100% contained</strong></span></li></ul></li></ol><p><span><strong>Resources:&nbsp;</strong>5 Type 2 Crews, 1 Type 2IA crew, 1 Type 3 helicopter, 6 engines, 1 dozers and 108 personnel<strong>.&nbsp;</strong></span></p><p><span><strong>Date and Cause Reported:&nbsp;</strong>The fires were reported on Wednesday, March 20, 2024, and Thursday, March 21, 2024. The causes of the fires are undetermined.&nbsp;</span></p><p><span><strong>Weather:&nbsp;</strong>Today unsettled weather continues as multiple rounds of showers and storms impact the region. &nbsp;A series of cold fronts sweep through the area Wednesday and Thursday, bringing windy conditions that last through the weekend. High pressure builds overhead Sunday into early next week</span><a><span>.</span></a></p><p><span><strong>Closures: </strong>For the protection of public health and safety, and for the protection of resources, <strong>please respect area, road and trail closures.</strong>&nbsp; Check the George Washington and Jefferson website for the full list of closures.&nbsp;</span><a href=\"http://www.fs.usda.gov/gwj\"><span>www.fs.usda.gov/gwj</span></a></p><p><span><strong>Advisories:&nbsp;</strong>We ask the public to avoid areas with active fire for their own safety and to allow firefighters to work safely. Public and firefighter safety is always our top priority. In addition, <strong>please do not fly drones</strong> near or over a wildfire. Drones and firefighting aircraft are a dangerous mix and could lead to accidents or slow down wildfire suppression. If you fly, we can\u2019t.</span></p><p><span><strong>Smoke and Air Quality:&nbsp;</strong>&nbsp;Air quality&nbsp;information&nbsp;is&nbsp;available&nbsp;at&nbsp;</span><a href=\"http://www.airnow.gov\"><span>www.airnow.gov</span></a><span>.&nbsp;</span></p><p><span><strong>General Fire Information:&nbsp;</strong></span></p><ul><li><span>Homeowners can learn how to make their homes less susceptible to wildfires by visiting:&nbsp; </span><a href=\"http://www.firewise.org\"><span>www.firewise.org</span></a><span>&nbsp;</span></li><li><span>Virginia\u2019s 4 p.m. Burning Law remains in effect until April 30, 2024. It bans open-air burning before 4 p.m. if the fire is within 300 feet of the woods or dry grass which could carry fire to the woods. Burning is allowed between 4 p.m. and midnight as long as the burner takes proper precautions and attends the fire at all times. For more information, please visit&nbsp;</span><a href=\"https://dof.virginia.gov/wildland-prescribed-fire/fire-laws/4-pm-burning-law\"><span>https://dof.virginia.gov/wildland-prescribed-fire/fire-laws/4-pm-burning-law</span></a><span>.</span></li></ul>",
                 "field_percent_of_perimeter": "100",
                 "field_title_and_unit": "VAVAF 2024 North Zone Complex",
                 "field_unit_code": "VAVAF",
                 "id": "317087",
                 "lat_deg": "38",
                 "lat_min": "46",
                 "lat_sec": "8",
@@ -773,19 +773,19 @@
                 "coordinates": [
                     -79.264106,
                     41.835161
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 2 days ago",
+                "changed": "2 weeks ago",
                 "created": "<time datetime=\"2024-04-02T12:36:35-04:00\">2024-04-02</time>\n",
                 "field_active": "1",
                 "field_incident_description": "We conduct prescribed fires with the safety of the public and firefighters as our highest priority.<br />\r\n<br />\r\nPrescribed fires reduce the amount of hazardous fuels that, when left unburned, can lead to uncontrolled wildfires that could threaten human life and property.<br />\r\n<br />\r\nWe use fire as a tool only when the parameters of our approved burn plan are met, including acceptable wind speed and direction, relative humidities, temperatures, fire danger, seasonal restrictions, and mitigation of potential smoke impacts.<br />\r\n<br />\r\nFire management staff, in collaboration with forest resource specialists, identified several ecological objectives for the planned burn activities. Objectives include hazardous wildfire fuels reduction, improving forest health with vegetation diversity, and enhancing important wildlife habitat. Fires are a historic and natural process for some ecosystems in the Allegheny National Forest, grasslands and oak-hickory forests are two prime examples. <br />\r\n<br />\r\nOak-hickory forests, which comprise approximately 16 percent of the Forest, require periodic fires to reduce competing undesirable vegetation, recycle soil nutrients, and stimulate the increased production of acorns, blueberries, blackberries, and other mast crops. White-tailed deer, turkey, butterflies, songbirds, grouse, snakes, turtles, and other wildlife species utilize burned areas for feeding, nesting, warming, and a place to raise their young.<br />\r\n<br />\r\n",
-                "field_incident_overview": "<p><span>The US Department of Agriculture, Forest Service plans to use prescribed fire as a forest management tool from early April until mid-May in the Allegheny National Forest. We do not have exact dates yet. Our operations are weather-dependent, and we will implement prescribed fires at the optimal time to achieve the best results. This spring, we plan to treat 400 acres spread across five project areas located in the Warren County portion of the Bradford Ranger District.\u00a0</span></p><p>We will notify communities near the burn sites 24 to 48 hours before ignitions. For public safety, we will post road signs and utilize road guards if necessary. To keep community members informed we will post information on our social media channels, @Allegheny_NF / Twitter and AlleghenyNF / Facebook.</p>",
+                "field_incident_overview": "<p><span>The US Department of Agriculture, Forest Service plans to use prescribed fire as a forest management tool from early April until mid-May in the Allegheny National Forest. We do not have exact dates yet. Our operations are weather-dependent, and we will implement prescribed fires at the optimal time to achieve the best results. This spring, we plan to treat 400 acres spread across five project areas located in the Warren County portion of the Bradford Ranger District.&nbsp;</span></p><p>We will notify communities near the burn sites 24 to 48 hours before ignitions. For public safety, we will post road signs and utilize road guards if necessary. To keep community members informed we will post information on our social media channels, @Allegheny_NF / Twitter and AlleghenyNF / Facebook.</p>",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "PAALF Spring Prescribed Fire Plan 2024",
                 "field_unit_code": "PAALF",
                 "id": "317115",
                 "lat_deg": "41",
                 "lat_min": "50",
                 "lat_sec": "6.58",
@@ -805,19 +805,19 @@
                 "coordinates": [
                     -89.180322,
                     46.269811
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 2 days ago",
+                "changed": "1 month 2 weeks ago",
                 "created": "<time datetime=\"2024-04-02T14:00:40-04:00\">2024-04-02</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p>All planned prescribed fires are weather-dependent and will likely be conducted between late April and early fall, when appropriate moisture, fuel and wind conditions are more likely.\u00a0</p><p><span><strong>Ottawa National Forest Proposed Prescribed Fire Projects</strong></span></p><p><span><strong>Project Name - Acres - Purpose of project</strong></span></p><p><span>Little Falls, \u00a020 acres, \u00a0Wildlife Habitat Improvement and Maintenance</span></p><p><span>1300 Railroad, \u00a027 acres, Wildlife Habitat Improvement and Maintenance</span></p><p><span>Bond Falls, \u00a080 acres, \u00a0Wildlife Habitat Improvement and Maintenance</span></p><p><span>Black Spruce, \u00a03 acres, Wildlife Habitat Improvement and Maintenance</span></p><p><span>Lucky Charm, 55 acres, \u00a0Enhance Oak Regeneration</span></p><p><span>Soo Hemlock, \u00a010 acres, \u00a0Enhance Hemlock Regeneration</span></p><p><span>Black Harbor 2 Enhance Native Plants/Pollinators</span></p><p><span>Cooks, \u00a093 acres, \u00a0Reduce Hazardous Fuels</span></p><p><span>Camp Nesbit, \u00a018 acres, \u00a0Reduce Hazardous Fuels</span></p><p><span>Dinner Lake Piles, \u00a021 acres, \u00a0Reduce Hazardous Fuels</span></p><p><span>Paystreak Piles, \u00a019 acres, \u00a0Reduce Hazardous Fuels</span></p><p><span><strong>Total Acres 348</strong></span></p><p><span>\u00a0</span></p><p><span>Maps for the units' possible 2024 prescribed fire are available here:</span></p><ul type=\"disc\"><li><a href=\"https://usfs.maps.arcgis.com/apps/instant/sidebar/index.html?appid=0b202f990a244b669a85acff82bc66c5\"><span>Upper Peninsula Fire Management Map</span></a></li></ul><p>\u00a0</p><p><span>During active burning, smoke and flames may be visible from roads and in areas downwind of the burn site. Smoke may settle in some areas in the evening hours; however, ignition days and times will be adjusted to avoid smoke sensitive areas. If you have health problems that may be aggravated by smoke, please contact your nearest Zone Fire Management Officer. Affected individuals will be notified of prescribed fires that are conducted on Forest Service Lands in their vicinity the day of the burn.</span></p><ul type=\"disc\"><li><span>Ottawa National Forest: Forest Paukert, \u00a0(906) 358-4036</span></li></ul><p><span>Prescribed burning provides benefits to our natural resources as well as reducing hazardous fuels on our National Forests. The Forest Service\u2019s goals in burning wildlife openings are:</span></p><ul type=\"disc\"><li><span>Provide improved breeding and foraging habitat for early successional and cavity dependent species.</span></li><li><span>Set back vegetative succession and maintain wildlife openings.</span></li><li><span>Maintain burn units as part of a system of fuel breaks (including safety zones, escape routes, staging areas and control lines).</span></li><li><span>Remove or reduce the impact of non-native invasive species.</span></li><li><span>Reduce the risk of wildfires by reducing hazardous fuels.</span></li><li><span>Train personnel in the use of wildland fire in a safe and efficient manner.</span></li></ul><p><span>The Forest Service\u2019s goals in conducting site preparation burns are:</span></p><ul type=\"disc\"><li><span>Naturally regenerate pine using prescribed fire.</span></li><li><span>Kill red pinecone borer larvae.</span></li><li><span>Stress over-story red pine to enhance cone production.</span></li><li><span>Reduce hazardous fuel loading within unit.</span></li></ul><p><span>Please contact your local Forest Service office (</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fhiawatha%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=SZkbm8EYVuEHhzlgk6%2B1DcvKdpeykMiRFSDYMGvqETk%3D&amp;reserved=0\"><span>Hiawatha offices</span></a><span>,\u00a0</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fottawa%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=w%2F8FCspTxl1hi9%2FEfPB3tcLsGTddMTlurHaGMEHi0zA%3D&amp;reserved=0\"><span>Ottawa offices</span></a><span>)\u00a0if you have any questions.</span></p><p><span>\u00a0</span></p>",
+                "field_incident_overview": "<p>All planned prescribed fires are weather-dependent and will likely be conducted between late April and early fall, when appropriate moisture, fuel and wind conditions are more likely.&nbsp;</p><p><span><strong>Ottawa National Forest Proposed Prescribed Fire Projects</strong></span></p><p><span><strong>Project Name - Acres - Purpose of project</strong></span></p><p><span>Little Falls, &nbsp;20 acres, &nbsp;Wildlife Habitat Improvement and Maintenance</span></p><p><span>1300 Railroad, &nbsp;27 acres, Wildlife Habitat Improvement and Maintenance</span></p><p><span>Bond Falls, &nbsp;80 acres, &nbsp;Wildlife Habitat Improvement and Maintenance</span></p><p><span>Black Spruce, &nbsp;3 acres, Wildlife Habitat Improvement and Maintenance</span></p><p><span>Lucky Charm, 55 acres, &nbsp;Enhance Oak Regeneration</span></p><p><span>Soo Hemlock, &nbsp;10 acres, &nbsp;Enhance Hemlock Regeneration</span></p><p><span>Black Harbor 2 Enhance Native Plants/Pollinators</span></p><p><span>Cooks, &nbsp;93 acres, &nbsp;Reduce Hazardous Fuels</span></p><p><span>Camp Nesbit, &nbsp;18 acres, &nbsp;Reduce Hazardous Fuels</span></p><p><span>Dinner Lake Piles, &nbsp;21 acres, &nbsp;Reduce Hazardous Fuels</span></p><p><span>Paystreak Piles, &nbsp;19 acres, &nbsp;Reduce Hazardous Fuels</span></p><p><span><strong>Total Acres 348</strong></span></p><p><span>&nbsp;</span></p><p><span>Maps for the units' possible 2024 prescribed fire are available here:</span></p><ul type=\"disc\"><li><a href=\"https://usfs.maps.arcgis.com/apps/instant/sidebar/index.html?appid=0b202f990a244b669a85acff82bc66c5\"><span>Upper Peninsula Fire Management Map</span></a></li></ul><p>&nbsp;</p><p><span>During active burning, smoke and flames may be visible from roads and in areas downwind of the burn site. Smoke may settle in some areas in the evening hours; however, ignition days and times will be adjusted to avoid smoke sensitive areas. If you have health problems that may be aggravated by smoke, please contact your nearest Zone Fire Management Officer. Affected individuals will be notified of prescribed fires that are conducted on Forest Service Lands in their vicinity the day of the burn.</span></p><ul type=\"disc\"><li><span>Ottawa National Forest: Forest Paukert, &nbsp;(906) 358-4036</span></li></ul><p><span>Prescribed burning provides benefits to our natural resources as well as reducing hazardous fuels on our National Forests. The Forest Service\u2019s goals in burning wildlife openings are:</span></p><ul type=\"disc\"><li><span>Provide improved breeding and foraging habitat for early successional and cavity dependent species.</span></li><li><span>Set back vegetative succession and maintain wildlife openings.</span></li><li><span>Maintain burn units as part of a system of fuel breaks (including safety zones, escape routes, staging areas and control lines).</span></li><li><span>Remove or reduce the impact of non-native invasive species.</span></li><li><span>Reduce the risk of wildfires by reducing hazardous fuels.</span></li><li><span>Train personnel in the use of wildland fire in a safe and efficient manner.</span></li></ul><p><span>The Forest Service\u2019s goals in conducting site preparation burns are:</span></p><ul type=\"disc\"><li><span>Naturally regenerate pine using prescribed fire.</span></li><li><span>Kill red pinecone borer larvae.</span></li><li><span>Stress over-story red pine to enhance cone production.</span></li><li><span>Reduce hazardous fuel loading within unit.</span></li></ul><p><span>Please contact your local Forest Service office (</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fhiawatha%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=SZkbm8EYVuEHhzlgk6%2B1DcvKdpeykMiRFSDYMGvqETk%3D&amp;reserved=0\"><span>Hiawatha offices</span></a><span>,&nbsp;</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fottawa%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=w%2F8FCspTxl1hi9%2FEfPB3tcLsGTddMTlurHaGMEHi0zA%3D&amp;reserved=0\"><span>Ottawa offices</span></a><span>)&nbsp;if you have any questions.</span></p><p><span>&nbsp;</span></p>",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "MIOTF 2024 Upper Peninsula Fire Management Unit Prescribed Fire Ottawa National Forest",
                 "field_unit_code": "MIOTF",
                 "id": "317117",
                 "lat_deg": "46",
                 "lat_min": "15",
                 "lat_sec": "71.32",
@@ -837,19 +837,19 @@
                 "coordinates": [
                     -87.022111,
                     45.856222
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 2 days ago",
+                "changed": "1 month 2 weeks ago",
                 "created": "<time datetime=\"2024-04-02T14:48:36-04:00\">2024-04-02</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p><strong>2024 USDA Forest Service Upper Peninsula Fire Management Unit Prescribed Fire Projects - Hiawatha NF West Zone\u00a0</strong></p><p>All planned prescribed fires are weather-dependent and will likely be conducted between late April and early fall, when appropriate moisture, fuel and wind conditions are more likely.\u00a0</p><p><span>Maps for the units' possible 2024 prescribed fire are available here:</span></p><ul type=\"disc\"><li><a href=\"https://usfs.maps.arcgis.com/apps/instant/sidebar/index.html?appid=0b202f990a244b669a85acff82bc66c5\"><span>Upper Peninsula Fire Management Map</span></a></li></ul><p><span><strong>Hiawatha National Forest West Zone Proposed Prescribed Fire Activity</strong></span></p><p><span><strong>Project name - Acres - Purpose of project\u00a0</strong></span></p><p><span>Little Ridge #3, 70 acres, \u00a0Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>East Point #1, 48 acres, Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>East Point #4, 10 acres, Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Pine Plains #7, 87 acres, Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Pine Plains #10, 8 acres, Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Ready Lake, \u00a0467 acres, Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Mormon Creek, \u00a073 acres, \u00a0Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Highbridge #2, \u00a025 acres, Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Kilpecker, \u00a025 acres, \u00a0Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>8 Mile Unit, \u00a0183 acres, \u00a0Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Farm Field, \u00a04 acres, \u00a0Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Mike White #1, \u00a079 acres, \u00a0Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Mike White #2, \u00a0129 acres, \u00a0Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>Dutch Mill #3, \u00a082 acres, \u00a0Wildlife Habitat Improvement and Maintenance\u00a0</span></p><p><span>East Lake #1, 566 acres, \u00a0Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>East Lake #2, \u00a060 acres, \u00a0Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>East Lake #3, \u00a054 acres, \u00a0Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>East Lake #4, \u00a08 acres, \u00a0Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Indian River #2, \u00a075 acres, \u00a0Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Indian River #3, \u00a060 acres, \u00a0Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Stueben Lake#1, \u00a098 acres, \u00a0Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Tombolo, \u00a034 acres, 1 Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Au Train, \u00a0170 acres, \u00a0Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Jack Pine Lodge, \u00a030 acres, \u00a0Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span><strong>Total Acres 2752</strong></span></p><p><span>During active burning, smoke and flames may be visible from roads and in areas downwind of the burn site. Smoke may settle in some areas in the evening hours; however, ignition days and times will be adjusted to avoid smoke sensitive areas. If you have health problems that may be aggravated by smoke, please contact your nearest Zone Fire Management Officer. Affected individuals will be notified of prescribed fires that are conducted on Forest Service Lands in their vicinity the day of the burn.</span></p><ul type=\"disc\"><li><span>Hiawatha West Zone: Cory Henry, \u00a0(906) 474-6442 ex 1014</span></li></ul><p><span>Prescribed burning provides benefits to our natural resources as well as reducing hazardous fuels on our National Forests. The Forest Service\u2019s goals in burning wildlife openings are:</span></p><ul type=\"disc\"><li><span>Provide improved breeding and foraging habitat for early successional and cavity dependent species.</span></li><li><span>Set back vegetative succession and maintain wildlife openings.</span></li><li><span>Maintain burn units as part of a system of fuel breaks (including safety zones, escape routes, staging areas and control lines).</span></li><li><span>Remove or reduce the impact of non-native invasive species.</span></li><li><span>Reduce the risk of wildfires by reducing hazardous fuels.</span></li><li><span>Train personnel in the use of wildland fire in a safe and efficient manner.</span></li></ul><p><span>The Forest Service\u2019s goals in conducting site preparation burns are:</span></p><ul type=\"disc\"><li><span>Naturally regenerate pine using prescribed fire.</span></li><li><span>Kill red pinecone borer larvae.</span></li><li><span>Stress over-story red pine to enhance cone production.</span></li><li><span>Reduce hazardous fuel loading within unit.</span></li></ul><p><span>Please contact your local Forest Service office (</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fhiawatha%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=SZkbm8EYVuEHhzlgk6%2B1DcvKdpeykMiRFSDYMGvqETk%3D&amp;reserved=0\"><span>Hiawatha offices</span></a><span>,\u00a0</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fottawa%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=w%2F8FCspTxl1hi9%2FEfPB3tcLsGTddMTlurHaGMEHi0zA%3D&amp;reserved=0\"><span>Ottawa offices</span></a><span>)\u00a0if you have any questions.</span></p><p><span>\u00a0</span></p>",
+                "field_incident_overview": "<p><strong>2024 USDA Forest Service Upper Peninsula Fire Management Unit Prescribed Fire Projects - Hiawatha NF West Zone&nbsp;</strong></p><p>All planned prescribed fires are weather-dependent and will likely be conducted between late April and early fall, when appropriate moisture, fuel and wind conditions are more likely.&nbsp;</p><p><span>Maps for the units' possible 2024 prescribed fire are available here:</span></p><ul type=\"disc\"><li><a href=\"https://usfs.maps.arcgis.com/apps/instant/sidebar/index.html?appid=0b202f990a244b669a85acff82bc66c5\"><span>Upper Peninsula Fire Management Map</span></a></li></ul><p><span><strong>Hiawatha National Forest West Zone Proposed Prescribed Fire Activity</strong></span></p><p><span><strong>Project name - Acres - Purpose of project&nbsp;</strong></span></p><p><span>Little Ridge #3, 70 acres, &nbsp;Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>East Point #1, 48 acres, Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>East Point #4, 10 acres, Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Pine Plains #7, 87 acres, Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Pine Plains #10, 8 acres, Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Ready Lake, &nbsp;467 acres, Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Mormon Creek, &nbsp;73 acres, &nbsp;Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Highbridge #2, &nbsp;25 acres, Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Kilpecker, &nbsp;25 acres, &nbsp;Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>8 Mile Unit, &nbsp;183 acres, &nbsp;Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Farm Field, &nbsp;4 acres, &nbsp;Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Mike White #1, &nbsp;79 acres, &nbsp;Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Mike White #2, &nbsp;129 acres, &nbsp;Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>Dutch Mill #3, &nbsp;82 acres, &nbsp;Wildlife Habitat Improvement and Maintenance&nbsp;</span></p><p><span>East Lake #1, 566 acres, &nbsp;Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>East Lake #2, &nbsp;60 acres, &nbsp;Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>East Lake #3, &nbsp;54 acres, &nbsp;Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>East Lake #4, &nbsp;8 acres, &nbsp;Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Indian River #2, &nbsp;75 acres, &nbsp;Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Indian River #3, &nbsp;60 acres, &nbsp;Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Stueben Lake#1, &nbsp;98 acres, &nbsp;Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Tombolo, &nbsp;34 acres, 1 Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Au Train, &nbsp;170 acres, &nbsp;Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span>Jack Pine Lodge, &nbsp;30 acres, &nbsp;Reintroduce Fire in a Fire-Dependent Ecosystem</span></p><p><span><strong>Total Acres 2752</strong></span></p><p><span>During active burning, smoke and flames may be visible from roads and in areas downwind of the burn site. Smoke may settle in some areas in the evening hours; however, ignition days and times will be adjusted to avoid smoke sensitive areas. If you have health problems that may be aggravated by smoke, please contact your nearest Zone Fire Management Officer. Affected individuals will be notified of prescribed fires that are conducted on Forest Service Lands in their vicinity the day of the burn.</span></p><ul type=\"disc\"><li><span>Hiawatha West Zone: Cory Henry, &nbsp;(906) 474-6442 ex 1014</span></li></ul><p><span>Prescribed burning provides benefits to our natural resources as well as reducing hazardous fuels on our National Forests. The Forest Service\u2019s goals in burning wildlife openings are:</span></p><ul type=\"disc\"><li><span>Provide improved breeding and foraging habitat for early successional and cavity dependent species.</span></li><li><span>Set back vegetative succession and maintain wildlife openings.</span></li><li><span>Maintain burn units as part of a system of fuel breaks (including safety zones, escape routes, staging areas and control lines).</span></li><li><span>Remove or reduce the impact of non-native invasive species.</span></li><li><span>Reduce the risk of wildfires by reducing hazardous fuels.</span></li><li><span>Train personnel in the use of wildland fire in a safe and efficient manner.</span></li></ul><p><span>The Forest Service\u2019s goals in conducting site preparation burns are:</span></p><ul type=\"disc\"><li><span>Naturally regenerate pine using prescribed fire.</span></li><li><span>Kill red pinecone borer larvae.</span></li><li><span>Stress over-story red pine to enhance cone production.</span></li><li><span>Reduce hazardous fuel loading within unit.</span></li></ul><p><span>Please contact your local Forest Service office (</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fhiawatha%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=SZkbm8EYVuEHhzlgk6%2B1DcvKdpeykMiRFSDYMGvqETk%3D&amp;reserved=0\"><span>Hiawatha offices</span></a><span>,&nbsp;</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fottawa%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=w%2F8FCspTxl1hi9%2FEfPB3tcLsGTddMTlurHaGMEHi0zA%3D&amp;reserved=0\"><span>Ottawa offices</span></a><span>)&nbsp;if you have any questions.</span></p><p><span>&nbsp;</span></p>",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "MIHIF 2024 Upper Peninsula Unit Prescribed Fire Hiawatha NF West Zone",
                 "field_unit_code": "MIHIF",
                 "id": "317119",
                 "lat_deg": "45",
                 "lat_min": "51",
                 "lat_sec": "22.4",
@@ -869,19 +869,19 @@
                 "coordinates": [
                     -84.83075,
                     45.87848
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "1 week 2 days ago",
+                "changed": "1 month 2 weeks ago",
                 "created": "<time datetime=\"2024-04-02T15:03:03-04:00\">2024-04-02</time>\n",
                 "field_active": "1",
                 "field_incident_description": "",
-                "field_incident_overview": "<p><strong>2024 USDA Forest Service Upper Peninsula Fire Management Unit Prescribed Fire Projects - Hiawatha NF East Zone\u00a0</strong></p><p>All planned prescribed fires are weather-dependent and will likely be conducted between late April and early fall, when appropriate moisture, fuel and wind conditions are more likely.\u00a0</p><p><span>Maps for the units' possible 2024 prescribed fire are available here:</span></p><ul type=\"disc\"><li><p><a href=\"https://usfs.maps.arcgis.com/apps/instant/sidebar/index.html?appid=0b202f990a244b669a85acff82bc66c5\"><span>Upper Peninsula Fire Management Map</span></a></p><p>\u00a0</p></li></ul><p><span><strong>Hiawatha National Forest East Zone Proposed Prescribed Fire Activity</strong></span></p><p><span><strong>Project Name - Acres - Purpose of project</strong></span></p><p><span>Betchler, \u00a04675 acres, Wildlife Habitat Improvement and Maintenance</span></p><p><span>Bramley, 161 acres, \u00a0Seed Collection</span></p><p><span>Cape Cod, \u00a045 acres, Site Prep for Regeneration</span></p><p><span>Crimson, 34 acres, \u00a0Wildlife Habitat Improvement and Maintenance</span></p><p><span>Fugi, \u00a0345 acres, \u00a0Site Prep for Regeneration</span></p><p><span>Gala, \u00a0402 acres, \u00a0Wildlife Habitat Improvement and Maintenance</span></p><p><span>Highbanks, \u00a0977 acres, Site Prep for Regeneration/ Reduce Hazardous Fuels</span></p><p><span>Inkwell, \u00a0138 acres, \u00a0Wildlife Habitat Improvement and Maintenance</span></p><p><span>North Rifle Range, \u00a099 acres, \u00a0Wildlife Habitat Improvement and Maintenance</span></p><p><span>Paula Red, \u00a064 acres, \u00a0Site Prep for Regeneration</span></p><p><span>Plantation, \u00a038 acres, \u00a0Reduce Hazardous Fuels</span></p><p><span>Rusty Waikiki, \u00a050 acres, \u00a0Site Prep for Regeneration</span></p><p><span><strong>Total Acres 7,128</strong></span></p><p><span>During active burning, smoke and flames may be visible from roads and in areas downwind of the burn site. Smoke may settle in some areas in the evening hours; however, ignition days and times will be adjusted to avoid smoke sensitive areas. If you have health problems that may be aggravated by smoke, please contact your nearest Zone Fire Management Officer. Affected individuals will be notified of prescribed fires that are conducted on Forest Service Lands in their vicinity the day of the burn.</span></p><ul type=\"disc\"><li><span>Hiawatha West Zone: Brian Wolvert,(906) 630-1386</span></li></ul><p><span>Prescribed burning provides benefits to our natural resources as well as reducing hazardous fuels on our National Forests. The Forest Service\u2019s goals in burning wildlife openings are:</span></p><ul type=\"disc\"><li><span>Provide improved breeding and foraging habitat for early successional and cavity dependent species.</span></li><li><span>Set back vegetative succession and maintain wildlife openings.</span></li><li><span>Maintain burn units as part of a system of fuel breaks (including safety zones, escape routes, staging areas and control lines).</span></li><li><span>Remove or reduce the impact of non-native invasive species.</span></li><li><span>Reduce the risk of wildfires by reducing hazardous fuels.</span></li><li><span>Train personnel in the use of wildland fire in a safe and efficient manner.</span></li></ul><p><span>The Forest Service\u2019s goals in conducting site preparation burns are:</span></p><ul type=\"disc\"><li><span>Naturally regenerate pine using prescribed fire.</span></li><li><span>Kill red pinecone borer larvae.</span></li><li><span>Stress over-story red pine to enhance cone production.</span></li><li><span>Reduce hazardous fuel loading within unit.</span></li></ul><p><span>Please contact your local Forest Service office (</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fhiawatha%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=SZkbm8EYVuEHhzlgk6%2B1DcvKdpeykMiRFSDYMGvqETk%3D&amp;reserved=0\"><span>Hiawatha offices</span></a><span>,\u00a0</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fottawa%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=w%2F8FCspTxl1hi9%2FEfPB3tcLsGTddMTlurHaGMEHi0zA%3D&amp;reserved=0\"><span>Ottawa offices</span></a><span>)\u00a0if you have any questions.</span></p><p><span>\u00a0</span></p>",
+                "field_incident_overview": "<p><strong>2024 USDA Forest Service Upper Peninsula Fire Management Unit Prescribed Fire Projects - Hiawatha NF East Zone&nbsp;</strong></p><p>All planned prescribed fires are weather-dependent and will likely be conducted between late April and early fall, when appropriate moisture, fuel and wind conditions are more likely.&nbsp;</p><p><span>Maps for the units' possible 2024 prescribed fire are available here:</span></p><ul type=\"disc\"><li><p><a href=\"https://usfs.maps.arcgis.com/apps/instant/sidebar/index.html?appid=0b202f990a244b669a85acff82bc66c5\"><span>Upper Peninsula Fire Management Map</span></a></p><p>&nbsp;</p></li></ul><p><span><strong>Hiawatha National Forest East Zone Proposed Prescribed Fire Activity</strong></span></p><p><span><strong>Project Name - Acres - Purpose of project</strong></span></p><p><span>Betchler, &nbsp;4675 acres, Wildlife Habitat Improvement and Maintenance</span></p><p><span>Bramley, 161 acres, &nbsp;Seed Collection</span></p><p><span>Cape Cod, &nbsp;45 acres, Site Prep for Regeneration</span></p><p><span>Crimson, 34 acres, &nbsp;Wildlife Habitat Improvement and Maintenance</span></p><p><span>Fugi, &nbsp;345 acres, &nbsp;Site Prep for Regeneration</span></p><p><span>Gala, &nbsp;402 acres, &nbsp;Wildlife Habitat Improvement and Maintenance</span></p><p><span>Highbanks, &nbsp;977 acres, Site Prep for Regeneration/ Reduce Hazardous Fuels</span></p><p><span>Inkwell, &nbsp;138 acres, &nbsp;Wildlife Habitat Improvement and Maintenance</span></p><p><span>North Rifle Range, &nbsp;99 acres, &nbsp;Wildlife Habitat Improvement and Maintenance</span></p><p><span>Paula Red, &nbsp;64 acres, &nbsp;Site Prep for Regeneration</span></p><p><span>Plantation, &nbsp;38 acres, &nbsp;Reduce Hazardous Fuels</span></p><p><span>Rusty Waikiki, &nbsp;50 acres, &nbsp;Site Prep for Regeneration</span></p><p><span><strong>Total Acres 7,128</strong></span></p><p><span>During active burning, smoke and flames may be visible from roads and in areas downwind of the burn site. Smoke may settle in some areas in the evening hours; however, ignition days and times will be adjusted to avoid smoke sensitive areas. If you have health problems that may be aggravated by smoke, please contact your nearest Zone Fire Management Officer. Affected individuals will be notified of prescribed fires that are conducted on Forest Service Lands in their vicinity the day of the burn.</span></p><ul type=\"disc\"><li><span>Hiawatha West Zone: Brian Wolvert,(906) 630-1386</span></li></ul><p><span>Prescribed burning provides benefits to our natural resources as well as reducing hazardous fuels on our National Forests. The Forest Service\u2019s goals in burning wildlife openings are:</span></p><ul type=\"disc\"><li><span>Provide improved breeding and foraging habitat for early successional and cavity dependent species.</span></li><li><span>Set back vegetative succession and maintain wildlife openings.</span></li><li><span>Maintain burn units as part of a system of fuel breaks (including safety zones, escape routes, staging areas and control lines).</span></li><li><span>Remove or reduce the impact of non-native invasive species.</span></li><li><span>Reduce the risk of wildfires by reducing hazardous fuels.</span></li><li><span>Train personnel in the use of wildland fire in a safe and efficient manner.</span></li></ul><p><span>The Forest Service\u2019s goals in conducting site preparation burns are:</span></p><ul type=\"disc\"><li><span>Naturally regenerate pine using prescribed fire.</span></li><li><span>Kill red pinecone borer larvae.</span></li><li><span>Stress over-story red pine to enhance cone production.</span></li><li><span>Reduce hazardous fuel loading within unit.</span></li></ul><p><span>Please contact your local Forest Service office (</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fhiawatha%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=SZkbm8EYVuEHhzlgk6%2B1DcvKdpeykMiRFSDYMGvqETk%3D&amp;reserved=0\"><span>Hiawatha offices</span></a><span>,&nbsp;</span><a href=\"https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.fs.usda.gov%2Fdetail%2Fottawa%2Fabout-forest%2Foffices&amp;data=05%7C01%7C%7C3b8d7b3f47cb42a5f59b08db34805475%7Ced5b36e701ee4ebc867ee03cfa0d4697%7C0%7C0%7C638161497993859060%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&amp;sdata=w%2F8FCspTxl1hi9%2FEfPB3tcLsGTddMTlurHaGMEHi0zA%3D&amp;reserved=0\"><span>Ottawa offices</span></a><span>)&nbsp;if you have any questions.</span></p><p><span>&nbsp;</span></p>",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "MIHIF 2024 Upper Peninsula Unit Prescribed Fire Hiawatha NF East Zone",
                 "field_unit_code": "MIHIF",
                 "id": "317120",
                 "lat_deg": "45",
                 "lat_min": "52",
                 "lat_sec": "42.528",
@@ -901,19 +901,19 @@
                 "coordinates": [
                     -106.978995,
                     33.934358
                 ],
                 "type": "Point"
             },
             "properties": {
-                "changed": "5 hours 7 minutes ago",
+                "changed": "2 days 13 hours ago",
                 "created": "<time datetime=\"2024-04-09T13:18:04-04:00\">2024-04-09</time>\n",
                 "field_active": "1",
-                "field_incident_description": "Pile burns work alongside both prescribed fire and mechanical thinning to remove fuels such as woody debris and logging scraps from the forest floor during times of opportune weather.<br />\r\n<br />\r\nFire managers make every effort to effectively plan and execute burn plans at times when weather allows for smoke impacts to be minimized and transport up and over communities.<br />\r\n<br />\r\nFor more information about prescribed burns and why wildfire is a necessary part of this ecosystem, please visit our website at coconinonationalforest.us.",
-                "field_incident_overview": "<p><strong>NAME: </strong>Cedar Creek Prescribed Burn Area</p><p><strong>DISTRICT: </strong>Smokey Bear Ranger District 1</p><p><strong>PLANNED ACRES: </strong>87</p><p><strong>DATES: </strong>April<strong> </strong>9-19</p><p><strong>CURRENT STATUS: </strong>ACTIVE</p><p>_____________________________________________________________________________________</p><p><strong>NAME: </strong>16 Springs Prescribed Burn Area</p><p><strong>DISTRICT: </strong>Sacramento Ranger District 2</p><p><strong>PLANNED ACRES: </strong>500</p><p><strong>DATES: </strong>April<strong> </strong>11-26</p><p><strong>CURRENT STATUS: </strong>ACTIVE</p>",
+                "field_incident_description": "Pile burns work alongside both prescribed fire and mechanical thinning to remove fuels such as woody debris and logging scraps from the forest floor during times of opportune weather.<br />\r\n<br />\r\nFire managers make every effort to effectively plan and execute burn plans at times when weather allows for smoke impacts to be minimized and transport up and over communities.<br />\r\n<br />\r\nFor more information about prescribed burns and why wildfire is a necessary part of this ecosystem, please visit our website at https://www.fs.usda.gov/lincoln",
+                "field_incident_overview": "<p>Date: May 18, 2024</p><p>Location: 16 Springs Prescribed Burn Area, Sacramento Ranger District, Lincoln National Forest</p><p>Size: 350 Acres</p><p>Crews are on-scene and proceeding with ignitions in the 16 Springs Prescribed Burn area. &nbsp;Signage has been put in place to mark the active burn area. Operations will continue through today, and the area will continue to be monitored through the next week for any hotspots.</p><p>&nbsp;</p>",
                 "field_percent_of_perimeter": "",
                 "field_title_and_unit": "NMLNF Lincoln National Forest prescribed fire and pile burns Spring 2024",
                 "field_unit_code": "NMLNF",
                 "id": "317128",
                 "lat_deg": "33.9343580",
                 "lat_min": "",
                 "lat_sec": "",
@@ -923,11 +923,971 @@
                 "measurement_type": "Acres",
                 "size": "",
                 "title": "Lincoln National Forest prescribed fire and pile burns (Spring 2024)",
                 "type": "Prescribed Fire",
                 "urlPath": "/nmlnf-lincoln-national-forest-prescribed-fire-and-pile-burns-spring-2024"
             },
             "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -107.701684,
+                    38.117535
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "3 weeks 3 days ago",
+                "created": "<time datetime=\"2024-04-16T19:09:02-04:00\">2024-04-16</time>\n",
+                "field_active": "1",
+                "field_incident_description": "On April 22, 2024, a 112 acre unit on a south-facing aspect in the middle of the Baldy Mountain Project area was treated using prescribed fire. Ignitions are complete for this portion of the project. Firefighters will continue to patrol the site until the fire is declared out. Residual smoke may be seen through the end of the week from the communities of Montrose, Ridgway, Ouray, Log Hill, and other dispersed areas along the Highway 550 corridor. ",
+                "field_incident_overview": "<p>The Baldy Mountain Landscape Resiliency and Habitat Improvement Project is located in Ouray County, approximately 2 miles southeast of Ridgeway, CO and 4.5 miles north of Ouray, CO.&nbsp;</p><p><span>On Tuesday, April 23, 2024, the Ouray Ranger District and BLM Uncompahgre Field Office were able to successfully implement the first of nine planned prescribed fire units associated with the&nbsp;</span><a href=\"https://www.nationalforests.org/regional-programs/rocky-mountain-region/baldy-mountain-landscape-resiliency-and-habitat-improvement-project\"><span>Baldy Mountain Landscape Resiliency and Habitat Improvement Project</span></a><span>. The 112-acre unit comprised of masticated oak, pinyon, juniper and aspen. It had been mechanically treated and prepped this past fall under a keystone agreement with the National Forest Foundation. Firefighters used a combination of hand and aerial ignitions with an UAS to conduct the burn. Fire managers state that the effort succeeded in producing the desired effects to meet project objectives.</span></p><p><span>Project objectives are to reduce the severity of wildfires, protect local communities, create higher quality wildlife habitat and improve the health and resiliency of the landscape. Prescribed burning reintroduces and maintains fire within a fire-dependent ecosystem, helping to stabilize and improve the resiliency of forest conditions while increasing public safety. Once ignited, firefighters will monitor and patrol the units until they declare the fire out.&nbsp;</span></p><p><span>Planning and implementation for this project have been a collaborative effort between the GMUG National Forests\u2019 Ouray Ranger District, BLM-Uncompahgre Field Office, the Natural Resources Conservation Service, the West Region Wildfire Council, the Mullin\u2019s Ranch and multiple other landowners. The project area includes lands managed by the U.S. Forest Service, BLM and private landowners. The National Forest Foundation (NFF) has been a key partner in coordinating the project.</span></p><p>&nbsp;</p><p><span>The safety of firefighters and the public is the most important factor considered when planning prescribed fires. Fire managers have developed a detailed prescribed fire plan and obtained smoke permits from the State of Colorado. For more information on how prescribed fire smoke may affect your health, please visit&nbsp;</span><a href=\"https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health\"><span>https://www.colorado.gov/pacific/cdphe/wood-smoke-and-health</span></a><span>.</span></p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "COGMF Baldy Mountain Landscape Resiliency and Habitat Improvement Project Prescribed Burn",
+                "field_unit_code": "COGMF",
+                "id": "317145",
+                "lat_deg": "38",
+                "lat_min": "7",
+                "lat_sec": "3.1270",
+                "long_deg": "107",
+                "long_min": "42",
+                "long_sec": "6.0606",
+                "measurement_type": "Acres",
+                "size": "112",
+                "title": "Baldy Mountain Landscape Resiliency and Habitat Improvement Project Prescribed Burn",
+                "type": "Prescribed Fire",
+                "urlPath": "/cogmf-baldy-mountain-landscape-resiliency-and-habitat-improvement-project-prescribed-burn"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -111.580278,
+                    35.228779
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "6 hours 57 minutes ago",
+                "created": "<time datetime=\"2024-04-17T18:30:09-04:00\">2024-04-17</time>\n",
+                "field_active": "1",
+                "field_incident_description": "Prescribed fire projects usually commence during the early spring months in northern Arizona. If you want to sign up to receive news releases about prescribed fire and other projects on Coconino National Forest, please visit https://www.fs.usda.gov/news/coconino/news-events and click on the blue &quot;Sign Up!&quot; icon in the right column.<br />\r\n<br />\r\nPrescribed fire is important part of forest restoration projects planned in accordance with the Forest Service\u2019s 10-year Wildfire Crisis Strategy. Prescribed fire and mechanical thinning work together to remove fuels such as woody debris and logging scraps from the forest floor during times of opportune weather. <br />\r\n<br />\r\nFire managers make every effort to effectively plan and execute burn plans at times when weather allows for smoke impacts to be minimized and transport up and over communities.<br />\r\n<br />\r\nFor more information about prescribed burns and why wildfire is a necessary part of this ecosystem, please visit our website at coconinonationalforest.us.",
+                "field_incident_overview": "<h2>The Flagstaff Ranger District of the Coconino National Forest has several prescribed fire plans slated for the spring of 2024. Plans are subject to change at any time due to wind and weather conditions.</h2><p>&nbsp;</p><h3>UPCOMING PROJECTS:</h3><h3>&nbsp;</h3><h3>Horseshoe (Wild Bill project area)</h3><ul><li><span><strong>Tentative dates:</strong> Project partially completed, work to resume May 21.</span></li><li><span><strong>Location:</strong> </span><a href=\"https://maps.app.goo.gl/gLjnatNsNioLWu8y8\"><span>14 miles northwest of Flagstaff</span></a><span>: 4.5 miles north of Bellemont. (</span><a href=\"https://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-05/PIO%20Wild%20Bill%20project%20area.pdf?VersionId=6wVFOoxAwO3wlcedq6whBfvcza3ndLym\"><span>Project map</span></a><span>)</span></li><li><span><strong>Size</strong>: 3,960 acres total (broken up into different amounts each day).</span></li><li><span><strong>Type of burn</strong>:</span><a href=\"https://www.fs.usda.gov/detail/coconino/fire/?cid=stelprdb5344667#methods\"><span> Broadcast, initial entry</span></a><span>. Initial entry burns mean wildfire has not been through the area in a very long time and thus results in thicker smoke due to a large amount of forest fuels being present that must be burned.</span></li><li><span><strong>Smoke impacts: </strong>Due to cold temperatures overnight, smoke will likely linger in surrounding areas longer than usual.<strong>&nbsp;</strong>Possible smoke impacts will be felt along Highway 180 and in and around Kendrick Park during the daytime. Possible smoke impacts may be felt in the Bellemont area and along Interstate 40 overnight.</span></li><li><span><strong>Why:</strong> This prescribed fire will reduce fuel loading in the project area. Additionally, it will provide protection to the Upper Rio de Flag watershed, which will reduce the ensuing risk of catastrophic wildfire and subsequent flood damage to the City of Flagstaff.</span></li><li><span><strong>Notes:</strong> There are no closures anticipated.</span></li></ul><h3>Horseshoe (Maxwell Springs project area)</h3><ul><li><span><strong>Tentative dates:</strong> Project partially completed, work to resume May 22.</span></li><li><span><strong>Location:</strong> </span><a href=\"https://maps.app.goo.gl/9nkXhggRwSBAx6aB9\"><span>11 miles northwest of Flagstaff</span></a><span>: 2.5 miles north of Bellemont. (</span><a href=\"https://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-05/PIO%20Maxwell%20Springs%20RX%20Project_Ryan%20Rawlinson.pdf?VersionId=vca5xRtwP_VN40gt.btqBWq_lM2qfM9F\"><span>Project map</span></a><span>)</span></li><li><span><strong>Size</strong>: 581 acres</span></li><li><span><strong>Type of burn</strong>: Broadcast, initial entry. Initial entry burns mean wildfire has not been through the area in a very long time and thus results in thicker smoke due to a large amount of forest fuels being present that must be burned.</span></li><li><span><strong>Smoke impacts:&nbsp;</strong>Possible smoke impacts will be felt along Highway 180 and in and around Kendrick Park during the daytime. Possible smoke impacts may be felt in the Bellemont area and along Interstate 40 overnight.</span></li><li><span><strong>Why:</strong> This prescribed fire will reduce fuel loading in the project area. Additionally, it will provide protection to the Upper Rio de Flag watershed, which will reduce the ensuing risk of catastrophic wildfire and subsequent flood damage to the City of Flagstaff.</span></li><li><span><strong>Notes:</strong> There are no closures anticipated.</span></li></ul><h3>Horseshoe (Peaks project area)</h3><ul><li><strong>Tentative dates:</strong> To be determined.</li><li><strong>Location:</strong> <a href=\"https://maps.app.goo.gl/rFGZxQEKhhNKRP1H8\">15 miles north of Flagstaff</a>: north of the San Francisco Peaks and west of Highway 89. (<a href=\"https://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-04/PIO%20Peaks%20Project%20Rx.pdf?VersionId=iiCJ7WxnJOCXUhRRV5XGK1oPbWcMjqnd\">Project map</a>)</li><li><strong>Size:</strong> 3,963 acres.</li><li><strong>Type of burn:</strong> Broadcast, maintenance. <span>Maintenance burns usually mean wildfire has recently been through the area, which tends to mean less smoke since forest fuels will not be as thick or built up over time. Broadcast burning means firefighters use tools, such as drip torches, to move fire across large swaths of land.</span></li><li><strong>Smoke impacts:</strong> Smoke is expected to travel to the northeast during ignitions. Possible impacts will be felt along Highway 89. Smoke may settle in low-lying areas overnight.</li><li><strong>Why:</strong> This prescribed fire will reduce fuel loading south of Flagstaff, thus lessening the risk of catastrophic unplanned wildfire during times of critical fire weather. This project also reintroduces fire into a fire-adapted ecosystem.</li><li><strong>Notes:</strong> There are no closures anticipated. A helicopter may be used during this project to assist with aerial ignitions.</li></ul><p>&nbsp;</p><h3>COMPLETED PROJECTS:</h3><h3>3-Echo/ Flagstaff Urban Interface South</h3><ul><li><strong>Dates: </strong>May 8 through May 10 (Wednesday through Friday).</li><li><strong>Location:</strong> <a href=\"https://maps.app.goo.gl/rgJf1dCQgSwSnD7PA\">5 miles south of Flagstaff</a>: between Lower Lake Mary and Mountainaire. (<a href=\"https://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-04/PIO%203%20Echo.pdf?VersionId=fc0hIJFgJTKXjffffiySx78hXiHgvlZr\">Project map</a>)</li><li><strong>Size:</strong> 4,622 acres total (broken up into different amounts each day)</li><li><strong>Type of burn:</strong> Broadcast, maintenance. <span>Maintenance burns usually mean wildfire has recently been through the area, which tends to mean less smoke since forest fuels will not be as thick or built up over time. Broadcast burning means firefighter</span></li><li><strong>Smoke impacts:</strong> Smoke will be highly visible from the City of Flagstaff and all surrounding areas. Smoke is expected to travel in an east or northeast direction during ignitions, and possible daytime impacts will be felt on the east side of Flagstaff, along Interstate 40, at Walnut Canyon National Monument, along Lake Mary Road south of Flagstaff and in the Continental community. Smoke may settle in low-lying areas overnight.</li><li><strong>Why:</strong> This prescribed fire will reduce fuel loading south of Flagstaff, thus lessening the risk of catastrophic unplanned wildfire during times of critical fire weather. This project also reintroduces fire into a fire-adapted ecosystem.</li><li><strong>Notes:</strong> There are no closures anticipated.</li></ul><h3>Mint West (Bar-M)</h3><ul><li><strong>Date:</strong> Saturday, May 18 (one day).</li><li><strong>Location:</strong> <a href=\"https://maps.app.goo.gl/E5ML5TQFApjPkYcu6\">25 miles south of Flagstaff</a>: South of Mormon Lake. (<a href=\"https://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-05/mint_west_project_map.pdf?VersionId=6GnGXHEdqJ_8.fypKFJ9.5bhaod3zIxB\">Project map</a>)</li><li><strong>Size:</strong> 1,742 acres.</li><li><strong>Type of burn:</strong> Broadcast, initial entry. <span>Initial entry burns mean wildfire has not been through the area in a very long time and thus results in thicker smoke due to a large amount of forest fuels being present that must be burned.</span></li><li><strong>Smoke impacts:</strong> Smoke impacts will be felt along Lake Mary Road and in the Mormon Lake Village area.</li><li><strong>Why:</strong> This prescribed fire will reduce fuel loading south of Mormon Lake, thus lessening the risk of catastrophic unplanned wildfire during times of critical fire weather. This project also reintroduces fire into a fire-adapted ecosystem.</li><li><strong>Notes: </strong>There are no closures anticipated.</li></ul><h3>&nbsp;</h3><h3>&nbsp;</h3>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "AZCOF Coconino National Forest Flagstaff Ranger District prescribed fire Spring 2024",
+                "field_unit_code": "AZCOF",
+                "id": "317151",
+                "lat_deg": "35",
+                "lat_min": "13",
+                "lat_sec": "43.6044",
+                "long_deg": "111",
+                "long_min": "34",
+                "long_sec": "49",
+                "measurement_type": "Acres",
+                "size": "",
+                "title": "Coconino National Forest - Flagstaff Ranger District prescribed fire Spring 2024",
+                "type": "Prescribed Fire",
+                "urlPath": "/azcof-coconino-national-forest-flagstaff-ranger-district-prescribed-fire-spring-2024"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -111.191434,
+                    34.611017
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 week ago",
+                "created": "<time datetime=\"2024-04-17T18:34:47-04:00\">2024-04-17</time>\n",
+                "field_active": "1",
+                "field_incident_description": "Prescribed fire projects usually commence during the early spring months in northern Arizona. If you want to sign up to receive news releases about prescribed fire and other projects on Coconino National Forest, please visit https://www.fs.usda.gov/news/coconino/news-events and click on the blue &quot;Sign Up!&quot; icon in the right column.<br />\r\n<br />\r\nPrescribed fire is important part of forest restoration projects planned in accordance with the Forest Service\u2019s 10-year Wildfire Crisis Strategy. Prescribed fire and mechanical thinning work together to remove fuels such as woody debris and logging scraps from the forest floor during times of opportune weather. <br />\r\n<br />\r\nFire managers make every effort to effectively plan and execute burn plans at times when weather allows for smoke impacts to be minimized and transport up and over communities.<br />\r\n<br />\r\nFor more information about prescribed burns and why wildfire is a necessary part of this ecosystem, please visit our website at coconinonationalforest.us.",
+                "field_incident_overview": "<h2>The Mogollon Rim Ranger District of the Coconino National Forest has several prescribed fire plans slated for the spring of 2024. More details regarding prescribed fire plans will be posted closer to time of ignition.</h2><h2>&nbsp;</h2><h2>Spring 2024 Prescribed Fire plans:</h2><p>&nbsp;</p><h3>Sawmill</h3><ul><li><strong>Tentative dates:</strong> Slated for week of May 20, 2024</li><li><strong>Location:</strong> Roughly 4.5 miles north of Happy Jack: west of Lake Mary Road.</li><li><strong>Size:</strong> 1,000 acres</li><li><strong>Type of burn:</strong> Broadcast, maintenance.</li><li><strong>Smoke impacts:</strong> To be determined</li><li><strong>Why:</strong> This project will reintroduce fire into a fire-adapted ecosystem.</li><li><strong>Notes:</strong> There are no closures anticipated.</li></ul><h3>Blue Ridge Urban Interface (<a href=\"https://inciweb-prod-media-bucket.s3.us-gov-west-1.amazonaws.com/s3fs-public/2024-05/BRUI_Visitor_map.jpg?VersionId=bD.rFm.HK1G7UK12Uvx6BIemBfWY_08w\">project map</a>)</h3><ul><li><strong>Tentative dates:</strong> Slated for spring 2024. Dates TBD</li><li><strong>Location: </strong><a href=\"https://maps.app.goo.gl/K6oPiVRZjtzpDafa6\">8.5 miles northeast of Clints Well</a>: near the Mogollon Rim Ranger Station</li><li><strong>Size:</strong> About 1350 acres</li><li><strong>Type of burn:</strong> Broadcast, maintenance. <span>Maintenance burns usually mean wildfire has recently been through the area, which tends to mean less smoke since forest fuels will not be as thick or built up over time. Broadcast burning means firefighters use tools, such as drip torches, to move fire across large swaths of land.</span></li><li><strong>Smoke impacts:</strong> Smoke may impact Highway 87 and the Blue Ridge subdivisions, as well as possible impacts to the Winslow and Holbrook areas. Due to recent land treatments, smoke impacts are expected to be light in duration.</li><li><strong>Why:</strong> This project will continue 20 years of routine fire treatment in the Blue Ridge area to protect nearby infrastructure and maintain landscape health.</li><li><strong>Notes:</strong> There are no closures anticipated. <span>However, Arizona Trail hikers are advised to avoid the project area.</span></li></ul><h3>Upper Beaver Creek</h3><ul><li><strong>Tentative dates: </strong>Slated for spring 2024. Dates TBD</li><li><strong>Location:</strong> Roughly 4.5 miles northwest of Happy Jack: southwest of Stoneman Lake.</li><li><strong>Size:</strong> To be determined</li><li><strong>Type of burn:</strong> Broadcast, maintenance.</li><li><strong>Smoke impacts:</strong> To be determined</li><li><strong>Why:</strong> This project will reintroduce fire into a fire-adapted ecosystem.</li><li><strong>Notes:</strong> There are no closures anticipated.</li></ul><h3>Clints</h3><ul><li><strong>Tentative dates:</strong> Slated for spring 2024. Dates TBD</li><li><strong>Location: </strong>Half a mile west of Clints Well.</li><li><strong>Size:</strong> To be determined</li><li><strong>Type of burn:</strong> Broadcast, maintenance.</li><li><strong>Smoke impacts:</strong> To be determined</li><li><strong>Why:</strong> This project will reintroduce fire into a fire-adapted ecosystem.</li><li><strong>Notes:</strong> There are no closures anticipated.</li></ul><h3>&nbsp;</h3>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "AZCOF Coconino National Forest Mogollon Rim Ranger District prescribed fire Spring 2024",
+                "field_unit_code": "AZCOF",
+                "id": "317152",
+                "lat_deg": "34",
+                "lat_min": "36",
+                "lat_sec": "39.6606",
+                "long_deg": "111",
+                "long_min": "11",
+                "long_sec": "29.1624",
+                "measurement_type": "Acres",
+                "size": "",
+                "title": "Coconino National Forest - Mogollon Rim Ranger District prescribed fire Spring 2024",
+                "type": "Prescribed Fire",
+                "urlPath": "/azcof-coconino-national-forest-mogollon-rim-ranger-district-prescribed-fire-spring-2024"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -113.119839,
+                    45.598717
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 week ago",
+                "created": "<time datetime=\"2024-04-18T11:42:18-04:00\">2024-04-18</time>\n",
+                "field_active": "1",
+                "field_incident_description": "Prescribed fire operations on the Beaverhead-Deerlodge National Forest. ",
+                "field_incident_overview": "<p>Every spring and fall, the Beaverhead-Deerlodge National Forest, along with its interagency partners and neighbors, plans to implement prescribed fire projects, as weather and fuels conditions allow.&nbsp;</p><p><br>Prescribed fires are carefully planned and conducted in accordance with a written burn plan. Prior to implementation, Forest fire managers coordinate with local cooperators, county officials, and interagency partners. When prescription criteria are met, firefighters implement, monitor, and patrol each burn to ensure it meets forest health and public safety objectives. All prescribed fires will be implemented in compliance with Montana air quality standards and coordinated with the Montana Department of Environmental Quality and the appropriate county health departments to minimize the impacts of smoke. Smoke may pool in drainage bottoms and along highway corridors overnight; impacts are expected to dissipate in a few days.</p><p><br>Why use prescribed fires? Prescribed fires help reduce surface fuels, increasing landscape wildfire resilience and reducing the risk of uncharacteristic wildfire effects on the landscape. In addition, they improve and maintain forest health and wildlife habitat and eliminate invasive species. The forest ecosystems in the Northern Rockies have evolved with fire, with many of them relying on periodic fires to establish and maintain forest health.&nbsp;</p><p>Benefits of prescribed fire as a forest management tool:<br>\u2022&nbsp;&nbsp;&nbsp;&nbsp;Protects communities and infrastructure by reducing hazardous fuels and the risk of future high-intensity wildfires.<br>\u2022&nbsp;&nbsp;&nbsp;&nbsp;Mitigates future wildfire risk and promote resilient fire-adapted landscapes.<br>\u2022&nbsp;&nbsp;&nbsp;&nbsp;Reduces build-up of flammable vegetation, dead and down trees, and overgrowth.<br>\u2022&nbsp;&nbsp;&nbsp;&nbsp;Improves and supports wildlife habitat for many species on the Forest.<br>\u2022&nbsp;&nbsp;&nbsp;&nbsp;Limits the spread of invasive plant species and minimizes the spread of pest insects and disease, maintaining native ecosystems.<br>\u2022&nbsp;&nbsp;&nbsp;&nbsp;Recycles nutrients back into the soil.<br>\u2022&nbsp;&nbsp;&nbsp;&nbsp;Promotes the growth of trees, plants, wildflowers, and other flora and fauna.<br>\u2022&nbsp;&nbsp;&nbsp;&nbsp;Continues the historic, natural fire regime of periodic disturbance by fire in forested ecosystems.&nbsp;<br>&nbsp;</p><p>How do we plan? Prescribed fires are planned for various units across the Forest; however, the window of opportunity for prescribed fire implementation is affected by several factors. Safety factors, weather conditions, air quality, personnel availability, and environmental regulations are continually monitored before implementation to determine feasibility of moving forward with the prescribed fire operations, during implementation, and after completion of the unit(s).&nbsp;<br>&nbsp;</p><p>Public notifications: Prior to initiating the prescribed fires, fire professionals assess conditions, conduct a test burn, and notify local governments and interested publics via website postings, email, social media, and news releases. Implementation and accomplishment updates will also be posted to the Forest website, Inciweb, and the Forest Facebook page.</p><p><br>Safety and monitoring: Trained fire professionals who have studied fire behavior and fire control techniques conduct prescribed fires in such a way to ensure the safety of the fire crew, nearby residents, and property.&nbsp;</p><p><br>&nbsp;</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "MTBDF BeaverheadDeerlodge NF Prescribed Fire Operations",
+                "field_unit_code": "MTBDF",
+                "id": "317157",
+                "lat_deg": "45",
+                "lat_min": "35",
+                "lat_sec": "55.38",
+                "long_deg": "113",
+                "long_min": "7",
+                "long_sec": "11.42",
+                "measurement_type": "Acres",
+                "size": "",
+                "title": "Beaverhead-Deerlodge NF Prescribed Fire Operations",
+                "type": "Prescribed Fire",
+                "urlPath": "/mtbdf-beaverheaddeerlodge-nf-prescribed-fire-operations"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -115.502639,
+                    46.640825
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 week 6 days ago",
+                "created": "<time datetime=\"2024-04-18T12:35:23-04:00\">2024-04-18</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span><strong>Given forecasted weather showing an increase in moisture and a decrease in temperatures, we will pause burning operations, until a more favorable weather window presents itself. Once operations have resumed, updates will be made available.</strong></span></p><p><span>The Nez Perce-Clearwater National Forests, the Idaho Department of Fish and Game, and the Rocky Mountain Elk Foundation have begun prescribed burns on the North Fork Clearwater Ranger District to improve elk habitat. The North Fork Ponderosa Pine Restoration Project had to be carefully timed to find a period of time when the moisture level of fuels was low enough and temperatures were high enough to enable the carefully planned burn.&nbsp;</span></p><p>The entirety of the project will treat 2,185 acres of mature ponderosa pine in 38 stands through a mixture of non-commercial thinning and prescribed burning. This project will ensure the long-term persistence of ponderosa pines by reducing the risk of loss due to wildfire by reducing fuels. It will also reduce overmatured brush and create desired vegetation conditions, providing more palatable, available, and nutritious browse for elk from the Lolo Herd in their primary winter habitat.</p><p>This project was made possible under the Good Neighbor Authority (GNA) which authorizes the Forest to utilize the unique capacities of local, state, and Tribal governments to achieve shared stewardship objectives. This authority allows partners to perform forest and watershed restoration work, fuels reduction, heritage and wildlife surveys on the Forest that directly benefit local communities and small businesses. Skowlund explained that \u201cGood Neighbor Authority projects provide the Forests and its partners the opportunity to leverage their respective strengths to achieve shared stewardship priorities.\u201d</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "IDNCF North Fork Ponderosa Pine Restoration Project",
+                "field_unit_code": "IDNCF",
+                "id": "317168",
+                "lat_deg": "46",
+                "lat_min": "38",
+                "lat_sec": "26.97",
+                "long_deg": "115",
+                "long_min": "30",
+                "long_sec": "9.50",
+                "measurement_type": "Acres",
+                "size": "864",
+                "title": "North Fork Ponderosa Pine Restoration Project",
+                "type": "Prescribed Fire",
+                "urlPath": "/idncf-north-fork-ponderosa-pine-restoration-project"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -116.418731,
+                    45.390986
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "4 days 8 hours ago",
+                "created": "<time datetime=\"2024-04-19T13:26:17-04:00\">2024-04-19</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p>Burning operations will continue today, May 16, as weather and fuel conditions remain favorable. Today's burn will be near the Seven Devils Road (National Forest Service Road #517).</p><p>The project is a part of the <a href=\"https://www.fs.usda.gov/detail/r1/landmanagement/?cid=FSP5_030798#:~:text=The%20Wildfire%20Crisis%20Strategy%20aims,Nez%20Perce%2DClearwater%2DLower%20Salmon\">Wildfire Crisis Strategy Landscape</a> and aims to reduce slash hazards associated with logging operations.&nbsp;</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "IDNCF Windy Shingle Timber Sale Project",
+                "field_unit_code": "IDNCF",
+                "id": "317173",
+                "lat_deg": "45",
+                "lat_min": "23",
+                "lat_sec": "27.55",
+                "long_deg": "116",
+                "long_min": "25",
+                "long_sec": "7.43",
+                "measurement_type": "Acres",
+                "size": "120",
+                "title": "Windy Shingle Timber Sale Project",
+                "type": "Prescribed Fire",
+                "urlPath": "/idncf-windy-shingle-timber-sale-project"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -115.532067,
+                    45.8256
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "10 hours 56 minutes ago",
+                "created": "<time datetime=\"2024-04-19T14:40:41-04:00\">2024-04-19</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><strong>With increased precipitation and decreased temperatures this week, the Dutch Oven Fuel Treatment paused prescribed burn operations.</strong></p><p>The primary purpose of this project is to reduce hazardous fuels within designated Rural Wildland Urban Interface lands adjacent to Elk City, ID. Activities are to reduce fuels created from logging operations and create planting sights for new trees post harvest. Like the Landscape burning it also helps reduce the potential for, and intensity of, subsequent wildfire and increase the chance for fire suppression strategies and tactics to be successful. There is a need to enhance wildfire suppression capability and provide for public and firefighter safety by reducing the amount of available fuel and implementing strategic treatments to provide safety zones and escape routes.&nbsp;</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "IDNCF Dutch Oven Fuel Treatment",
+                "field_unit_code": "IDNCF",
+                "id": "317174",
+                "lat_deg": "45",
+                "lat_min": "49",
+                "lat_sec": "32.16",
+                "long_deg": "115",
+                "long_min": "31",
+                "long_sec": "55.44",
+                "measurement_type": "Acres",
+                "size": "236",
+                "title": "Dutch Oven Fuel Treatment",
+                "type": "Prescribed Fire",
+                "urlPath": "/idncf-dutch-oven-fuel-treatment"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -116.601722,
+                    46.982019
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 week ago",
+                "created": "<time datetime=\"2024-04-19T16:22:34-04:00\">2024-04-19</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span>Units burned at the end of last weekend will be patrolled this week.</span></p><p><span>This project is located one and a half miles west of Horse Camp Trailhead and about one and a half miles east of Highway 6.</span></p><p>The objective of burning this slash is to remove fuel accumulations and create areas for planting new trees.&nbsp;</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "IDNCF Greenhorn Stewardship Project",
+                "field_unit_code": "IDNCF",
+                "id": "317175",
+                "lat_deg": "46",
+                "lat_min": "58",
+                "lat_sec": "55.27",
+                "long_deg": "116",
+                "long_min": "36",
+                "long_sec": "6.20",
+                "measurement_type": "Acres",
+                "size": "188",
+                "title": "Greenhorn Stewardship Project",
+                "type": "Prescribed Fire",
+                "urlPath": "/idncf-greenhorn-stewardship-project"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -115.729,
+                    46.095
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "10 hours 39 minutes ago",
+                "created": "<time datetime=\"2024-04-19T16:56:50-04:00\">2024-04-19</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><strong>Prescribed burning operations have paused, due to increased precipitation and decrease in temperatures. Available resources continue to monitor previously burned units and begin preparing other units for the next prescribed burn window.</strong></p><p>The Tinker Bugs Timber Sale Project encompasses a total of 7,636 acres in the Big Smith Creek, Middle Fork Clearwater River sub-watersheds that drain into the Middle Fork Clearwater River.</p><p>The overall purpose of the &nbsp;project is to restore vegetation species composition, structure, and distributions to early seral species (Ponderosa pine, western larch, and white pine); reduce ladder fuels created by shade-tolerant species and create more natural patch sizes by emulating mix-severity fire; improve big game habitat for winter range; and utilize timber outputs produced through forest management activities to support the economic structure of local communities, and provide for regional needs.<br>Burning should cover the majority of the unit to provide adequate spacing for seedling establishment.</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "IDNCF Tinker Bugs Timber Sale Project",
+                "field_unit_code": "IDNCF",
+                "id": "317176",
+                "lat_deg": "46",
+                "lat_min": "5",
+                "lat_sec": "42",
+                "long_deg": "115",
+                "long_min": "43",
+                "long_sec": "44.4",
+                "measurement_type": "Acres",
+                "size": "189",
+                "title": "Tinker Bugs Timber Sale Project",
+                "type": "Prescribed Fire",
+                "urlPath": "/idncf-tinker-bugs-timber-sale-project"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -122.681944,
+                    41.729167
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "4 weeks ago",
+                "created": "<time datetime=\"2024-04-19T18:37:55-04:00\">2024-04-19</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p>April 16, 2024\u2014 Klamath National Forest fire managers are shifting gears from pile burning operations to preparing for prescribed underburning this spring.</p><p>Fire managers use prescribed underburning to decrease fuel loadings and mimic the effects of the natural fire regime that local ecosystems evolved with. Historically, fire was ignited by lightning and by Indigenous people tending the land. Fire in its natural role reduces dead vegetation, replenishes nutrients in the soil, stimulates new growth, and maintains biological diversity.</p><p>Fire was effectively removed from these systems with the arrival of settlers. After many years of fire exclusion, an ecosystem that needs periodic fire becomes unhealthy. Trees become stressed by overcrowding, fire-dependent species disappear, and an unnatural buildup of flammable fuels that can become hazardous when wildfires occur. Over a century of fire suppression has resulted in wildfires burning more severely than they historically did, threatening communities and ecosystems.</p><p>\u201cPrescribed fire is an excellent opportunity to reintroduce a natural process and critical element back into the ecosystem on our terms and in strategic locations,\u201d said Kelsey Lofdahl, Assistant Forest Fire Management Officer on the Klamath National Forest. \u201cIt is one of the most useful tools to help reduce fuels, restore our forests, and protect our communities and natural resources.\u201d</p><p>Recent research conducted by the Pacific Southwest Research Station on the Klamath National Forest has illustrated the effectiveness of prescribed burning at reducing the severity of wildfires within treated areas. The study, released in February of this year, found that where the 2021 Antelope Fire intersected with previously completed fuels treatments, including prescribed burning, the severity of the burned area decreased compared to untreated areas.</p><p>Several prescribed burns are planned across the Klamath National Forest this spring. Timing of implementation will be dependent on fuel and weather conditions at each specific project location.</p><p>Happy Camp/Oak Knoll Ranger District<br>\u2022The Cade Mountain prescribed burn (111 acres) is 3 miles northeast of Happy Camp in mixed conifer and hardwood forest. The project aims to reduce fuels in the area and enhance the growth of Hazel for Tribal use.</p><p>Salmon/Scott River Ranger District<br>\u2022Crews plan to pick up where they left off last fall continuing ignitions out at the Scott Bar Mountain prescribed burn (500 acres) about 12 miles west of Fort Jones. The burn goals are to improve defensibility of homes in the area, increase resiliency of the forested stand against future wildfire events, and improve wildlife habitat. Scott Bar Mountain connects to a series of ridgetop fuels treatments, many of which were planned and implemented through collaborative efforts with partners. These treatments create a landscape-scale fuel break that can be used during wildfire events to protect communities, infrastructure, and natural resources.<br>\u2022Just east of the Scott Bar Mountain project area lies the Singleton Project (500 acres), which is in mixed conifer stands and will tie in to the same strategic ridgetop fuel break.</p><p>Goosenest Ranger District<br>\u2022The Van Bremmer (160 acres) and Tamarack (369 acres) underburns are two adjacent projects located three miles northeast of Tennant. The projects\u2019 goals are to reduce hazardous fuels, promote browse for big game, and increase stand resilience against the effects of insects, disease, and wildfire. Both projects are in ponderosa pine stands with an understory of brush and white fir saplings.&nbsp;<br>\u2022The First Creek prescribed burn (up to 1,174 acres) project is north of the Grass Lake Rest Area in mixed conifer with an understory of bitterbrush, manzanita, and snowbrush. Prescribed fire is being used to reduce surface fuel loads and reducing fire-intolerant white fir to create openings that favor fire-tolerant ponderosa pine regeneration.<br>\u2022The Cedar Mountain prescribed burn (up to 3,650 acres) is just north of Antelope Sink, in ponderosa pine stands with areas of juniper and brush. Prescribed fire will be used to reduce fuels to improve defensible space for the community of Tennant and outlying residences. Other goals for the burn are to improve big game habitat, reduce juniper, encourage aspen regeneration, and promote forested stands that are resilient against drought, wildfire, and forest pests.</p><p>Prescribed burning activities on the Klamath National Forest are in conjunction with the efforts of Klamath River Basin Landscape, which is part of the USDA Forest Service\u2019s Wildfire Crisis Strategy. The strategy, with funding from the Bipartisan Infrastructure Law and the Inflation Reduction Act, aims to reduce risk to communities, critical infrastructure, and natural resources from the ongoing wildfire crisis.</p><p>For more information on Klamath National Forest\u2019s spring prescribed burning projects, contact Jennifer Erickson, Forest Fire Prevention Officer at 530-841-4469.</p><p>Monitor the Klamath National Forest\u2019s Facebook site for more timely information about these projects as they are implemented.&nbsp;<br>&nbsp;</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "CAKNF 2024 Klamath NF Spring Prescribed Burning",
+                "field_unit_code": "CAKNF",
+                "id": "317181",
+                "lat_deg": "41",
+                "lat_min": "43",
+                "lat_sec": "45",
+                "long_deg": "122",
+                "long_min": "40",
+                "long_sec": "55",
+                "measurement_type": "Acres",
+                "size": "",
+                "title": "2024 Klamath NF Spring Prescribed Burning",
+                "type": "Prescribed Fire",
+                "urlPath": "/caknf-2024-klamath-nf-spring-prescribed-burning"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -112.096017,
+                    35.92812
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "3 days 14 hours ago",
+                "created": "<time datetime=\"2024-04-29T11:22:59-04:00\">2024-04-29</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span>Fire managers on the Tusayan Ranger District of the Kaibab National Forest are planning to conduct prescribed fires throughout the spring of 2024 as conditions allow.&nbsp;</span></p><p><span>Exact ignition dates are unknown as burning is dependent upon daily agency administrator approval and conditions within the ranges outlined in each prescribed fire plan. However, we are committed to providing the public with ongoing updates and as much advance notice as possible. </span><a href=\"https://www.fs.usda.gov/detail/kaibab/about-forest/contactus/?cid=fseprd1042331\"><span>Sign up to receive Kaibab NF news releases in your email</span></a><span>.</span></p><p><span>Our land management strategy is centered on long-term forest health, including reducing forest fuels and using prescribed fire on the landscape. Prescribed fires help reduce hazardous fuels that have accumulated due to drought, climate change, insects and disease, and decades of fire suppression. Fire also recycles nutrients back to the soil, promotes the growth of trees, wildflowers, and other plants, and improves habitat for threatened and endangered species. These efforts align with the </span><a href=\"https://www.fs.usda.gov/managing-land/wildfire-crisis\"><span>Forest Service\u2019s 10-year Wildfire Crisis Strategy</span></a><span> which aims to increase prescribed fire and other treatments to improve forest resiliency for generations to come.</span></p><p><span>We recognize that smoke can impact residents, visitors, and our fire personnel. We will continue to coordinate closely with our partners and communities to minimize smoke impacts as much as possible. All prescribed fires on the Kaibab National Forest are subject to Arizona Department of Environmental Quality. The department\u2019s </span><a href=\"https://legacy.azdeq.gov/environ/air/smoke/index.html\"><span>Air Quality Division: Smoke Management webpage</span></a><span> provides details about its air quality program.</span></p><p>&nbsp;</p><h3><strong>Tusayan Ranger District</strong></h3><ul><li><span><strong>Blue Stem Project</strong></span><ul><li><span>Location:&nbsp;Located on the eastern side of the Tusayan Ranger District, 16 miles east-southeast of the Town of Tusayan at Russell Tank;</span></li><li><span>Acres: up to&nbsp;2,724 acres</span></li><li><span>Notes:&nbsp;Minimal smoke impacts are expected, temporary re-route of the Arizona Trail around the burn unit.</span></li></ul></li></ul>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "AZKNF Kaibab NF Spring Prescribed Fires 2024 Tusayan Ranger District",
+                "field_unit_code": "AZKNF",
+                "id": "317203",
+                "lat_deg": "35",
+                "lat_min": "55",
+                "lat_sec": "41.232",
+                "long_deg": "112",
+                "long_min": "5",
+                "long_sec": "45.6612",
+                "measurement_type": "Acres",
+                "size": "",
+                "title": "Kaibab NF Spring Prescribed Fires 2024 - Tusayan Ranger District",
+                "type": "Prescribed Fire",
+                "urlPath": "/azknf-kaibab-nf-spring-prescribed-fires-2024-tusayan-ranger-district"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -112.221667,
+                    36.565556
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "3 days 14 hours ago",
+                "created": "<time datetime=\"2024-04-29T11:34:46-04:00\">2024-04-29</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span>Fire managers on the North Kaibab Ranger District of the Kaibab National Forest are planning to conduct prescribed fires throughout the spring of 2024 as conditions allow. The National Park Service will also be conducting the 50-acre Bright Angel Project on the North Rim near the developed area.</span></p><p><span>Exact ignition dates are unknown as burning is dependent upon daily agency administrator approval and conditions within the ranges outlined in each prescribed fire plan. However, we are committed to providing the public with ongoing updates and as much advance notice as possible. </span><a href=\"https://www.fs.usda.gov/detail/kaibab/about-forest/contactus/?cid=fseprd1042331\"><span><strong>Sign up to receive Kaibab NF news releases in your email</strong></span></a><span>.</span></p><p><span>Our land management strategy is centered on long-term forest health, including reducing forest fuels and using prescribed fire on the landscape. Prescribed fires help reduce hazardous fuels that have accumulated due to drought, climate change, insects and disease, and decades of fire suppression. Fire also recycles nutrients back to the soil, promotes the growth of trees, wildflowers, and other plants, and improves habitat for threatened and endangered species. These efforts align with the </span><a href=\"https://www.fs.usda.gov/managing-land/wildfire-crisis\"><span><strong>Forest Service\u2019s 10-year Wildfire Crisis Strategy</strong></span></a><span> which aims to increase prescribed fire and other treatments to improve forest resiliency for generations to come.</span></p><p><span>We recognize that smoke can impact residents, visitors, and our fire personnel. We will continue to coordinate closely with our partners and communities to minimize smoke impacts as much as possible. All prescribed fires on the Kaibab National Forest are subject to Arizona Department of Environmental Quality. The department\u2019s </span><a href=\"https://legacy.azdeq.gov/environ/air/smoke/index.html\"><span><strong>Air Quality Division: Smoke Management webpage</strong></span></a><span> provides details about its air quality program.</span></p><h3><strong>North Kaibab Ranger District</strong></h3><ul><li><span><strong>Billy Sink Phase 2 Project</strong></span><ul><li><span>Location: located .25 miles south of Jacob Lake along and east of State Route 67.</span></li><li><span>Acres: Up to 260</span></li><li><span>Notes: Smoke may impact Jacob Lake, State Route 67, and US 89A.</span></li></ul></li></ul><p>&nbsp;</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "AZKNF Kaibab NF Spring Prescribed Fires 2024 North Kaibab Ranger District",
+                "field_unit_code": "AZKNF",
+                "id": "317204",
+                "lat_deg": "36",
+                "lat_min": "33",
+                "lat_sec": "56",
+                "long_deg": "112",
+                "long_min": "13",
+                "long_sec": "18",
+                "measurement_type": "Acres",
+                "size": "",
+                "title": "Kaibab NF Spring Prescribed Fires 2024 - North Kaibab Ranger District",
+                "type": "Prescribed Fire",
+                "urlPath": "/azknf-kaibab-nf-spring-prescribed-fires-2024-north-kaibab-ranger-district"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -112.075833,
+                    35.306389
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "3 days 14 hours ago",
+                "created": "<time datetime=\"2024-04-29T11:39:57-04:00\">2024-04-29</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span>Fire managers on the Williams Ranger District of the Kaibab National Forest are planning to conduct prescribed fires throughout the spring of 2024 as conditions allow.&nbsp;</span></p><p><span>Exact ignition dates are unknown as burning is dependent upon daily agency administrator approval and conditions within the ranges outlined in each prescribed fire plan. However, we are committed to providing the public with ongoing updates and as much advance notice as possible. </span><a href=\"https://www.fs.usda.gov/detail/kaibab/about-forest/contactus/?cid=fseprd1042331\"><span><strong>Sign up to receive Kaibab NF news releases in your email</strong></span></a><span>.</span></p><p><span>Our land management strategy is centered on long-term forest health, including reducing forest fuels and using prescribed fire on the landscape. Prescribed fires help reduce hazardous fuels that have accumulated due to drought, climate change, insects and disease, and decades of fire suppression. Fire also recycles nutrients back to the soil, promotes the growth of trees, wildflowers, and other plants, and improves habitat for threatened and endangered species. These efforts align with the </span><a href=\"https://www.fs.usda.gov/managing-land/wildfire-crisis\"><span><strong>Forest Service\u2019s 10-year Wildfire Crisis Strategy</strong></span></a><span> which aims to increase prescribed fire and other treatments to improve forest resiliency for generations to come.</span></p><p><span>We recognize that smoke can impact residents, visitors, and our fire personnel. We will continue to coordinate closely with our partners and communities to minimize smoke impacts as much as possible. All prescribed fires on the Kaibab National Forest are subject to Arizona Department of Environmental Quality. The department\u2019s </span><a href=\"https://legacy.azdeq.gov/environ/air/smoke/index.html\"><span><strong>Air Quality Division: Smoke Management webpage</strong></span></a><span> provides details about its air quality program.</span></p><p>&nbsp;</p><h3><strong>Williams Ranger District</strong></h3><ul><li><strong>Three Sisters Project</strong><ul><li>Location: along the north shore of Kaibab Lake, 1.5 miles northeast of the City of Williams;</li><li>Acres: up to 2,245</li><li>Notes: Smoke impacts expected around Kaibab Lake area.</li></ul></li><li><span><strong>Marteen East Project</strong></span><ul><li><span>Location: west of Pumpkin Center Road, 12 miles north of the community of Parks.</span></li><li><span>Acres: up to 5,613</span></li><li><span>Notes: Smoke possible in the areas of Spring Valley Cabin and Forest Road 141, ignitions may occur on this unit should conditions not be appropriate to safely conduce the Three Sisters Project.</span></li></ul></li></ul>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "AZKNF Kaibab NF Spring Prescribed Fires 2024 Williams Ranger District",
+                "field_unit_code": "AZKNF",
+                "id": "317205",
+                "lat_deg": "35",
+                "lat_min": "18",
+                "lat_sec": "23",
+                "long_deg": "112",
+                "long_min": "04",
+                "long_sec": "33",
+                "measurement_type": "Acres",
+                "size": "",
+                "title": "Kaibab NF Spring Prescribed Fires 2024 - Williams Ranger District",
+                "type": "Prescribed Fire",
+                "urlPath": "/azknf-kaibab-nf-spring-prescribed-fires-2024-williams-ranger-district"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -111.35223,
+                    34.578963
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "5 hours 57 minutes ago",
+                "created": "<time datetime=\"2024-04-30T11:46:09-04:00\">2024-04-30</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span>The Wolf Fire, reported the morning of April 29, is&nbsp;</span><a href=\"https://maps.app.goo.gl/WYTuBUA5KSTAZ8949\"><span>located about 3 miles northwest of Clints Well</span></a><span>.</span></p><p><span>Fire managers treated roughly 10,000 acres of land on the Wolf Fire.</span></p>",
+                "field_percent_of_perimeter": "100",
+                "field_title_and_unit": "AZCOF Wolf Fire",
+                "field_unit_code": "AZCOF",
+                "id": "317208",
+                "lat_deg": "34",
+                "lat_min": "34",
+                "lat_sec": "44.2668",
+                "long_deg": "111",
+                "long_min": "21",
+                "long_sec": "8.028",
+                "measurement_type": "Acres",
+                "size": "9896",
+                "title": "Wolf Fire",
+                "type": "Wildfire",
+                "urlPath": "/azcof-wolf-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -106.414444,
+                    36.488611
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 day 14 hours ago",
+                "created": "<time datetime=\"2024-05-02T14:22:07-04:00\">2024-05-02</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><em>Crews finished ignitions on May 18, accomplishing 835 acres. They will continue to patrol and monitor the fire until it is called out. Read the </em><a href=\"https://inciweb.wildfire.gov/incident-news/nmcaf-montoya-prescribed-fire\"><em>latest news release</em></a><em> for a full summary.&nbsp;</em></p><p><span>The 899-acre Montoya Prescribed Fire is part of the Canjilon Wildland Urban Interface Project, a collaborative project over 10 years in the making to reduce the risk of wildfire to the communities of Canjilon and Placita Garcia and the watersheds they depend on. The unit is directly adjacent to Canjilon\u2019s east side.</span></p><p><span>To reduce the risk, Forest Service staff and partners have invested over $10 million in forest restoration in the area since 2011. Many adjacent private landowners, with the assistance of the state, are contributing by thinning and applying prescribed fire on their own properties.</span></p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "NMCAF Montoya Prescribed Fire",
+                "field_unit_code": "NMCAF",
+                "id": "317212",
+                "lat_deg": "36",
+                "lat_min": "29",
+                "lat_sec": "19",
+                "long_deg": "106",
+                "long_min": "24",
+                "long_sec": "52",
+                "measurement_type": "Acres",
+                "size": "835",
+                "title": "Montoya Prescribed Fire",
+                "type": "Prescribed Fire",
+                "urlPath": "/nmcaf-montoya-prescribed-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -121.442222,
+                    43.023333
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 week ago",
+                "created": "<time datetime=\"2024-05-04T20:52:42-04:00\">2024-05-04</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p>This lightning-caused wildfire is being utilized to return natural fire to the landscape in an effort to restore forest health and reduce fuels. Our group of experienced, professional wildland firefighters will conduct a series of firing operations to safely and methodically burn the fuels between the main fire and our established containment lines, reintroducing low-intensity fire to the landscape. Some of the benefits include;</p><ul><li>Enhancing meadows by reducing the encroachment of pines into these areas&nbsp;and increasing wildlife forage.</li><li>Minimizing the spread of disease and insects in the forest</li><li>Removing unwanted non-native, invasive plant species</li><li>Recycling nutrients to promote healthy soils</li><li>Reducing fuel loading by consuming dead and downed woody material, including logs, brush, needle cast, and stumps</li><li>Reducing ladder fuels and stand density by eliminating smaller-diameter trees</li></ul><p>&nbsp;</p><p>The plan for the Little Yamsay Fire is to systematically and safely burn approximately 6,000 acres in a <a href=\"https://youtu.be/8R7vW0LoViw?si=cZm7w-r1zejg-0sQ\">three-phase sequence</a>. An additional phase four block is also being prepared for a firing operation if conditions allow. Our effort will add to the&nbsp;existing footprint&nbsp;of the&nbsp;3,200 acre&nbsp;Dillon Creek Fire, which will result in nearly a 10,000-acre treated buffer to protect values at risk from future wildfires.</p><p>&nbsp;</p><p>A Type 3 Incident Management Team (IMT) assumed command of the Little Yamsay Fire Tuesday, April 30 at 0600 to allow the <a href=\"https://www.fs.usda.gov/fremont-winema/\">Fremont-Winema National Forest</a> to focus on conducting prescribed fire.</p><p>Fire managers have developed a plan consisting of three phases of firing operations to achieve objectives:&nbsp;</p><ul><li><a href=\"https://ftp.wildfire.gov/public/incident_specific_data/pacific_nw/2024_Incidents_Oregon/2024_Little_Yamsay_ORFWF240107/GIS/20240429/ops_phase1_arch_e_port_20240429_1245_Little%20Yamsay_ORFWF240107.pdf\">Phase One</a> will increase the fire footprint by 1,208 acres. Phase One was completed May 3.</li><li><a href=\"https://ftp.wildfire.gov/public/incident_specific_data/pacific_nw/2024_Incidents_Oregon/2024_Little_Yamsay_ORFWF240107/GIS/20240429/ops_phase2_arch_e_port_20240429_1245_Little%20Yamsay_ORFWF240107.pdf\">Phase Two</a> will add another 1,055 acres. Phase Two was completed May 9.</li><li><a href=\"https://ftp.wildfire.gov/public/incident_specific_data/pacific_nw/2024_Incidents_Oregon/2024_Little_Yamsay_ORFWF240107/GIS/20240429/ops_phase3_arch_e_port_20240429_1245_Little%20Yamsay_ORFWF240107.pdf\">Phase Three</a> will include additional 3,712 acres. Phase Three was completed May 12 with additional acreage from the Yota precribed fire unit.</li></ul><p>The <a href=\"https://ftp.wildfire.gov/public/incident_specific_data/pacific_nw/2024_Incidents_Oregon/2024_Little_Yamsay_ORFWF240107/GIS/20240429/ops_arch_e_port_20240429_1239_Little%20Yamsay_ORFWF240107.pdf\">three-phase</a> firing operation is complete. The final size Little Yamsay Fire is 6,340 acres. Here's the <a href=\"https://ftp.wildfire.gov/public/incident_specific_data/pacific_nw/2024_Incidents_Oregon/2024_Little_Yamsay_ORFWF240107/GIS/20240513/prog_arch_e_port_20240512_1758_Little_Yamsay_ORFWF240107_0513.pdf\">progression map</a> with acres burned with corresponding dates. As of May 13, 2024 fire managers are evaluating conditions to bring fire into phase 4, which would increase the total acreage by 815 acres.&nbsp;</p><p>&nbsp;</p><p>Fire reintroduced into the landscape creates&nbsp;significant buffers which will&nbsp;break up the landscape into 10,000 to 20,000 acre treated parcels that will&nbsp;protect&nbsp;against catastrophic wildfires like the <a href=\"https://en.wikipedia.org/wiki/Bootleg_Fire\">Bootleg Fire</a>. A successful wildfire buffer was observed in the Blackhills Project Area that the Bootleg Fire burned through.</p><p>&nbsp;</p><p>Natural ignitions&nbsp;are an excellent opportunity&nbsp;to get fire back on the landscape&nbsp;and encouraged in the <a href=\"https://www.fs.usda.gov/sites/default/files/fs_media/fs_document/Confronting-the-Wildfire-Crisis.pdf\">Wildfire Crisis Strategy</a>. Without reintroducing fire onto the landscape at the proper scale, more catastrophic fires that burn up entire ranger districts and towns will continue to happen.</p><p>&nbsp;</p><p>&nbsp;</p>",
+                "field_percent_of_perimeter": "53",
+                "field_title_and_unit": "ORFWF Little Yamsay Fire",
+                "field_unit_code": "ORFWF",
+                "id": "317214",
+                "lat_deg": "43",
+                "lat_min": "1",
+                "lat_sec": "24",
+                "long_deg": "121",
+                "long_min": "26",
+                "long_sec": "32",
+                "measurement_type": "Acres",
+                "size": "6340",
+                "title": "Little Yamsay Fire",
+                "type": "Wildfire",
+                "urlPath": "/orfwf-little-yamsay-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -106.045556,
+                    36.682222
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 week 6 days ago",
+                "created": "<time datetime=\"2024-05-07T11:42:24-04:00\">2024-05-07</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><em>Tentative dates for ignitions have not been determined.</em></p><p>The 2,962-acre Esquibel Prescribed Fire is part of the Rio Tusas-Lower San Antonio Landscape Project, which aims to restore the forest health throughout nearly half of the Tres Piedras Ranger District.</p><p>Over the last century, forested areas departed from conditions suitable for healthy and vibrant ecosystem. This is especially true in frequent fire forest types, such as ponderosa and mixed conifer, where stands are unnaturally dense and lacking recent fire history.</p><p>This work is part of the larger <a href=\"https://www.fs.usda.gov/features/common-ground-rio-chama\">Rio Chama Collaborative Forest Landscape Restoration Project</a>, which spans 3.8-million acres between Northern New Mexico and Southern Colorado.&nbsp;</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "NMCAF Esquibel Prescribed Fire",
+                "field_unit_code": "NMCAF",
+                "id": "317223",
+                "lat_deg": "36",
+                "lat_min": "40",
+                "lat_sec": "56",
+                "long_deg": "106",
+                "long_min": "02",
+                "long_sec": "44",
+                "measurement_type": "Acres",
+                "size": "",
+                "title": "Esquibel Prescribed Fire",
+                "type": "Prescribed Fire",
+                "urlPath": "/nmcaf-esquibel-prescribed-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -106.086944,
+                    36.616111
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 week 6 days ago",
+                "created": "<time datetime=\"2024-05-07T11:46:48-04:00\">2024-05-07</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><em>Tentative dates for ignitions have not been determined.</em></p><p>The 1,009-acre American Creek Prescribed Fire is part of the Rio Tusas-Lower San Antonio Landscape Project, which aims to restore the forest health throughout nearly half of the Tres Piedras Ranger District.</p><p>Over the last century, forested areas departed from conditions suitable for healthy and vibrant ecosystem. This is especially true in frequent fire forest types, such as ponderosa and mixed conifer, where stands are unnaturally dense and lacking recent fire history.</p><p>This work is part of the larger <a href=\"https://www.fs.usda.gov/features/common-ground-rio-chama\"><strong>Rio Chama Collaborative Forest Landscape Restoration Project</strong></a>, which spans 3.8-million acres between Northern New Mexico and Southern Colorado.&nbsp;</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "NMCAF American Creek Prescribed Fire",
+                "field_unit_code": "NMCAF",
+                "id": "317225",
+                "lat_deg": "36",
+                "lat_min": "36",
+                "lat_sec": "58",
+                "long_deg": "106",
+                "long_min": "05",
+                "long_sec": "13",
+                "measurement_type": "Acres",
+                "size": "",
+                "title": "American Creek Prescribed Fire",
+                "type": "Prescribed Fire",
+                "urlPath": "/nmcaf-american-creek-prescribed-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -111.691667,
+                    33.95
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 week ago",
+                "created": "<time datetime=\"2024-05-07T18:17:53-04:00\">2024-05-07</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p>Fire crews are responded to the <a href=\"https://www.facebook.com/hashtag/horsefire?__eep__=6&amp;__cft__%5B0%5D=AZXDEaSoeR-3MgQnzCG6gQTcgLCLh2r0itBV6IJbnUZuDaU6Bd4F0cGFfa597DokZh5xe-NvqwUbFc6wkjNHP-3b8C1BpRbj32TLnGOSdPyCo47XShXaK7-cBTSQgytjcJTo2VMKTDbrG0tOA48ll4Ipdj3Z7mT9IFiqvAozFO3aeGCtVYq7WC8ZeRKeLbXFZDVzYFI92SAf01zFjfDrVGuU&amp;__tn__=*NK-R\">#HorseFire</a> on the Cave Creek Ranger District at MM 8 off Horseshoe Lake Road on Sunday around 1600. Crews will be working overnight conducting fire suppression operations. Four engines, one helicopter including Mesa and Payson Interagency Hotshot Crews are actively working the fire to protect the KA Ranch, Horse Dam infrastructure and Forest Service campgrounds. Earlier the <a href=\"https://www.facebook.com/MCSOaz?__cft__%5B0%5D=AZXDEaSoeR-3MgQnzCG6gQTcgLCLh2r0itBV6IJbnUZuDaU6Bd4F0cGFfa597DokZh5xe-NvqwUbFc6wkjNHP-3b8C1BpRbj32TLnGOSdPyCo47XShXaK7-cBTSQgytjcJTo2VMKTDbrG0tOA48ll4Ipdj3Z7mT9IFiqvAozFO3aeGCtVYq7WC8ZeRKeLbXFZDVzYFI92SAf01zFjfDrVGuU&amp;__tn__=-%5DK-R\">Maricopa County Sheriff's Office</a> assisted with providing food, water and supplies to the KA Ranch.</p><p>A closure will be in effect for the entire portion of NFSR 205, also known as Horseshoe Dam Road, starting from NFSR 19, also known as Bartlett Dam Road beginning 9 p.m. Sunday, May 5, through June 5, 2024, until 6 p.m., unless rescinded. For the safety of firefighters and the public, please avoid the area during fire suppression operations.</p>",
+                "field_percent_of_perimeter": "50",
+                "field_title_and_unit": "AZTNF Horse Fire Aztnf",
+                "field_unit_code": "AZTNF",
+                "id": "317231",
+                "lat_deg": "33",
+                "lat_min": "57",
+                "lat_sec": "0",
+                "long_deg": "111",
+                "long_min": "41.5",
+                "long_sec": "0",
+                "measurement_type": "Acres",
+                "size": "512",
+                "title": "Horse Fire Aztnf",
+                "type": "Wildfire",
+                "urlPath": "/aztnf-horse-fire-aztnf"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -113.653333,
+                    36.974722
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 week 4 days ago",
+                "created": "<time datetime=\"2024-05-09T14:52:40-04:00\">2024-05-09</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p>Forward progression has stopped. Crews are working toward containment. Fire cause is under investigation.</p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "AZASD Black Fire",
+                "field_unit_code": "AZASD",
+                "id": "317245",
+                "lat_deg": "36",
+                "lat_min": "58",
+                "lat_sec": "29",
+                "long_deg": "113",
+                "long_min": "39",
+                "long_sec": "12",
+                "measurement_type": "Acres",
+                "size": "77",
+                "title": "Black Fire",
+                "type": "Wildfire",
+                "urlPath": "/azasd-black-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -120.084444,
+                    39.402778
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "3 days 12 hours ago",
+                "created": "<time datetime=\"2024-05-09T20:15:42-04:00\">2024-05-09</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<ul type=\"disc\"><li><span><strong>Name of project</strong>:&nbsp;East Zone Roadside Underburn</span></li><li><span><strong>Type of burn:</strong> Underburn</span></li><li><span><strong>Project potential acreage:</strong> 115</span></li><li><span><strong>Ignition dates:</strong>&nbsp; Beginning as early as May 10 for up to 7 days, conditions permitting</span></li></ul><p><span>Tahoe National Forest will begin a prescribed underburn along Forest Service roads near Boca and Stampede Reservoirs in the Truckee, Calif. area. Fire and fuels personnel plan to prescribed burn up to 115 acres starting as early as Friday, May 10 and continuing for approximately 7 days, conditions permitting.</span></p><p><span>This prescribed burn is a continuation of critical roadside fuels reduction work that began in 2023 along Tahoe National Forest roads to establish fuel breaks in the event of a wildfire. Fuel breaks can provide improved opportunities for fire suppression. Along roads, they also help establish safe ingress and egress routes for the public and firefighting resources should a wildfire impact the area.</span></p><p><br><strong>Why Are We Burning?</strong></p><p><span>The goal of this prescribed burn is to decrease the existing fire hazard and to prevent and reduce the impact of future fires in the area. Other benefits include enhancing wildlife habitat and reintroducing fire into a fire-adapted ecosystem.</span></p><p><strong>Why Now?</strong></p><p><span>Current conditions allow for prescribed burning. Each prescribed fire operation follows a prescribed fire burn plan, which considers temperature, humidity, wind, moisture of the vegetation, and conditions for the dispersal of smoke. This information is used to decide when and where to burn. The Tahoe National Forest strives to give as much advance notice as possible before burning, but some operations may be conducted on short notice.</span></p><p><strong>Smoke</strong></p><p><span>Smoke from prescribed fire operations is normal and may continue for several days after an ignition depending on the project size and environmental conditions. Smoke may settle into the valleys in the evening and lift in the morning. The Tahoe National Forest coordinates with state and local county air pollution control districts and monitors weather conditions closely prior to prescribed fire ignition. Crews also conduct test burns before igniting a larger area, to verify how effectively fuels are consumed and how smoke will travel.</span></p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "CATNF East Zone Roadside Underburn",
+                "field_unit_code": "CATNF",
+                "id": "317246",
+                "lat_deg": "39",
+                "lat_min": "24",
+                "lat_sec": "10",
+                "long_deg": "120",
+                "long_min": "05",
+                "long_sec": "04",
+                "measurement_type": "Acres",
+                "size": "115",
+                "title": "East Zone Roadside Underburn",
+                "type": "Prescribed Fire",
+                "urlPath": "/catnf-east-zone-roadside-underburn"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -110.456111,
+                    33.293611
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "4 days 10 hours ago",
+                "created": "<time datetime=\"2024-05-13T20:20:03-04:00\">2024-05-13</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span>After an intense and concentrated effort over the last week, the Toyo fire activity has reached the point that it\u2019s time to transition the management of the fire back to the local unit. The majority of resources will be returning to their home units today.&nbsp;</span></p><p><span>Southwest Team 1 has appreciated the support of the communities, the Tribal Council, and the San Carlos Agency. Wildfire suppression \u201ctakes a village\u201d, and this village has been great to be a part of our success.</span></p>",
+                "field_percent_of_perimeter": "90",
+                "field_title_and_unit": "AZSCA Toyo Fire",
+                "field_unit_code": "AZSCA",
+                "id": "317268",
+                "lat_deg": "33",
+                "lat_min": "17",
+                "lat_sec": "37",
+                "long_deg": "110",
+                "long_min": "27",
+                "long_sec": "22",
+                "measurement_type": "Acres",
+                "size": "1778",
+                "title": "Toyo Fire",
+                "type": "Wildfire",
+                "urlPath": "/azsca-toyo-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -91.433361,
+                    47.647028
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 day 10 hours ago",
+                "created": "<time datetime=\"2024-05-15T17:03:12-04:00\">2024-05-15</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span>Ignitions were started on a Fry Prescribed Fire unit at 10:50am on May 15, 2024, under conditions that were within the guidelines outlined in the approved Burn Plan. Shortly after 12noon a spot fire was detected within the overall prescribed fire project area, outside the planned burn unit and in an area of denser fuels. Immediate action was taken to suppress the spot fire using both assigned and contingency resources.&nbsp;</span></p><p><span>The spot fire was declared a wildfire at 1:00pm CT when it was determined that additional resources not already assigned to the prescribed fire would be needed. In addition, the Lake County Emergency Manager was notified of the situation. Water dropping aircraft were ordered to help suppress the fire and after several hours were effective in slowing the fire spread.&nbsp;</span></p><p>Containment is now at 100% on May 19, 2024. A reduction in acreage has been made due to more accurate mapping.</p><p>No additional updates are planned after May 19, 2024. The public is encouraged to please go to <a href=\"https://www.facebook.com/SuperiorNF\">https://www.facebook.com/SuperiorNF</a> for updates when needed about prescribed fires and wildfires.</p>",
+                "field_percent_of_perimeter": "100",
+                "field_title_and_unit": "MNSUF Fry Fire",
+                "field_unit_code": "MNSUF",
+                "id": "317279",
+                "lat_deg": "47",
+                "lat_min": "38",
+                "lat_sec": "49.3",
+                "long_deg": "91",
+                "long_min": "26",
+                "long_sec": ".1",
+                "measurement_type": "Acres",
+                "size": "186",
+                "title": "Fry Fire",
+                "type": "Wildfire",
+                "urlPath": "/mnsuf-fry-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -107.686333,
+                    35.256533
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 day 15 hours ago",
+                "created": "<time datetime=\"2024-05-16T14:41:30-04:00\">2024-05-16</time>\n",
+                "field_active": "1",
+                "field_incident_description": "East La Jara prescribed fire (RX) on the Mt Taylor Ranger District of the Cibola National Forest and National Grasslands<br />\r\nImplementation as early as Friday May 17, 2024. <br />\r\nFire crews plan to burn approximately 956 acres 7 miles NE of Grants NM. <br />\r\nSmoke may be visible from Grants, Acoma, Laguna, Cubero and Seboyeta.<br />\r\n",
+                "field_incident_overview": "<p>May 16, 2024</p><p><span>Pending favorable conditions, fire managers on the Cibola National Forest &amp; National Grasslands (NF &amp; NGs) may implement the previously announced East La Jara prescribed fire (RX) on the Mt Taylor Ranger District as early as Friday May 17, 2024.&nbsp;</span></p><p><span>Fire crews plan to burn approximately 956 acres 7 miles NE of Grants NM. <strong>See map attached.&nbsp;</strong></span></p><p><span>Smoke may be visible from Grants, Acoma, Laguna, Cubero and Seboyeta.</span></p><p><span lang=\"EN\">Ignition will depend upon agency administrator approval and conditions within the ranges outlined in the prescribed fire plan. Desired conditions will result in effective smoke ventilation and dispersal and help achieve the effects needed to accomplish the burn plan objectives.&nbsp;</span></p><p><span lang=\"EN\">The Cibola NF &amp; NGs manages all prescribed fires in compliance with New Mexico state air quality and smoke management regulations.&nbsp;</span><span>However, s</span><span lang=\"EN\">moke may settle into drainages and lower elevations at night but is expected to dissipate as daytime temperatures increase.&nbsp;</span><span>Information on air quality and protecting your health can be found online at the&nbsp;</span><a href=\"http://www.airnow.gov/\"><span lang=\"EN-US\">www.airnow.gov/</span></a><span lang=\"EN\"></span></p><p><span lang=\"EN\">Our land management strategy is centered on long-term forest health, including reducing forest fuels and using prescribed fire on the landscape. Prescribed fires are intended to reduce hazardous fuels accumulated due to drought, climate change, insects and disease, and decades of fire suppression. Additionally, fire managers use prescribed fire to improve forest health, remove hazardous fuels, increase firefighter safety, enhance wildlife habitat, and protect communities and watersheds. Prescribed burns are designed to meet specific objectives and are always managed with firefighter and public safety as the priority.</span></p>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "NMCIF Mt Taylor RD East La Jara Prescribed Fire",
+                "field_unit_code": "NMCIF",
+                "id": "317283",
+                "lat_deg": "35",
+                "lat_min": "15",
+                "lat_sec": "23.52",
+                "long_deg": "107",
+                "long_min": "41",
+                "long_sec": "10.8",
+                "measurement_type": "Acres",
+                "size": "956",
+                "title": "Mt Taylor RD: East La Jara Prescribed Fire",
+                "type": "Prescribed Fire",
+                "urlPath": "/nmcif-mt-taylor-rd-east-la-jara-prescribed-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -115.585167,
+                    45.849667
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "10 hours 59 minutes ago",
+                "created": "<time datetime=\"2024-05-16T14:47:55-04:00\">2024-05-16</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><strong>The Muddy Moose Prescribed Burn Project is complete for the spring. This will be the last update on Muddy Moose Project.</strong></p><p>The overall project area will contain approximately 243 acres of logging slash burning that will reduce hazardous fuel accumulations in areas of designated Rural Wildland Urban Interface near Elk City, ID. Further objectives for this project include:</p><ul><li>reducing fuels created from logging operations to create new planting sites for new trees post-harvest</li><li>reduce the potential risk and intensity of catastrophic wildfire</li><li>increase the success of wildfire suppression strategies and tactics, while providing for firefighter safety</li><li>improving potential safety zones and escape routes for firefighters to further protect firefighter health and well-being.</li></ul>",
+                "field_percent_of_perimeter": "",
+                "field_title_and_unit": "IDNCF Muddy Moose Project",
+                "field_unit_code": "IDNCF",
+                "id": "317284",
+                "lat_deg": "45",
+                "lat_min": "50",
+                "lat_sec": "58.8",
+                "long_deg": "115",
+                "long_min": "35",
+                "long_sec": "6.6",
+                "measurement_type": "Acres",
+                "size": "55",
+                "title": "Muddy Moose Project",
+                "type": "Prescribed Fire",
+                "urlPath": "/idncf-muddy-moose-project"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -108.302222,
+                    37.523333
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 hour 49 minutes ago",
+                "created": "<time datetime=\"2024-05-16T17:38:02-04:00\">2024-05-16</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p>The Spruce Creek Fire was started by lightning on May 14, 2024. It is burning on the Dolores Ranger District of the San Juan National Forest, 11 miles northeast of Dolores, Colorado. It is burning, at low-to-moderate intensity, inside a network of Forest System Roads. Two Interagency Hotshot Crews, two Wildland Fire Modules and several US Forest Service and BLM engines and crews are staffing the fire. Additional resources are arriving. A San Juan National Forest Incident Management Team will take command of the fire on May 21 in order to provide additional overhead and logistical support to the incident. The intent is to lower long-term risk on the landscape by bring low-to-moderate intensity fire, conditions permitting, across approximately 4500 acres of aspen/spruce/ponderosa pine/gambel oak forest.</p>",
+                "field_percent_of_perimeter": "0",
+                "field_title_and_unit": "COSJF 2024 Spruce Creek CO",
+                "field_unit_code": "COSJF",
+                "id": "317286",
+                "lat_deg": " 37",
+                "lat_min": "31",
+                "lat_sec": "24",
+                "long_deg": "108",
+                "long_min": "18",
+                "long_sec": "8",
+                "measurement_type": "Acres",
+                "size": "1644",
+                "title": "2024 Spruce Creek CO",
+                "type": "Wildfire",
+                "urlPath": "/cosjf-2024-spruce-creek-co"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -111.754444,
+                    33.849722
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "30 minutes 56 seconds ago",
+                "created": "<time datetime=\"2024-05-19T03:45:05-04:00\">2024-05-19</time>\n",
+                "field_active": "1",
+                "field_incident_description": " ",
+                "field_incident_overview": "<p>The <a href=\"https://www.facebook.com/hashtag/wildcatfire?__eep__=6&amp;__cft__[0]=AZUxq4MZbWTSNEatkmiGvRFoQUZ-sG9OBD0qtlJUIDZt3sG5GHWLyMx7eBuHFWiKkKGf7rbadNvZwh5s_qFbPomkAVn4UBiV_dU8GEbNOwF3saJU2h2DmuaXcWmbdCD8UL6ccZEW29neD_FDmYkXHkmgG6Ut_j8eHyihzNJhptcEiyzA28oFjHqFPoXKWB_FL8zxHallrAP3rX_GSpGmFcxo&amp;__tn__=*NK-R\"><span>Wildcat Fire</span></a> was reported at approximately 9:20 a.m. Saturday morning near Vista Verde north of Dynamite Blvd and 136th Street, west of Bartlett Lake on the Cave Creek Ranger District.&nbsp;</p><p>Maricopa County Sheriff\u2019s Office has closed Bartlett Dam Road as the fire is burning on both sides of the road and visitors are carefully being escorted from Bartlett Lake. For firefighter and public safety, please avoid the area while crews conduct fire suppression operations. The public is urged to sign up for the <a href=\"https://www.maricopa.gov/1755/CENS\">Maricopa County Emergency Notification System</a> to be quickly notified of possible emergency evacuations if necessary.</p><p>To learn more about the Arizona Emergency Information Network visit <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fein.az.gov%2Fready-set-go%3Ffbclid%3DIwZXh0bgNhZW0CMTAAAR2kv_ksA0jK4JeLXrl2XoIoDYlSN_J6bPLyBUF22l2IbbjS5GAFdPbMyaE_aem_AYHL5oBOZBVOtHd3rXv75JNmCbYeuOzSSJJtfbHTxfUEjWB1P7lJjLZKVY4ChLonUHxbo9AeHAT5hS3MaT8fHDF-%23County%2FTribal%2520Emergency%2520Notification%2520Systems&amp;h=AT0CqXF0eWqKTaqvzIzQW6zn8NeQBGfnuKkL-vyzfIaXbyeeQmB0cQZGqVDB4UQD2qebFSgC0mIXzR-i80EdSbr_lU6ziXr-v9NPhi3kDThKXai-0XFGJq4n6kvKocmq4zuD&amp;__tn__=-UK-R&amp;c[0]=AT1Pq68qxpladtg0huruy_wBRPB-kqTclxE53A7NbVNnOCzmvVOvS8rj_xfhgEHhWW9zvERKcJWx1M8tlNgdksdnYFVye55mGUIqEmsPcjmjdfZnn3afEk1HZ1PLa49Asvfu1X5nFQSJuMpDQDOO7_4VXu7ywqneBr4WaWN5EbzXh07nirS398M4HyoplwBp3_2weSi2qYbpC8qgEnBCug_YCDYuZL7BsSCYW818h5Ug9Cek\"><span>https://ein.az.gov/ready-set-go...</span></a>.</p><p>Remember, drones and firefighting aircraft are a dangerous mix and could lead to accidents or slow down wildfire suppression operations. If you fly, we can\u2019t.</p>",
+                "field_percent_of_perimeter": "23",
+                "field_title_and_unit": "AZTNF Wildcat Fire",
+                "field_unit_code": "AZTNF",
+                "id": "317296",
+                "lat_deg": "33",
+                "lat_min": "50",
+                "lat_sec": "59",
+                "long_deg": "111",
+                "long_min": "45",
+                "long_sec": "16",
+                "measurement_type": "Acres",
+                "size": "14283",
+                "title": "Wildcat Fire",
+                "type": "Wildfire",
+                "urlPath": "/aztnf-wildcat-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -105.794722,
+                    33.430556
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "2 hours 38 minutes ago",
+                "created": "<time datetime=\"2024-05-19T11:53:06-04:00\">2024-05-19</time>\n",
+                "field_active": "1",
+                "field_incident_description": "Lightning-caused fires in White Mountain Designated Wilderness Area.",
+                "field_incident_overview": "<p><span>On May 17, 2024, two lightning-caused fires were detected in the White Mountain Wilderness in the Smokey Bear Ranger District, Lincoln National Forest. Blue Fire and Blue Fire 2 are being closely monitored by the Smokey Bear Ranger District. &nbsp;</span></p><p class=\"text-align-justify\"><span>Currently, the overall strategy on the Blue Fires is to allow the low-to-moderate intensity of spread to play its natural role on the landscape. Recent precipitation, as well as the slow spread of the fires and rocky terrain, have all led to this determination. Crews will take appropriate actions to keep the fire within the designated planned boundaries while protecting private land, infrastructure, and natural resources.&nbsp; The fire is being monitored by air and ground resources, to help predict expected fire behavior and rates of spread.</span></p><p class=\"text-align-justify\"><span dir=\"ltr\">Crews are continuing to monitor the Blue Fires and scout area to assess safe locations for engagement if necessary. &nbsp;The fire is growing at a low-medium intensity, and putting off more smoke. &nbsp;It is currently estimated to be 45 acres in size.</span></p>",
+                "field_percent_of_perimeter": "0",
+                "field_title_and_unit": "NMLNF Blue 2 Fire",
+                "field_unit_code": "NMLNF",
+                "id": "317298",
+                "lat_deg": "33",
+                "lat_min": "25",
+                "lat_sec": "50",
+                "long_deg": "105",
+                "long_min": "47",
+                "long_sec": "41",
+                "measurement_type": "Acres",
+                "size": "45",
+                "title": "Blue 2 Fire",
+                "type": "Wildfire",
+                "urlPath": "/nmlnf-blue-2-fire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -106.702222,
+                    36.289167
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "2 hours 3 minutes ago",
+                "created": "<time datetime=\"2024-05-20T17:17:27-04:00\">2024-05-20</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p><span>The Indios Fire is a lightning caused wildfire located in the Coyote Ranger District, about 7 miles north of the village of Coyote, N.M within the Chama River Canyon Wilderness.</span></p><p><span>Firefighters were not able to safely engage the fire due to steep and inaccessible terrain. Firefighters have spent the last couple days scouting roads and gaining access to the fire area to locate potential control lines.</span></p><p><span>Fire managers are evaluating a variety of management strategies for the Indios Wildfire, which can range from full suppression to managing the fire to restore its natural role in the ecosystem while meeting resource objectives on the landscape.&nbsp;</span></p>",
+                "field_percent_of_perimeter": "0",
+                "field_title_and_unit": "NMSNF Indios Wildfire",
+                "field_unit_code": "NMSNF",
+                "id": "317309",
+                "lat_deg": "36",
+                "lat_min": "17",
+                "lat_sec": "21",
+                "long_deg": "106",
+                "long_min": "42",
+                "long_sec": "08",
+                "measurement_type": "Acres",
+                "size": "255",
+                "title": "Indios Wildfire",
+                "type": "Wildfire",
+                "urlPath": "/nmsnf-indios-wildfire"
+            },
+            "type": "Feature"
+        },
+        {
+            "geometry": {
+                "coordinates": [
+                    -105.69368,
+                    32.960819
+                ],
+                "type": "Point"
+            },
+            "properties": {
+                "changed": "1 second ago",
+                "created": "<time datetime=\"2024-05-20T19:20:50-04:00\">2024-05-20</time>\n",
+                "field_active": "1",
+                "field_incident_description": "",
+                "field_incident_overview": "<p>The Moser Fire started 4 miles east of Cloudcroft along Highway 82 past the Cloudcroft Ski area. The fire is moving in a North, North East direction.</p><p>The cause is unknown and under investigation. Please see the Announcements Tab for evacuations. Numerous firefighting and aviation assets have been mobilized to the fire. This is an evolving situation. Please check back for updates.&nbsp;</p>",
+                "field_percent_of_perimeter": "0",
+                "field_title_and_unit": "NMLNF Moser Fire 2024",
+                "field_unit_code": "NMLNF",
+                "id": "317312",
+                "lat_deg": "32",
+                "lat_min": "57",
+                "lat_sec": "38.9484",
+                "long_deg": "105",
+                "long_min": "41",
+                "long_sec": "37.248",
+                "measurement_type": "Acres",
+                "size": "145",
+                "title": "Moser Fire 2024",
+                "type": "Wildfire",
+                "urlPath": "/nmlnf-moser-fire-2024"
+            },
+            "type": "Feature"
         }
     ],
     "type": "FeatureCollection"
 }
```

### Comparing `inciweb-wildfires-1.0.0/docs/Makefile` & `inciweb-wildfires-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-1.0.0/docs/index.md` & `inciweb-wildfires-1.1.0/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-```{include} _templates/nav.html
-```
-
 # inciweb-wildfires
 
 Download wildfire incidents data from [InciWeb](https://inciweb.nwcg.gov/).
 
 ```{contents} Table of contents
 :local:
 :depth: 2
@@ -34,14 +31,20 @@
 
 Download active fire incidents from inciweb.
 
 ```sh
 inciwebwildfires incidents
 ```
 
+Download prescribed fire incidents from inciweb.
+```sh
+inciwebwildfires prescribed_fires
+```
+
+
 ## Python usage
 
 Import the library.
 
 ```python
 import inciweb_wildfires
 ```
```

### Comparing `inciweb-wildfires-1.0.0/inciweb_wildfires/__init__.py` & `inciweb-wildfires-1.1.0/inciweb_wildfires/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 from __future__ import annotations
 
 import requests
 from geojson import Feature, FeatureCollection, Point
 
 
-def get_incidents() -> FeatureCollection:
+def get_data(t) -> FeatureCollection:
     """
-    Get active incidents data from InciWeb.
+    Get all incidents data from InciWeb.
+
+    Passes in 't' parameter used to specify type of data (Wildfire, Prescribed Fire)
+    Incident Types
 
     Returns GeoJson FeatureCollection.
     """
     # Get the URL
     url = "https://inciweb.wildfire.gov/api/map_data"
     r = requests.get(url)
 
@@ -24,27 +27,51 @@
 
     # Get the JSON data
     data = r.json()
 
     # Loop through all the placemarks
     feature_list = []
     for d in data:
-        # Reformat as GeoJSON
-        x = convert_coords(d["long_deg"], d["long_min"], d["long_sec"])
-        y = convert_coords(d["lat_deg"], d["lat_min"], d["lat_sec"])
-        if x > 0:
-            x = -x
-        p = Point((x, y))
-        f = Feature(geometry=p, properties=d)
+        # Only type specified
+        if d['type'] == t:
+            # Reformat as GeoJSON
+            x = convert_coords(d["long_deg"], d["long_min"], d["long_sec"])
+            y = convert_coords(d["lat_deg"], d["lat_min"], d["lat_sec"])
+            if x > 0:
+                x = -x
+            p = Point((x, y))
+            f = Feature(geometry=p, properties=d)
+            # Add it to the list
+            feature_list.append(f)
+        else:
+            continue
+    # Pass it out
+    return FeatureCollection(feature_list)
+
 
-        # Add it to the list
-        feature_list.append(f)
+def get_incidents() -> FeatureCollection:
+    """
+    Get all active wildfire incidents from InciWeb.
+    Returns GeoJson FeatureCollection.
+    """
+    features = get_data("Wildfire")
 
     # Pass it out
-    return FeatureCollection(feature_list)
+    return features
+
+
+def get_prescribed_fires() -> FeatureCollection:
+    """
+    Get all active prescribed fire incidents from InciWeb.
+    Returns GeoJson FeatureCollection.
+    """
+    features = get_data("Prescribed Fire")
+
+    # Pass it out
+    return features
 
 
 def convert_coords(deg: str, min: str, sec: str) -> float:
     """Handle the flawed coordinates published by InciWeb."""
     if not min.strip():
         min = '0'
     if not sec.strip():
```

### Comparing `inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/PKG-INFO` & `inciweb-wildfires-1.1.0/inciweb_wildfires.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inciweb-wildfires
-Version: 1.0.0
+Version: 1.1.0
 Summary: Download wildfire incidents data from InciWeb
 Home-page: http://www.github.com/datadesk/inciweb-wildfires
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/inciweb-wildfires
```

### Comparing `inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/SOURCES.txt` & `inciweb-wildfires-1.1.0/inciweb_wildfires.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 .github/workflows/docs.yml
 .github/workflows/scrape.yml
 data/incidents.json
 data/timestamp.txt
 docs/Makefile
 docs/conf.py
 docs/index.md
-docs/make.bat
-docs/requirements.txt
-docs/_static/css/custom.css
-docs/_templates/nav.html
 inciweb_wildfires/__init__.py
 inciweb_wildfires/cli.py
 inciweb_wildfires.egg-info/PKG-INFO
 inciweb_wildfires.egg-info/SOURCES.txt
 inciweb_wildfires.egg-info/dependency_links.txt
 inciweb_wildfires.egg-info/entry_points.txt
 inciweb_wildfires.egg-info/requires.txt
```

### Comparing `inciweb-wildfires-1.0.0/setup.py` & `inciweb-wildfires-1.1.0/setup.py`

 * *Files identical despite different names*

