# Comparing `tmp/nrtk_explorer-0.2.1.tar.gz` & `tmp/nrtk_explorer-0.2.2.tar.gz`

## Comparing `nrtk_explorer-0.2.1.tar` & `nrtk_explorer-0.2.2.tar`

### file list

```diff
@@ -1,119 +1,117 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.codespellrc
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.flake8
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    29029 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/MANIFEST.in
--rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/screenshot.png
--rw-r--r--   0        0        0  4643872 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/usage.png
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.github/workflows/create_release.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.github/workflows/push_to_release.yaml
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/README.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/create_exe.bat
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/create_linux.sh
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/create_mac.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/requirements.txt
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/run.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/DEPLOY.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/Dockerfile
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/captain-definition
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/scripts/build_image.sh
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/scripts/build_server.sh
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/scripts/run_image.sh
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/scripts/run_server.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/setup/apps.yml
--rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/setup/initialize.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/setup/requirements.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/examples/jupyter/show.ipynb
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/__init__.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/applet.py
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/core.py
--rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/embeddings.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/filtering.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/jupyter.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/main.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/parameters.py
--rw-r--r--   0        0        0    16333 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/quasar.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/vuetify2.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/vuetify3.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/collapsible_card.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/image_list.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/layout.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/result_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/dataset.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/dimension_reducers.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/embeddings_extractor.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/filtering.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/images_manager.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/ml_models.py
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/nrtk_transforms.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/object_detector.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/transforms.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/assets/__init__.py
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/assets/imagenet_classes.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/module/.gitignore
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/module/__init__.py
--rw-r--r--   0        0        0   725513 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/module/serve/styles.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/__init__.py
--rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
--rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
--rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
--rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
--rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
--rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
--rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
--rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
--rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
--rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
--rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
--rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
--rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
--rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
--rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
--rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
--rw-r--r--   0        0        0   237505 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/widgets/__init__.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/widgets/nrtk_explorer.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/requirements.txt
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/test_embeddings.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/test_filtering.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/test_import.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/test_object_detector.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/.editorconfig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/.eslintrc.cjs
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/.prettierrc.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/env.d.ts
--rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/package-lock.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/tsconfig.app.json
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/tsconfig.json
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/tsconfig.node.json
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/vite.config.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/public/styles.css
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/main.js
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/FilterOperatorWidget.vue
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/FilterOptionsWidget.vue
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/ImageDetection.vue
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/ParamWidget.vue
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/ParamsWidget.vue
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/ScatterPlot.vue
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/index.js
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/types/index.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/utilities/colors.ts
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/LICENSE
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/hatch_build.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/.codespellrc
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/.flake8
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/MANIFEST.in
+-rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/screenshot.png
+-rw-r--r--   0        0        0  4643872 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/usage.png
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/.github/workflows/create_release.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/.github/workflows/push_to_release.yaml
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/desktop/README.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/desktop/create_exe.bat
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/desktop/create_linux.sh
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/desktop/create_mac.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/desktop/requirements.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/desktop/run.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/DEPLOY.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/Dockerfile
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/captain-definition
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/scripts/build_image.sh
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/scripts/build_server.sh
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/scripts/run_image.sh
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/scripts/run_server.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/setup/apps.yml
+-rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/setup/initialize.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/bundles/docker/setup/requirements.txt
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/examples/jupyter/show.ipynb
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/__init__.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/applet.py
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/core.py
+-rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/embeddings.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/filtering.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/jupyter.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/main.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/parameters.py
+-rw-r--r--   0        0        0    16058 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/test/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/test/quasar.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/test/vuetify2.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/test/vuetify3.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/ui/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/ui/collapsible_card.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/ui/image_list.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/app/ui/layout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/dataset.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/dimension_reducers.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/embeddings_extractor.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/filtering.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/images_manager.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/nrtk_transforms.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/object_detector.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/transforms.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/assets/__init__.py
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/library/assets/imagenet_classes.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/module/.gitignore
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/module/__init__.py
+-rw-r--r--   0        0        0   725513 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/module/serve/styles.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/__init__.py
+-rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
+-rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
+-rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
+-rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
+-rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
+-rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
+-rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
+-rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
+-rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
+-rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
+-rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
+-rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
+-rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
+-rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
+-rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
+-rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
+-rw-r--r--   0        0        0   237505 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/widgets/__init__.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/src/nrtk_explorer/widgets/nrtk_explorer.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/tests/requirements.txt
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/tests/test_embeddings.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/tests/test_filtering.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/tests/test_import.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/tests/test_object_detector.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/.editorconfig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/.eslintrc.cjs
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/.prettierrc.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/env.d.ts
+-rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/package-lock.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/tsconfig.app.json
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/tsconfig.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/tsconfig.node.json
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/vite.config.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/public/styles.css
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/main.js
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/components/FilterOperatorWidget.vue
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/components/FilterOptionsWidget.vue
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/components/ImageDetection.vue
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/components/ParamWidget.vue
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/components/ParamsWidget.vue
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/components/ScatterPlot.vue
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/components/index.js
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/types/index.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/vue-components/src/utilities/colors.ts
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/hatch_build.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.2/PKG-INFO
```

