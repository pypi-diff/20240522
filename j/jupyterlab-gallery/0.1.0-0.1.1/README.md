# Comparing `tmp/jupyterlab_gallery-0.1.0.tar.gz` & `tmp/jupyterlab_gallery-0.1.1.tar.gz`

## Comparing `jupyterlab_gallery-0.1.0.tar` & `jupyterlab_gallery-0.1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/babel.config.js
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/conftest.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jest.config.js
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/junit.xml
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/tsconfig.test.json
--rw-r--r--   0        0        0   374798 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/yarn.lock
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyter-config/server-config/jupyterlab_gallery.json
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/_version.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/gitpuller.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/handlers.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/package.json
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/package.json.orig
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/plugin.json
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/static/274.5cfaaf1bd2162eaab3ef.js
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/static/728.3bf722b918aa1abe3220.js
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/static/remoteEntry.05bb9899f8da7cfad93b.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/tests/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/jupyterlab_gallery/tests/test_handlers.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/schema/plugin.json
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/src/gallery.tsx
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/src/handler.ts
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/src/icons.ts
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/src/index.ts
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/src/svg.d.ts
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/src/types.ts
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/src/__tests__/jupyterlab_gallery.spec.ts
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/style/index.js
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/style/icons/md/LICENSE
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/style/icons/md/gallery.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/ui-tests/tests/jupyterlab_gallery.spec.ts
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/LICENSE
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/README.md
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/.copier-answers.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/babel.config.js
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/conftest.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jest.config.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/junit.xml
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/tsconfig.test.json
+-rw-r--r--   0        0        0   374798 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/yarn.lock
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyter-config/server-config/jupyterlab_gallery.json
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/_version.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/gitpuller.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/handlers.py
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/package.json
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/package.json.orig
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/plugin.json
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/static/274.65854fd2800238c6f003.js
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/static/728.3bf722b918aa1abe3220.js
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/static/remoteEntry.5612c0eb3fdd124695fe.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/tests/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/jupyterlab_gallery/tests/test_handlers.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/schema/plugin.json
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/src/gallery.tsx
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/src/handler.ts
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/src/icons.ts
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/src/index.ts
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/src/svg.d.ts
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/src/types.ts
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/src/__tests__/jupyterlab_gallery.spec.ts
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/style/index.js
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/style/icons/md/gallery.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/ui-tests/tests/jupyterlab_gallery.spec.ts
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/README.md
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.1/PKG-INFO
```

### Comparing `jupyterlab_gallery-0.1.0/.copier-answers.yml` & `jupyterlab_gallery-0.1.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/RELEASE.md` & `jupyterlab_gallery-0.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/jest.config.js` & `jupyterlab_gallery-0.1.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/package.json` & `jupyterlab_gallery-0.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlab_gallery-0.1.0/tsconfig.json` & `jupyterlab_gallery-0.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/yarn.lock` & `jupyterlab_gallery-0.1.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/jupyterlab_gallery/__init__.py` & `jupyterlab_gallery-0.1.1/jupyterlab_gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/jupyterlab_gallery/gitpuller.py` & `jupyterlab_gallery-0.1.1/jupyterlab_gallery/gitpuller.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/jupyterlab_gallery/handlers.py` & `jupyterlab_gallery-0.1.1/jupyterlab_gallery/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     # timestamp from .git/FETCH_HEAD of the cloned repo
     exposed_config["lastUpdated"] = "2024-05-01"
     exposed_config["currentTag"] = "v3.2.4"
     # the UI can show that there are X updates available; it could also show
     # a summary of the commits available, or tags available; possibly the name
     # of the most recent tag and would be sufficient over sending the list of commits,
     # which can be long and delay the initialization.