### Comparing `nrtk_explorer-0.2.1/CHANGELOG.md` & `nrtk_explorer-0.2.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 # CHANGELOG
 
 
 
+## v0.2.2 (2024-05-22)
+
+### Chore
+
+* chore: remove unused python module ([`5a9271c`](https://github.com/Kitware/nrtk-explorer/commit/5a9271caeb5a9924cc272780fa3ecb143a26a523))
+
+### Fix
+
+* fix: remove unused libraries and python modules ([`f82b46c`](https://github.com/Kitware/nrtk-explorer/commit/f82b46c2bf7e93e0b11c24bee06c4a415497964b))
+
+### Unknown
+
+* Merge main to release ([`7b2e41e`](https://github.com/Kitware/nrtk-explorer/commit/7b2e41ebc0f282e0f8630052156b0d6e3db036d1))
+
+* Auto-merge release back to main ([`cbb920a`](https://github.com/Kitware/nrtk-explorer/commit/cbb920a5d164f45667556c2fbee935dc917ef457))
+
+
 ## v0.2.1 (2024-05-21)
 
 ### Ci
 
 * ci: create_release only in release branch ([`d07bdf4`](https://github.com/Kitware/nrtk-explorer/commit/d07bdf4ad712a8a2936782b1fab8a934858cedd3))
 
 ### Fix
```

### Comparing `nrtk_explorer-0.2.1/CONTRIBUTING.rst` & `nrtk_explorer-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/screenshot.png` & `nrtk_explorer-0.2.2/screenshot.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/usage.png` & `nrtk_explorer-0.2.2/usage.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/.github/workflows/ci.yml` & `nrtk_explorer-0.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/.github/workflows/create_release.yaml` & `nrtk_explorer-0.2.2/.github/workflows/create_release.yaml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/.github/workflows/push_to_release.yaml` & `nrtk_explorer-0.2.2/.github/workflows/push_to_release.yaml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/bundles/desktop/README.md` & `nrtk_explorer-0.2.2/bundles/desktop/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/bundles/docker/DEPLOY.md` & `nrtk_explorer-0.2.2/bundles/docker/DEPLOY.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/bundles/docker/README.md` & `nrtk_explorer-0.2.2/bundles/docker/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/examples/jupyter/show.ipynb` & `nrtk_explorer-0.2.2/examples/jupyter/show.ipynb`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/applet.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/applet.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/core.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/core.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/embeddings.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/filtering.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/jupyter.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/parameters.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/parameters.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/transforms.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,14 @@
 
 import nrtk_explorer.library.transforms as trans
 import nrtk_explorer.library.nrtk_transforms as nrtk_trans
 from nrtk_explorer.library import images_manager, object_detector
 from nrtk_explorer.app import ui
 from nrtk_explorer.app.applet import Applet
 from nrtk_explorer.app.parameters import ParametersApp
-from nrtk_explorer.library.ml_models import (
-    ClassificationResNet50,
-    ClassificationAlexNet,
-    ClassificationVgg16,
-)
 import nrtk_explorer.test_data
 
 import json
 import os
 
 
 logger = logging.getLogger(__name__)
@@ -62,22 +57,20 @@
         self.is_standalone_app = self.server.state.parent is None
         if self.is_standalone_app:
             self.context.images_manager = images_manager.ImagesManager()
 
         if self.context["image_objects"] is None:
             self.context["image_objects"] = {}
 
-        self.models = {
-            "ClassificationResNet50": ClassificationResNet50(server),
-            "ClassificationAlexNet": ClassificationAlexNet(server),
-            "ClassificationVgg16": ClassificationVgg16(server),
-        }
-
         self._on_transform_fn = None
-        self.state.models = [k for k in self.models.keys()]
+        self.state.models = [
+            "ClassificationResNet50",
+            "ClassificationAlexNet",
+            "ClassificationVgg16",
+        ]
         self.state.feature_extraction_model = self.state.models[0]
 
         self._transforms: Dict[str, trans.ImageTransform] = {
             "identity": trans.IdentityTransform(),
             "blur": trans.GaussianBlurTransform(),
             "invert": trans.InvertTransform(),
             "downsample": trans.DownSampleTransform(),
```

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/quasar.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/test/quasar.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/vuetify2.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/test/vuetify2.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/vuetify3.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/test/vuetify3.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/collapsible_card.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/ui/collapsible_card.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/image_list.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/ui/image_list.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/layout.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/app/ui/layout.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/library/dimension_reducers.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/library/dimension_reducers.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/library/embeddings_extractor.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/library/embeddings_extractor.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/library/filtering.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/library/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/library/images_manager.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/library/images_manager.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/library/nrtk_transforms.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/library/nrtk_transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/library/object_detector.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/library/object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/library/transforms.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/library/transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/library/assets/imagenet_classes.txt` & `nrtk_explorer-0.2.2/src/nrtk_explorer/library/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js` & `nrtk_explorer-0.2.2/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json` & `nrtk_explorer-0.2.2/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/src/nrtk_explorer/widgets/nrtk_explorer.py` & `nrtk_explorer-0.2.2/src/nrtk_explorer/widgets/nrtk_explorer.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/tests/conftest.py` & `nrtk_explorer-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/tests/test_embeddings.py` & `nrtk_explorer-0.2.2/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/tests/test_filtering.py` & `nrtk_explorer-0.2.2/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/tests/test_object_detector.py` & `nrtk_explorer-0.2.2/tests/test_object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/package-lock.json` & `nrtk_explorer-0.2.2/vue-components/package-lock.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/package.json` & `nrtk_explorer-0.2.2/vue-components/package.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/vite.config.ts` & `nrtk_explorer-0.2.2/vue-components/vite.config.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/src/components/FilterOperatorWidget.vue` & `nrtk_explorer-0.2.2/vue-components/src/components/FilterOperatorWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/src/components/FilterOptionsWidget.vue` & `nrtk_explorer-0.2.2/vue-components/src/components/FilterOptionsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/src/components/ImageDetection.vue` & `nrtk_explorer-0.2.2/vue-components/src/components/ImageDetection.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/src/components/ParamWidget.vue` & `nrtk_explorer-0.2.2/vue-components/src/components/ParamWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/src/components/ParamsWidget.vue` & `nrtk_explorer-0.2.2/vue-components/src/components/ParamsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/src/components/ScatterPlot.vue` & `nrtk_explorer-0.2.2/vue-components/src/components/ScatterPlot.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/src/types/index.ts` & `nrtk_explorer-0.2.2/vue-components/src/types/index.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/vue-components/src/utilities/colors.ts` & `nrtk_explorer-0.2.2/vue-components/src/utilities/colors.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/LICENSE` & `nrtk_explorer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/README.md` & `nrtk_explorer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/hatch_build.py` & `nrtk_explorer-0.2.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.1/pyproject.toml` & `nrtk_explorer-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="nrtk-explorer"
-version="0.2.1"
+version="0.2.2"
 description="Model Visualizer"
 authors = [
   {name = "Alessandro Genova", email = "alessandro.genova@kitware.com"},
   {name = "Vicente Adolfo Bolea Sanchez", email = "vicente.bolea@kitware.com"},
 ]
 readme = "README.md"
 keywords = [
@@ -27,31 +27,24 @@
 ]
 
 dependencies = [
     "nrtk",
     "numpy",
     "Pillow",
     "scikit-learn==1.4.2",
-    "smqtk-classifier==0.19.0",
     "accelerate",
-    "smqtk-core==0.19.0",
-    "smqtk-dataprovider==0.18.0",
-    "smqtk-descriptors==0.19.0",
-    "smqtk-detection[torch,centernet]==0.20.1",
-    "smqtk-image-io==0.17.1",
     "tabulate",
     "transformers",
     "timm",
     "torch",
     "torchvision",
     "trame",
     "trame-client>=2.15.0",
     "trame-quasar",
     "trame-server>=2.15.0",
-    "ubelt==1.3.5",
     "umap-learn",
     "tabulate",
 ]
 
 [project.optional-dependencies]
 dev = [
   "black",
```

### Comparing `nrtk_explorer-0.2.1/PKG-INFO` & `nrtk_explorer-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nrtk-explorer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Model Visualizer
 Author-email: Alessandro Genova <alessandro.genova@kitware.com>, Vicente Adolfo Bolea Sanchez <vicente.bolea@kitware.com>
 License-File: LICENSE
 Keywords: Application,Framework,Interactive,Python,Web
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: Other/Proprietary License
@@ -15,30 +15,23 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: accelerate
 Requires-Dist: nrtk
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: scikit-learn==1.4.2
-Requires-Dist: smqtk-classifier==0.19.0
-Requires-Dist: smqtk-core==0.19.0
-Requires-Dist: smqtk-dataprovider==0.18.0
-Requires-Dist: smqtk-descriptors==0.19.0
-Requires-Dist: smqtk-detection[centernet,torch]==0.20.1
-Requires-Dist: smqtk-image-io==0.17.1
 Requires-Dist: tabulate
 Requires-Dist: timm
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: trame
 Requires-Dist: trame-client>=2.15.0
 Requires-Dist: trame-quasar
 Requires-Dist: trame-server>=2.15.0
 Requires-Dist: transformers
-Requires-Dist: ubelt==1.3.5
 Requires-Dist: umap-learn
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: tabulate; extra == 'dev'
```