-    exposed_config["updatesAvailable"] = True
+    exposed_config["updatesAvailable"] = False
     exposed_config["isCloned"] = local_path.exists()
     exposed_config["newestTag"] = "v3.2.5"
     exposed_config["updates"] = [
         {
             "revision": "02f04c339f880540064d2223176830afdd02f5fa",
             "title": "commit description",
             "description": "long commit description",
```

### Comparing `jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/package.json` & `jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5612c0eb3fdd124695fe.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -110,15 +110,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-gallery",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.05bb9899f8da7cfad93b.js",
+            "load": "static/remoteEntry.5612c0eb3fdd124695fe.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_gallery"
                 },
@@ -207,9 +207,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/package.json.orig` & `jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/static/274.5cfaaf1bd2162eaab3ef.js` & `jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/static/274.65854fd2800238c6f003.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -140,15 +140,15 @@
                     onClick: () => {
                         a.open(t)
                     }
                 }, "Open") : n.createElement(l.Button, {
                     onClick: async () => {
                         s("Downloading"), await a.download(t)
                     }
-                }, "Setup up"), t.updatesAvailable ? n.createElement(l.Button, null, "Update") : null))
+                }, "Setup up"), t.isCloned && t.updatesAvailable ? n.createElement(l.Button, null, "Update") : null))
             }
             const m = new l.LabIcon({
                     name: "jupyterlab-gallery:gallery",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path class="jp-icon3" fill="rgb(97,97,97)" d="M1 3V21H23V3H1M21 5V14H3V5H21M11 16V19H8V16H11M3 16H6V19H3V16M13 19V16H16V19H13M18 19V16H21V19H18Z" /></svg>'
                 }),
                 b = {
                     id: "jupyterlab-gallery:plugin",
```

### Comparing `jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/static/728.3bf722b918aa1abe3220.js` & `jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/static/728.3bf722b918aa1abe3220.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/static/remoteEntry.05bb9899f8da7cfad93b.js` & `jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/static/remoteEntry.5612c0eb3fdd124695fe.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, l, u, s, f, d, p, c, h, v, b, g = {
+    var e, r, t, n, a, o, i, l, u, f, s, p, d, c, h, v, b, g = {
             607: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(274).then((() => () => t(274))),
                         "./extension": () => t.e(274).then((() => () => t(274))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,49 +43,49 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        274: "5cfaaf1bd2162eaab3ef",
+        274: "65854fd2800238c6f003",
         728: "3bf722b918aa1abe3220"
     } [e] + ".js?v=" + {
-        274: "5cfaaf1bd2162eaab3ef",
+        274: "65854fd2800238c6f003",
         728: "3bf722b918aa1abe3220"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab-gallery:", m.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var f = u[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
-                        i = f;
+                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
+                    var s = u[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
+                        i = s;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var p = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(d);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                d = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         l = a[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (a[r] = {
                         get: () => m.e(274).then((() => () => m(274))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-gallery", "0.1.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("jupyterlab-gallery", "0.1.1"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,67 +164,67 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var s, f, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !u || ("u" == d ? l > n && !a : "" == d != a);
-                if ("u" == f) {
-                    if (!u || "u" != d) return !1
+                var f, s, p = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == p ? l > n && !a : "" == p != a);
+                if ("u" == s) {
+                    if (!u || "u" != p) return !1
                 } else if (u)
-                    if (d == f)
+                    if (p == s)
                         if (l <= n) {
-                            if (s != e[l]) return !1
+                            if (f != e[l]) return !1
                         } else {
-                            if (a ? s > e[l] : s < e[l]) return !1;
-                            s != e[l] && (u = !1)
+                            if (a ? f > e[l] : f < e[l]) return !1;
+                            f != e[l] && (u = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != p && "n" != p) {
                     if (a || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || f < d != a) return !1;
+                    if (l <= n || s < p != a) return !1;
                     u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                } else "s" != p && "n" != p && (u = !1, l--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var d = [],
+            c = d.pop.bind(d);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
         var a = l(e, t);
-        return o(n, a) || f(u(e, t, a, n)), d(e[t][a])
-    }, f = e => {
+        return o(n, a) || s(u(e, t, a, n)), p(e[t][a])
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, a) {
+    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, a) {
         var o = m.I(r);
         return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
-        265: () => p("default", "@jupyterlab/translation", [1, 4, 2, 0]),
-        345: () => p("default", "react", [1, 18, 2, 0]),
-        527: () => p("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
-        602: () => p("default", "@lumino/signaling", [1, 2, 0, 0]),
-        670: () => p("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
-        702: () => p("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
-        825: () => p("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
-        861: () => p("default", "@jupyterlab/services", [1, 7, 2, 0]),
-        923: () => p("default", "@jupyterlab/apputils", [1, 4, 3, 0])
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
+        265: () => d("default", "@jupyterlab/translation", [1, 4, 2, 0]),
+        345: () => d("default", "react", [1, 18, 2, 0]),
+        527: () => d("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
+        602: () => d("default", "@lumino/signaling", [1, 2, 0, 0]),
+        670: () => d("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
+        702: () => d("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
+        825: () => d("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
+        861: () => d("default", "@jupyterlab/services", [1, 7, 2, 0]),
+        923: () => d("default", "@jupyterlab/apputils", [1, 4, 3, 0])
     }, v = {
         274: [265, 345, 527, 602, 670, 702, 825, 861, 923]
     }, b = {}, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(c, e)) return r.push(c[e]);
             if (!b[e]) {
                 var t = r => {
```

### Comparing `jupyterlab_gallery-0.1.0/jupyterlab_gallery/labextension/static/third-party-licenses.json` & `jupyterlab_gallery-0.1.1/jupyterlab_gallery/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/src/gallery.tsx` & `jupyterlab_gallery-0.1.1/src/gallery.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -160,12 +160,14 @@
             onClick={() => {
               actions.open(exhibit);
             }}
           >
             Open
           </Button>
         )}
-        {exhibit.updatesAvailable ? <Button>Update</Button> : null}
+        {exhibit.isCloned && exhibit.updatesAvailable ? (
+          <Button>Update</Button>
+        ) : null}
       </div>
     </div>
   );
 }
```

### Comparing `jupyterlab_gallery-0.1.0/src/handler.ts` & `jupyterlab_gallery-0.1.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/src/index.ts` & `jupyterlab_gallery-0.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/style/icons/md/LICENSE` & `jupyterlab_gallery-0.1.1/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/ui-tests/README.md` & `jupyterlab_gallery-0.1.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/ui-tests/tests/jupyterlab_gallery.spec.ts` & `jupyterlab_gallery-0.1.1/ui-tests/tests/jupyterlab_gallery.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/.gitignore` & `jupyterlab_gallery-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/LICENSE` & `jupyterlab_gallery-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/README.md` & `jupyterlab_gallery-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # jupyterlab-gallery
 
+![Extension status](https://img.shields.io/badge/status-draft-critical 'Not yet working')
 [![Github Actions Status](https://github.com/nebari-dev/jupyterlab-gallery/workflows/Build/badge.svg)](https://github.com/nebari-dev/jupyterlab-gallery/actions/workflows/build.yml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nebari-dev/jupyterlab-gallery/main?urlpath=lab)
 
 A JupyterLab gallery extension for presenting and downloading examples from remote repositories
 
 This extension is composed of a Python package named `jupyterlab-gallery`
 for the server extension and a NPM package named `jupyterlab-gallery`
```

### Comparing `jupyterlab_gallery-0.1.0/pyproject.toml` & `jupyterlab_gallery-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.0/PKG-INFO` & `jupyterlab_gallery-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-gallery
-Version: 0.1.0
+Version: 0.1.1
 Dynamic: Keywords
 Summary: A JupyterLab gallery extension for presenting and downloading examples from remote repositories
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-gallery
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-gallery/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-gallery.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
@@ -61,14 +61,15 @@
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-jupyter[server]>=0.6.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # jupyterlab-gallery
 
+![Extension status](https://img.shields.io/badge/status-draft-critical 'Not yet working')
 [![Github Actions Status](https://github.com/nebari-dev/jupyterlab-gallery/workflows/Build/badge.svg)](https://github.com/nebari-dev/jupyterlab-gallery/actions/workflows/build.yml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nebari-dev/jupyterlab-gallery/main?urlpath=lab)
 
 A JupyterLab gallery extension for presenting and downloading examples from remote repositories
 
 This extension is composed of a Python package named `jupyterlab-gallery`
 for the server extension and a NPM package named `jupyterlab-gallery`
```

