# Comparing `tmp/jupyterlab_amphi-0.3.3.tar.gz` & `tmp/jupyterlab_amphi-0.3.4.tar.gz`

## Comparing `jupyterlab_amphi-0.3.3.tar` & `jupyterlab_amphi-0.3.4.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/.yarnrc.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/MANIFEST.in
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/install.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/lerna.json
--rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/output.json
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/package.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/tsconfig.eslint.json
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/tsconfigbase.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/_version.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/package.json
--rw-r--r--   0        0        0   126222 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/116.a2462f90d7701c371aa8.js
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
--rw-r--r--   0        0        0    22345 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js.LICENSE.txt
--rw-r--r--   0        0        0  1441798 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/687.82f4edc6966c97595e01.js
--rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/687.82f4edc6966c97595e01.js.LICENSE.txt
--rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/remoteEntry.1ce7c98af16331b594f6.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/style.js
--rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/third-party-licenses.json
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/package.json
--rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
--rw-r--r--   0        0        0    56724 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/142.1ffdd6d84b9f153e1c84.js
--rw-r--r--   0        0        0    27269 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js.LICENSE.txt
--rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
--rw-r--r--   0        0        0  1437524 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/422.87216a9371fbc611f07f.js
--rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/422.87216a9371fbc611f07f.js.LICENSE.txt
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
--rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
--rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
--rw-r--r--   0        0        0   439969 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/841.17235cce88409653d379.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/841.17235cce88409653d379.js.LICENSE.txt
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/remoteEntry.e7b2fd7c27479971192a.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/style.js
--rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/third-party-licenses.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/package.json
--rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
--rw-r--r--   0        0        0    33113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/412.23a82146827c21626eae.js
--rw-r--r--   0        0        0    27297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
--rw-r--r--   0        0        0  1447496 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/735.c92310c8c2bc6a1bb9f6.js
--rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/735.c92310c8c2bc6a1bb9f6.js.LICENSE.txt
--rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/remoteEntry.9e0521f3ade01710154b.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/style.js
--rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/third-party-licenses.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/package.json
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/432.4a34574395b64c0ecb2a.js
--rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/684.c971d4662ee41caa2dda.js
--rw-r--r--   0        0        0   751978 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/818.9952ec63ac4e7e5b37d1.js
--rw-r--r--   0        0        0    13950 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/818.9952ec63ac4e7e5b37d1.js.LICENSE.txt
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/remoteEntry.5034e9c3d84820fce19f.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/style.js
--rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/third-party-licenses.json
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/package.json
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
--rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/static/remoteEntry.16d4e872755a30ebdc97.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/static/third-party-licenses.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi_extension/_version.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/install.json
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/tsconfig.json
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
--rw-r--r--   0        0        0    14658 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/CodeGenerator.tsx
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/CustomHandle.tsx
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/PipelineComponent.tsx
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/PipelineService.tsx
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/RequestService.tsx
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/configUtils.tsx
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/connectionUtils.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/declarations.d.ts
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/generatorUtils.tsx
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/icons.ts
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/index.ts
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/rendererUtils.tsx
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/InputRegular.tsx
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/dataMapping.tsx
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectColumn.tsx
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectColumns.tsx
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectRegular.tsx
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/transferData.tsx
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/base.css
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/crosshair-16.svg
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/minus-16.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/play-16.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/play-circle-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/plus-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/plus-24.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/search-16.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/search-24.svg
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/settings-16.svg
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/settings-24.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/trash-16.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/trash-24.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/x-16.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/x-square-16.svg
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/install.json
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/package.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/pipeline-16.svg
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/pipeline-24.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/tailwind.config.js
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/tsconfig.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/schema/extension.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/schema/plugin copy.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/schema/plugin.json
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/Dropzone.tsx
--rw-r--r--   0        0        0    20782 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/PipelineEditorWidget.tsx
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/customEdge.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/declarations.d.ts
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/icons.ts
--rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/index.ts
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/canvas.css
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/index.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/index.js
--rw-r--r--   0        0        0    22125 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/output.css
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/pipeline-category-icon.svg
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/react-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/tailwinds_preflight.css
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/api-24.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/file-plus-24.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/file-text-24.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/monitor-24.svg
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/.gitignore
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/.yarnrc.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/MANIFEST.in
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/install.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/lerna.json
+-rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/output.json
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/tsconfig.eslint.json
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/tsconfigbase.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/_version.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/package.json
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
+-rw-r--r--   0        0        0    22345 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js.LICENSE.txt
+-rw-r--r--   0        0        0  1441949 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/687.e44561a1742c6083cba0.js
+-rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/687.e44561a1742c6083cba0.js.LICENSE.txt
+-rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
+-rw-r--r--   0        0        0   143367 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/remoteEntry.1144a177b5daf1c9977c.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/style.js
+-rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
+-rw-r--r--   0        0        0    56966 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js
+-rw-r--r--   0        0        0    27269 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js.LICENSE.txt
+-rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
+-rw-r--r--   0        0        0  1437675 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/422.27a4f789109562c256e8.js
+-rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/422.27a4f789109562c256e8.js.LICENSE.txt
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
+-rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
+-rw-r--r--   0        0        0   439969 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/841.6f47bec498543a801840.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/841.6f47bec498543a801840.js.LICENSE.txt
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/remoteEntry.001fdc1b89863b0cb38e.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/style.js
+-rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/package.json
+-rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
+-rw-r--r--   0        0        0    33113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/412.23a82146827c21626eae.js
+-rw-r--r--   0        0        0    27297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
+-rw-r--r--   0        0        0  1447644 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/735.711b3b299b885104b862.js
+-rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/735.711b3b299b885104b862.js.LICENSE.txt
+-rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/remoteEntry.bfb171550404534afb06.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/style.js
+-rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/package.json
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js
+-rw-r--r--   0        0        0   751992 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/595.853e8b63deafdcf653a9.js
+-rw-r--r--   0        0        0    13950 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/595.853e8b63deafdcf653a9.js.LICENSE.txt
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/remoteEntry.871deda2d395cf3ebdb5.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/style.js
+-rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/package.json
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
+-rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/remoteEntry.9bc842b6cc0c70b4b0c3.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/third-party-licenses.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi_extension/_version.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/install.json
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/tsconfig.json
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
+-rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/CodeGenerator.tsx
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/CustomHandle.tsx
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/PipelineComponent.tsx
+-rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/PipelineService.tsx
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/RequestService.tsx
+-rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/configUtils.tsx
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/connectionUtils.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/declarations.d.ts
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/generatorUtils.tsx
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/icons.ts
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/index.ts
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/rendererUtils.tsx
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/InputRegular.tsx
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
+-rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/dataMapping.tsx
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectColumn.tsx
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectColumns.tsx
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectRegular.tsx
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/transferData.tsx
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/base.css
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/crosshair-16.svg
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/minus-16.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/play-16.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/play-circle-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/plus-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/plus-24.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/search-16.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/search-24.svg
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/settings-16.svg
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/settings-24.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/trash-16.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/trash-24.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/x-16.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/x-square-16.svg
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/install.json
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/package.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/pipeline-16.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/pipeline-24.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/tailwind.config.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/tsconfig.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/extension.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/plugin copy.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/plugin.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/Dropzone.tsx
+-rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/PipelineEditorWidget.tsx
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/customEdge.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/declarations.d.ts
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/icons.ts
+-rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/index.ts
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/canvas.css
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/index.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/index.js
+-rw-r--r--   0        0        0    22125 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/output.css
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/pipeline-category-icon.svg
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/react-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/tailwinds_preflight.css
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/api-24.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/file-plus-24.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/file-text-24.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/monitor-24.svg
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/.gitignore
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/PKG-INFO
```

### Comparing `jupyterlab_amphi-0.3.3/output.json` & `jupyterlab_amphi-0.3.4/output.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/package.json` & `jupyterlab_amphi-0.3.4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.4'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.3.3",
+    "version": "0.3.4",
     "workspaces": {
         "packages": [
             "packages/pipeline-editor",
             "packages/pipeline-components-manager",
             "packages/pipeline-components-core",
             "packages/pipeline-console",
             "packages/pipeline-metadata-panel"
```

### Comparing `jupyterlab_amphi-0.3.3/tsconfigbase.json` & `jupyterlab_amphi-0.3.4/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/package.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.1144a177b5daf1c9977c.js'}}",*

 * * "'version'": "'0.3.3'"}*

```diff
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1ce7c98af16331b594f6.js",
+            "load": "static/remoteEntry.1144a177b5daf1c9977c.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-core",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -83,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.3.3"
 }
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/116.a2462f90d7701c371aa8.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (self.webpackChunk_amphi_pipeline_components_core = self.webpackChunk_amphi_pipeline_components_core || []).push([
-    [116], {
-        4116: (e, n, t) => {
+    [792], {
+        5792: (e, n, t) => {
             t.r(n), t.d(n, {
-                default: () => Qe
+                default: () => tn
             });
             var o = t(3254),
                 a = t(3345),
                 s = t.n(a),
                 r = t(2473),
                 l = t(1527);
             const d = new l.LabIcon({
@@ -49,22 +49,22 @@
                     name: "amphi:expandIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M23 12a.75.75 0 00-.232-.543l-5.5-5.25a.75.75 0 00-1.036 1.086L21.164 12l-4.932 4.707a.75.75 0 001.036 1.085l5.5-5.25A.75.75 0 0023 12zM1 12a.75.75 0 01.232-.543l5.5-5.25a.75.75 0 111.036 1.086L2.836 12l4.932 4.707a.75.75 0 01-1.036 1.085l-5.5-5.25A.75.75 0 011 12z"/><path d="M8 11a1 1 0 100 2h.01a1 1 0 100-2H8zM11 12a1 1 0 011-1h.01a1 1 0 110 2H12a1 1 0 01-1-1zM16 11a1 1 0 100 2h.01a1 1 0 100-2H16z"/></g></svg>'
                 }),
                 v = new l.LabIcon({
                     name: "amphi:dedupIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M3.75 1A2.75 2.75 0 001 3.75v10.5A2.75 2.75 0 003.75 17h1a.75.75 0 000-1.5h-1c-.69 0-1.25-.56-1.25-1.25V3.75c0-.69.56-1.25 1.25-1.25h10.5c.69 0 1.25.56 1.25 1.25v1a.75.75 0 001.5 0v-1A2.75 2.75 0 0014.25 1H3.75z"/><path fill-rule="evenodd" d="M9.75 7A2.75 2.75 0 007 9.75v10.5A2.75 2.75 0 009.75 23h10.5A2.75 2.75 0 0023 20.25V9.75A2.75 2.75 0 0020.25 7H9.75zM8.5 9.75c0-.69.56-1.25 1.25-1.25h10.5c.69 0 1.25.56 1.25 1.25v10.5c0 .69-.56 1.25-1.25 1.25H9.75c-.69 0-1.25-.56-1.25-1.25V9.75z" clip-rule="evenodd"/></g></svg>'
                 }),
-                C = (new l.LabIcon({
+                I = (new l.LabIcon({
                     name: "amphi:globeIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path fill="currentColor" fill-rule="evenodd" d="M12 1C5.925 1 1 5.925 1 12s4.925 11 11 11 11-4.925 11-11S18.075 1 12 1zm-1.673 1.647A9.506 9.506 0 002.552 11h4.747a16.673 16.673 0 013.028-8.353zm3.346 0A16.673 16.673 0 0116.701 11h4.747a9.506 9.506 0 00-7.775-8.353zM15.196 11A15.149 15.149 0 0012 2.916 15.149 15.149 0 008.804 11h6.392zm-6.427 1.5h6.462A15.16 15.16 0 0112 21.084 15.16 15.16 0 018.769 12.5zm-1.502 0H2.513c.23 4.45 3.525 8.091 7.814 8.853a16.683 16.683 0 01-3.06-8.853zm6.406 8.853a16.683 16.683 0 003.06-8.853h4.754c-.23 4.45-3.525 8.091-7.814 8.853z" clip-rule="evenodd"/></svg>'
                 }), new l.LabIcon({
                     name: "amphi:sortIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M3 5.75A.75.75 0 013.75 5h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 5.75zM3.75 9a.75.75 0 000 1.5h9.5a.75.75 0 000-1.5h-9.5zM16.963 20.443a.747.747 0 00.817-.163l4-4a.75.75 0 10-1.06-1.06L18 17.94V9.75a.75.75 0 00-1.5 0v8.19l-2.72-2.72a.75.75 0 10-1.06 1.06l4 4a.748.748 0 00.243.163zM3.75 13a.75.75 0 000 1.5h5.5a.75.75 0 000-1.5h-5.5zM3 17.75a.75.75 0 01.75-.75h3.5a.75.75 0 010 1.5h-3.5a.75.75 0 01-.75-.75z"/></g></svg>'
                 })),
-                I = new l.LabIcon({
+                C = new l.LabIcon({
                     name: "amphi:editIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path fill-rule="evenodd" d="M17.055 2.884a2.75 2.75 0 013.89 0l.171.171a2.75 2.75 0 010 3.89l-9.005 9.005A4.75 4.75 0 0110.516 17L6.28 18.696a.75.75 0 01-.975-.975l1.695-4.237a4.749 4.749 0 011.051-1.595l9.005-9.005zm2.829 1.06a1.25 1.25 0 00-1.768 0l-.555.556L19.5 6.44l.555-.556a1.25 1.25 0 000-1.768l-.171-.172zM18.439 7.5L16.5 5.56l-7.39 7.39a3.25 3.25 0 00-.719 1.09l-1.045 2.614 2.613-1.046a3.25 3.25 0 001.091-.719L18.44 7.5z" clip-rule="evenodd"/><path d="M3.75 4.5c-.69 0-1.25.56-1.25 1.25v14.5c0 .69.56 1.25 1.25 1.25h14.5c.69 0 1.25-.56 1.25-1.25V13a.75.75 0 011.5 0v7.25A2.75 2.75 0 0118.25 23H3.75A2.75 2.75 0 011 20.25V5.75A2.75 2.75 0 013.75 3H11a.75.75 0 010 1.5H3.75z"/></g></svg>'
                 }),
                 b = new l.LabIcon({
                     name: "amphi:typeIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path fill="currentColor" d="M3 3.75A.75.75 0 013.75 3h16a.75.75 0 01.75.75v2.5a.75.75 0 01-1.5 0V4.5h-6.5v15h2a.75.75 0 010 1.5H9a.75.75 0 010-1.5h2v-15H4.5v1.75a.75.75 0 01-1.5 0v-2.5z"/></svg>'
                 }),
@@ -103,17 +103,21 @@
                 E = new l.LabIcon({
                     name: "amphi:openAiIcon",
                     svgstr: '<?xml version="1.0" encoding="utf-8"?>\x3c!-- Uploaded to: SVG Repo, www.svgrepo.com, Generator: SVG Repo Mixer Tools --\x3e\n<svg fill="#000000" width="800px" height="800px" viewBox="0 0 24 24" role="img" xmlns="http://www.w3.org/2000/svg"><title>OpenAI icon</title><path d="M22.2819 9.8211a5.9847 5.9847 0 0 0-.5157-4.9108 6.0462 6.0462 0 0 0-6.5098-2.9A6.0651 6.0651 0 0 0 4.9807 4.1818a5.9847 5.9847 0 0 0-3.9977 2.9 6.0462 6.0462 0 0 0 .7427 7.0966 5.98 5.98 0 0 0 .511 4.9107 6.051 6.051 0 0 0 6.5146 2.9001A5.9847 5.9847 0 0 0 13.2599 24a6.0557 6.0557 0 0 0 5.7718-4.2058 5.9894 5.9894 0 0 0 3.9977-2.9001 6.0557 6.0557 0 0 0-.7475-7.0729zm-9.022 12.6081a4.4755 4.4755 0 0 1-2.8764-1.0408l.1419-.0804 4.7783-2.7582a.7948.7948 0 0 0 .3927-.6813v-6.7369l2.02 1.1686a.071.071 0 0 1 .038.052v5.5826a4.504 4.504 0 0 1-4.4945 4.4944zm-9.6607-4.1254a4.4708 4.4708 0 0 1-.5346-3.0137l.142.0852 4.783 2.7582a.7712.7712 0 0 0 .7806 0l5.8428-3.3685v2.3324a.0804.0804 0 0 1-.0332.0615L9.74 19.9502a4.4992 4.4992 0 0 1-6.1408-1.6464zM2.3408 7.8956a4.485 4.485 0 0 1 2.3655-1.9728V11.6a.7664.7664 0 0 0 .3879.6765l5.8144 3.3543-2.0201 1.1685a.0757.0757 0 0 1-.071 0l-4.8303-2.7865A4.504 4.504 0 0 1 2.3408 7.872zm16.5963 3.8558L13.1038 8.364 15.1192 7.2a.0757.0757 0 0 1 .071 0l4.8303 2.7913a4.4944 4.4944 0 0 1-.6765 8.1042v-5.6772a.79.79 0 0 0-.407-.667zm2.0107-3.0231l-.142-.0852-4.7735-2.7818a.7759.7759 0 0 0-.7854 0L9.409 9.2297V6.8974a.0662.0662 0 0 1 .0284-.0615l4.8303-2.7866a4.4992 4.4992 0 0 1 6.6802 4.66zM8.3065 12.863l-2.02-1.1638a.0804.0804 0 0 1-.038-.0567V6.0742a4.4992 4.4992 0 0 1 7.3757-3.4537l-.142.0805L8.704 5.459a.7948.7948 0 0 0-.3927.6813zm1.0976-2.3654l2.602-1.4998 2.6069 1.4998v2.9994l-2.5974 1.4997-2.6067-1.4997Z"/></svg>'
                 }),
                 T = new l.LabIcon({
                     name: "amphi:settings-config-icon",
                     svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   width="16"\n   height="16"\n   fill="none"\n   viewBox="0 0 16 16"\n   version="1.1"\n   id="svg2"\n   sodipodi:docname="settings-16.svg"\n   inkscape:version="1.3 (0e150ed, 2023-07-21)"\n   xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape"\n   xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd"\n   xmlns="http://www.w3.org/2000/svg"\n   xmlns:svg="http://www.w3.org/2000/svg">\n  <defs\n     id="defs2" />\n  <sodipodi:namedview\n     id="namedview2"\n     pagecolor="#505050"\n     bordercolor="#eeeeee"\n     borderopacity="1"\n     inkscape:showpageshadow="0"\n     inkscape:pageopacity="0"\n     inkscape:pagecheckerboard="0"\n     inkscape:deskcolor="#505050"\n     inkscape:zoom="34.875"\n     inkscape:cx="8"\n     inkscape:cy="7.9856631"\n     inkscape:window-width="1392"\n     inkscape:window-height="922"\n     inkscape:window-x="0"\n     inkscape:window-y="75"\n     inkscape:window-maximized="0"\n     inkscape:current-layer="svg2" />\n  <g\n     fill="currentColor"\n     fill-rule="evenodd"\n     clip-rule="evenodd"\n     id="g2">\n    <path\n       d="M8 5a3 3 0 100 6 3 3 0 000-6zM6.5 8a1.5 1.5 0 113 0 1.5 1.5 0 01-3 0z"\n       id="path1" />\n    <path\n       d="M7.5 0a1.75 1.75 0 00-1.75 1.75v.15c-.16.06-.318.125-.472.196l-.106-.106a1.75 1.75 0 00-2.475 0l-.707.707a1.75 1.75 0 000 2.475l.106.106a6.46 6.46 0 00-.196.472h-.15A1.75 1.75 0 000 7.5v1c0 .966.784 1.75 1.75 1.75h.15c.06.16.125.318.196.472l-.106.107a1.75 1.75 0 000 2.474l.707.708a1.75 1.75 0 002.475 0l.106-.107c.154.071.312.137.472.196v.15c0 .966.784 1.75 1.75 1.75h1a1.75 1.75 0 001.75-1.75v-.15c.16-.06.318-.125.472-.196l.106.107a1.75 1.75 0 002.475 0l.707-.707a1.75 1.75 0 000-2.475l-.106-.107c.071-.154.137-.311.196-.472h.15A1.75 1.75 0 0016 8.5v-1a1.75 1.75 0 00-1.75-1.75h-.15a6.455 6.455 0 00-.196-.472l.106-.106a1.75 1.75 0 000-2.475l-.707-.707a1.75 1.75 0 00-2.475 0l-.106.106a6.46 6.46 0 00-.472-.196v-.15A1.75 1.75 0 008.5 0h-1zm-.25 1.75a.25.25 0 01.25-.25h1a.25.25 0 01.25.25v.698c0 .339.227.636.555.724.42.113.817.28 1.186.492a.75.75 0 00.905-.12l.493-.494a.25.25 0 01.354 0l.707.708a.25.25 0 010 .353l-.494.494a.75.75 0 00-.12.904c.213.369.38.767.492 1.186a.75.75 0 00.724.555h.698a.25.25 0 01.25.25v1a.25.25 0 01-.25.25h-.698a.75.75 0 00-.724.555c-.113.42-.28.817-.492 1.186a.75.75 0 00.12.905l.494.493a.25.25 0 010 .354l-.707.707a.25.25 0 01-.354 0l-.494-.494a.75.75 0 00-.904-.12 4.966 4.966 0 01-1.186.492.75.75 0 00-.555.724v.698a.25.25 0 01-.25.25h-1a.25.25 0 01-.25-.25v-.698a.75.75 0 00-.555-.724 4.966 4.966 0 01-1.186-.491.75.75 0 00-.904.12l-.494.493a.25.25 0 01-.354 0l-.707-.707a.25.25 0 010-.354l.494-.493a.75.75 0 00.12-.905 4.966 4.966 0 01-.492-1.186.75.75 0 00-.724-.555H1.75a.25.25 0 01-.25-.25v-1a.25.25 0 01.25-.25h.698a.75.75 0 00.724-.555c.113-.42.28-.817.491-1.186a.75.75 0 00-.12-.904L3.05 4.11a.25.25 0 010-.353l.707-.708a.25.25 0 01.354 0l.493.494c.24.24.611.289.905.12a4.965 4.965 0 011.186-.492.75.75 0 00.555-.724V1.75z"\n       id="path2" />\n  </g>\n</svg>\n'
+                }),
+                k = new l.LabIcon({
+                    name: "amphi:postgres-icon",
+                    svgstr: '<?xml version="1.0"?>\r\n<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"\r\n  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">\r\n\r\n<svg width="432.071pt" height="445.383pt" viewBox="0 0 432.071 445.383" xml:space="preserve" xmlns="http://www.w3.org/2000/svg">\r\n<g id="orginal" style="fill-rule:nonzero;clip-rule:nonzero;stroke:#000000;stroke-miterlimit:4;">\r\n\t</g>\r\n<g id="Layer_x0020_3" style="fill-rule:nonzero;clip-rule:nonzero;fill:none;stroke:#FFFFFF;stroke-width:12.4651;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:4;">\r\n<path style="fill:#000000;stroke:#000000;stroke-width:37.3953;stroke-linecap:butt;stroke-linejoin:miter;" d="M323.205,324.227c2.833-23.601,1.984-27.062,19.563-23.239l4.463,0.392c13.517,0.615,31.199-2.174,41.587-7c22.362-10.376,35.622-27.7,13.572-23.148c-50.297,10.376-53.755-6.655-53.755-6.655c53.111-78.803,75.313-178.836,56.149-203.322    C352.514-5.534,262.036,26.049,260.522,26.869l-0.482,0.089c-9.938-2.062-21.06-3.294-33.554-3.496c-22.761-0.374-40.032,5.967-53.133,15.904c0,0-161.408-66.498-153.899,83.628c1.597,31.936,45.777,241.655,98.47,178.31    c19.259-23.163,37.871-42.748,37.871-42.748c9.242,6.14,20.307,9.272,31.912,8.147l0.897-0.765c-0.281,2.876-0.157,5.689,0.359,9.019c-13.572,15.167-9.584,17.83-36.723,23.416c-27.457,5.659-11.326,15.734-0.797,18.367c12.768,3.193,42.305,7.716,62.268-20.224    l-0.795,3.188c5.325,4.26,4.965,30.619,5.72,49.452c0.756,18.834,2.017,36.409,5.856,46.771c3.839,10.36,8.369,37.05,44.036,29.406c29.809-6.388,52.6-15.582,54.677-101.107"/>\r\n<path style="fill:#336791;stroke:none;" d="M402.395,271.23c-50.302,10.376-53.76-6.655-53.76-6.655c53.111-78.808,75.313-178.843,56.153-203.326c-52.27-66.785-142.752-35.2-144.262-34.38l-0.486,0.087c-9.938-2.063-21.06-3.292-33.56-3.496c-22.761-0.373-40.026,5.967-53.127,15.902    c0,0-161.411-66.495-153.904,83.63c1.597,31.938,45.776,241.657,98.471,178.312c19.26-23.163,37.869-42.748,37.869-42.748c9.243,6.14,20.308,9.272,31.908,8.147l0.901-0.765c-0.28,2.876-0.152,5.689,0.361,9.019c-13.575,15.167-9.586,17.83-36.723,23.416    c-27.459,5.659-11.328,15.734-0.796,18.367c12.768,3.193,42.307,7.716,62.266-20.224l-0.796,3.188c5.319,4.26,9.054,27.711,8.428,48.969c-0.626,21.259-1.044,35.854,3.147,47.254c4.191,11.4,8.368,37.05,44.042,29.406c29.809-6.388,45.256-22.942,47.405-50.555    c1.525-19.631,4.976-16.729,5.194-34.28l2.768-8.309c3.192-26.611,0.507-35.196,18.872-31.203l4.463,0.392c13.517,0.615,31.208-2.174,41.591-7c22.358-10.376,35.618-27.7,13.573-23.148z"/>\r\n<path d="M215.866,286.484c-1.385,49.516,0.348,99.377,5.193,111.495c4.848,12.118,15.223,35.688,50.9,28.045c29.806-6.39,40.651-18.756,45.357-46.051c3.466-20.082,10.148-75.854,11.005-87.281"/>\r\n<path d="M173.104,38.256c0,0-161.521-66.016-154.012,84.109c1.597,31.938,45.779,241.664,98.473,178.316c19.256-23.166,36.671-41.335,36.671-41.335"/>\r\n<path d="M260.349,26.207c-5.591,1.753,89.848-34.889,144.087,34.417c19.159,24.484-3.043,124.519-56.153,203.329"/>\r\n<path style="stroke-linejoin:bevel;" d="M348.282,263.953c0,0,3.461,17.036,53.764,6.653c22.04-4.552,8.776,12.774-13.577,23.155c-18.345,8.514-59.474,10.696-60.146-1.069c-1.729-30.355,21.647-21.133,19.96-28.739c-1.525-6.85-11.979-13.573-18.894-30.338    c-6.037-14.633-82.796-126.849,21.287-110.183c3.813-0.789-27.146-99.002-124.553-100.599c-97.385-1.597-94.19,119.762-94.19,119.762"/>\r\n<path d="M188.604,274.334c-13.577,15.166-9.584,17.829-36.723,23.417c-27.459,5.66-11.326,15.733-0.797,18.365c12.768,3.195,42.307,7.718,62.266-20.229c6.078-8.509-0.036-22.086-8.385-25.547c-4.034-1.671-9.428-3.765-16.361,3.994z"/>\r\n<path d="M187.715,274.069c-1.368-8.917,2.93-19.528,7.536-31.942c6.922-18.626,22.893-37.255,10.117-96.339c-9.523-44.029-73.396-9.163-73.436-3.193c-0.039,5.968,2.889,30.26-1.067,58.548c-5.162,36.913,23.488,68.132,56.479,64.938"/>\r\n<path style="fill:#FFFFFF;stroke-width:4.155;stroke-linecap:butt;stroke-linejoin:miter;" d="M172.517,141.7c-0.288,2.039,3.733,7.48,8.976,8.207c5.234,0.73,9.714-3.522,9.998-5.559c0.284-2.039-3.732-4.285-8.977-5.015c-5.237-0.731-9.719,0.333-9.996,2.367z"/>\r\n<path style="fill:#FFFFFF;stroke-width:2.0775;stroke-linecap:butt;stroke-linejoin:miter;" d="M331.941,137.543c0.284,2.039-3.732,7.48-8.976,8.207c-5.238,0.73-9.718-3.522-10.005-5.559c-0.277-2.039,3.74-4.285,8.979-5.015c5.239-0.73,9.718,0.333,10.002,2.368z"/>\r\n<path d="M350.676,123.432c0.863,15.994-3.445,26.888-3.988,43.914c-0.804,24.748,11.799,53.074-7.191,81.435"/>\r\n<path style="stroke-width:3;" d="M0,60.232"/>\r\n</g>\r\n</svg>'
                 });
-            var P, k, A, V, H, O, D, z, M, U, L, j, R, B, q, J, G, W, Q, K, Z, X, Y, ee, ne, te, oe, ae, se, re, le, de, ie, me;
-            class ce extends((0, o.PipelineComponent)()) {
+            var P, A, O, V, D, M, H, z, U, L, R, j, q, B, Q, G, J, W, Y, K, Z, X, ee, ne, te, oe, ae, se, re, le, de, ie, me, ce, pe, ue;
+            class ge extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "CSV File Input", this._id = "csvFileInput", this._type = "pandas_df_input", this._fileDrop = ["csv", "tsv"], this._category = "input", this._icon = d, this._default = {
                         csvOptions: {
                             sep: ","
                         }
                     }, this._form = {
                         idPrefix: "component__form",
@@ -213,44 +217,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: ce.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: ge.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: ce.Name,
-                        ConfigForm: ce.ConfigForm({
+                        name: ge.Name,
+                        ConfigForm: ge.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: ce.Icon,
+                        Icon: ge.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -264,15 +268,15 @@
                         ...e.csvOptions
                     };
                     "infer" === t.sep && (t.sep = "None", t.engine = "python"), "number" != typeof e.header && "None" !== e.header || (t.header = e.header), e.names && Array.isArray(e.names) && e.names.length > 0 && (t.names = `['${e.names.join("', '")}']`, t.header = 0);
                     let o = Object.entries(t).filter((([e, n]) => null !== n && "" !== n && !("sep" === e && "infer" === n))).map((([e, n]) => "header" !== e || "number" != typeof n && "None" !== n ? "names" === e ? `${e}=${n}` : "string" == typeof n && "None" !== n ? `${e}="${n}"` : `${e}=${n}` : `${e}=${n}`)).join(", ");
                     return `\n# Reading data from ${e.filePath}\n${n} = pd.read_csv("${e.filePath}"${o?`, ${o}`:""}).convert_dtypes()\n`
                 }
             }
-            P = ce, ce.ConfigForm = ({
+            P = ge, ge.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
@@ -308,15 +312,15 @@
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class pe extends((0, o.PipelineComponent)()) {
+            class he extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "JSON File Input", this._id = "jsonFileInput", this._type = "pandas_df_input", this._fileDrop = ["json", "jsonl"], this._category = "input", this._icon = d, this._default = {
                         jsonOptions: {}
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
@@ -379,44 +383,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: pe.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: he.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: pe.Name,
-                        ConfigForm: pe.ConfigForm({
+                        name: he.Name,
+                        ConfigForm: he.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: pe.Icon,
+                        Icon: he.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -427,25 +431,25 @@
                     outputName: n
                 }) {
                     let t = Object.entries(e.jsonOptions || {}).filter((([e, n]) => null !== n && "" !== n)).map((([e, n]) => `${e}="${n}"`)).join(", ");
                     const o = t ? `, ${t}` : "";
                     return `\n${n} = pd.read_json("${e.filePath}"${o}).convert_dtypes()\n`
                 }
             }
-            k = pe, pe.ConfigForm = ({
+            A = he, he.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = k.Default,
+                const c = A.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -460,26 +464,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: k.Type,
-                    name: k.Name,
-                    form: k.Form,
+                    type: A.Type,
+                    name: A.Name,
+                    form: A.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class ue extends((0, o.PipelineComponent)()) {
+            class fe extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Excel File Input", this._id = "excelfileInput", this._type = "pandas_df_input", this._category = "input", this._icon = d, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
@@ -549,44 +553,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: ue.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: fe.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: ue.Name,
-                        ConfigForm: ue.ConfigForm({
+                        name: fe.Name,
+                        ConfigForm: fe.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: ue.Icon,
+                        Icon: fe.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -596,25 +600,25 @@
                     config: e,
                     outputName: n
                 }) {
                     let t = e.excelOptions ? Object.entries(e.excelOptions).filter((([e, n]) => null !== n && "" !== n)).map((([e, n]) => `${e}='${n}'`)).join(", ") : null;
                     return t ? `${n} = pd.read_excel("${e.filePath}", ${t}).convert_dtypes()\n` : `${n} = pd.read_excel("${e.filePath}").convert_dtypes()\n`
                 }
             }
-            A = ue, ue.ConfigForm = ({
+            O = fe, fe.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = A.Default,
+                const c = O.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -629,26 +633,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: A.Type,
-                    name: A.Name,
-                    form: A.Form,
+                    type: O.Type,
+                    name: O.Name,
+                    form: O.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class ge extends((0, o.PipelineComponent)()) {
+            class ve extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "REST Input", this._id = "restInput", this._type = "pandas_df_input", this._category = "input.API", this._icon = c, this._default = {
                         method: "GET",
                         headers: []
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
@@ -714,44 +718,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: ge.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: ve.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: ge.Name,
-                        ConfigForm: ge.ConfigForm({
+                        name: ve.Name,
+                        ConfigForm: ve.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: ge.Icon,
+                        Icon: ve.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -768,15 +772,15 @@
                     let a = "";
                     a = e.jsonPath && "" !== e.jsonPath.trim() ? `jsonpath_expr = parse('${e.jsonPath}')\nselected_data = [match.value for match in jsonpath_expr.find(data)] if jsonpath_expr.find(data) else []\n${n} = pd.DataFrame(selected_data).convert_dtypes() if selected_data else pd.DataFrame()\n` : `${n} = pd.DataFrame([data]).convert_dtypes() if isinstance(data, dict) else pd.DataFrame(data).convert_dtypes()\n`;
                     const s = `${o}${t}`,
                         r = s.endsWith(", ") ? s.slice(0, -2) : s;
                     return `\nimport requests\nfrom jsonpath_ng import parse\nresponse = requests.request(\n  method="${e.method}",\n  url="${e.url}"${r?", "+r:""}\n)\ndata = response.json()\n${a}\n`
                 }
             }
-            V = ge, ge.ConfigForm = ({
+            V = ve, ve.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
@@ -812,15 +816,15 @@
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class he extends((0, o.PipelineComponent)()) {
+            class Ie extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Parquet File Input", this._id = "parquetFileInput", this._type = "pandas_df_input", this._category = "input", this._icon = d, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
@@ -850,44 +854,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: he.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Ie.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: he.Name,
-                        ConfigForm: he.ConfigForm({
+                        name: Ie.Name,
+                        ConfigForm: Ie.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: he.Icon,
+                        Icon: Ie.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -896,25 +900,25 @@
                 generateComponentCode({
                     config: e,
                     outputName: n
                 }) {
                     return `\n# Reading data from ${e.filePath}\n${n} = pd.read_parquet("${e.filePath}").convert_dtypes()\n`
                 }
             }
-            H = he, he.ConfigForm = ({
+            D = Ie, Ie.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = H.Default,
+                const c = D.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -929,26 +933,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: H.Type,
-                    name: H.Name,
-                    form: H.Form,
+                    type: D.Type,
+                    name: D.Name,
+                    form: D.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class fe extends((0, o.PipelineComponent)()) {
+            class Ce extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "XML File Input", this._id = "xmlFileInput", this._type = "pandas_df_input", this._fileDrop = ["xml"], this._category = "input", this._icon = d, this._default = {
                         xmlOptions: {
                             xpath: ""
                         }
                     }, this._form = {
                         idPrefix: "component__form",
@@ -987,44 +991,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: fe.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Ce.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: fe.Name,
-                        ConfigForm: fe.ConfigForm({
+                        name: Ce.Name,
+                        ConfigForm: Ce.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: fe.Icon,
+                        Icon: Ce.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -1036,25 +1040,25 @@
                 }) {
                     const t = `${n}_tree`,
                         o = `${n}_root`;
                     let a = e.xmlOptions.xpath ? `"${e.xmlOptions.xpath}"` : "'.'";
                     return `\n${t} = ET.parse("${e.filePath}")\n${o} = ${t}.getroot()\n${n} = ${o}.findall(${a})\n    `
                 }
             }
-            O = fe, fe.ConfigForm = ({
+            M = Ce, Ce.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = O.Default,
+                const c = M.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -1069,26 +1073,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: O.Type,
-                    name: O.Name,
-                    form: O.Form,
+                    type: M.Type,
+                    name: M.Name,
+                    form: M.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class ve extends((0, o.PipelineComponent)()) {
+            class be extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "G. Sheets Input", this._id = "googleSheetsInput", this._type = "pandas_df_input", this._category = "input", this._icon = x, this._default = {
                         sheetOptions: {
                             spreadsheetId: "",
                             range: "Sheet1"
                         }
                     }, this._form = {
@@ -1138,44 +1142,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: ve.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: be.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: ve.Name,
-                        ConfigForm: ve.ConfigForm({
+                        name: be.Name,
+                        ConfigForm: be.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: ve.Icon,
+                        Icon: be.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -1191,25 +1195,25 @@
                     const o = !!e.filePath && "" !== e.filePath.trim();
                     Object.entries(t).filter((([e, n]) => null !== n && "" !== n)).map((([e, n]) => `${e}="${n}"`)).join(", ");
                     const a = `${n}Client`,
                         s = `${n}Sheet`;
                     return `\n# Reading data from Google Sheets\n${o?`# Authentication with service account\nscope = ["https://spreadsheets.google.com/feeds","https://www.googleapis.com/auth/drive"]\ncreds = ServiceAccountCredentials.from_json_keyfile_name("${e.filePath}", scope)\n${a} = gspread.authorize(creds)\n`:`# Accessing public sheet without authentication\n${a} = gspread.service_account()\n`}\n# Open the spreadsheet\n${s} = ${a}.open_by_key(${t.spreadsheetId?`"${t.spreadsheetId}"`:"None"}).worksheet(${t.range?`"${t.range.split("!")[0]}"`:"None"})\n  \n# Convert to DataFrame\n${n} = pd.DataFrame(${s}.get_all_records())\n`
                 }
             }
-            D = ve, ve.ConfigForm = ({
+            H = be, be.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = D.Default,
+                const c = H.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -1224,26 +1228,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: D.Type,
-                    name: D.Name,
-                    form: D.Form,
+                    type: H.Type,
+                    name: H.Name,
+                    form: H.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Ce extends((0, o.PipelineComponent)()) {
+            class ye extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "MySQL Input", this._id = "mySQLInput", this._type = "pandas_df_input", this._category = "input", this._icon = w, this._default = {
                         dbOptions: {
                             host: "localhost",
                             port: "3306",
                             databaseName: "",
                             username: "",
@@ -1282,14 +1286,23 @@
                             inputType: "password",
                             advanced: !0
                         }, {
                             type: "input",
                             label: "Table Name",
                             id: "dbOptions.tableName",
                             placeholder: "Enter table name"
+                        }, {
+                            type: "codeTextarea",
+                            label: "SQL Query",
+                            height: "50px",
+                            mode: "sql",
+                            placeholder: "SELECT * FROM table_name",
+                            id: "dbOptions.sqlQuery",
+                            tooltip: "Optional. By default the SQL query is: SELECT * FROM table_name_provided. If specified, the SQL Query is used.",
+                            advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: n,
                     context: t,
@@ -1309,62 +1322,62 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Ce.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: ye.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Ce.Name,
-                        ConfigForm: Ce.ConfigForm({
+                        name: ye.Name,
+                        ConfigForm: ye.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Ce.Icon,
+                        Icon: ye.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd", "import sqlalchemy", "import pymysql"]
                 }
                 generateComponentCode({
                     config: e,
                     outputName: n
                 }) {
                     const t = `${n}_Engine`;
-                    return `\n# Connect to the MySQL database\n${t} = sqlalchemy.create_engine("mysql+pymysql://${e.dbOptions.username}:${e.dbOptions.password}@${e.dbOptions.host}:${e.dbOptions.port}/${e.dbOptions.databaseName}")\nwith ${t}.connect() as conn:\n  ${n} = pd.read_sql_table(\n    name="${e.dbOptions.tableName}",\n    con=conn.connection\n  ).convert_dtypes()\n`
+                    return `\n# Connect to the MySQL database\n${t} = sqlalchemy.create_engine("mysql+pymysql://${e.dbOptions.username}:${e.dbOptions.password}@${e.dbOptions.host}:${e.dbOptions.port}/${e.dbOptions.databaseName}")\nwith ${t}.connect() as conn:\n    ${n} = pd.read_sql(\n        "${e.dbOptions.sqlQuery&&e.dbOptions.sqlQuery.trim()?e.dbOptions.sqlQuery:`SELECT * FROM ${e.dbOptions.tableName}`}",\n        con=conn.connection\n    ).convert_dtypes()\n`
                 }
             }
-            z = Ce, Ce.ConfigForm = ({
+            z = ye, ye.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
@@ -1400,15 +1413,203 @@
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Ie extends((0, o.PipelineComponent)()) {
+            class _e extends((0, o.PipelineComponent)()) {
+                constructor() {
+                    super(...arguments), this._name = "Postgres Input", this._id = "postgresInput", this._type = "pandas_df_input", this._category = "input", this._icon = k, this._default = {
+                        dbOptions: {
+                            host: "localhost",
+                            port: "5432",
+                            databaseName: "",
+                            username: "",
+                            password: "",
+                            schema: "public",
+                            tableName: ""
+                        }
+                    }, this._form = {
+                        fields: [{
+                            type: "input",
+                            label: "Host",
+                            id: "dbOptions.host",
+                            placeholder: "Enter database host",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "Port",
+                            id: "dbOptions.port",
+                            placeholder: "Enter database port",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "Database Name",
+                            id: "dbOptions.databaseName",
+                            placeholder: "Enter database name"
+                        }, {
+                            type: "input",
+                            label: "Username",
+                            id: "dbOptions.username",
+                            placeholder: "Enter username",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "Password",
+                            id: "dbOptions.password",
+                            placeholder: "Enter password",
+                            inputType: "password",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "Schema",
+                            id: "dbOptions.schema",
+                            placeholder: "Enter schema name"
+                        }, {
+                            type: "input",
+                            label: "Table Name",
+                            id: "dbOptions.tableName",
+                            placeholder: "Enter table name"
+                        }, {
+                            type: "codeTextarea",
+                            label: "SQL Query",
+                            height: "50px",
+                            mode: "sql",
+                            placeholder: "SELECT * FROM table_name",
+                            id: "dbOptions.sqlQuery",
+                            tooltip: "Optional. By default the SQL query is: SELECT * FROM table_name_provided. If specified, the SQL Query is used.",
+                            advanced: !0
+                        }]
+                    }
+                }
+                UIComponent({
+                    id: e,
+                    data: n,
+                    context: t,
+                    componentService: l,
+                    manager: d,
+                    commands: i
+                }) {
+                    const {
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
+                            nodes: [{
+                                id: e
+                            }]
+                        })
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), I = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, C = s().createElement(o.renderHandle, {
+                        type: _e.Type,
+                        Handle: r.Handle,
+                        Position: r.Position,
+                        internals: I
+                    });
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
+                        id: e,
+                        data: n,
+                        context: t,
+                        manager: d,
+                        commands: i,
+                        name: _e.Name,
+                        ConfigForm: _e.ConfigForm({
+                            nodeId: e,
+                            data: n,
+                            context: t,
+                            componentService: l,
+                            manager: d,
+                            commands: i,
+                            store: u,
+                            setNodes: m
+                        }),
+                        Icon: _e.Icon,
+                        showContent: h,
+                        handle: C,
+                        deleteNode: g,
+                        setViewport: p
+                    }))
+                }
+                provideDependencies({
+                    config: e
+                }) {
+                    let n = [];
+                    return n.push("psycopg2-binary"), n
+                }
+                provideImports({
+                    config: e
+                }) {
+                    return ["import pandas as pd", "import sqlalchemy", "import psycopg2"]
+                }
+                generateComponentCode({
+                    config: e,
+                    outputName: n
+                }) {
+                    let t = `postgresql://${e.dbOptions.username}:${e.dbOptions.password}@${e.dbOptions.host}:${e.dbOptions.port}/${e.dbOptions.databaseName}`;
+                    const o = `${n}_Engine`,
+                        a = e.dbOptions.schema && "public" !== e.dbOptions.schema.toLowerCase() ? `${e.dbOptions.schema}.${e.dbOptions.tableName}` : e.dbOptions.tableName;
+                    return `\n# Connect to the PostgreSQL database\n${o} = sqlalchemy.create_engine("${t}")\nwith ${o}.connect() as conn:\n    ${n} = pd.read_sql(\n        "${e.dbOptions.sqlQuery&&e.dbOptions.sqlQuery.trim()?e.dbOptions.sqlQuery:`SELECT * FROM ${a}`}",\n        con=conn.connection\n    ).convert_dtypes()\n`
+                }
+            }
+            U = _e, _e.ConfigForm = ({
+                nodeId: e,
+                data: n,
+                context: t,
+                componentService: r,
+                manager: l,
+                commands: d,
+                store: i,
+                setNodes: m
+            }) => {
+                const c = U.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((n, t) => {
+                    (0, o.onChange)({
+                        evtTargetValue: n,
+                        field: t,
+                        nodeId: e,
+                        store: i,
+                        setNodes: m
+                    })
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
+                    nodeId: e,
+                    type: U.Type,
+                    name: U.Name,
+                    form: U.Form,
+                    data: n,
+                    context: t,
+                    componentService: r,
+                    manager: l,
+                    commands: d,
+                    handleChange: u
+                }))
+            };
+            class xe extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "HTML File Input", this._id = "htmlInput", this._type = "pandas_df_input", this._fileDrop = ["html", "htm"], this._category = "input", this._icon = d, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
@@ -1438,44 +1639,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Ie.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: xe.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Ie.Name,
-                        ConfigForm: Ie.ConfigForm({
+                        name: xe.Name,
+                        ConfigForm: xe.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Ie.Icon,
+                        Icon: xe.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -1486,25 +1687,25 @@
                     config: e,
                     outputName: n
                 }) {
                     let t = "";
                     return Object.entries(e.jsonOptions || {}).filter((([e, n]) => null !== n && "" !== n)).map((([e, n]) => `${e}='${n}'`)).join(", "), t += `\n# Retrieve raw HTML from ${e.filePath}\n${n}_elements = partition_html(filename="${e.filePath}")\n${n} = convert_to_dataframe(${n}_elements)\n`, t
                 }
             }
-            M = Ie, Ie.ConfigForm = ({
+            L = xe, xe.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = M.Default,
+                const c = L.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -1519,26 +1720,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: M.Type,
-                    name: M.Name,
-                    form: M.Form,
+                    type: L.Type,
+                    name: L.Name,
+                    form: L.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class be extends((0, o.PipelineComponent)()) {
+            class we extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "PDF File Input", this._id = "pdfInput", this._type = "pandas_df_input", this._fileDrop = ["pdf"], this._category = "input", this._icon = d, this._default = {
                         strategy: "fast"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
@@ -1578,44 +1779,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: be.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: we.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: be.Name,
-                        ConfigForm: be.ConfigForm({
+                        name: we.Name,
+                        ConfigForm: we.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: be.Icon,
+                        Icon: we.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideDependencies({
                     config: e
                 }) {
@@ -1632,25 +1833,25 @@
                     config: e,
                     outputName: n
                 }) {
                     let t = "";
                     return t += `\n# Read PDF and retrieve text from ${e.filePath}\n${n}_elements = partition_pdf(\n  filename="${e.filePath}",\n  strategy="${e.strategy}",\n  extract_images_in_pdf=False\n)\n${n} = convert_to_dataframe(${n}_elements)\n`, t
                 }
             }
-            U = be, be.ConfigForm = ({
+            R = we, we.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = U.Default,
+                const c = R.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -1665,26 +1866,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: U.Type,
-                    name: U.Name,
-                    form: U.Form,
+                    type: R.Type,
+                    name: R.Name,
+                    form: R.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class ye extends((0, o.PipelineComponent)()) {
+            class Ne extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Reddit Input", this._id = "redditInput", this._type = "pandas_df_input", this._category = "input.API", this._icon = S, this._default = {
                         submission: "all",
                         limit: 20,
                         sort: "hot",
                         userAgent: "Sumbission extraction by Amphi"
                     }, this._form = {
@@ -1741,44 +1942,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: ye.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Ne.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: ye.Name,
-                        ConfigForm: ye.ConfigForm({
+                        name: Ne.Name,
+                        ConfigForm: Ne.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: ye.Icon,
+                        Icon: Ne.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -1790,25 +1991,25 @@
                 }) {
                     const t = e.submission,
                         o = e.limit || 10,
                         a = t.startsWith("http") || t.startsWith("www") ? `${n}_submission = ${n}_reddit.submission(url="${t}")` : `${n}_submission = ${n}_reddit.submission("${t}")`;
                     return `\n${n}_reddit = praw.Reddit(client_id="${e.clientId}", client_secret="${e.secretId}", user_agent="${e.userAgent}")\n${a}\n\n${n}_comments_data = []\n${n}_submission.comments.replace_more(limit=${o})\nfor comment in ${n}_submission.comments.list():\n    ${n}_comments_data.append({\n        "comment_id": comment.id,\n        "comment_body": comment.body,\n        "comment_author": comment.author.name if comment.author else None,\n        "comment_score": comment.score,\n        "comment_created_utc": comment.created_utc,\n        "parent_id": comment.parent_id\n    })\n\n${n} = pd.DataFrame(${n}_comments_data)\n`
                 }
             }
-            L = ye, ye.ConfigForm = ({
+            j = Ne, Ne.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = L.Default,
+                const c = j.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -1823,26 +2024,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: L.Type,
-                    name: L.Name,
-                    form: L.Form,
+                    type: j.Type,
+                    name: j.Name,
+                    form: j.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class _e extends((0, o.PipelineComponent)()) {
+            class Se extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Drop Columns", this._id = "filterColumn", this._type = "pandas_df_processor", this._category = "transform", this._icon = $, this._default = {
                         columns: {
                             sourceData: [],
                             targetKeys: []
                         }
                     }, this._form = {
@@ -1875,44 +2076,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: _e.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Se.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: _e.Name,
-                        ConfigForm: _e.ConfigForm({
+                        name: Se.Name,
+                        ConfigForm: Se.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: _e.Icon,
+                        Icon: Se.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -1923,25 +2124,25 @@
                     inputName: n,
                     outputName: t
                 }) {
                     const o = e.columns.sourceData;
                     return `\n# Filter and order columns\n${t} = ${n}[[${e.columns.targetKeys.map((e=>{const n=o.find((n=>n.value===e));return n&&n.named?`"${e.trim()}"`:`${e.trim()}`})).join(", ")}]]\n`
                 }
             }
-            j = _e, _e.ConfigForm = ({
+            q = Se, Se.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = j.Default,
+                const c = q.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -1956,28 +2157,28 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: j.Type,
-                    name: j.Name,
-                    form: j.Form,
+                    type: q.Type,
+                    name: q.Name,
+                    form: q.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class xe extends((0, o.PipelineComponent)()) {
+            class $e extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Rename Columns", this._id = "rename", this._type = "pandas_df_processor", this._category = "transform", this._icon = I, this._default = {}, this._form = {
+                    super(...arguments), this._name = "Rename Columns", this._id = "rename", this._type = "pandas_df_processor", this._category = "transform", this._icon = C, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "keyvalueColumns",
                             label: "Columns",
                             id: "columns",
                             placeholders: {
                                 key: "column name",
@@ -2007,44 +2208,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: xe.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: $e.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: xe.Name,
-                        ConfigForm: xe.ConfigForm({
+                        name: $e.Name,
+                        ConfigForm: $e.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: xe.Icon,
+                        Icon: $e.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -2055,25 +2256,25 @@
                     inputName: n,
                     outputName: t
                 }) {
                     let o = "{";
                     return e.columns && e.columns.length > 0 ? (o += e.columns.map((e => e.key.named ? `"${e.key.value}": "${e.value}"` : `${e.key.value}: "${e.value}"`)).join(", "), o += "}") : o = "{}", `\n# Rename columns\n${t} = ${n}.rename(columns=${o})\n`
                 }
             }
-            R = xe, xe.ConfigForm = ({
+            B = $e, $e.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = R.Default,
+                const c = B.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -2088,26 +2289,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: R.Type,
-                    name: R.Name,
-                    form: R.Form,
+                    type: B.Type,
+                    name: B.Name,
+                    form: B.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class we extends((0, o.PipelineComponent)()) {
+            class Fe extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Filter Rows", this._id = "filter", this._type = "pandas_df_processor", this._category = "transform", this._icon = u, this._default = {
                         condition: "=="
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "column",
@@ -2137,34 +2338,34 @@
                             }, {
                                 value: "<=",
                                 label: "<="
                             }, {
                                 value: "notnull",
                                 label: "Not Null"
                             }, {
+                                value: "isnull",
+                                label: "Is Null"
+                            }, {
                                 value: "notempty",
                                 label: "Not Empty"
                             }, {
+                                value: "isempty",
+                                label: "Is Empty"
+                            }, {
                                 value: "contains",
                                 label: "Contains (string)"
                             }, {
                                 value: "not contains",
                                 label: "Not contains (string)"
                             }, {
                                 value: "startswith",
                                 label: "Starts With (string)"
                             }, {
                                 value: "endswith",
                                 label: "Ends With (string)"
-                            }, {
-                                value: "is NaN",
-                                label: "Is Not a Number (Leave value field empty)"
-                            }, {
-                                value: "is not N",
-                                label: "Is a Number (Leave value field empty)"
                             }]
                         }, {
                             type: "input",
                             label: "Value",
                             id: "conditionValue",
                             placeholder: "Any string of characters (enforce numbers if needed)"
                         }, {
@@ -2195,44 +2396,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: we.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Fe.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: we.Name,
-                        ConfigForm: we.ConfigForm({
+                        name: Fe.Name,
+                        ConfigForm: Fe.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: we.Icon,
+                        Icon: Fe.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -2241,73 +2442,77 @@
                 generateComponentCode({
                     config: e,
                     inputName: n,
                     outputName: t
                 }) {
                     const o = e.column.value,
                         a = e.column.type,
-                        s = (e.column.named, e.condition),
-                        r = e.conditionValue;
-                    let l;
+                        s = e.column.named,
+                        r = e.condition,
+                        l = e.conditionValue;
+                    let d;
                     switch (e.enforceString, a) {
                         case "string":
                         case "Object":
                         case "category":
-                            l = `${r.toString().replace(/"/g,'\\"')}`;
+                            d = `${l.toString().replace(/"/g,'\\"')}`;
                             break;
                         case "datetime64":
-                            l = `${new Date(r).toISOString()}`;
+                            d = `${new Date(l).toISOString()}`;
                             break;
                         case "bool":
-                            l = r.toString().toLowerCase();
+                            d = l.toString().toLowerCase();
                             break;
                         case "timedelta[ns]":
-                            l = `pd.to_timedelta(${r}, unit='ms')`;
+                            d = `pd.to_timedelta(${l}, unit='ms')`;
                             break;
                         case "period":
-                            l = `P${r.toString()}`;
+                            d = `P${l.toString()}`;
                             break;
                         default:
-                            l = isNaN(Number(r)) ? `'${r.toString()}'` : r.toString()
+                            d = isNaN(Number(l)) ? `'${l.toString()}'` : l.toString()
                     }
-                    let d, i = "\n# Filter rows based on condition\n";
-                    switch (s) {
+                    let i, m = "\n# Filter rows based on condition\n";
+                    const c = s ? `'${o}'` : o;
+                    switch (r) {
                         case "==":
                         case "!=":
                         default:
-                            d = `${o} ${s} '${l}'`, i += `${t} = ${n}.query("${d}")`;
+                            i = `${c} ${r} '${d}'`, m += `${t} = ${n}.query("${i}")`;
                             break;
                         case "contains":
                         case "not contains":
                             if (!["string", "Object", "category"].includes(a)) throw new Error("Invalid operation for the data type");
-                            d = `${"not contains"===s?"~":""}${n}[${n}['${o}'].str.contains("${l}", na=False)]`, i += `${t} = ${d}`;
+                            i = `${n}[${"not contains"===r?"~":""}${n}[${c}].str.contains("${d}", na=False)]`, m += `${t} = ${i}`;
                             break;
                         case "startswith":
                         case "endswith":
                             if (!["string", "Object", "category"].includes(a)) throw new Error("Invalid operation for the data type");
-                            d = `${n}[${n}['${o}'].str.${s}("${l.slice(1,-1)}", na=False)]`, i += `${t} = ${d}`;
+                            i = `${n}[${n}[${c}].str.${r}("${d.slice(1,-1)}", na=False)]`, m += `${t} = ${i}`;
                             break;
-                        case "isna":
-                        case "notna":
-                            d = `${n}[${n}['${o}'].${s}()]`, i += `${t} = ${d}`
+                        case "notnull":
+                            i = `${n}.dropna(subset=[${c}])`, m += `${t} = ${i}`;
+                            break;
+                        case "isnull":
+                            i = `${n}[${n}[${c}].isna()]`, m += `${t} = ${i}`
                     }
-                    return i
+                    return m
                 }
             }
-            B = we, we.ConfigForm = ({
+            Q = Fe, Fe.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = B.Default,
+                const c = Q.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -2322,26 +2527,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: B.Type,
-                    name: B.Name,
-                    form: B.Form,
+                    type: Q.Type,
+                    name: Q.Name,
+                    form: Q.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Ne extends((0, o.PipelineComponent)()) {
+            class Ee extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Aggregate", this._id = "aggregate", this._type = "pandas_df_processor", this._icon = g, this._category = "transform", this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "columns",
                             label: "Group by",
                             id: "groupByColumns",
@@ -2390,44 +2595,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Ne.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Ee.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Ne.Name,
-                        ConfigForm: Ne.ConfigForm({
+                        name: Ee.Name,
+                        ConfigForm: Ee.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Ne.Icon,
+                        Icon: Ee.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -2448,25 +2653,25 @@
                     }));
                     let s = `\n${t} = ${n}.groupby([`;
                     return o.forEach((e => {
                         s += `"${e}",`
                     })), s += `]).agg(${a}).reset_index()\n`, s
                 }
             }
-            q = Ne, Ne.ConfigForm = ({
+            G = Ee, Ee.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = q.Default,
+                const c = G.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -2481,26 +2686,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: q.Type,
-                    name: q.Name,
-                    form: q.Form,
+                    type: G.Type,
+                    name: G.Name,
+                    form: G.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Se extends((0, o.PipelineComponent)()) {
+            class Te extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Join Datasets", this._id = "join", this._type = "pandas_df_double_processor", this._category = "transform", this._icon = h, this._default = {
                         condition: "=="
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "column",
@@ -2556,44 +2761,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Se.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Te.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Se.Name,
-                        ConfigForm: Se.ConfigForm({
+                        name: Te.Name,
+                        ConfigForm: Te.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Se.Icon,
+                        Icon: Te.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -2613,15 +2818,15 @@
                         value: l,
                         type: d,
                         named: i
                     } = e.rightKeyColumn;
                     return `\n# Join ${n} and ${t}\n${o} = pd.merge(${n}, ${t}, left_on=${r?`"${a}"`:a}, right_on=${i?`"${l}"`:l}${e.how?`, how="${e.how}"`:""})\n`
                 }
             }
-            J = Se, Se.ConfigForm = ({
+            J = Te, Te.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
@@ -2657,15 +2862,15 @@
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class $e extends((0, o.PipelineComponent)()) {
+            class ke extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Type Converter", this._id = "typeConverter", this._type = "pandas_df_processor", this._category = "transform", this._icon = b, this._default = {
                         dataType: "string"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "column",
@@ -2788,44 +2993,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: $e.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: ke.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: $e.Name,
-                        ConfigForm: $e.ConfigForm({
+                        name: ke.Name,
+                        ConfigForm: ke.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: $e.Icon,
+                        Icon: ke.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -2841,33 +3046,28 @@
                         s = e.column.named,
                         r = e.dataType[e.dataType.length - 1];
                     let l = "\n\n# Initialize the output DataFrame\n";
                     return l += `${t} = ${n}.copy()\n`, l += `# Convert ${o} from ${a} to ${r}\n`, l += this.generateConversionCode(n, t, o, a, r, s), l
                 }
                 generateConversionCode(e, n, t, o, a, s) {
                     let r, l = "";
-                    if (a.startsWith("datetime")) a.includes("[") && (l = `, unit="${a.split("[")[1].split("]")[0]}"`), r = "pd.to_datetime";
-                    else {
-                        if (o.startsWith("float") && a.startsWith("int")) return r = `${e}["${t}"].astype("float").fillna(0).astype("${a}")`, s ? `${n}["${t}"] = ${r}\n` : `${n}.iloc[:, ${t}] = ${r}\n`;
-                        r = `astype("${a}")`
-                    }
-                    return s ? `${n}["${t}"] = ${e}["${t}"].${r}${l}\n` : `${n}.iloc[:, ${t}] = ${e}.iloc[:, ${t}].${r}${l}\n`
+                    return a.startsWith("datetime") ? (a.includes("[") && (l = `, unit="${a.split("[")[1].split("]")[0]}"`), r = `pd.to_datetime(${e}["${t}"]${l})`, s ? `${n}["${t}"] = ${r}\n` : `${n}.iloc[:, ${t}] = ${r}\n`) : o.startsWith("float") && a.startsWith("int") ? (r = `${e}["${t}"].astype("float").fillna(0).astype("${a}")`, s ? `${n}["${t}"] = ${r}\n` : `${n}.iloc[:, ${t}] = ${r}\n`) : (r = `astype("${a}")`, s ? `${n}["${t}"] = ${e}["${t}"].${r}\n` : `${n}.iloc[:, ${t}] = ${e}.iloc[:, ${t}].${r}\n`)
                 }
             }
-            G = $e, $e.ConfigForm = ({
+            W = ke, ke.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = G.Default,
+                const c = W.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -2882,26 +3082,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: G.Type,
-                    name: G.Name,
-                    form: G.Form,
+                    type: W.Type,
+                    name: W.Name,
+                    form: W.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Fe extends((0, o.PipelineComponent)()) {
+            class Pe extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Split Column", this._id = "splitColumn", this._type = "pandas_df_processor", this._category = "transform", this._icon = _, this._default = {
                         keepOriginalColumn: !1
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "column",
@@ -2957,44 +3157,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Fe.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Pe.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Fe.Name,
-                        ConfigForm: Fe.ConfigForm({
+                        name: Pe.Name,
+                        ConfigForm: Pe.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Fe.Icon,
+                        Icon: Pe.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -3009,25 +3209,25 @@
                         a = e.column.type,
                         s = `${t}_split`;
                     let r = "\n# Create a new DataFrame from the split operation\n";
                     const l = e.column.named ? `"${o}"` : o;
                     return "string" !== a && (r += `${n}[${l}] = ${n}[${l}].astype("string")\n`), r += `${s} = ${n}[${l}].str.split("${e.delimiter}", expand=True)\n`, r += `${s}.columns  = [f"${o}_{i}" for i in range(${s}.shape[1])]\n`, r += `${t} = pd.concat([${n}, ${s}], axis=1)\n`, e.keepOriginalColumn || (r += "\n# Remove the original column used for split\n", r += `${t}.drop(columns=[${l}], inplace=True)\n`), r
                 }
             }
-            W = Fe, Fe.ConfigForm = ({
+            Y = Pe, Pe.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = W.Default,
+                const c = Y.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -3042,26 +3242,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: W.Type,
-                    name: W.Name,
-                    form: W.Form,
+                    type: Y.Type,
+                    name: Y.Name,
+                    form: Y.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Ee extends((0, o.PipelineComponent)()) {
+            class Ae extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Extract", this._id = "extract", this._type = "pandas_df_processor", this._category = "transform", this._icon = y, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "column",
                             label: "Column name",
                             id: "column",
@@ -3148,44 +3348,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Ee.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Ae.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Ee.Name,
-                        ConfigForm: Ee.ConfigForm({
+                        name: Ae.Name,
+                        ConfigForm: Ae.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Ee.Icon,
+                        Icon: Ae.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -3205,25 +3405,25 @@
                         d = Array.from({
                             length: l
                         }, ((e, n) => `"${t}_${n+1}"`)).join(", "),
                         i = `${t}_extracted`;
                     return `\n# Extract data using regex\n${i} = ${n}[${a}].str.extract(r"${s}"${r})\n${i}.columns = [${d}]\n${t} = ${n}.join(${i}, rsuffix="_extracted")\n`
                 }
             }
-            Q = Ee, Ee.ConfigForm = ({
+            K = Ae, Ae.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = Q.Default,
+                const c = K.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -3238,28 +3438,28 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: Q.Type,
-                    name: Q.Name,
-                    form: Q.Form,
+                    type: K.Type,
+                    name: K.Name,
+                    form: K.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Te extends((0, o.PipelineComponent)()) {
+            class Oe extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Sort Rows", this._id = "sort", this._type = "pandas_df_processor", this._category = "transform", this._icon = C, this._default = {
+                    super(...arguments), this._name = "Sort Rows", this._id = "sort", this._type = "pandas_df_processor", this._category = "transform", this._icon = I, this._default = {
                         order: "True"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "columns",
                             label: "Columns",
                             id: "by",
@@ -3303,44 +3503,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Te.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Oe.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Te.Name,
-                        ConfigForm: Te.ConfigForm({
+                        name: Oe.Name,
+                        ConfigForm: Oe.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Te.Icon,
+                        Icon: Oe.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -3350,25 +3550,25 @@
                     config: e,
                     inputName: n,
                     outputName: t
                 }) {
                     return `\n# Sort rows \n${t} = ${n}.sort_values(by=[${e.by.map((e=>e.named?`"${e.value}"`:e.value)).join(", ")}]${void 0!==e.order?`, ascending=${e.order}`:""}${e.ignoreIndex?`, ignore_index=${e.ignoreIndex}`:""})\n`
                 }
             }
-            K = Te, Te.ConfigForm = ({
+            Z = Oe, Oe.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = K.Default,
+                const c = Z.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -3383,26 +3583,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: K.Type,
-                    name: K.Name,
-                    form: K.Form,
+                    type: Z.Type,
+                    name: Z.Name,
+                    form: Z.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Pe extends((0, o.PipelineComponent)()) {
+            class Ve extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Deduplicate", this._id = "deduplicateData", this._type = "pandas_df_processor", this._category = "transform", this._icon = v, this._default = {
                         keep: "first"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "select",
@@ -3447,44 +3647,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Pe.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Ve.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Pe.Name,
-                        ConfigForm: Pe.ConfigForm({
+                        name: Ve.Name,
+                        ConfigForm: Ve.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Pe.Icon,
+                        Icon: Ve.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -3497,25 +3697,25 @@
                 }) {
                     let o = "\n# Deduplicate rows\n";
                     const a = e.subset.length > 0 ? `subset=[${e.subset.map((e=>e.named?`"${e.value.trim()}"`:e.value)).join(", ")}]` : "",
                         s = "boolean" == typeof e.keep ? e.keep ? '"first"' : "" : `"${e.keep}"`;
                     return o += `${t} = ${n}.drop_duplicates(${a}${s?`, keep=${s}`:""})\n`, o
                 }
             }
-            Z = Pe, Pe.ConfigForm = ({
+            X = Ve, Ve.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = Z.Default,
+                const c = X.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -3530,26 +3730,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: Z.Type,
-                    name: Z.Name,
-                    form: Z.Form,
+                    type: X.Type,
+                    name: X.Name,
+                    form: X.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class ke extends((0, o.PipelineComponent)()) {
+            class De extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Expand JSON List", this._id = "expandList", this._type = "pandas_df_processor", this._category = "transform", this._icon = f, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "column",
                             label: "Column",
                             id: "column",
@@ -3577,44 +3777,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: ke.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: De.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: ke.Name,
-                        ConfigForm: ke.ConfigForm({
+                        name: De.Name,
+                        ConfigForm: De.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: ke.Icon,
+                        Icon: De.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -3625,25 +3825,25 @@
                     inputName: n,
                     outputName: t
                 }) {
                     let o = "# Expand the list in the specified column\n";
                     return o += "import pandas as pd\n", o += `${t} = ${n}["${e.column.value}"].apply(pd.Series)\n`, o
                 }
             }
-            X = ke, ke.ConfigForm = ({
+            ee = De, De.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = X.Default,
+                const c = ee.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -3658,26 +3858,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: X.Type,
-                    name: X.Name,
-                    form: X.Form,
+                    type: ee.Type,
+                    name: ee.Name,
+                    form: ee.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Ae extends((0, o.PipelineComponent)()) {
+            class Me extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Sample Datasets", this._id = "sample", this._type = "pandas_df_processor", this._category = "transform", this._icon = F, this._default = {
                         mode: "random"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "inputNumber",
@@ -3723,44 +3923,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Ae.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Me.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Ae.Name,
-                        ConfigForm: Ae.ConfigForm({
+                        name: Me.Name,
+                        ConfigForm: Me.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Ae.Icon,
+                        Icon: Me.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -3771,25 +3971,25 @@
                     inputName: n,
                     outputName: t
                 }) {
                     let o = "";
                     return "random" === e.mode ? o = `${t} = ${n}.sample(n=${e.rows})` : "tail" === e.mode ? o = `${t} = ${n}.tail(${e.rows})` : "head" === e.mode && (o = `${t} = ${n}.head(${e.rows})`), `\n${o}\n`
                 }
             }
-            Y = Ae, Ae.ConfigForm = ({
+            ne = Me, Me.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = Y.Default,
+                const c = ne.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -3804,26 +4004,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: Y.Type,
-                    name: Y.Name,
-                    form: Y.Form,
+                    type: ne.Type,
+                    name: ne.Name,
+                    form: ne.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Ve extends((0, o.PipelineComponent)()) {
+            class He extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "SQL Query", this._id = "sqlQuery", this._type = "pandas_df_processor", this._category = "transform", this._icon = N, this._default = {
                         query: "SELECT * FROM input_df1"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "codeTextarea",
@@ -3855,44 +4055,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Ve.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: He.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Ve.Name,
-                        ConfigForm: Ve.ConfigForm({
+                        name: He.Name,
+                        ConfigForm: He.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Ve.Icon,
+                        Icon: He.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -3902,25 +4102,25 @@
                     config: e,
                     inputName: n,
                     outputName: t
                 }) {
                     return `\n# Execute SQL Query using DuckDB\n${t} = duckdb.query("${e.query.replace("input_df1",n)}").to_df().convert_dtypes()\n\n`
                 }
             }
-            ee = Ve, Ve.ConfigForm = ({
+            te = He, He.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = ee.Default,
+                const c = te.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -3935,32 +4135,37 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: ee.Type,
-                    name: ee.Name,
-                    form: ee.Form,
+                    type: te.Type,
+                    name: te.Name,
+                    form: te.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class He extends((0, o.PipelineComponent)()) {
+            class ze extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Custom Code", this._id = "customTransformations", this._type = "pandas_df_processor", this._category = "transform", this._icon = p, this._default = {
                         code: "output = input"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
+                            type: "info",
+                            label: "Instructions",
+                            id: "instructions",
+                            text: "Write Python code with input as a dataframe input and output as the dataframe output."
+                        }, {
                             type: "codeTextarea",
                             label: "Imports",
                             id: "import",
                             placeholder: "import pandas as pd",
                             height: "50px",
                             advanced: !0
                         }, {
@@ -3994,44 +4199,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: He.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: ze.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: He.Name,
-                        ConfigForm: He.ConfigForm({
+                        name: ze.Name,
+                        ConfigForm: ze.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: He.Icon,
+                        Icon: ze.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports(e) {
                     return e.imports ? e.imports.split("\n").filter((e => e.startsWith("import "))) : []
                 }
@@ -4040,25 +4245,25 @@
                     inputName: n,
                     outputName: t
                 }) {
                     let o = `\n${e.code}`.replace(/input/g, n);
                     return o = o.replace(/output/g, t), o
                 }
             }
-            ne = He, He.ConfigForm = ({
+            oe = ze, ze.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = ne.Default,
+                const c = oe.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -4073,28 +4278,28 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: ne.Type,
-                    name: ne.Name,
-                    form: ne.Form,
+                    type: oe.Type,
+                    name: oe.Name,
+                    form: oe.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Oe extends((0, o.PipelineComponent)()) {
+            class Ue extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "OpenAI Prompt", this._id = "openAiLookup", this._type = "pandas_df_processor", this._category = "transform", this._icon = E, this._default = {
+                    super(...arguments), this._name = "OpenAI Prompt", this._id = "openAiLookup", this._type = "pandas_df_processor", this._category = "AI", this._icon = E, this._default = {
                         maxToken: 256,
                         temperature: .3,
                         model: "gpt-3.5-turbo",
                         systemPrompt: "You are part of a Python data pipeline using Pandas. Your task is to generate responses for each row of a DataFrame. Just provide the response as short as possible, don't write any sentence."
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
@@ -4175,44 +4380,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Oe.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Ue.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Oe.Name,
-                        ConfigForm: Oe.ConfigForm({
+                        name: Ue.Name,
+                        ConfigForm: Ue.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Oe.Icon,
+                        Icon: Ue.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -4229,25 +4434,25 @@
                     inputName: n,
                     outputName: t
                 }) {
                     const o = e.columns.map((e => e.value));
                     return `\n# Set the OpenAI API key for authentication\n${t}_client = OpenAI(\n  # This is the default and can be omitted\n  api_key="${e.token}"\n)\n\n# OpenAI request parameters\n${t}_user_prompt = "${e.prompt}"\n${t}_system_prompt = "${e.systemPrompt}"\n${t}_model = "${e.model}"  # Model to use for generating responses\n${t}_max_tokens = ${e.maxToken}  # Maximum number of tokens for the generated response\n${t}_temperature = ${e.temperature}  # Response variability based on the specified temperature\n\n# Apply the function to generate output for each row\n${n}['gpt_${t}'] = ${n}.apply(lambda row: generate_gpt_response(\n  row, \n  ["${o.join('", "')}"], \n  ${t}_client,\n  ${t}_user_prompt,\n  ${t}_system_prompt, \n  ${t}_model, \n  ${t}_max_tokens, \n  ${t}_temperature\n), axis=1)\n${t} = ${n}  # Set the modified DataFrame to the output variable\n`
                 }
             }
-            te = Oe, Oe.ConfigForm = ({
+            ae = Ue, Ue.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = te.Default,
+                const c = ae.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -4262,26 +4467,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: te.Type,
-                    name: te.Name,
-                    form: te.Form,
+                    type: ae.Type,
+                    name: ae.Name,
+                    form: ae.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class De extends((0, o.PipelineComponent)()) {
+            class Le extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "CSV File Output", this._id = "csvFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
                         csvOptions: {
                             sep: ","
                         }
                     }, this._form = {
                         idPrefix: "component__form",
@@ -4356,44 +4561,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: De.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Le.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: De.Name,
-                        ConfigForm: De.ConfigForm({
+                        name: Le.Name,
+                        ConfigForm: Le.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: De.Icon,
+                        Icon: Le.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -4403,25 +4608,25 @@
                     config: e,
                     inputName: n
                 }) {
                     let t = Object.entries(e.csvOptions).filter((([e, n]) => null !== n && "" !== n)).map((([e, n]) => `${e}='${n}'`)).join(", ");
                     return t = t ? `, ${t}` : "", `\n${n}.to_csv("${e.filePath}", index=False${t})\n`
                 }
             }
-            oe = De, De.ConfigForm = ({
+            se = Le, Le.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = oe.Default,
+                const c = se.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -4436,26 +4641,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: oe.Type,
-                    name: oe.Name,
-                    form: oe.Form,
+                    type: se.Type,
+                    name: se.Name,
+                    form: se.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class ze extends((0, o.PipelineComponent)()) {
+            class Re extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "JSON File Output", this._id = "jsonFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
                         jsonOptions: {
                             orient: "records"
                         }
                     }, this._form = {
                         idPrefix: "component__form",
@@ -4510,44 +4715,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: ze.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Re.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: ze.Name,
-                        ConfigForm: ze.ConfigForm({
+                        name: Re.Name,
+                        ConfigForm: Re.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: ze.Icon,
+                        Icon: Re.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -4558,25 +4763,25 @@
                     inputName: n
                 }) {
                     let t = Object.entries(e.jsonOptions || {}).filter((([e, n]) => null !== n && "" !== n)).map((([e, n]) => `${e}="${n}"`)).join(", ");
                     const o = t ? `, ${t}` : "";
                     return `\n${n}.to_json("${e.filePath}"${o})\n`
                 }
             }
-            ae = ze, ze.ConfigForm = ({
+            re = Re, Re.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = ae.Default,
+                const c = re.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -4591,26 +4796,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: ae.Type,
-                    name: ae.Name,
-                    form: ae.Form,
+                    type: re.Type,
+                    name: re.Name,
+                    form: re.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Me extends((0, o.PipelineComponent)()) {
+            class je extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Excel File Output", this._id = "excelFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
                         excelOptions: {}
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
@@ -4659,44 +4864,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Me.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: je.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Me.Name,
-                        ConfigForm: Me.ConfigForm({
+                        name: je.Name,
+                        ConfigForm: je.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Me.Icon,
+                        Icon: je.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideDependencies({
                     config: e
                 }) {
@@ -4719,25 +4924,25 @@
                     delete o.mode;
                     let a = Object.entries(o).filter((([e, n]) => null !== n && "" !== n)).map((([e, n]) => `${e}='${n}'`)).join(", ");
                     a = a ? `, ${a}` : "";
                     let s = "";
                     return s = t ? `with pd.ExcelWriter("${e.filePath}", mode="a") as writer:\n    ${n}.to_excel(writer, index=False${a})\n  ` : `\n${n}.to_excel("${e.filePath}", index=False${a})\n  `, s
                 }
             }
-            se = Me, Me.ConfigForm = ({
+            le = je, je.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = se.Default,
+                const c = le.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -4752,26 +4957,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: se.Type,
-                    name: se.Name,
-                    form: se.Form,
+                    type: le.Type,
+                    name: le.Name,
+                    form: le.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Ue extends((0, o.PipelineComponent)()) {
+            class qe extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Parquet File Output", this._id = "parquetFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
                         parquetOptions: {
                             compression: "snappy"
                         }
                     }, this._form = {
                         idPrefix: "component__form",
@@ -4823,44 +5028,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Ue.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: qe.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Ue.Name,
-                        ConfigForm: Ue.ConfigForm({
+                        name: qe.Name,
+                        ConfigForm: qe.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Ue.Icon,
+                        Icon: qe.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -4870,25 +5075,25 @@
                     config: e,
                     inputName: n
                 }) {
                     let t = Object.entries(e.parquetOptions || {}).filter((([e, n]) => null !== n && "" !== n)).map((([e, n]) => `${e}="${n}"`)).join(", ");
                     return t = t ? `, ${t}` : "", `\n${n}.to_parquet("${e.filePath}"${t})\n`
                 }
             }
-            re = Ue, Ue.ConfigForm = ({
+            de = qe, qe.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = re.Default,
+                const c = de.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -4903,26 +5108,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: re.Type,
-                    name: re.Name,
-                    form: re.Form,
+                    type: de.Type,
+                    name: de.Name,
+                    form: de.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Le extends((0, o.PipelineComponent)()) {
+            class Be extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "XML File Output", this._id = "xmlFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
@@ -4952,44 +5157,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Le.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Be.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Le.Name,
-                        ConfigForm: Le.ConfigForm({
+                        name: Be.Name,
+                        ConfigForm: Be.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Le.Icon,
+                        Icon: Be.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -5000,25 +5205,25 @@
                     inputName: n
                 }) {
                     const t = `${n}_xml_output`,
                         o = `${n}_file`;
                     return `\n# Output the XML content to a file\n${t} = ${n}.to_xml()\nwith open("${e.filePath}", "w") as ${o}:\n    ${o}.write(${t})\n`
                 }
             }
-            le = Le, Le.ConfigForm = ({
+            ie = Be, Be.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = le.Default,
+                const c = ie.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -5033,26 +5238,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: le.Type,
-                    name: le.Name,
-                    form: le.Form,
+                    type: ie.Type,
+                    name: ie.Name,
+                    form: ie.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class je extends((0, o.PipelineComponent)()) {
+            class Qe extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "G. Sheets Output", this._id = "googleSheetsOutput", this._type = "pandas_df_output", this._category = "output", this._icon = x, this._default = {
                         sheetOptions: {
                             spreadsheetId: "",
                             range: "Sheet1"
                         }
                     }, this._form = {
@@ -5101,44 +5306,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: je.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Qe.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: je.Name,
-                        ConfigForm: je.ConfigForm({
+                        name: Qe.Name,
+                        ConfigForm: Qe.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: je.Icon,
+                        Icon: Qe.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -5152,25 +5357,25 @@
                         ...e.sheetOptions
                     };
                     const o = `${n}Client`,
                         a = `${n}Sheet`;
                     return `\n# Outputting data to Google Sheets\nscope = ["https://spreadsheets.google.com/feeds","https://www.googleapis.com/auth/drive"]\ncreds = ServiceAccountCredentials.from_json_keyfile_name(${e.filePath?`"${e.filePath}"`:"None"}, scope)\n${o} = gspread.authorize(creds)\n\n# Open the spreadsheet and select the right worksheet\n${a} = ${o}.open_by_key(${t.spreadsheetId?`"${t.spreadsheetId}"`:"None"}).worksheet(${t.range?`"${t.range.split("!")[0]}"`:"None"})\n\n# Update the sheet with dataframe's data\n${a}.update([${n}.columns.values.tolist()] + ${n}.values.tolist())\n`
                 }
             }
-            de = je, je.ConfigForm = ({
+            me = Qe, Qe.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = de.Default,
+                const c = me.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -5185,26 +5390,26 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: de.Type,
-                    name: de.Name,
-                    form: de.Form,
+                    type: me.Type,
+                    name: me.Name,
+                    form: me.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Re extends((0, o.PipelineComponent)()) {
+            class Ge extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "MySQL Output", this._id = "mySQLOutput", this._type = "pandas_df_output", this._category = "output", this._icon = w, this._default = {
                         dbOptions: {
                             host: "localhost",
                             port: "3306",
                             databaseName: "",
                             tableName: "",
@@ -5272,19 +5477,21 @@
                             options: [{
                                 value: "insert",
                                 label: "INSERT"
                             }],
                             advanced: !0
                         }, {
                             type: "dataMapping",
+                            imports: ["pymysql"],
                             label: "Mapping",
                             id: "mapping",
                             tooltip: "By default the mapping is inferred from the input data. By specifying a schema you override the incoming schema.",
                             outputType: "relationalDatabase",
                             drivers: "mysql+pymysql",
+                            query: "DESCRIBE {{table}}",
                             typeOptions: [{
                                 value: "INT",
                                 label: "INT"
                             }, {
                                 value: "VARCHAR",
                                 label: "VARCHAR"
                             }, {
@@ -5357,44 +5564,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Re.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Ge.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Re.Name,
-                        ConfigForm: Re.ConfigForm({
+                        name: Ge.Name,
+                        ConfigForm: Ge.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Re.Icon,
+                        Icon: Ge.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -5415,28 +5622,28 @@
                     if (e.mapping && e.mapping.length > 0) {
                         const t = e.mapping.filter((e => e.input && (e.input.value || "number" == typeof e.input.value))).map((e => {
                             if (e.input.value != e.value) return e.input.named ? `"${e.input.value}": "${e.value}"` : `${e.input.value}: "${e.value}"`
                         })).filter((e => void 0 !== e));
                         t.length > 0 && (a = `\n# Rename columns based on the mapping\n${n} = ${n}.rename(columns={${t.join(", ")}})\n`), "" !== r && void 0 !== r && (s = `\n# Only keep relevant columns\n${n} = ${n}[[${r}]]\n`)
                     }
                     const l = "fail" === e.ifTableExists ? "fail" : "replace";
-                    return `\n# Connect to MySQL and output into table\n${o} = sqlalchemy.create_engine("${t}")\n${a}${s}\n${n}.to_sql(\n  name="${e.dbOptions.tableName}",\n  con=${o},\n  if_exists="${l}",\n  index=False\n)\n`
+                    return `\n# Connect to MySQL and output into table\n${o} = sqlalchemy.create_engine("${t}")\n${a}\n${s}\n${n}.to_sql(\n  name="${e.dbOptions.tableName}",\n  con=${o},\n  if_exists="${l}",\n  index=False\n)\n`
                 }
             }
-            ie = Re, Re.ConfigForm = ({
+            ce = Ge, Ge.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = ie.Default,
+                const c = ce.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -5451,26 +5658,349 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: ie.Type,
-                    name: ie.Name,
-                    form: ie.Form,
+                    type: ce.Type,
+                    name: ce.Name,
+                    form: ce.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            class Be extends((0, o.PipelineComponent)()) {
+            class Je extends((0, o.PipelineComponent)()) {
+                constructor() {
+                    super(...arguments), this._name = "Postgres Output", this._id = "postgresOutput", this._type = "pandas_df_output", this._category = "output", this._icon = k, this._default = {
+                        dbOptions: {
+                            host: "localhost",
+                            port: "5432",
+                            databaseName: "",
+                            schema: "public",
+                            tableName: "",
+                            username: "",
+                            password: ""
+                        },
+                        ifTableExists: "fail",
+                        mode: "insert"
+                    }, this._form = {
+                        idPrefix: "component__form",
+                        fields: [{
+                            type: "input",
+                            label: "Host",
+                            id: "dbOptions.host",
+                            placeholder: "Enter database host",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "Port",
+                            id: "dbOptions.port",
+                            placeholder: "Enter database port",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "Database Name",
+                            id: "dbOptions.databaseName",
+                            placeholder: "Enter database name"
+                        }, {
+                            type: "input",
+                            label: "Schema",
+                            id: "dbOptions.schema",
+                            placeholder: "Enter schema name"
+                        }, {
+                            type: "input",
+                            label: "Table Name",
+                            id: "dbOptions.tableName",
+                            placeholder: "Enter table name"
+                        }, {
+                            type: "input",
+                            label: "Username",
+                            id: "dbOptions.username",
+                            placeholder: "Enter username",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            inputType: "password",
+                            label: "Password",
+                            id: "dbOptions.password",
+                            placeholder: "Enter password",
+                            advanced: !0
+                        }, {
+                            type: "radio",
+                            label: "If Table Exists",
+                            id: "ifTableExists",
+                            options: [{
+                                value: "fail",
+                                label: "Fail"
+                            }, {
+                                value: "replace",
+                                label: "Replace"
+                            }, {
+                                value: "append",
+                                label: "Append"
+                            }],
+                            advanced: !0
+                        }, {
+                            type: "radio",
+                            label: "Mode",
+                            id: "mode",
+                            options: [{
+                                value: "insert",
+                                label: "INSERT"
+                            }],
+                            advanced: !0
+                        }, {
+                            type: "dataMapping",
+                            label: "Mapping",
+                            id: "mapping",
+                            tooltip: "By default the mapping is inferred from the input data. By specifying a schema you override the incoming schema.",
+                            outputType: "relationalDatabase",
+                            imports: ["psycopg2-binary"],
+                            drivers: "postgresql",
+                            query: '\nSELECT \n    column_name AS "Field",\n    data_type AS "Type",\n    is_nullable AS "Null",\n    column_default AS "Default",\n    CASE \n        WHEN character_maximum_length IS NOT NULL THEN character_maximum_length::text\n        ELSE \'\'\n    END AS "Extra"\nFROM \n    information_schema.columns\nWHERE \n    table_schema = \'{{schema}}\' AND\n    table_name = \'{{table}}\';',
+                            typeOptions: [{
+                                value: "SMALLINT",
+                                label: "SMALLINT"
+                            }, {
+                                value: "INTEGER",
+                                label: "INTEGER"
+                            }, {
+                                value: "BIGINT",
+                                label: "BIGINT"
+                            }, {
+                                value: "SERIAL",
+                                label: "SERIAL"
+                            }, {
+                                value: "BIGSERIAL",
+                                label: "BIGSERIAL"
+                            }, {
+                                value: "DECIMAL",
+                                label: "DECIMAL"
+                            }, {
+                                value: "NUMERIC",
+                                label: "NUMERIC"
+                            }, {
+                                value: "REAL",
+                                label: "REAL"
+                            }, {
+                                value: "DOUBLE PRECISION",
+                                label: "DOUBLE PRECISION"
+                            }, {
+                                value: "SMALLSERIAL",
+                                label: "SMALLSERIAL"
+                            }, {
+                                value: "MONEY",
+                                label: "MONEY"
+                            }, {
+                                value: "CHAR",
+                                label: "CHAR"
+                            }, {
+                                value: "VARCHAR",
+                                label: "VARCHAR"
+                            }, {
+                                value: "TEXT",
+                                label: "TEXT"
+                            }, {
+                                value: "BYTEA",
+                                label: "BYTEA"
+                            }, {
+                                value: "TIMESTAMP",
+                                label: "TIMESTAMP"
+                            }, {
+                                value: "DATE",
+                                label: "DATE"
+                            }, {
+                                value: "TIME",
+                                label: "TIME"
+                            }, {
+                                value: "INTERVAL",
+                                label: "INTERVAL"
+                            }, {
+                                value: "BOOLEAN",
+                                label: "BOOLEAN"
+                            }, {
+                                value: "UUID",
+                                label: "UUID"
+                            }, {
+                                value: "XML",
+                                label: "XML"
+                            }, {
+                                value: "JSON",
+                                label: "JSON"
+                            }, {
+                                value: "JSONB",
+                                label: "JSONB"
+                            }, {
+                                value: "ARRAY",
+                                label: "ARRAY"
+                            }, {
+                                value: "CIDR",
+                                label: "CIDR"
+                            }, {
+                                value: "INET",
+                                label: "INET"
+                            }, {
+                                value: "MACADDR",
+                                label: "MACADDR"
+                            }, {
+                                value: "BIT",
+                                label: "BIT"
+                            }, {
+                                value: "TSVECTOR",
+                                label: "TSVECTOR"
+                            }, {
+                                value: "TSQUERY",
+                                label: "TSQUERY"
+                            }],
+                            advanced: !0
+                        }]
+                    }
+                }
+                UIComponent({
+                    id: e,
+                    data: n,
+                    context: t,
+                    componentService: l,
+                    manager: d,
+                    commands: i
+                }) {
+                    const {
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
+                            nodes: [{
+                                id: e
+                            }]
+                        })
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), I = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, C = s().createElement(o.renderHandle, {
+                        type: Je.Type,
+                        Handle: r.Handle,
+                        Position: r.Position,
+                        internals: I
+                    });
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
+                        id: e,
+                        data: n,
+                        context: t,
+                        manager: d,
+                        commands: i,
+                        name: Je.Name,
+                        ConfigForm: Je.ConfigForm({
+                            nodeId: e,
+                            data: n,
+                            context: t,
+                            componentService: l,
+                            manager: d,
+                            commands: i,
+                            store: u,
+                            setNodes: m
+                        }),
+                        Icon: Je.Icon,
+                        showContent: h,
+                        handle: C,
+                        deleteNode: g,
+                        setViewport: p
+                    }))
+                }
+                provideDependencies({
+                    config: e
+                }) {
+                    let n = [];
+                    return n.push("psycopg2-binary"), n
+                }
+                provideImports({
+                    config: e
+                }) {
+                    return ["import pandas as pd", "import sqlalchemy", "import psycopg2"]
+                }
+                generateComponentCode({
+                    config: e,
+                    inputName: n
+                }) {
+                    const t = `postgresql://${e.dbOptions.username}:${e.dbOptions.password}@${e.dbOptions.host}:${e.dbOptions.port}/${e.dbOptions.databaseName}`,
+                        o = `${n}Engine`;
+                    let a = "",
+                        s = "";
+                    const r = e.mapping.filter((e => {
+                        var n, t;
+                        return null !== e.value && void 0 !== e.value && null !== (null === (n = e.input) || void 0 === n ? void 0 : n.value) && void 0 !== (null === (t = e.input) || void 0 === t ? void 0 : t.value)
+                    })).map((e => `"${e.value}"`)).join(", ");
+                    if (e.mapping && e.mapping.length > 0) {
+                        const t = e.mapping.filter((e => e.input && (e.input.value || "number" == typeof e.input.value))).map((e => {
+                            if (e.input.value != e.value) return e.input.named ? `"${e.input.value}": "${e.value}"` : `${e.input.value}: "${e.value}"`
+                        })).filter((e => void 0 !== e));
+                        t.length > 0 && (a = `\n# Rename columns based on the mapping\n${n} = ${n}.rename(columns={${t.join(", ")}})\n`), "" !== r && void 0 !== r && (s = `\n# Only keep relevant columns\n${n} = ${n}[[${r}]]\n`)
+                    }
+                    const l = "fail" === e.ifTableExists ? "fail" : "replace",
+                        d = e.dbOptions.schema && "public" !== e.dbOptions.schema.toLowerCase() ? `,\nschema="${e.dbOptions.schema}"` : "";
+                    return `\n# Connect to Postgres and output into table\n${o} = sqlalchemy.create_engine("${t}")\n${a}${s}\n${n}.to_sql(\n  name="${e.dbOptions.tableName}",\n  con=${o},\n  if_exists="${l}",\n  index=False${d}\n)\n`
+                }
+            }
+            pe = Je, Je.ConfigForm = ({
+                nodeId: e,
+                data: n,
+                context: t,
+                componentService: r,
+                manager: l,
+                commands: d,
+                store: i,
+                setNodes: m
+            }) => {
+                const c = pe.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((n, t) => {
+                    (0, o.onChange)({
+                        evtTargetValue: n,
+                        field: t,
+                        nodeId: e,
+                        store: i,
+                        setNodes: m
+                    })
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
+                    nodeId: e,
+                    type: pe.Type,
+                    name: pe.Name,
+                    form: pe.Form,
+                    data: n,
+                    context: t,
+                    componentService: r,
+                    manager: l,
+                    commands: d,
+                    handleChange: u
+                }))
+            };
+            class We extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Console", this._id = "console", this._type = "pandas_df_output", this._category = "output", this._icon = m, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "inputNumber",
                             label: "Records limit",
                             id: "limit",
@@ -5499,44 +6029,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: Be.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: We.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: Be.Name,
-                        ConfigForm: Be.ConfigForm({
+                        name: We.Name,
+                        ConfigForm: We.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: Be.Icon,
+                        Icon: We.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -5545,25 +6075,25 @@
                 generateComponentCode({
                     config: e,
                     inputName: n
                 }) {
                     return e.limit && (n += `.head(${e.limit})`), `\nprint(${n})\n`
                 }
             }
-            me = Be, Be.ConfigForm = ({
+            ue = We, We.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
                 setNodes: m
             }) => {
-                const c = me.Default,
+                const c = ue.Default,
                     p = (0, a.useCallback)((() => {
                         (0, o.setDefaultConfig)({
                             nodeId: e,
                             store: i,
                             setNodes: m,
                             defaultConfig: c
                         })
@@ -5578,28 +6108,28 @@
                         nodeId: e,
                         store: i,
                         setNodes: m
                     })
                 }), [e, i, m]);
                 return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: me.Type,
-                    name: me.Name,
-                    form: me.Form,
+                    type: ue.Type,
+                    name: ue.Name,
+                    form: ue.Form,
                     data: n,
                     context: t,
                     componentService: r,
                     manager: l,
                     commands: d,
                     handleChange: u
                 }))
             };
-            var qe, Je = t(4810),
-                Ge = t(3518);
-            class We extends((0, o.PipelineComponent)()) {
+            var Ye, Ke, Ze = t(4810),
+                Xe = t(3518);
+            class en extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Env. Variables", this._id = "envVariables", this._type = "env_variables", this._category = "other", this._icon = h, this._default = {}, this._form = {}
                 }
                 UIComponent({
                     id: e,
                     data: n,
                     context: t,
@@ -5619,44 +6149,44 @@
                         })
                     }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
                         nodeInternals: f,
                         edges: v
                     } = (0, r.useStore)((e => ({
                         nodeInternals: e.nodeInternals,
                         edges: e.edges
-                    }))), C = {
+                    }))), I = {
                         nodeInternals: f,
                         edges: v,
                         nodeId: e
-                    }, I = s().createElement(o.renderHandle, {
-                        type: We.Type,
+                    }, C = s().createElement(o.renderHandle, {
+                        type: en.Type,
                         Handle: r.Handle,
                         Position: r.Position,
-                        internals: C
+                        internals: I
                     });
                     return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: n,
                         context: t,
                         manager: d,
                         commands: i,
-                        name: We.Name,
-                        ConfigForm: We.ConfigForm({
+                        name: en.Name,
+                        ConfigForm: en.ConfigForm({
                             nodeId: e,
                             data: n,
                             context: t,
                             componentService: l,
                             manager: d,
                             commands: i,
                             store: u,
                             setNodes: m
                         }),
-                        Icon: We.Icon,
+                        Icon: en.Icon,
                         showContent: h,
-                        handle: I,
+                        handle: C,
                         deleteNode: g,
                         setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
@@ -5667,15 +6197,15 @@
                 }) {
                     let n = "";
                     return e.variables.forEach((e => {
                         e.value && (n += `os.environ["${e.name}"] = "${e.value}"\n`)
                     })), n += "\n", n
                 }
             }
-            qe = We, We.ConfigForm = ({
+            Ye = en, en.ConfigForm = ({
                 nodeId: e,
                 data: n,
                 context: t,
                 componentService: r,
                 manager: l,
                 commands: d,
                 store: i,
@@ -5699,22 +6229,22 @@
                     const n = [...u],
                         t = n.findIndex((n => e.key === n.key)),
                         o = n[t];
                     n.splice(t, 1, {
                         ...o,
                         ...e
                     }), g(n)
-                }, C = {
+                }, I = {
                     body: {
                         row: ({
                             index: e,
                             ...n
                         }) => {
-                            const [t] = Je.Form.useForm();
-                            return s().createElement(Je.Form, {
+                            const [t] = Ze.Form.useForm();
+                            return s().createElement(Ze.Form, {
                                 form: t,
                                 component: !1
                             }, s().createElement(p.Provider, {
                                 value: t
                             }, s().createElement("tr", {
                                 ...n
                             })))
@@ -5747,24 +6277,24 @@
                                             ...e
                                         })
                                     } catch (e) {
                                         console.log("Save failed:", e)
                                     }
                                 };
                             let v = t;
-                            return n && (v = m ? s().createElement(Je.Form.Item, {
+                            return n && (v = m ? s().createElement(Ze.Form.Item, {
                                 style: {
                                     margin: 0
                                 },
                                 name: o,
                                 rules: d ? [{
                                     required: !0,
                                     message: `${e} is required.`
                                 }] : []
-                            }, s().createElement(Je.Input, {
+                            }, s().createElement(Ze.Input, {
                                 ref: u,
                                 onPressEnter: f,
                                 onBlur: f,
                                 onKeyDown: e => e.stopPropagation(),
                                 autoComplete: "off"
                             })) : s().createElement("div", {
                                 className: "editable-cell-value-wrap",
@@ -5778,15 +6308,15 @@
                             }, t)), s().createElement("td", {
                                 ...i
                             }, s().createElement("div", {
                                 onDoubleClick: e => e.stopPropagation()
                             }, v))
                         }
                     }
-                }, I = [{
+                }, C = [{
                     title: "Name",
                     dataIndex: "name",
                     width: "30%",
                     editable: !0,
                     required: !0
                 }, {
                     title: "Value",
@@ -5799,87 +6329,236 @@
                     dataIndex: "default",
                     width: "30%",
                     editable: !0,
                     required: !1
                 }, {
                     title: "",
                     dataIndex: "operation",
-                    render: (e, n) => u.length >= 1 ? s().createElement(Je.Popconfirm, {
+                    render: (e, n) => u.length >= 1 ? s().createElement(Ze.Popconfirm, {
                         title: "Sure to delete?",
                         onConfirm: () => (e => {
                             const n = u.filter((n => n.key !== e));
                             g(n)
                         })(n.key)
-                    }, s().createElement(Ge.A, null)) : null
+                    }, s().createElement(Xe.A, null)) : null
                 }].map((e => e.editable ? {
                     ...e,
                     onCell: n => ({
                         record: n,
                         editable: e.editable,
                         dataIndex: e.dataIndex,
                         title: e.title,
                         required: e.required,
                         handleSave: v
                     })
-                } : e)), [b, y] = (0, a.useState)(!1);
-                return s().createElement(s().Fragment, null, s().createElement(Je.ConfigProvider, {
+                } : e)), [b, y] = (0, a.useState)(!1), {
+                    Paragraph: _,
+                    Text: x
+                } = Ze.Typography, w = s().createElement("span", null, "Specify Environment Variables and select them in components' inputs by typing ", s().createElement(x, {
+                    keyboard: !0
+                }, "{ "));
+                return s().createElement(s().Fragment, null, s().createElement(Ze.ConfigProvider, {
                     theme: {
                         token: {
                             colorPrimary: "#5F9B97"
                         }
                     }
-                }, s().createElement(Je.Form, {
+                }, s().createElement(Ze.Form, {
                     layout: "vertical",
                     size: "small"
                 }, s().createElement("div", {
                     className: "flex justify-center mt-1 pt-1.5 space-x-4"
-                }, s().createElement("span", {
+                }, s().createElement(Ze.Space, {
+                    direction: "vertical",
+                    size: "middle"
+                }, s().createElement(Ze.Space.Compact, null, s().createElement(_, {
+                    style: {
+                        padding: "5px"
+                    }
+                }, w)), s().createElement(Ze.Space.Compact, null, s().createElement("span", {
                     onClick: () => y(!0),
                     className: "inline-flex items-center justify-center cursor-pointer group"
                 }, s().createElement(T.react, {
                     className: "h-3 w-3 group-hover:text-primary"
-                }))), s().createElement(Je.Modal, {
-                    title: qe.Name,
+                }))))), s().createElement(Ze.Modal, {
+                    title: Ye.Name,
                     centered: !0,
                     open: b,
                     onOk: () => y(!1),
                     onCancel: () => y(!1),
                     width: 800,
                     footer: (e, {
                         OkBtn: n
                     }) => s().createElement(s().Fragment, null, s().createElement(n, null))
-                }, s().createElement(Je.Form, {
+                }, s().createElement(Ze.Form, {
                     layout: "vertical"
-                }, s().createElement("div", null, s().createElement(Je.Button, {
+                }, s().createElement("div", null, s().createElement(_, {
+                    style: {
+                        padding: "5px"
+                    }
+                }, w), s().createElement(Ze.Button, {
                     onClick: () => {
                         const e = {
                             key: h,
                             name: `ENV_${h}`,
                             value: "",
                             default: ""
                         };
                         g([...u, e]), f(h + 1)
                     },
                     type: "primary",
                     style: {
                         marginBottom: 16
                     }
-                }, "Add environment variable"), s().createElement(Je.Table, {
-                    components: C,
+                }, "Add environment variable"), s().createElement(Ze.Table, {
+                    components: I,
                     rowClassName: () => "editable-row",
                     bordered: !0,
                     dataSource: u,
-                    columns: I
+                    columns: C
                 })))))))
             };
-            const Qe = {
+            class nn extends((0, o.PipelineComponent)()) {
+                constructor() {
+                    super(...arguments), this._name = "Env. File", this._id = "envFile", this._type = "env_file", this._category = "other", this._icon = h, this._default = {
+                        filePath: ".env"
+                    }, this._form = {
+                        idPrefix: "component__form",
+                        fields: [{
+                            type: "info",
+                            label: "Instructions",
+                            id: "instructions",
+                            text: "Import an environment file and use the environment variable in components by typing {."
+                        }, {
+                            type: "file",
+                            label: "Environment File",
+                            id: "filePath",
+                            placeholder: ".env"
+                        }]
+                    }
+                }
+                UIComponent({
+                    id: e,
+                    data: n,
+                    context: t,
+                    componentService: l,
+                    manager: d,
+                    commands: i
+                }) {
+                    const {
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
+                            nodes: [{
+                                id: e
+                            }]
+                        })
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), I = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, C = s().createElement(o.renderHandle, {
+                        type: nn.Type,
+                        Handle: r.Handle,
+                        Position: r.Position,
+                        internals: I
+                    });
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
+                        id: e,
+                        data: n,
+                        context: t,
+                        manager: d,
+                        commands: i,
+                        name: nn.Name,
+                        ConfigForm: nn.ConfigForm({
+                            nodeId: e,
+                            data: n,
+                            context: t,
+                            componentService: l,
+                            manager: d,
+                            commands: i,
+                            store: u,
+                            setNodes: m
+                        }),
+                        Icon: nn.Icon,
+                        showContent: h,
+                        handle: C,
+                        deleteNode: g,
+                        setViewport: p
+                    }))
+                }
+                provideImports({
+                    config: e
+                }) {
+                    return ["from python-dotenv import load_dotenv"]
+                }
+                generateComponentCode({
+                    config: e
+                }) {
+                    let n = `\n# Load environment variables from ${e.filePath}\nload_dotenv(dotenv_path="${e.filePath}")\n`;
+                    return n += "\n", n
+                }
+            }
+            Ke = nn, nn.ConfigForm = ({
+                nodeId: e,
+                data: n,
+                context: t,
+                componentService: r,
+                manager: l,
+                commands: d,
+                store: i,
+                setNodes: m
+            }) => {
+                const c = Ke.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((n, t) => {
+                    (0, o.onChange)({
+                        evtTargetValue: n,
+                        field: t,
+                        nodeId: e,
+                        store: i,
+                        setNodes: m
+                    })
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
+                    nodeId: e,
+                    type: Ke.Type,
+                    name: Ke.Name,
+                    form: Ke.Form,
+                    data: n,
+                    context: t,
+                    componentService: r,
+                    manager: l,
+                    commands: d,
+                    handleChange: u
+                }))
+            };
+            const tn = {
                 id: "@amphi/pipeline-components-core",
                 description: "Adds a step counter/button (1 of 3 related examples). This extension holds the UI/interface",
                 autoStart: !0,
                 requires: [o.ComponentManager],
                 activate: (e, n) => {
-                    console.log("JupyterLab extension pipeline-components-core is activated!"), n.addComponent(ce.getInstance()), n.addComponent(pe.getInstance()), n.addComponent(ue.getInstance()), n.addComponent(ge.getInstance()), n.addComponent(he.getInstance()), n.addComponent(fe.getInstance()), n.addComponent(ve.getInstance()), n.addComponent(Ce.getInstance()), n.addComponent(Ie.getInstance()), n.addComponent(be.getInstance()), n.addComponent(ye.getInstance()), n.addComponent(_e.getInstance()), n.addComponent(xe.getInstance()), n.addComponent(we.getInstance()), n.addComponent(Ne.getInstance()), n.addComponent(Se.getInstance()), n.addComponent($e.getInstance()), n.addComponent(Fe.getInstance()), n.addComponent(Ee.getInstance()), n.addComponent(Te.getInstance()), n.addComponent(Pe.getInstance()), n.addComponent(ke.getInstance()), n.addComponent(Ae.getInstance()), n.addComponent(Ve.getInstance()), n.addComponent(He.getInstance()), n.addComponent(Oe.getInstance()), n.addComponent(De.getInstance()), n.addComponent(ze.getInstance()), n.addComponent(Me.getInstance()), n.addComponent(Ue.getInstance()), n.addComponent(Le.getInstance()), n.addComponent(je.getInstance()), n.addComponent(Re.getInstance()), n.addComponent(Be.getInstance()), n.addComponent(We.getInstance())
+                    console.log("JupyterLab extension pipeline-components-core is activated!"), n.addComponent(ge.getInstance()), n.addComponent(he.getInstance()), n.addComponent(fe.getInstance()), n.addComponent(ve.getInstance()), n.addComponent(Ie.getInstance()), n.addComponent(Ce.getInstance()), n.addComponent(be.getInstance()), n.addComponent(ye.getInstance()), n.addComponent(_e.getInstance()), n.addComponent(xe.getInstance()), n.addComponent(we.getInstance()), n.addComponent(Ne.getInstance()), n.addComponent(Se.getInstance()), n.addComponent($e.getInstance()), n.addComponent(Fe.getInstance()), n.addComponent(Ee.getInstance()), n.addComponent(Te.getInstance()), n.addComponent(ke.getInstance()), n.addComponent(Pe.getInstance()), n.addComponent(Ae.getInstance()), n.addComponent(Oe.getInstance()), n.addComponent(Ve.getInstance()), n.addComponent(De.getInstance()), n.addComponent(Me.getInstance()), n.addComponent(He.getInstance()), n.addComponent(ze.getInstance()), n.addComponent(Ue.getInstance()), n.addComponent(Le.getInstance()), n.addComponent(Re.getInstance()), n.addComponent(je.getInstance()), n.addComponent(qe.getInstance()), n.addComponent(Be.getInstance()), n.addComponent(Qe.getInstance()), n.addComponent(Ge.getInstance()), n.addComponent(Je.getInstance()), n.addComponent(We.getInstance()), n.addComponent(en.getInstance()), n.addComponent(nn.getInstance())
                 }
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/687.82f4edc6966c97595e01.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/687.e44561a1742c6083cba0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 687.82f4edc6966c97595e01.js.LICENSE.txt */
+/*! For license information please see 687.e44561a1742c6083cba0.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_components_core = self.webpackChunk_amphi_pipeline_components_core || []).push([
     [687], {
         7687: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 Affix: () => Ko,
                 Alert: () => $i,
@@ -98,15 +98,18 @@
                 m = n.n(f);
 
             function g(e) {
                 return e instanceof HTMLElement || e instanceof SVGElement
             }
 
             function h(e) {
-                return e && "object" === (0, p.A)(e) && g(e.nativeElement) ? e.nativeElement : g(e) ? e : e instanceof r().Component ? m().findDOMNode(e) : null
+                var t, n = function(e) {
+                    return e && "object" === (0, p.A)(e) && g(e.nativeElement) ? e.nativeElement : g(e) ? e : null
+                }(e);
+                return n || (e instanceof r().Component ? null === (t = m().findDOMNode) || void 0 === t ? void 0 : t.call(m(), e) : null)
             }
 
             function v(e, t, n) {
                 var r = o.useRef({});
                 return "value" in r.current && !n(r.current.condition, t) || (r.current.value = e(), r.current.condition = t), r.current.value
             }
             var b = function(e, t) {
@@ -15037,51 +15040,52 @@
                     }), [H.id, H.maps]),
                     F = D && v && (Math.max(s * v.length, L) > c || !!$),
                     W = "rtl" === x,
                     _ = a()(r, (0, Ee.A)({}, "".concat(r, "-rtl"), W), i),
                     V = v || Om,
                     K = (0, o.useRef)(),
                     X = (0, o.useRef)(),
-                    q = (0, o.useState)(0),
-                    G = (0, ke.A)(q, 2),
-                    Y = G[0],
-                    U = G[1],
-                    Q = (0, o.useState)(0),
-                    Z = (0, ke.A)(Q, 2),
-                    J = Z[0],
-                    ee = Z[1],
-                    te = (0, o.useState)(!1),
-                    ne = (0, ke.A)(te, 2),
-                    oe = ne[0],
-                    re = ne[1],
-                    ie = function() {
-                        re(!0)
-                    },
+                    q = (0, o.useRef)(),
+                    G = (0, o.useState)(0),
+                    Y = (0, ke.A)(G, 2),
+                    U = Y[0],
+                    Q = Y[1],
+                    Z = (0, o.useState)(0),
+                    J = (0, ke.A)(Z, 2),
+                    ee = J[0],
+                    te = J[1],
+                    ne = (0, o.useState)(!1),
+                    oe = (0, ke.A)(ne, 2),
+                    re = oe[0],
+                    ie = oe[1],
                     ae = function() {
-                        re(!1)
+                        ie(!0)
+                    },
+                    le = function() {
+                        ie(!1)
                     },
-                    le = {
+                    se = {
                         getKey: j
                     };
 
-                function se(e) {
-                    U((function(t) {
+                function ue(e) {
+                    Q((function(t) {
                         var n = function(e) {
                             var t = e;
-                            return Number.isNaN(Me.current) || (t = Math.min(t, Me.current)), t = Math.max(t, 0)
+                            return Number.isNaN(je.current) || (t = Math.min(t, je.current)), t = Math.max(t, 0)
                         }("function" == typeof e ? e(t) : e);
                         return K.current.scrollTop = n, n
                     }))
                 }
-                var ue = (0, o.useRef)({
+                var de = (0, o.useRef)({
                         start: 0,
                         end: V.length
                     }),
-                    de = (0, o.useRef)(),
-                    pe = function(e, t, n) {
+                    pe = (0, o.useRef)(),
+                    fe = function(e, t, n) {
                         var r = o.useState(e),
                             i = (0, ke.A)(r, 2),
                             a = i[0],
                             l = i[1],
                             c = o.useState(null),
                             s = (0, ke.A)(c, 2),
                             u = s[0],
@@ -15110,17 +15114,17 @@
                                     index: s,
                                     multiple: u
                                 }
                             }(a || [], e || [], t);
                             void 0 !== (null == o ? void 0 : o.index) && (null == n || n(o.index), d(e[o.index])), l(e)
                         }), [e]), [u]
                     }(V, j),
-                    fe = (0, ke.A)(pe, 1)[0];
-                de.current = fe;
-                var me = o.useMemo((function() {
+                    me = (0, ke.A)(fe, 1)[0];
+                pe.current = me;
+                var ge = o.useMemo((function() {
                         if (!D) return {
                             scrollHeight: void 0,
                             start: 0,
                             end: V.length - 1,
                             offset: void 0
                         };
                         var e;
@@ -15131,84 +15135,84 @@
                             offset: void 0
                         };
                         for (var t, n, o, r = 0, i = V.length, a = 0; a < i; a += 1) {
                             var l = V[a],
                                 u = j(l),
                                 d = H.get(u),
                                 p = r + (void 0 === d ? s : d);
-                            p >= Y && void 0 === t && (t = a, n = r), p > Y + c && void 0 === o && (o = a), r = p
+                            p >= U && void 0 === t && (t = a, n = r), p > U + c && void 0 === o && (o = a), r = p
                         }
                         return void 0 === t && (t = 0, n = 0, o = Math.ceil(c / s)), void 0 === o && (o = V.length - 1), {
                             scrollHeight: r,
                             start: t,
                             end: o = Math.min(o + 1, V.length - 1),
                             offset: n
                         }
-                    }), [F, D, Y, V, B, c]),
-                    ge = me.scrollHeight,
-                    he = me.start,
-                    ve = me.end,
-                    be = me.offset;
-                ue.current.start = he, ue.current.end = ve;
-                var ye = o.useState({
+                    }), [F, D, U, V, B, c]),
+                    he = ge.scrollHeight,
+                    ve = ge.start,
+                    be = ge.end,
+                    ye = ge.offset;
+                de.current.start = ve, de.current.end = be;
+                var xe = o.useState({
                         width: 0,
                         height: c
                     }),
-                    xe = (0, ke.A)(ye, 2),
-                    $e = xe[0],
-                    we = xe[1],
-                    Se = (0, o.useRef)(),
+                    $e = (0, ke.A)(xe, 2),
+                    we = $e[0],
+                    Se = $e[1],
                     Oe = (0, o.useRef)(),
-                    Ae = o.useMemo((function() {
-                        return Em($e.width, $)
-                    }), [$e.width, $]),
+                    Ae = (0, o.useRef)(),
                     Ie = o.useMemo((function() {
-                        return Em($e.height, ge)
-                    }), [$e.height, ge]),
-                    Ne = ge - c,
-                    Me = (0, o.useRef)(Ne);
-                Me.current = Ne;
-                var je = Y <= 0,
-                    Pe = Y >= Ne,
-                    Re = bm(je, Pe),
-                    ze = function() {
+                        return Em(we.width, $)
+                    }), [we.width, $]),
+                    Ne = o.useMemo((function() {
+                        return Em(we.height, he)
+                    }), [we.height, he]),
+                    Me = he - c,
+                    je = (0, o.useRef)(Me);
+                je.current = Me;
+                var Pe = U <= 0,
+                    Re = U >= Me,
+                    ze = bm(Pe, Re),
+                    Te = function() {
                         return {
-                            x: W ? -J : J,
-                            y: Y
+                            x: W ? -ee : ee,
+                            y: U
                         }
                     },
-                    Te = (0, o.useRef)(ze()),
-                    He = wn((function(e) {
+                    He = (0, o.useRef)(Te()),
+                    Be = wn((function(e) {
                         if (k) {
-                            var t = (0, d.A)((0, d.A)({}, ze()), e);
-                            Te.current.x === t.x && Te.current.y === t.y || (k(t), Te.current = t)
+                            var t = (0, d.A)((0, d.A)({}, Te()), e);
+                            He.current.x === t.x && He.current.y === t.y || (k(t), He.current = t)
                         }
                     }));
 
-                function Be(e, t) {
+                function De(e, t) {
                     var n = e;
                     t ? ((0, f.flushSync)((function() {
-                        ee(n)
-                    })), He()) : se(n)
+                        te(n)
+                    })), Be()) : ue(n)
                 }
-                var De = function(e) {
+                var Le = function(e) {
                         var t = e,
-                            n = $ ? $ - $e.width : 0;
+                            n = $ ? $ - we.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    Le = wn((function(e, t) {
+                    Fe = wn((function(e, t) {
                         t ? ((0, f.flushSync)((function() {
-                            ee((function(t) {
-                                return De(t + (W ? -e : e))
+                            te((function(t) {
+                                return Le(t + (W ? -e : e))
                             }))
-                        })), He()) : se((function(t) {
+                        })), Be()) : ue((function(t) {
                             return t + e
                         }))
                     })),
-                    Fe = function(e, t, n, r, i) {
+                    We = function(e, t, n, r, i) {
                         var a = (0, o.useRef)(0),
                             l = (0, o.useRef)(null),
                             c = (0, o.useRef)(null),
                             s = (0, o.useRef)(!1),
                             u = bm(t, n),
                             d = (0, o.useRef)(null),
                             p = (0, o.useRef)(null);
@@ -15233,18 +15237,18 @@
                                 }(t, g) : function(e, t) {
                                     i(t, !0), vm || e.preventDefault()
                                 }(t, m)
                             }
                         }, function(t) {
                             e && (s.current = t.detail === c.current)
                         }]
-                    }(D, je, Pe, !!$, Le),
-                    We = (0, ke.A)(Fe, 2),
-                    _e = We[0],
-                    Ve = We[1];
+                    }(D, Pe, Re, !!$, Fe),
+                    _e = (0, ke.A)(We, 2),
+                    Ve = _e[0],
+                    Ke = _e[1];
                 ! function(e, t, n) {
                     var r, i = (0, o.useRef)(!1),
                         a = (0, o.useRef)(0),
                         l = (0, o.useRef)(null),
                         c = (0, o.useRef)(null),
                         s = function(e) {
                             if (i.current) {
@@ -15267,40 +15271,40 @@
                         return e && t.current.addEventListener("touchstart", d),
                             function() {
                                 var e;
                                 null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", d), r(), clearInterval(c.current)
                             }
                     }), [e])
                 }(D, K, (function(e, t) {
-                    return !Re(e, t) && (_e({
+                    return !ze(e, t) && (Ve({
                         preventDefault: function() {},
                         deltaY: e
                     }), !0)
                 })), it((function() {
                     function e(e) {
                         D && e.preventDefault()
                     }
                     var t = K.current;
-                    return t.addEventListener("wheel", _e), t.addEventListener("DOMMouseScroll", Ve), t.addEventListener("MozMousePixelScroll", e),
+                    return t.addEventListener("wheel", Ve), t.addEventListener("DOMMouseScroll", Ke), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", _e), t.removeEventListener("DOMMouseScroll", Ve), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", Ve), t.removeEventListener("DOMMouseScroll", Ke), t.removeEventListener("MozMousePixelScroll", e)
                         }
                 }), [D]), it((function() {
                     if ($) {
-                        var e = De(J);
-                        ee(e), He({
+                        var e = Le(ee);
+                        te(e), Be({
                             x: e
                         })
                     }
-                }), [$e.width, $]);
-                var Ke = function() {
+                }), [we.width, $]);
+                var Xe = function() {
                         var e, t;
-                        null === (e = Se.current) || void 0 === e || e.delayHidden(), null === (t = Oe.current) || void 0 === t || t.delayHidden()
+                        null === (e = Oe.current) || void 0 === e || e.delayHidden(), null === (t = Ae.current) || void 0 === t || t.delayHidden()
                     },
-                    Xe = function(e, t, n, r, i, a, l, c) {
+                    qe = function(e, t, n, r, i, a, l, c) {
                         var s = o.useRef(),
                             u = o.useState(null),
                             f = (0, ke.A)(u, 2),
                             m = f[0],
                             g = f[1];
                         return it((function() {
                                 if (m && m.times < 10) {
@@ -15368,30 +15372,31 @@
                                             originAlign: o
                                         })
                                     }
                                 } else c()
                             }
                     }(K, V, H, s, j, (function() {
                         return T(!0)
-                    }), se, Ke);
+                    }), ue, Xe);
                 o.useImperativeHandle(t, (function() {
                     return {
-                        getScrollInfo: ze,
+                        nativeElement: q.current,
+                        getScrollInfo: Te,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ee(De(e.left)), Xe(e.top)) : Xe(e)
+                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && te(Le(e.left)), qe(e.top)) : qe(e)
                         }
                     }
                 })), it((function() {
                     if (O) {
-                        var e = V.slice(he, ve + 1);
+                        var e = V.slice(ve, be + 1);
                         O(e, V)
                     }
-                }), [he, ve, V]);
-                var qe = function(e, t, n, r) {
+                }), [ve, be, V]);
+                var Ge = function(e, t, n, r) {
                         var i = o.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, r]),
                             a = (0, ke.A)(i, 2),
                             l = a[0],
                             c = a[1];
                         return function(o) {
@@ -15408,99 +15413,101 @@
                                 }
                             return {
                                 top: c[a - 1] || 0,
                                 bottom: c[s]
                             }
                         }
                     }(V, j, H, s),
-                    Ge = null == I ? void 0 : I({
-                        start: he,
-                        end: ve,
+                    Ye = null == I ? void 0 : I({
+                        start: ve,
+                        end: be,
                         virtual: F,
-                        offsetX: J,
-                        offsetY: be,
+                        offsetX: ee,
+                        offsetY: ye,
                         rtl: W,
-                        getSize: qe
+                        getSize: Ge
                     }),
-                    Ye = function(e, t, n, r, i, a, l) {
-                        var c = l.getKey;
+                    Ue = function(e, t, n, r, i, a, l, c) {
+                        var s = c.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
-                            var l = a(e, t + n, {
+                            var c = l(e, t + n, {
                                     style: {
                                         width: r
-                                    }
+                                    },
+                                    offsetX: i
                                 }),
-                                s = c(e);
+                                u = s(e);
                             return o.createElement(hm, {
-                                key: s,
+                                key: u,
                                 setRef: function(t) {
-                                    return i(e, t)
+                                    return a(e, t)
                                 }
-                            }, l)
+                            }, c)
                         }))
-                    }(V, he, ve, $, z, b, le),
-                    Ue = null;
-                c && (Ue = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), Am), D && (Ue.overflowY = "hidden", $ && (Ue.overflowX = "hidden"), oe && (Ue.pointerEvents = "none")));
-                var Qe = {};
-                return W && (Qe.dir = "rtl"), o.createElement("div", (0, l.A)({
+                    }(V, ve, be, $, ee, z, b, se),
+                    Qe = null;
+                c && (Qe = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), Am), D && (Qe.overflowY = "hidden", $ && (Qe.overflowX = "hidden"), re && (Qe.pointerEvents = "none")));
+                var Ze = {};
+                return W && (Ze.dir = "rtl"), o.createElement("div", (0, l.A)({
+                    ref: q,
                     style: (0, d.A)((0, d.A)({}, g), {}, {
                         position: "relative"
                     }),
                     className: _
-                }, Qe, M), o.createElement(ce, {
+                }, Ze, M), o.createElement(ce, {
                     onResize: function(e) {
-                        we({
+                        Se({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, o.createElement(S, {
                     className: "".concat(r, "-holder"),
-                    style: Ue,
+                    style: Qe,
                     ref: K,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== Y && se(t), null == E || E(e), He()
+                        t !== U && ue(t), null == E || E(e), Be()
                     },
-                    onMouseEnter: Ke
+                    onMouseEnter: Xe
                 }, o.createElement(gm, {
                     prefixCls: r,
-                    height: ge,
-                    offsetX: J,
-                    offsetY: be,
+                    height: he,
+                    offsetX: ee,
+                    offsetY: ye,
                     scrollWidth: $,
                     onInnerResize: T,
                     ref: X,
                     innerProps: A,
                     rtl: W,
-                    extra: Ge
-                }, Ye))), F && ge > c && o.createElement(wm, {
-                    ref: Se,
+                    extra: Ye
+                }, Ue))), F && he > c && o.createElement(wm, {
+                    ref: Oe,
                     prefixCls: r,
-                    scrollOffset: Y,
-                    scrollRange: ge,
+                    scrollOffset: U,
+                    scrollRange: he,
                     rtl: W,
-                    onScroll: Be,
-                    onStartMove: ie,
-                    onStopMove: ae,
-                    spinSize: Ie,
-                    containerSize: $e.height,
+                    onScroll: De,
+                    onStartMove: ae,
+                    onStopMove: le,
+                    spinSize: Ne,
+                    containerSize: we.height,
                     style: null == N ? void 0 : N.verticalScrollBar,
                     thumbStyle: null == N ? void 0 : N.verticalScrollBarThumb
-                }), F && $ > $e.width && o.createElement(wm, {
-                    ref: Oe,
+                }), F && $ > we.width && o.createElement(wm, {
+                    ref: Ae,
                     prefixCls: r,
-                    scrollOffset: J,
+                    scrollOffset: ee,
                     scrollRange: $,
                     rtl: W,
-                    onScroll: Be,
-                    onStartMove: ie,
-                    onStopMove: ae,
-                    spinSize: Ae,
-                    containerSize: $e.width,
+                    onScroll: De,
+                    onStartMove: ae,
+                    onStopMove: le,
+                    spinSize: Ie,
+                    containerSize: we.width,
                     horizontal: !0,
                     style: null == N ? void 0 : N.horizontalScrollBar,
                     thumbStyle: null == N ? void 0 : N.horizontalScrollBarThumb
                 }))
             }
             var Nm = o.forwardRef(Im);
             Nm.displayName = "List";
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/687.82f4edc6966c97595e01.js.LICENSE.txt` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/687.e44561a1742c6083cba0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/remoteEntry.1ce7c98af16331b594f6.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/remoteEntry.1144a177b5daf1c9977c.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, s, c, f, p, d, h, v, m, b, g, y, w = {
+    var e, r, t, n, o, a, i, l, u, s, c, p, f, d, h, b, v, m, g, y, w = {
             2212: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(518), t.e(345), t.e(116)]).then((() => () => t(4116))),
-                        "./extension": () => Promise.all([t.e(518), t.e(345), t.e(116)]).then((() => () => t(4116))),
+                        "./index": () => Promise.all([t.e(518), t.e(345), t.e(792)]).then((() => () => t(5792))),
+                        "./extension": () => Promise.all([t.e(518), t.e(345), t.e(792)]).then((() => () => t(5792))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -43,29 +43,29 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        116: "a2462f90d7701c371aa8",
         345: "d33854e26caa385d0f56",
         432: "0fc640989ce2150a2305",
         518: "f70a8c5cdb51fc55b510",
         628: "6bee9242bd295a15f79b",
-        687: "82f4edc6966c97595e01",
-        713: "986c30f40fc55619b937"
+        687: "e44561a1742c6083cba0",
+        713: "986c30f40fc55619b937",
+        792: "7de2deb742ba9e036dda"
     } [e] + ".js?v=" + {
-        116: "a2462f90d7701c371aa8",
         345: "d33854e26caa385d0f56",
         432: "0fc640989ce2150a2305",
         518: "f70a8c5cdb51fc55b510",
         628: "6bee9242bd295a15f79b",
-        687: "82f4edc6966c97595e01",
-        713: "986c30f40fc55619b937"
+        687: "e44561a1742c6083cba0",
+        713: "986c30f40fc55619b937",
+        792: "7de2deb742ba9e036dda"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -78,24 +78,24 @@
                     var c = u[s];
                     if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + o) {
                         i = c;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var p = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(f);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                f = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -117,15 +117,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-components-core", "0.3.2", (() => Promise.all([S.e(518), S.e(345), S.e(116)]).then((() => () => S(4116))))), l("antd", "5.16.4", (() => Promise.all([S.e(687), S.e(518), S.e(628), S.e(345)]).then((() => () => S(7687))))), l("reactflow", "11.7.2", (() => Promise.all([S.e(713), S.e(628), S.e(345)]).then((() => () => S(5713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-components-core", "0.3.3", (() => Promise.all([S.e(518), S.e(345), S.e(792)]).then((() => () => S(5792))))), l("antd", "5.16.4", (() => Promise.all([S.e(687), S.e(518), S.e(628), S.e(345)]).then((() => () => S(7687))))), l("reactflow", "11.7.2", (() => Promise.all([S.e(713), S.e(628), S.e(345)]).then((() => () => S(5713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -175,92 +175,92 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var s, c, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (c = (typeof(s = r[i]))[0])) return !u || ("u" == f ? l > n && !o : "" == f != o);
+                var s, c, p = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (c = (typeof(s = r[i]))[0])) return !u || ("u" == p ? l > n && !o : "" == p != o);
                 if ("u" == c) {
-                    if (!u || "u" != f) return !1
+                    if (!u || "u" != p) return !1
                 } else if (u)
-                    if (f == c)
+                    if (p == c)
                         if (l <= n) {
                             if (s != e[l]) return !1
                         } else {
                             if (o ? s > e[l] : s < e[l]) return !1;
                             s != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != p && "n" != p) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || c < f != o) return !1;
+                    if (l <= n || c < p != o) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != p && "n" != p && (u = !1, l--)
             }
         }
-        var p = [],
-            d = p.pop.bind(p);
+        var f = [],
+            d = f.pop.bind(f);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? a(h, r) : !d())
+            f.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? a(h, r) : !d())
         }
         return !!d()
     }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || f(u(e, t, o, n)), p(e[t][o])
+        return a(n, o) || p(u(e, t, o, n)), f(e[t][o])
     }, c = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, f = e => {
+    }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (d = e => function(r, t, n, o) {
+    }, f = e => (e.loaded = 1, e.get()), h = (d = e => function(r, t, n, o) {
         var a = S.I(r);
         return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = d(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), b = d(((e, r, t, n, o) => {
         var a = r && S.o(r, t) && c(r, t, n);
-        return a ? p(a) : o()
-    })), m = {}, b = {
+        return a ? f(a) : o()
+    })), v = {}, m = {
         3345: () => h("default", "react", [1, 18, 2, 0]),
         1527: () => h("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
-        2473: () => v("default", "reactflow", [4, 11, 9, 4], (() => Promise.all([S.e(713), S.e(628)]).then((() => () => S(5713))))),
+        2473: () => b("default", "reactflow", [4, 11, 9, 4], (() => Promise.all([S.e(713), S.e(628)]).then((() => () => S(5713))))),
         3254: () => h("default", "@amphi/pipeline-components-manager", [0]),
-        4810: () => v("default", "antd", [4, 5, 16, 4], (() => Promise.all([S.e(687), S.e(628)]).then((() => () => S(7687))))),
+        4810: () => b("default", "antd", [4, 5, 16, 4], (() => Promise.all([S.e(687), S.e(628)]).then((() => () => S(7687))))),
         7628: () => h("default", "react-dom", [1, 18, 2, 0])
     }, g = {
-        116: [1527, 2473, 3254, 4810],
         345: [3345],
-        628: [7628]
+        628: [7628],
+        792: [1527, 2473, 3254, 4810]
     }, y = {}, S.f.consumes = (e, r) => {
         S.o(g, e) && g[e].forEach((e => {
-            if (S.o(m, e)) return r.push(m[e]);
+            if (S.o(v, e)) return r.push(v[e]);
             if (!y[e]) {
                 var t = r => {
-                    m[e] = 0, S.m[e] = t => {
+                    v[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
                 };
                 y[e] = !0;
                 var n = r => {
-                    delete m[e], S.m[e] = t => {
+                    delete v[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
                 try {
-                    var o = b[e]();
-                    o.then ? r.push(m[e] = o.then(t).catch(n)) : t(o)
+                    var o = m[e]();
+                    o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-core/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985795454545454%*

 * *Differences: {"'packages'": "{74: {'versionInfo': '5.41.0'}, 75: {'versionInfo': '3.14.0'}}"}*

```diff
@@ -444,21 +444,21 @@
             "name": "rc-upload",
             "versionInfo": "4.5.2"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014-present yiminghe\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-util",
-            "versionInfo": "5.40.1"
+            "versionInfo": "5.41.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.12.0"
+            "versionInfo": "3.14.0"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react",
             "versionInfo": "18.3.1"
         },
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.001fdc1b89863b0cb38e.js'}}",*

 * * "'version'": "'0.3.3'"}*

```diff
@@ -49,15 +49,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e7b2fd7c27479971192a.js",
+            "load": "static/remoteEntry.001fdc1b89863b0cb38e.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundle": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.3.3"
 }
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/142.1ffdd6d84b9f153e1c84.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -603,15 +603,15 @@
 
                 function v(e) {
                     const t = r.get(e) || 0;
                     r.set(e, t + 1)
                 }
                 e.nodes.forEach((e => {
                     const n = t.getComponent(e.type)._type;
-                    "annotation" !== n && ("logger" === n ? c.set(e.id, e) : "env_variables" === n ? m.set(e.id, e) : i.set(e.id, e))
+                    "annotation" !== n && ("logger" === n ? c.set(e.id, e) : "env_variables" === n || "env_file" === n ? m.set(e.id, e) : i.set(e.id, e))
                 }));
                 const f = new Set,
                     E = new Map,
                     y = (t, n) => {
                         if (f.has(t)) {
                             const e = E.get(t) || new Set;
                             return void E.set(t, new Set([...e, ...n]))
@@ -730,15 +730,15 @@
                     e = e.split("\n").map((e => n + e)).join("\n"), l = l.split("\n").map((e => n + e)).join("\n"), l = `\ntry:\n${l}\nexcept Exception as e:\n    print(f"An error occurred: {e}")\n${e}\n`
                 }
                 const b = new Date,
                     x = `# Source code generated by Amphi\n# Date: ${b.getFullYear()}-${(b.getMonth()+1).toString().padStart(2,"0")}-${b.getDate().toString().padStart(2,"0")} ${b.getHours().toString().padStart(2,"0")}:${b.getMinutes().toString().padStart(2,"0")}:${b.getSeconds().toString().padStart(2,"0")}`,
                     S = `# Additional dependencies: ${Array.from(g).join(", ")}`;
                 return l = $.convertToFString(l), `${x}\n${S}\n${Array.from(p).join("\n")}\n\n${w}${Array.from(h).join("\n\n")}\n${l}`
             };
-            class R {
+            class V {
                 static retrieveDataframeColumns(e, t, n, a, l, o, r, i, s) {
                     o(!0);
                     const d = _.filterPipeline(t.model.toString());
                     let c = "";
                     try {
                         let e = s ? _.findMultiplePreviousNodeIds(d, r)[i] : r;
                         c = L.generateCodeUntil(t.model.toString(), n, a, e, t)
@@ -776,52 +776,55 @@
                                 o(!1);
                                 const t = e.content;
                                 console.error(`Received error: ${t.ename}: ${t.evalue}`)
                             }
                         } : ("error" == e.content.status || e.content.status, o(!1))
                     }) : o(!1)
                 }
-                static retrieveTableColumns(e, t, n, a, l, o, r, i, s, d) {
-                    s(!0);
-                    const c = `\n!pip install --quiet pymysql --disable-pip-version-check\nimport pandas as pd\nfrom sqlalchemy import create_engine\nschema = pd.read_sql("${a}", con = create_engine("${t}"))\ncolumn_info = schema[["Field", "Type"]]\nformatted_output = ", ".join([f"{row['Field']} ({row['Type']})" for _, row in column_info.iterrows()])\nprint(formatted_output)\n`;
-                    console.log("code: " + c);
-                    const m = l.sessionContext.session.kernel.requestExecute({
-                        code: c
+                static retrieveTableColumns(e, t, n, a, l, o, r, i, s, d, c, m) {
+                    c(!0);
+                    const u = t.join(", ");
+                    let p = o.replace(/"/g, '\\"');
+                    p = p.replace(/{{schema}}/g, a).replace(/{{table}}/g, l);
+                    let g = `\n!pip install --quiet ${u} --disable-pip-version-check\nimport pandas as pd\nfrom sqlalchemy import create_engine\nquery = """\n${p}\n"""\nschema = pd.read_sql(query, con = create_engine("${n}"))\ncolumn_info = schema[["Field", "Type"]]\nformatted_output = ", ".join([f"{row['Field']} ({row['Type']})" for _, row in column_info.iterrows()])\nprint(formatted_output)\n`;
+                    g = L.convertToFString(g), console.log("code: " + g);
+                    const h = r.sessionContext.session.kernel.requestExecute({
+                        code: g
                     });
-                    m.onReply = e => {
-                        "ok" == e.content.status ? console.log("OK") : "error" == e.content.status ? (console.log("error"), s(!1)) : "abort" == e.content.status ? (console.log("abort"), s(!1)) : (console.log("Other"), s(!1))
-                    }, m.onIOPub = e => {
+                    h.onReply = e => {
+                        "ok" == e.content.status ? console.log("OK") : "error" == e.content.status ? (console.log("error"), c(!1)) : "abort" == e.content.status ? (console.log("abort"), c(!1)) : (console.log("Other"), c(!1))
+                    }, h.onIOPub = e => {
                         if ("stream" === e.header.msg_type) {
                             const t = e.content.text,
                                 n = /([^\s,]+)\s+\(((?:[^()]+|\([^)]*\))*)\)/g,
                                 a = [];
                             let l;
                             for (; null !== (l = n.exec(t));) {
                                 const [e, t, n, o] = l;
                                 a.push({
                                     input: {},
                                     value: t,
                                     key: t,
                                     type: n.toUpperCase()
                                 })
                             }
-                            i((e => {
+                            d((e => {
                                 const t = new Set(e.map((e => e.key))),
                                     n = a.filter((e => !t.has(e.key)));
                                 return [...e, ...n]
-                            })), s(!1)
+                            })), c(!1)
                         } else if ("error" === e.header.msg_type) {
-                            s(!1);
+                            c(!1);
                             const t = e.content;
                             console.error(`Received error: ${t.ename}: ${t.evalue}`)
                         }
                     }
                 }
             }
-            const V = ({
+            const R = ({
                     field: e,
                     handleChange: t,
                     defaultValues: n,
                     context: a,
                     componentService: i,
                     commands: s,
                     nodeId: d,
@@ -893,15 +896,15 @@
                                 display: "flex",
                                 justifyContent: "center",
                                 alignItems: "center",
                                 padding: "0 2px 2px"
                             }
                         }, o().createElement(r.Button, {
                             type: "primary",
-                            onClick: e => R.retrieveDataframeColumns(e, a, s, i, u, C, d, w, !0),
+                            onClick: e => V.retrieveDataframeColumns(e, a, s, i, u, C, d, w, !0),
                             loading: y
                         }, "Retrieve columns")), o().createElement(r.Divider, {
                             style: {
                                 margin: "8px 0"
                             }
                         }), o().createElement(r.Space, {
                             style: {
@@ -922,15 +925,15 @@
                             label: e.label,
                             value: e.value,
                             type: e.type
                         }))),
                         optionRender: e => o().createElement(r.Space, null, o().createElement("span", null, " ", e.data.label), o().createElement(r.Tag, null, e.data.type))
                     }))
                 },
-                z = ({
+                T = ({
                     field: e,
                     handleChange: t,
                     defaultValue: n,
                     context: a,
                     componentService: i,
                     commands: s,
                     nodeId: d,
@@ -1009,15 +1012,15 @@
                                 display: "flex",
                                 justifyContent: "center",
                                 alignItems: "center",
                                 padding: "0 2px 2px"
                             }
                         }, o().createElement(r.Button, {
                             type: "primary",
-                            onClick: e => R.retrieveDataframeColumns(e, a, s, i, p, w, d, b, !0),
+                            onClick: e => V.retrieveDataframeColumns(e, a, s, i, p, w, d, b, !0),
                             loading: C
                         }, "Retrieve columns")), o().createElement(r.Divider, {
                             style: {
                                 margin: "8px 0"
                             }
                         }), o().createElement(r.Space, {
                             style: {
@@ -1039,15 +1042,15 @@
                             value: e.value,
                             type: e.type,
                             named: e.named
                         }))),
                         optionRender: e => o().createElement(r.Space, null, o().createElement("span", null, " ", e.data.label), o().createElement(r.Tag, null, e.data.type))
                     }))
                 },
-                T = ({
+                z = ({
                     field: e,
                     handleChange: t,
                     initialValues: n,
                     context: a,
                     componentService: i,
                     commands: s,
                     nodeId: d,
@@ -1074,15 +1077,15 @@
                         style: {
                             textAlign: "center"
                         }
                     }, o().createElement(r.Empty, {
                         image: r.Empty.PRESENTED_IMAGE_SIMPLE
                     }), o().createElement(r.Button, {
                         type: "primary",
-                        onClick: e => R.retrieveDataframeColumns(e, a, s, i, v, g, d, 0, !0),
+                        onClick: e => V.retrieveDataframeColumns(e, a, s, i, v, g, d, 0, !0),
                         loading: p
                     }, "Retrieve columns")), k = e => {
                         e.preventDefault(), v([...h, {
                             value: C,
                             label: C
                         }]), w(""), setTimeout((() => {
                             var e;
@@ -1227,15 +1230,15 @@
                         style: {
                             textAlign: "center"
                         }
                     }, o().createElement(r.Empty, {
                         image: r.Empty.PRESENTED_IMAGE_SIMPLE
                     }), o().createElement(r.Button, {
                         type: "primary",
-                        onClick: e => R.retrieveDataframeColumns(e, a, s, i, v, g, d, 0, !0),
+                        onClick: e => V.retrieveDataframeColumns(e, a, s, i, v, g, d, 0, !0),
                         loading: p
                     }, "Retrieve columns")), D = e => {
                         e.preventDefault(), v([...h, {
                             value: b,
                             label: b
                         }]), x(""), setTimeout((() => {
                             var e;
@@ -1545,15 +1548,17 @@
                             if ("left" === (null == t ? void 0 : t.direction)) return o().createElement(r.Button, {
                                 type: "primary",
                                 size: "small",
                                 style: {
                                     float: "left",
                                     margin: 5
                                 },
-                                onClick: e => R.retrieveDataframeColumns(e, a, s, i, p, y, d, 0, !0),
+                                onClick: e => {
+                                    p([]), V.retrieveDataframeColumns(e, a, s, i, p, y, d, 0, !0)
+                                },
                                 loading: E
                             }, "Retrieve columns")
                         }
                     }), o().createElement(r.Space, {
                         style: {
                             marginTop: 16
                         }
@@ -1796,15 +1801,15 @@
                                                 justifyContent: "center",
                                                 alignItems: "center",
                                                 padding: "0 2px 2px"
                                             }
                                         }, o().createElement(r.Button, {
                                             type: "primary",
                                             onClick: e => {
-                                                R.retrieveDataframeColumns(e, i, d, s, E, g, c, 0, !0)
+                                                V.retrieveDataframeColumns(e, i, d, s, E, g, c, 0, !0)
                                             },
                                             loading: p
                                         }, "Retrieve columns"))),
                                         options: f.map((e => ({
                                             label: e.label,
                                             value: e.value,
                                             type: e.type,
@@ -1830,15 +1835,16 @@
                     return o().createElement(o().Fragment, null, o().createElement("div", null, "relationalDatabase" === t.outputType ? o().createElement(r.Button, {
                         type: "primary",
                         size: "small",
                         style: {
                             marginBottom: 16
                         },
                         onClick: n => {
-                            C([]), R.retrieveTableColumns(n, `${t.drivers}://${e.dbOptions.username}:${e.dbOptions.password}@${e.dbOptions.host}:${e.dbOptions.port}/${e.dbOptions.databaseName}`, `${e.dbOptions.tableName}`, `DESCRIBE ${e.dbOptions.tableName}`, i, d, s, C, v, c)
+                            var a;
+                            C([]), V.retrieveTableColumns(n, t.imports, `${t.drivers}://${e.dbOptions.username}:${e.dbOptions.password}@${e.dbOptions.host}:${e.dbOptions.port}/${e.dbOptions.databaseName}`, `${null!==(a=e.dbOptions.schema)&&void 0!==a?a:"public"}`, `${e.dbOptions.tableName}`, `${t.query}`, i, d, s, C, v, c)
                         },
                         loading: h
                     }, "Retrieve schema") : null, o().createElement(r.Table, {
                         components: k,
                         rowClassName: () => "editable-row",
                         bordered: !0,
                         dataSource: y,
@@ -2175,15 +2181,15 @@
                                 className: "nodrag",
                                 ...e.required ? {
                                     required: e.required
                                 } : {},
                                 ...e.tooltip ? {
                                     tooltip: e.tooltip
                                 } : {}
-                            }, o().createElement(V, {
+                            }, o().createElement(R, {
                                 field: e,
                                 handleChange: E,
                                 defaultValues: b,
                                 context: u,
                                 componentService: p,
                                 commands: f,
                                 nodeId: t,
@@ -2199,15 +2205,15 @@
                                 className: "nodrag",
                                 ...e.required ? {
                                     required: e.required
                                 } : {},
                                 ...e.tooltip ? {
                                     tooltip: e.tooltip
                                 } : {}
-                            }, o().createElement(z, {
+                            }, o().createElement(T, {
                                 field: e,
                                 handleChange: E,
                                 defaultValue: w,
                                 context: u,
                                 componentService: p,
                                 commands: f,
                                 nodeId: t,
@@ -2353,15 +2359,15 @@
                                 className: "nodrag",
                                 ...e.required ? {
                                     required: e.required
                                 } : {},
                                 ...e.tooltip ? {
                                     tooltip: e.tooltip
                                 } : {}
-                            }, o().createElement(T, {
+                            }, o().createElement(z, {
                                 field: e,
                                 handleChange: E,
                                 initialValues: b,
                                 context: u,
                                 componentService: p,
                                 commands: f,
                                 nodeId: t,
@@ -2464,15 +2470,19 @@
                                 nodeId: t,
                                 inDialog: C
                             }));
                         case "info":
                             const {
                                 Paragraph: l
                             } = r.Typography;
-                            return o().createElement(l, null, e.text);
+                            return o().createElement(l, {
+                                style: {
+                                    padding: "5px"
+                                }
+                            }, e.text);
                         default:
                             return null
                     }
                 })));
 
             function ae({
                 name: e,
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/422.87216a9371fbc611f07f.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/422.27a4f789109562c256e8.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 422.87216a9371fbc611f07f.js.LICENSE.txt */
+/*! For license information please see 422.27a4f789109562c256e8.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_components_manager = self.webpackChunk_amphi_pipeline_components_manager || []).push([
     [422], {
         5422: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 Affix: () => Ko,
                 Alert: () => Ci,
@@ -98,15 +98,18 @@
                 m = n.n(f);
 
             function g(e) {
                 return e instanceof HTMLElement || e instanceof SVGElement
             }
 
             function h(e) {
-                return e && "object" === (0, p.A)(e) && g(e.nativeElement) ? e.nativeElement : g(e) ? e : e instanceof r().Component ? m().findDOMNode(e) : null
+                var t, n = function(e) {
+                    return e && "object" === (0, p.A)(e) && g(e.nativeElement) ? e.nativeElement : g(e) ? e : null
+                }(e);
+                return n || (e instanceof r().Component ? null === (t = m().findDOMNode) || void 0 === t ? void 0 : t.call(m(), e) : null)
             }
 
             function v(e, t, n) {
                 var r = o.useRef({});
                 return "value" in r.current && !n(r.current.condition, t) || (r.current.value = e(), r.current.condition = t), r.current.value
             }
             var b = function(e, t) {
@@ -15011,51 +15014,52 @@
                     }), [H.id, H.maps]),
                     F = D && v && (Math.max(s * v.length, L) > c || !!$),
                     W = "rtl" === x,
                     _ = a()(r, (0, Ee.A)({}, "".concat(r, "-rtl"), W), i),
                     V = v || Em,
                     K = (0, o.useRef)(),
                     X = (0, o.useRef)(),
-                    q = (0, o.useState)(0),
-                    G = (0, ke.A)(q, 2),
-                    Y = G[0],
-                    U = G[1],
-                    Q = (0, o.useState)(0),
-                    Z = (0, ke.A)(Q, 2),
-                    J = Z[0],
-                    ee = Z[1],
-                    te = (0, o.useState)(!1),
-                    ne = (0, ke.A)(te, 2),
-                    oe = ne[0],
-                    re = ne[1],
-                    ie = function() {
-                        re(!0)
-                    },
+                    q = (0, o.useRef)(),
+                    G = (0, o.useState)(0),
+                    Y = (0, ke.A)(G, 2),
+                    U = Y[0],
+                    Q = Y[1],
+                    Z = (0, o.useState)(0),
+                    J = (0, ke.A)(Z, 2),
+                    ee = J[0],
+                    te = J[1],
+                    ne = (0, o.useState)(!1),
+                    oe = (0, ke.A)(ne, 2),
+                    re = oe[0],
+                    ie = oe[1],
                     ae = function() {
-                        re(!1)
+                        ie(!0)
+                    },
+                    le = function() {
+                        ie(!1)
                     },
-                    le = {
+                    se = {
                         getKey: j
                     };
 
-                function se(e) {
-                    U((function(t) {
+                function ue(e) {
+                    Q((function(t) {
                         var n = function(e) {
                             var t = e;
-                            return Number.isNaN(Me.current) || (t = Math.min(t, Me.current)), t = Math.max(t, 0)
+                            return Number.isNaN(je.current) || (t = Math.min(t, je.current)), t = Math.max(t, 0)
                         }("function" == typeof e ? e(t) : e);
                         return K.current.scrollTop = n, n
                     }))
                 }
-                var ue = (0, o.useRef)({
+                var de = (0, o.useRef)({
                         start: 0,
                         end: V.length
                     }),
-                    de = (0, o.useRef)(),
-                    pe = function(e, t, n) {
+                    pe = (0, o.useRef)(),
+                    fe = function(e, t, n) {
                         var r = o.useState(e),
                             i = (0, ke.A)(r, 2),
                             a = i[0],
                             l = i[1],
                             c = o.useState(null),
                             s = (0, ke.A)(c, 2),
                             u = s[0],
@@ -15084,17 +15088,17 @@
                                     index: s,
                                     multiple: u
                                 }
                             }(a || [], e || [], t);
                             void 0 !== (null == o ? void 0 : o.index) && (null == n || n(o.index), d(e[o.index])), l(e)
                         }), [e]), [u]
                     }(V, j),
-                    fe = (0, ke.A)(pe, 1)[0];
-                de.current = fe;
-                var me = o.useMemo((function() {
+                    me = (0, ke.A)(fe, 1)[0];
+                pe.current = me;
+                var ge = o.useMemo((function() {
                         if (!D) return {
                             scrollHeight: void 0,
                             start: 0,
                             end: V.length - 1,
                             offset: void 0
                         };
                         var e;
@@ -15105,84 +15109,84 @@
                             offset: void 0
                         };
                         for (var t, n, o, r = 0, i = V.length, a = 0; a < i; a += 1) {
                             var l = V[a],
                                 u = j(l),
                                 d = H.get(u),
                                 p = r + (void 0 === d ? s : d);
-                            p >= Y && void 0 === t && (t = a, n = r), p > Y + c && void 0 === o && (o = a), r = p
+                            p >= U && void 0 === t && (t = a, n = r), p > U + c && void 0 === o && (o = a), r = p
                         }
                         return void 0 === t && (t = 0, n = 0, o = Math.ceil(c / s)), void 0 === o && (o = V.length - 1), {
                             scrollHeight: r,
                             start: t,
                             end: o = Math.min(o + 1, V.length - 1),
                             offset: n
                         }
-                    }), [F, D, Y, V, B, c]),
-                    ge = me.scrollHeight,
-                    he = me.start,
-                    ve = me.end,
-                    be = me.offset;
-                ue.current.start = he, ue.current.end = ve;
-                var ye = o.useState({
+                    }), [F, D, U, V, B, c]),
+                    he = ge.scrollHeight,
+                    ve = ge.start,
+                    be = ge.end,
+                    ye = ge.offset;
+                de.current.start = ve, de.current.end = be;
+                var xe = o.useState({
                         width: 0,
                         height: c
                     }),
-                    xe = (0, ke.A)(ye, 2),
-                    $e = xe[0],
-                    we = xe[1],
-                    Se = (0, o.useRef)(),
+                    $e = (0, ke.A)(xe, 2),
+                    we = $e[0],
+                    Se = $e[1],
                     Oe = (0, o.useRef)(),
-                    Ae = o.useMemo((function() {
-                        return wm($e.width, $)
-                    }), [$e.width, $]),
+                    Ae = (0, o.useRef)(),
                     Ie = o.useMemo((function() {
-                        return wm($e.height, ge)
-                    }), [$e.height, ge]),
-                    Ne = ge - c,
-                    Me = (0, o.useRef)(Ne);
-                Me.current = Ne;
-                var je = Y <= 0,
-                    Pe = Y >= Ne,
-                    Re = hm(je, Pe),
-                    Te = function() {
+                        return wm(we.width, $)
+                    }), [we.width, $]),
+                    Ne = o.useMemo((function() {
+                        return wm(we.height, he)
+                    }), [we.height, he]),
+                    Me = he - c,
+                    je = (0, o.useRef)(Me);
+                je.current = Me;
+                var Pe = U <= 0,
+                    Re = U >= Me,
+                    Te = hm(Pe, Re),
+                    ze = function() {
                         return {
-                            x: W ? -J : J,
-                            y: Y
+                            x: W ? -ee : ee,
+                            y: U
                         }
                     },
-                    ze = (0, o.useRef)(Te()),
-                    He = wn((function(e) {
+                    He = (0, o.useRef)(ze()),
+                    Be = wn((function(e) {
                         if (k) {
-                            var t = (0, d.A)((0, d.A)({}, Te()), e);
-                            ze.current.x === t.x && ze.current.y === t.y || (k(t), ze.current = t)
+                            var t = (0, d.A)((0, d.A)({}, ze()), e);
+                            He.current.x === t.x && He.current.y === t.y || (k(t), He.current = t)
                         }
                     }));
 
-                function Be(e, t) {
+                function De(e, t) {
                     var n = e;
                     t ? ((0, f.flushSync)((function() {
-                        ee(n)
-                    })), He()) : se(n)
+                        te(n)
+                    })), Be()) : ue(n)
                 }
-                var De = function(e) {
+                var Le = function(e) {
                         var t = e,
-                            n = $ ? $ - $e.width : 0;
+                            n = $ ? $ - we.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    Le = wn((function(e, t) {
+                    Fe = wn((function(e, t) {
                         t ? ((0, f.flushSync)((function() {
-                            ee((function(t) {
-                                return De(t + (W ? -e : e))
+                            te((function(t) {
+                                return Le(t + (W ? -e : e))
                             }))
-                        })), He()) : se((function(t) {
+                        })), Be()) : ue((function(t) {
                             return t + e
                         }))
                     })),
-                    Fe = function(e, t, n, r, i) {
+                    We = function(e, t, n, r, i) {
                         var a = (0, o.useRef)(0),
                             l = (0, o.useRef)(null),
                             c = (0, o.useRef)(null),
                             s = (0, o.useRef)(!1),
                             u = hm(t, n),
                             d = (0, o.useRef)(null),
                             p = (0, o.useRef)(null);
@@ -15207,18 +15211,18 @@
                                 }(t, g) : function(e, t) {
                                     i(t, !0), gm || e.preventDefault()
                                 }(t, m)
                             }
                         }, function(t) {
                             e && (s.current = t.detail === c.current)
                         }]
-                    }(D, je, Pe, !!$, Le),
-                    We = (0, ke.A)(Fe, 2),
-                    _e = We[0],
-                    Ve = We[1];
+                    }(D, Pe, Re, !!$, Fe),
+                    _e = (0, ke.A)(We, 2),
+                    Ve = _e[0],
+                    Ke = _e[1];
                 ! function(e, t, n) {
                     var r, i = (0, o.useRef)(!1),
                         a = (0, o.useRef)(0),
                         l = (0, o.useRef)(null),
                         c = (0, o.useRef)(null),
                         s = function(e) {
                             if (i.current) {
@@ -15241,40 +15245,40 @@
                         return e && t.current.addEventListener("touchstart", d),
                             function() {
                                 var e;
                                 null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", d), r(), clearInterval(c.current)
                             }
                     }), [e])
                 }(D, K, (function(e, t) {
-                    return !Re(e, t) && (_e({
+                    return !Te(e, t) && (Ve({
                         preventDefault: function() {},
                         deltaY: e
                     }), !0)
                 })), it((function() {
                     function e(e) {
                         D && e.preventDefault()
                     }
                     var t = K.current;
-                    return t.addEventListener("wheel", _e), t.addEventListener("DOMMouseScroll", Ve), t.addEventListener("MozMousePixelScroll", e),
+                    return t.addEventListener("wheel", Ve), t.addEventListener("DOMMouseScroll", Ke), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", _e), t.removeEventListener("DOMMouseScroll", Ve), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", Ve), t.removeEventListener("DOMMouseScroll", Ke), t.removeEventListener("MozMousePixelScroll", e)
                         }
                 }), [D]), it((function() {
                     if ($) {
-                        var e = De(J);
-                        ee(e), He({
+                        var e = Le(ee);
+                        te(e), Be({
                             x: e
                         })
                     }
-                }), [$e.width, $]);
-                var Ke = function() {
+                }), [we.width, $]);
+                var Xe = function() {
                         var e, t;
-                        null === (e = Se.current) || void 0 === e || e.delayHidden(), null === (t = Oe.current) || void 0 === t || t.delayHidden()
+                        null === (e = Oe.current) || void 0 === e || e.delayHidden(), null === (t = Ae.current) || void 0 === t || t.delayHidden()
                     },
-                    Xe = function(e, t, n, r, i, a, l, c) {
+                    qe = function(e, t, n, r, i, a, l, c) {
                         var s = o.useRef(),
                             u = o.useState(null),
                             f = (0, ke.A)(u, 2),
                             m = f[0],
                             g = f[1];
                         return it((function() {
                                 if (m && m.times < 10) {
@@ -15342,30 +15346,31 @@
                                             originAlign: o
                                         })
                                     }
                                 } else c()
                             }
                     }(K, V, H, s, j, (function() {
                         return z(!0)
-                    }), se, Ke);
+                    }), ue, Xe);
                 o.useImperativeHandle(t, (function() {
                     return {
-                        getScrollInfo: Te,
+                        nativeElement: q.current,
+                        getScrollInfo: ze,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ee(De(e.left)), Xe(e.top)) : Xe(e)
+                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && te(Le(e.left)), qe(e.top)) : qe(e)
                         }
                     }
                 })), it((function() {
                     if (O) {
-                        var e = V.slice(he, ve + 1);
+                        var e = V.slice(ve, be + 1);
                         O(e, V)
                     }
-                }), [he, ve, V]);
-                var qe = function(e, t, n, r) {
+                }), [ve, be, V]);
+                var Ge = function(e, t, n, r) {
                         var i = o.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, r]),
                             a = (0, ke.A)(i, 2),
                             l = a[0],
                             c = a[1];
                         return function(o) {
@@ -15382,99 +15387,101 @@
                                 }
                             return {
                                 top: c[a - 1] || 0,
                                 bottom: c[s]
                             }
                         }
                     }(V, j, H, s),
-                    Ge = null == I ? void 0 : I({
-                        start: he,
-                        end: ve,
+                    Ye = null == I ? void 0 : I({
+                        start: ve,
+                        end: be,
                         virtual: F,
-                        offsetX: J,
-                        offsetY: be,
+                        offsetX: ee,
+                        offsetY: ye,
                         rtl: W,
-                        getSize: qe
+                        getSize: Ge
                     }),
-                    Ye = function(e, t, n, r, i, a, l) {
-                        var c = l.getKey;
+                    Ue = function(e, t, n, r, i, a, l, c) {
+                        var s = c.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
-                            var l = a(e, t + n, {
+                            var c = l(e, t + n, {
                                     style: {
                                         width: r
-                                    }
+                                    },
+                                    offsetX: i
                                 }),
-                                s = c(e);
+                                u = s(e);
                             return o.createElement(mm, {
-                                key: s,
+                                key: u,
                                 setRef: function(t) {
-                                    return i(e, t)
+                                    return a(e, t)
                                 }
-                            }, l)
+                            }, c)
                         }))
-                    }(V, he, ve, $, T, b, le),
-                    Ue = null;
-                c && (Ue = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), km), D && (Ue.overflowY = "hidden", $ && (Ue.overflowX = "hidden"), oe && (Ue.pointerEvents = "none")));
-                var Qe = {};
-                return W && (Qe.dir = "rtl"), o.createElement("div", (0, l.A)({
+                    }(V, ve, be, $, ee, T, b, se),
+                    Qe = null;
+                c && (Qe = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), km), D && (Qe.overflowY = "hidden", $ && (Qe.overflowX = "hidden"), re && (Qe.pointerEvents = "none")));
+                var Ze = {};
+                return W && (Ze.dir = "rtl"), o.createElement("div", (0, l.A)({
+                    ref: q,
                     style: (0, d.A)((0, d.A)({}, g), {}, {
                         position: "relative"
                     }),
                     className: _
-                }, Qe, M), o.createElement(ce, {
+                }, Ze, M), o.createElement(ce, {
                     onResize: function(e) {
-                        we({
+                        Se({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, o.createElement(S, {
                     className: "".concat(r, "-holder"),
-                    style: Ue,
+                    style: Qe,
                     ref: K,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== Y && se(t), null == E || E(e), He()
+                        t !== U && ue(t), null == E || E(e), Be()
                     },
-                    onMouseEnter: Ke
+                    onMouseEnter: Xe
                 }, o.createElement(fm, {
                     prefixCls: r,
-                    height: ge,
-                    offsetX: J,
-                    offsetY: be,
+                    height: he,
+                    offsetX: ee,
+                    offsetY: ye,
                     scrollWidth: $,
                     onInnerResize: z,
                     ref: X,
                     innerProps: A,
                     rtl: W,
-                    extra: Ge
-                }, Ye))), F && ge > c && o.createElement(xm, {
-                    ref: Se,
+                    extra: Ye
+                }, Ue))), F && he > c && o.createElement(xm, {
+                    ref: Oe,
                     prefixCls: r,
-                    scrollOffset: Y,
-                    scrollRange: ge,
+                    scrollOffset: U,
+                    scrollRange: he,
                     rtl: W,
-                    onScroll: Be,
-                    onStartMove: ie,
-                    onStopMove: ae,
-                    spinSize: Ie,
-                    containerSize: $e.height,
+                    onScroll: De,
+                    onStartMove: ae,
+                    onStopMove: le,
+                    spinSize: Ne,
+                    containerSize: we.height,
                     style: null == N ? void 0 : N.verticalScrollBar,
                     thumbStyle: null == N ? void 0 : N.verticalScrollBarThumb
-                }), F && $ > $e.width && o.createElement(xm, {
-                    ref: Oe,
+                }), F && $ > we.width && o.createElement(xm, {
+                    ref: Ae,
                     prefixCls: r,
-                    scrollOffset: J,
+                    scrollOffset: ee,
                     scrollRange: $,
                     rtl: W,
-                    onScroll: Be,
-                    onStartMove: ie,
-                    onStopMove: ae,
-                    spinSize: Ae,
-                    containerSize: $e.width,
+                    onScroll: De,
+                    onStartMove: ae,
+                    onStopMove: le,
+                    spinSize: Ie,
+                    containerSize: we.width,
                     horizontal: !0,
                     style: null == N ? void 0 : N.horizontalScrollBar,
                     thumbStyle: null == N ? void 0 : N.horizontalScrollBarThumb
                 }))
             }
             var Am = o.forwardRef(Om);
             Am.displayName = "List";
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/422.87216a9371fbc611f07f.js.LICENSE.txt` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/422.27a4f789109562c256e8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/841.17235cce88409653d379.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/841.6f47bec498543a801840.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 841.17235cce88409653d379.js.LICENSE.txt */
+/*! For license information please see 841.6f47bec498543a801840.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_components_manager = self.webpackChunk_amphi_pipeline_components_manager || []).push([
     [841], {
         1841: (e, t, n) => {
             e = n.nmd(e),
                 function() {
                     var e = function() {
                         return this
@@ -665,15 +665,15 @@
                         if ("function" == typeof n.require) return n.require(e)
                     }, t.setModuleLoader = function(e, n) {
                         t.dynamicModules[e] = n
                     };
                     var c = function() {
                         l.basePath || l.workerPath || l.modePath || l.themePath || Object.keys(l.$moduleUrls).length || (console.error("Unable to infer path to ace from script src,", "use ace.config.set('basePath', 'path') to enable dynamic loading of modes and themes", "or with webpack use ace/webpack-resolver"), c = function() {})
                     };
-                    t.version = "1.33.2"
+                    t.version = "1.33.3"
                 })), ace.define("ace/loader_build", ["require", "exports", "module", "ace/lib/fixoldbrowsers", "ace/config"], (function(e, t, i) {
                     "use strict";
                     e("./lib/fixoldbrowsers");
                     var o = e("./config");
                     o.setLoader((function(t, n) {
                         e([t], (function(e) {
                             n(null, e)
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/remoteEntry.e7b2fd7c27479971192a.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/remoteEntry.001fdc1b89863b0cb38e.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, d, l, f, c, u, s, p, h, m, b, v, g, y, w = {
+    var e, r, t, a, n, o, i, d, l, f, u, c, s, p, h, b, m, v, g, y, w = {
             5548: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(173), t.e(725), t.e(345), t.e(628), t.e(142)]).then((() => () => t(8142))),
                         "./extension": () => Promise.all([t.e(173), t.e(725), t.e(345), t.e(628), t.e(142)]).then((() => () => t(8142))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -48,69 +48,69 @@
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         12: "e1b4412a18535c560cd1",
         85: "227e3aea03a3014cd80a",
-        142: "1ffdd6d84b9f153e1c84",
+        142: "acbbd4c680da3a899eb9",
         173: "254dd13d95daff6ca4b4",
         186: "e77a90422af9cbab4e47",
         271: "3095f6e27a6de7c0174d",
         345: "39215b57fd3910de833c",
-        422: "87216a9371fbc611f07f",
+        422: "27a4f789109562c256e8",
         432: "1d493bea1143efe37c80",
         454: "b60aaa09eed0e7e4a124",
         628: "f8b00c70c263432a40ab",
         725: "90ddd44d4e0f0fae78c2",
-        841: "17235cce88409653d379"
+        841: "6f47bec498543a801840"
     } [e] + ".js?v=" + {
         12: "e1b4412a18535c560cd1",
         85: "227e3aea03a3014cd80a",
-        142: "1ffdd6d84b9f153e1c84",
+        142: "acbbd4c680da3a899eb9",
         173: "254dd13d95daff6ca4b4",
         186: "e77a90422af9cbab4e47",
         271: "3095f6e27a6de7c0174d",
         345: "39215b57fd3910de833c",
-        422: "87216a9371fbc611f07f",
+        422: "27a4f789109562c256e8",
         432: "1d493bea1143efe37c80",
         454: "b60aaa09eed0e7e4a124",
         628: "f8b00c70c263432a40ab",
         725: "90ddd44d4e0f0fae78c2",
-        841: "17235cce88409653d379"
+        841: "6f47bec498543a801840"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-components-manager:", S.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, d;
             if (void 0 !== n)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var c = l[f];
-                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + n) {
-                        i = c;
+                    var u = l[f];
+                    if (u.getAttribute("src") == t || u.getAttribute("data-webpack") == r + n) {
+                        i = u;
                         break
                     }
                 }
             i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var u = (r, a) => {
+            var c = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                s = setTimeout(u.bind(null, void 0, {
+                s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = u.bind(null, i.onerror), i.onload = u.bind(null, i.onload), d && document.head.appendChild(i)
+            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), d && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -132,15 +132,15 @@
                         (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (d("@amphi/pipeline-components-manager", "0.3.2", (() => Promise.all([S.e(173), S.e(725), S.e(345), S.e(628), S.e(142)]).then((() => () => S(8142))))), d("ace-builds", "1.33.2", (() => S.e(841).then((() => () => S(1841))))), d("antd", "5.16.4", (() => Promise.all([S.e(422), S.e(173), S.e(345), S.e(628)]).then((() => () => S(5422))))), d("react-ace", "11.0.1", (() => Promise.all([S.e(271), S.e(345), S.e(186)]).then((() => () => S(6271))))), d("react-dnd-html5-backend", "16.0.1", (() => S.e(454).then((() => () => S(6454))))), d("react-dnd", "16.0.1", (() => Promise.all([S.e(12), S.e(345), S.e(85)]).then((() => () => S(4631)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@amphi/pipeline-components-manager", "0.3.3", (() => Promise.all([S.e(173), S.e(725), S.e(345), S.e(628), S.e(142)]).then((() => () => S(8142))))), d("ace-builds", "1.33.3", (() => S.e(841).then((() => () => S(1841))))), d("antd", "5.16.4", (() => Promise.all([S.e(422), S.e(173), S.e(345), S.e(628)]).then((() => () => S(5422))))), d("react-ace", "11.0.1", (() => Promise.all([S.e(271), S.e(345), S.e(186)]).then((() => () => S(6271))))), d("react-dnd-html5-backend", "16.0.1", (() => S.e(454).then((() => () => S(6454))))), d("react-dnd", "16.0.1", (() => Promise.all([S.e(12), S.e(345), S.e(85)]).then((() => () => S(4631)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -190,33 +190,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, d = 1, l = !0;; d++, i++) {
-                var f, c, u = d < e.length ? (typeof e[d])[0] : "";
-                if (i >= r.length || "o" == (c = (typeof(f = r[i]))[0])) return !l || ("u" == u ? d > a && !n : "" == u != n);
-                if ("u" == c) {
-                    if (!l || "u" != u) return !1
+                var f, u, c = d < e.length ? (typeof e[d])[0] : "";
+                if (i >= r.length || "o" == (u = (typeof(f = r[i]))[0])) return !l || ("u" == c ? d > a && !n : "" == c != n);
+                if ("u" == u) {
+                    if (!l || "u" != c) return !1
                 } else if (l)
-                    if (u == c)
+                    if (c == u)
                         if (d <= a) {
                             if (f != e[d]) return !1
                         } else {
                             if (n ? f > e[d] : f < e[d]) return !1;
                             f != e[d] && (l = !1)
                         }
-                else if ("s" != u && "n" != u) {
+                else if ("s" != c && "n" != c) {
                     if (n || d <= a) return !1;
                     l = !1, d--
                 } else {
-                    if (d <= a || c < u != n) return !1;
+                    if (d <= a || u < c != n) return !1;
                     l = !1
-                } else "s" != u && "n" != u && (l = !1, d--)
+                } else "s" != c && "n" != c && (l = !1, d--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
@@ -227,63 +227,63 @@
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
         var n = d(e, t);
-        return o(a, n) || u(l(e, t, n, a)), s(e[t][n])
-    }, c = (e, r, t) => {
+        return o(a, n) || c(l(e, t, n, a)), s(e[t][n])
+    }, u = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, u = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, a, n)) : e(r, S.S[r], t, a, n)
-    })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), m = p(((e, r, t, a, n) => {
-        var o = r && S.o(r, t) && c(r, t, a);
+    })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), b = p(((e, r, t, a, n) => {
+        var o = r && S.o(r, t) && u(r, t, a);
         return o ? s(o) : n()
-    })), b = {}, v = {
+    })), m = {}, v = {
         3345: () => h("default", "react", [1, 18, 2, 0]),
         7628: () => h("default", "react-dom", [1, 18, 2, 0]),
-        1029: () => m("default", "react-dnd-html5-backend", [1, 16, 0, 1], (() => S.e(454).then((() => () => S(6454))))),
+        1029: () => b("default", "react-dnd-html5-backend", [1, 16, 0, 1], (() => S.e(454).then((() => () => S(6454))))),
         1527: () => h("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
         4670: () => h("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
-        4761: () => m("default", "react-ace", [1, 11, 0, 1], (() => Promise.all([S.e(271), S.e(186)]).then((() => () => S(6271))))),
-        4810: () => m("default", "antd", [4, 5, 16, 4], (() => S.e(422).then((() => () => S(5422))))),
+        4761: () => b("default", "react-ace", [1, 11, 0, 1], (() => Promise.all([S.e(271), S.e(186)]).then((() => () => S(6271))))),
+        4810: () => b("default", "antd", [4, 5, 16, 4], (() => S.e(422).then((() => () => S(5422))))),
         5256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        5709: () => m("default", "react-dnd", [1, 16, 0, 1], (() => S.e(12).then((() => () => S(4631))))),
+        5709: () => b("default", "react-dnd", [1, 16, 0, 1], (() => S.e(12).then((() => () => S(4631))))),
         5923: () => h("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
         7262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         8702: () => h("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
-        9186: () => m("default", "ace-builds", [1, 1, 32, 8], (() => S.e(841).then((() => () => S(1841)))))
+        9186: () => b("default", "ace-builds", [1, 1, 32, 8], (() => S.e(841).then((() => () => S(1841)))))
     }, g = {
         142: [1029, 1527, 4670, 4761, 4810, 5256, 5709, 5923, 7262, 8702],
         186: [9186],
         345: [3345],
         628: [7628]
     }, y = {}, S.f.consumes = (e, r) => {
         S.o(g, e) && g[e].forEach((e => {
-            if (S.o(b, e)) return r.push(b[e]);
+            if (S.o(m, e)) return r.push(m[e]);
             if (!y[e]) {
                 var t = r => {
-                    b[e] = 0, S.m[e] = t => {
+                    m[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
                 };
                 y[e] = !0;
                 var a = r => {
-                    delete b[e], S.m[e] = t => {
+                    delete m[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
                 try {
                     var n = v[e]();
-                    n.then ? r.push(b[e] = n.then(t).catch(a)) : t(n)
+                    n.then ? r.push(m[e] = n.then(t).catch(a)) : t(n)
                 } catch (e) {
                     a(e)
                 }
             }
         }))
     }, (() => {
         var e = {
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-components-manager/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998046875%*

 * *Differences: {"'packages'": "{20: {'versionInfo': '1.33.3'}, 79: {'versionInfo': '5.41.0'}, 80: {'versionInfo': "*

 * *               "'3.14.0'}}"}*

```diff
@@ -120,15 +120,15 @@
             "name": "@reactflow/core",
             "versionInfo": "11.7.2"
         },
         {
             "extractedText": "Copyright (c) 2010, Ajax.org B.V.\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n    * Redistributions of source code must retain the above copyright\n      notice, this list of conditions and the following disclaimer.\n    * Redistributions in binary form must reproduce the above copyright\n      notice, this list of conditions and the following disclaimer in the\n      documentation and/or other materials provided with the distribution.\n    * Neither the name of Ajax.org B.V. nor the\n      names of its contributors may be used to endorse or promote products\n      derived from this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\" AND\nANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED\nWARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL AJAX.ORG B.V. BE LIABLE FOR ANY\nDIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES\n(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;\nLOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND\nON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT\n(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS\nSOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "ace-builds",
-            "versionInfo": "1.33.2"
+            "versionInfo": "1.33.3"
         },
         {
             "extractedText": "MIT LICENSE\n\nCopyright (c) 2015-present Ant UED, https://xtech.antfin.com/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "antd",
             "versionInfo": "5.16.4"
         },
@@ -474,21 +474,21 @@
             "name": "rc-upload",
             "versionInfo": "4.5.2"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014-present yiminghe\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-util",
-            "versionInfo": "5.40.1"
+            "versionInfo": "5.41.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.12.0"
+            "versionInfo": "3.14.0"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react",
             "versionInfo": "18.3.1"
         },
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.3.4'"}*

```diff
@@ -45,19 +45,14 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.9e0521f3ade01710154b.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
                 "singleton": true
             },
@@ -103,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.3.4"
 }
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt` & `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/412.23a82146827c21626eae.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/412.23a82146827c21626eae.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/735.c92310c8c2bc6a1bb9f6.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/735.711b3b299b885104b862.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 735.c92310c8c2bc6a1bb9f6.js.LICENSE.txt */
+/*! For license information please see 735.711b3b299b885104b862.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_editor = self.webpackChunk_amphi_pipeline_editor || []).push([
     [735], {
         1735: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 Affix: () => Wr,
                 Alert: () => Ta,
@@ -182,15 +182,18 @@
                 S = n.n(w);
 
             function E(e) {
                 return e instanceof HTMLElement || e instanceof SVGElement
             }
 
             function k(e) {
-                return e && "object" === b(e) && E(e.nativeElement) ? e.nativeElement : E(e) ? e : e instanceof r().Component ? S().findDOMNode(e) : null
+                var t, n = function(e) {
+                    return e && "object" === b(e) && E(e.nativeElement) ? e.nativeElement : E(e) ? e : null
+                }(e);
+                return n || (e instanceof r().Component ? null === (t = S().findDOMNode) || void 0 === t ? void 0 : t.call(S(), e) : null)
             }
 
             function O(e, t, n) {
                 var r = o.useRef({});
                 return "value" in r.current && !n(r.current.condition, t) || (r.current.value = e(), r.current.condition = t), r.current.value
             }
             var I = function(e, t) {
@@ -15859,48 +15862,49 @@
                     }), [D.id, D.maps]),
                     W = A && p && (Math.max(s * p.length, F) > c || !!y),
                     _ = "rtl" === v,
                     V = a()(r, C({}, "".concat(r, "-rtl"), _), i),
                     K = p || Hg,
                     q = (0, o.useRef)(),
                     X = (0, o.useRef)(),
-                    G = He((0, o.useState)(0), 2),
-                    Y = G[0],
-                    U = G[1],
-                    Q = He((0, o.useState)(0), 2),
-                    Z = Q[0],
-                    J = Q[1],
-                    ee = He((0, o.useState)(!1), 2),
-                    te = ee[0],
-                    ne = ee[1],
-                    oe = function() {
-                        ne(!0)
-                    },
+                    G = (0, o.useRef)(),
+                    Y = He((0, o.useState)(0), 2),
+                    U = Y[0],
+                    Q = Y[1],
+                    Z = He((0, o.useState)(0), 2),
+                    J = Z[0],
+                    ee = Z[1],
+                    te = He((0, o.useState)(!1), 2),
+                    ne = te[0],
+                    oe = te[1],
                     re = function() {
-                        ne(!1)
+                        oe(!0)
+                    },
+                    ie = function() {
+                        oe(!1)
                     },
-                    ie = {
+                    ae = {
                         getKey: R
                     };
 
-                function ae(e) {
-                    U((function(t) {
+                function le(e) {
+                    Q((function(t) {
                         var n = function(e) {
                             var t = e;
-                            return Number.isNaN(Se.current) || (t = Math.min(t, Se.current)), t = Math.max(t, 0)
+                            return Number.isNaN(Ee.current) || (t = Math.min(t, Ee.current)), t = Math.max(t, 0)
                         }("function" == typeof e ? e(t) : e);
                         return q.current.scrollTop = n, n
                     }))
                 }
-                var le = (0, o.useRef)({
+                var ce = (0, o.useRef)({
                         start: 0,
                         end: K.length
                     }),
-                    ce = (0, o.useRef)(),
-                    se = He(function(e, t, n) {
+                    se = (0, o.useRef)(),
+                    ue = He(function(e, t, n) {
                         var r = He(o.useState(e), 2),
                             i = r[0],
                             a = r[1],
                             l = He(o.useState(null), 2),
                             c = l[0],
                             s = l[1];
                         return o.useEffect((function() {
@@ -15927,16 +15931,16 @@
                                     index: s,
                                     multiple: u
                                 }
                             }(i || [], e || [], t);
                             void 0 !== (null == o ? void 0 : o.index) && (null == n || n(o.index), s(e[o.index])), a(e)
                         }), [e]), [c]
                     }(K, R), 1)[0];
-                ce.current = se;
-                var ue = o.useMemo((function() {
+                se.current = ue;
+                var de = o.useMemo((function() {
                         if (!A) return {
                             scrollHeight: void 0,
                             start: 0,
                             end: K.length - 1,
                             offset: void 0
                         };
                         var e;
@@ -15947,83 +15951,83 @@
                             offset: void 0
                         };
                         for (var t, n, o, r = 0, i = K.length, a = 0; a < i; a += 1) {
                             var l = K[a],
                                 u = R(l),
                                 d = D.get(u),
                                 f = r + (void 0 === d ? s : d);
-                            f >= Y && void 0 === t && (t = a, n = r), f > Y + c && void 0 === o && (o = a), r = f
+                            f >= U && void 0 === t && (t = a, n = r), f > U + c && void 0 === o && (o = a), r = f
                         }
                         return void 0 === t && (t = 0, n = 0, o = Math.ceil(c / s)), void 0 === o && (o = K.length - 1), {
                             scrollHeight: r,
                             start: t,
                             end: o = Math.min(o + 1, K.length - 1),
                             offset: n
                         }
-                    }), [W, A, Y, K, L, c]),
-                    de = ue.scrollHeight,
-                    fe = ue.start,
-                    pe = ue.end,
-                    me = ue.offset;
-                le.current.start = fe, le.current.end = pe;
-                var ge = He(o.useState({
+                    }), [W, A, U, K, L, c]),
+                    fe = de.scrollHeight,
+                    pe = de.start,
+                    me = de.end,
+                    ge = de.offset;
+                ce.current.start = pe, ce.current.end = me;
+                var he = He(o.useState({
                         width: 0,
                         height: c
                     }), 2),
-                    he = ge[0],
-                    be = ge[1],
-                    ye = (0, o.useRef)(),
+                    be = he[0],
+                    ye = he[1],
                     Ce = (0, o.useRef)(),
-                    xe = o.useMemo((function() {
-                        return Tg(he.width, y)
-                    }), [he.width, y]),
+                    xe = (0, o.useRef)(),
                     $e = o.useMemo((function() {
-                        return Tg(he.height, de)
-                    }), [he.height, de]),
-                    we = de - c,
-                    Se = (0, o.useRef)(we);
-                Se.current = we;
-                var Ee = Y <= 0,
-                    ke = Y >= we,
-                    Oe = Og(Ee, ke),
-                    Ie = function() {
+                        return Tg(be.width, y)
+                    }), [be.width, y]),
+                    we = o.useMemo((function() {
+                        return Tg(be.height, fe)
+                    }), [be.height, fe]),
+                    Se = fe - c,
+                    Ee = (0, o.useRef)(Se);
+                Ee.current = Se;
+                var ke = U <= 0,
+                    Oe = U >= Se,
+                    Ie = Og(ke, Oe),
+                    Me = function() {
                         return {
-                            x: _ ? -Z : Z,
-                            y: Y
+                            x: _ ? -J : J,
+                            y: U
                         }
                     },
-                    Me = (0, o.useRef)(Ie()),
-                    je = Vn((function(e) {
+                    je = (0, o.useRef)(Me()),
+                    Pe = Vn((function(e) {
                         if (O) {
-                            var t = $($({}, Ie()), e);
-                            Me.current.x === t.x && Me.current.y === t.y || (O(t), Me.current = t)
+                            var t = $($({}, Me()), e);
+                            je.current.x === t.x && je.current.y === t.y || (O(t), je.current = t)
                         }
                     }));
 
-                function Pe(e, t) {
+                function Re(e, t) {
                     var n = e;
                     t ? ((0, w.flushSync)((function() {
-                        J(n)
-                    })), je()) : ae(n)
+                        ee(n)
+                    })), Pe()) : le(n)
                 }
-                var Re = function(e) {
+                var Te = function(e) {
                         var t = e,
-                            n = y ? y - he.width : 0;
+                            n = y ? y - be.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    Te = Vn((function(e, t) {
+                    ze = Vn((function(e, t) {
                         t ? ((0, w.flushSync)((function() {
-                            J((function(t) {
-                                return Re(t + (_ ? -e : e))
+                            ee((function(t) {
+                                return Te(t + (_ ? -e : e))
                             }))
-                        })), je()) : ae((function(t) {
+                        })), Pe()) : le((function(t) {
                             return t + e
                         }))
                     })),
-                    ze = He(function(e, t, n, r, i) {
+                    Be = He(function(e, t, n, r, i) {
                         var a = (0, o.useRef)(0),
                             l = (0, o.useRef)(null),
                             c = (0, o.useRef)(null),
                             s = (0, o.useRef)(!1),
                             u = Og(t, n),
                             d = (0, o.useRef)(null),
                             f = (0, o.useRef)(null);
@@ -16048,17 +16052,17 @@
                                 }(t, g) : function(e, t) {
                                     i(t, !0), kg || e.preventDefault()
                                 }(t, m)
                             }
                         }, function(t) {
                             e && (s.current = t.detail === c.current)
                         }]
-                    }(A, Ee, ke, !!y, Te), 2),
-                    Be = ze[0],
-                    De = ze[1];
+                    }(A, ke, Oe, !!y, ze), 2),
+                    De = Be[0],
+                    Le = Be[1];
                 ! function(e, t, n) {
                     var r, i = (0, o.useRef)(!1),
                         a = (0, o.useRef)(0),
                         l = (0, o.useRef)(null),
                         c = (0, o.useRef)(null),
                         s = function(e) {
                             if (i.current) {
@@ -16081,40 +16085,40 @@
                         return e && t.current.addEventListener("touchstart", d),
                             function() {
                                 var e;
                                 null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", d), r(), clearInterval(c.current)
                             }
                     }), [e])
                 }(A, q, (function(e, t) {
-                    return !Oe(e, t) && (Be({
+                    return !Ie(e, t) && (De({
                         preventDefault: function() {},
                         deltaY: e
                     }), !0)
                 })), kt((function() {
                     function e(e) {
                         A && e.preventDefault()
                     }
                     var t = q.current;
-                    return t.addEventListener("wheel", Be), t.addEventListener("DOMMouseScroll", De), t.addEventListener("MozMousePixelScroll", e),
+                    return t.addEventListener("wheel", De), t.addEventListener("DOMMouseScroll", Le), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", Be), t.removeEventListener("DOMMouseScroll", De), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", De), t.removeEventListener("DOMMouseScroll", Le), t.removeEventListener("MozMousePixelScroll", e)
                         }
                 }), [A]), kt((function() {
                     if (y) {
-                        var e = Re(Z);
-                        J(e), je({
+                        var e = Te(J);
+                        ee(e), Pe({
                             x: e
                         })
                     }
-                }), [he.width, y]);
-                var Le = function() {
+                }), [be.width, y]);
+                var Ae = function() {
                         var e, t;
-                        null === (e = ye.current) || void 0 === e || e.delayHidden(), null === (t = Ce.current) || void 0 === t || t.delayHidden()
+                        null === (e = Ce.current) || void 0 === e || e.delayHidden(), null === (t = xe.current) || void 0 === t || t.delayHidden()
                     },
-                    Ae = function(e, t, n, r, i, a, l, c) {
+                    Fe = function(e, t, n, r, i, a, l, c) {
                         var s = o.useRef(),
                             u = He(o.useState(null), 2),
                             d = u[0],
                             f = u[1];
                         return kt((function() {
                                 if (d && d.times < 10) {
                                     if (!e.current) return void f((function(e) {
@@ -16181,30 +16185,31 @@
                                             originAlign: o
                                         })
                                     }
                                 } else c()
                             }
                     }(q, K, D, s, R, (function() {
                         return B(!0)
-                    }), ae, Le);
+                    }), le, Ae);
                 o.useImperativeHandle(t, (function() {
                     return {
-                        getScrollInfo: Ie,
+                        nativeElement: G.current,
+                        getScrollInfo: Me,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === b(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && J(Re(e.left)), Ae(e.top)) : Ae(e)
+                            (t = e) && "object" === b(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ee(Te(e.left)), Fe(e.top)) : Fe(e)
                         }
                     }
                 })), kt((function() {
                     if (I) {
-                        var e = K.slice(fe, pe + 1);
+                        var e = K.slice(pe, me + 1);
                         I(e, K)
                     }
-                }), [fe, pe, K]);
-                var Fe = function(e, t, n, r) {
+                }), [pe, me, K]);
+                var We = function(e, t, n, r) {
                         var i = He(o.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, r]), 2),
                             a = i[0],
                             l = i[1];
                         return function(o) {
                             var i = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : o,
@@ -16220,99 +16225,101 @@
                                 }
                             return {
                                 top: l[c - 1] || 0,
                                 bottom: l[s]
                             }
                         }
                     }(K, R, D, s),
-                    We = null == M ? void 0 : M({
-                        start: fe,
-                        end: pe,
+                    _e = null == M ? void 0 : M({
+                        start: pe,
+                        end: me,
                         virtual: W,
-                        offsetX: Z,
-                        offsetY: me,
+                        offsetX: J,
+                        offsetY: ge,
                         rtl: _,
-                        getSize: Fe
+                        getSize: We
                     }),
-                    _e = function(e, t, n, r, i, a, l) {
-                        var c = l.getKey;
+                    Ve = function(e, t, n, r, i, a, l, c) {
+                        var s = c.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
-                            var l = a(e, t + n, {
+                            var c = l(e, t + n, {
                                     style: {
                                         width: r
-                                    }
+                                    },
+                                    offsetX: i
                                 }),
-                                s = c(e);
+                                u = s(e);
                             return o.createElement(Eg, {
-                                key: s,
+                                key: u,
                                 setRef: function(t) {
-                                    return i(e, t)
+                                    return a(e, t)
                                 }
-                            }, l)
+                            }, c)
                         }))
-                    }(K, fe, pe, y, H, m, ie),
-                    Ve = null;
-                c && (Ve = $(C({}, d ? "height" : "maxHeight", c), Bg), A && (Ve.overflowY = "hidden", y && (Ve.overflowX = "hidden"), te && (Ve.pointerEvents = "none")));
-                var Ke = {};
-                return _ && (Ke.dir = "rtl"), o.createElement("div", l({
+                    }(K, pe, me, y, J, H, m, ae),
+                    Ke = null;
+                c && (Ke = $(C({}, d ? "height" : "maxHeight", c), Bg), A && (Ke.overflowY = "hidden", y && (Ke.overflowX = "hidden"), ne && (Ke.pointerEvents = "none")));
+                var qe = {};
+                return _ && (qe.dir = "rtl"), o.createElement("div", l({
+                    ref: G,
                     style: $($({}, f), {}, {
                         position: "relative"
                     }),
                     className: V
-                }, Ke, P), o.createElement(ve, {
+                }, qe, P), o.createElement(ve, {
                     onResize: function(e) {
-                        be({
+                        ye({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, o.createElement(S, {
                     className: "".concat(r, "-holder"),
-                    style: Ve,
+                    style: Ke,
                     ref: q,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== Y && ae(t), null == E || E(e), je()
+                        t !== U && le(t), null == E || E(e), Pe()
                     },
-                    onMouseEnter: Le
+                    onMouseEnter: Ae
                 }, o.createElement(Sg, {
                     prefixCls: r,
-                    height: de,
-                    offsetX: Z,
-                    offsetY: me,
+                    height: fe,
+                    offsetX: J,
+                    offsetY: ge,
                     scrollWidth: y,
                     onInnerResize: B,
                     ref: X,
                     innerProps: N,
                     rtl: _,
-                    extra: We
-                }, _e))), W && de > c && o.createElement(Pg, {
-                    ref: ye,
+                    extra: _e
+                }, Ve))), W && fe > c && o.createElement(Pg, {
+                    ref: Ce,
                     prefixCls: r,
-                    scrollOffset: Y,
-                    scrollRange: de,
+                    scrollOffset: U,
+                    scrollRange: fe,
                     rtl: _,
-                    onScroll: Pe,
-                    onStartMove: oe,
-                    onStopMove: re,
-                    spinSize: $e,
-                    containerSize: he.height,
+                    onScroll: Re,
+                    onStartMove: re,
+                    onStopMove: ie,
+                    spinSize: we,
+                    containerSize: be.height,
                     style: null == j ? void 0 : j.verticalScrollBar,
                     thumbStyle: null == j ? void 0 : j.verticalScrollBarThumb
-                }), W && y > he.width && o.createElement(Pg, {
-                    ref: Ce,
+                }), W && y > be.width && o.createElement(Pg, {
+                    ref: xe,
                     prefixCls: r,
-                    scrollOffset: Z,
+                    scrollOffset: J,
                     scrollRange: y,
                     rtl: _,
-                    onScroll: Pe,
-                    onStartMove: oe,
-                    onStopMove: re,
-                    spinSize: xe,
-                    containerSize: he.width,
+                    onScroll: Re,
+                    onStartMove: re,
+                    onStopMove: ie,
+                    spinSize: $e,
+                    containerSize: be.width,
                     horizontal: !0,
                     style: null == j ? void 0 : j.horizontalScrollBar,
                     thumbStyle: null == j ? void 0 : j.horizontalScrollBarThumb
                 }))
             }
             var Lg = o.forwardRef(Dg);
             Lg.displayName = "List";
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/735.c92310c8c2bc6a1bb9f6.js.LICENSE.txt` & `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/735.711b3b299b885104b862.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/remoteEntry.9e0521f3ade01710154b.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/remoteEntry.bfb171550404534afb06.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, l, u, f, d, s, p, c, h, v, b, m, g, y, w, j, P, S, E = {
+    var e, r, t, a, n, o, i, l, u, f, s, d, p, c, h, v, m, b, g, y, w, j, P, S, E = {
             8535: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(345), t.e(550), t.e(412)]).then((() => () => t(8412))),
                         "./extension": () => Promise.all([t.e(345), t.e(550), t.e(412)]).then((() => () => t(8412))),
                         "./style": () => Promise.all([t.e(550), t.e(631)]).then((() => () => t(7631)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -49,53 +49,53 @@
     }, _.f = {}, _.e = e => Promise.all(Object.keys(_.f).reduce(((r, t) => (_.f[t](e, r), r)), [])), _.u = e => e + "." + {
         285: "f1fef15430d9554bfba0",
         345: "4aa5390d29af88207b53",
         412: "23a82146827c21626eae",
         550: "025783cb8476390cbadc",
         628: "d05f56a756fb73f1c255",
         631: "20cdac1e84cf987a8781",
-        735: "c92310c8c2bc6a1bb9f6"
+        735: "711b3b299b885104b862"
     } [e] + ".js?v=" + {
         285: "f1fef15430d9554bfba0",
         345: "4aa5390d29af88207b53",
         412: "23a82146827c21626eae",
         550: "025783cb8476390cbadc",
         628: "d05f56a756fb73f1c255",
         631: "20cdac1e84cf987a8781",
-        735: "c92310c8c2bc6a1bb9f6"
+        735: "711b3b299b885104b862"
     } [e], _.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), _.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-editor:", _.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== n)
                 for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var d = u[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                    var s = u[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
+                        i = s;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, _.nc && i.setAttribute("nonce", _.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var s = (r, a) => {
+            var d = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, _.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -117,15 +117,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-editor", "0.3.2", (() => Promise.all([_.e(345), _.e(550), _.e(412)]).then((() => () => _(8412))))), l("antd", "5.16.4", (() => Promise.all([_.e(735), _.e(628), _.e(345)]).then((() => () => _(1735))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(628), _.e(345)]).then((() => () => _(1285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-editor", "0.3.3", (() => Promise.all([_.e(345), _.e(550), _.e(412)]).then((() => () => _(8412))))), l("antd", "5.16.4", (() => Promise.all([_.e(735), _.e(628), _.e(345)]).then((() => () => _(1735))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(628), _.e(345)]).then((() => () => _(1285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         _.g.importScripts && (e = _.g.location + "");
         var r = _.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -175,33 +175,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, d, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !u || ("u" == s ? l > a && !n : "" == s != n);
-                if ("u" == d) {
-                    if (!u || "u" != s) return !1
+                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > a && !n : "" == d != n);
+                if ("u" == s) {
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (s == d)
+                    if (d == s)
                         if (l <= a) {
                             if (f != e[l]) return !1
                         } else {
                             if (n ? f > e[l] : f < e[l]) return !1;
                             f != e[l] && (u = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (n || l <= a) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || d < s != n) return !1;
+                    if (l <= a || s < d != n) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -213,37 +213,37 @@
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", d = (e, r, t, a) => {
+    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", s = (e, r, t, a) => {
         var n = u(e, t);
         return o(a, n) || c(f(e, t, n, a)), v(e[t][n])
-    }, s = (e, r, t) => {
+    }, d = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, p = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, a) => {
         c(p(e, r, t, a))
-    }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, a, n) {
+    }, v = e => (e.loaded = 1, e.get()), b = (m = e => function(r, t, a, n) {
         var o = _.I(r);
         return o && o.then ? o.then(e.bind(e, r, _.S[r], t, a, n)) : e(r, _.S[r], t, a, n)
-    })(((e, r, t, a) => (i(e, t), v(s(r, t, a) || h(r, e, t, a) || l(r, t))))), g = b(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), y = b(((e, r, t, a, n) => {
-        var o = r && _.o(r, t) && s(r, t, a);
+    })(((e, r, t, a) => (i(e, t), v(d(r, t, a) || h(r, e, t, a) || l(r, t))))), g = m(((e, r, t, a) => (i(e, t), s(r, 0, t, a)))), y = m(((e, r, t, a, n) => {
+        var o = r && _.o(r, t) && d(r, t, a);
         return o ? v(o) : n()
     })), w = {}, j = {
         3345: () => g("default", "react", [1, 18, 2, 0]),
         1527: () => g("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
-        2774: () => m("default", "@jupyterlab/docregistry", [1, 4, 2, 0]),
+        2774: () => b("default", "@jupyterlab/docregistry", [1, 4, 2, 0]),
         2825: () => g("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
         3254: () => g("default", "@amphi/pipeline-components-manager", [0]),
         3613: () => y("default", "reactflow", [4, 11, 9, 4], (() => Promise.all([_.e(285), _.e(628)]).then((() => () => _(1285))))),
         4236: () => g("default", "@jupyterlab/rendermime", [1, 4, 2, 0]),
         4670: () => g("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
         4810: () => y("default", "antd", [4, 5, 16, 4], (() => Promise.all([_.e(735), _.e(628)]).then((() => () => _(1735))))),
         5923: () => g("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-editor/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985632183908046%*

 * *Differences: {"'packages'": "{74: {'versionInfo': '5.41.0'}, 75: {'versionInfo': '3.14.0'}}"}*

```diff
@@ -444,21 +444,21 @@
             "name": "rc-upload",
             "versionInfo": "4.5.2"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014-present yiminghe\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-util",
-            "versionInfo": "5.40.1"
+            "versionInfo": "5.41.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.12.0"
+            "versionInfo": "3.14.0"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react-is",
             "versionInfo": "18.3.1"
         },
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/package.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.871deda2d395cf3ebdb5.js'}}",*

 * * "'version'": "'0.3.3'"}*

```diff
@@ -52,15 +52,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5034e9c3d84820fce19f.js",
+            "load": "static/remoteEntry.871deda2d395cf3ebdb5.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-log-console",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.3.3"
 }
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/432.4a34574395b64c0ecb2a.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             t.d(e, {
                 A: () => c
             });
             var o = t(6758),
                 r = t.n(o),
                 a = t(935),
                 i = t.n(a)()(r());
-            i.push([n.id, ".amphi-Console {\n  flex-direction: column;\n  overflow: auto;\n  font-size: var(--jp-ui-font-size0);\n}\n\n.amphi-Console-table {\n  font-family: monospace;\n  border-collapse: collapse;\n  margin: auto;\n  width: 100%;\n  color: var(--jp-content-font-color1);\n}\n\n.amphi-Console-table-row {\n}\n\n.amphi-Console-date {\n  vertical-align: top;\n  width: 9em;\n  min-width: 9em;\n  max-width: 9em;\n}\n\n.amphi-Console pre {\n  font-size: 11px;\n}\n\n.amphi-Console-title {\n  font-size: var(--jp-ui-font-size1);\n  color: var(--jp-content-font-color1);\n  text-align: left;\n  padding-left: 10px;\n}\n\n.type-button {\n  color: var(--jp-ui-font-color0);\n}\n\n.name-button {\n  color: var(--jp-ui-font-color1);\n}\n\n.filter-list {\n  display: flex;\n}", ""]);
+            i.push([n.id, ".amphi-Console {\n  flex-direction: column;\n  overflow: auto;\n  font-size: var(--jp-ui-font-size0);\n}\n\n.amphi-Console-table {\n  font-family: monospace;\n  border-collapse: collapse;\n  margin: auto;\n  width: 100%;\n  max-width: 100%;\n  color: var(--jp-content-font-color1);\n}\n\n.amphi-Console-table-row td {\n  word-wrap: break-word;\n  white-space: normal;\n}\n\n.amphi-Console-table-row div, .amphi-Console-table-row pre {\n  word-wrap: break-word;\n  white-space: normal;\n}\n\n.amphi-Console-date {\n  vertical-align: top;\n  width: 9em;\n  min-width: 9em;\n  max-width: 9em;\n}\n\n.amphi-Console pre {\n  font-size: 11px;\n}\n\n.amphi-Console-title {\n  font-size: var(--jp-ui-font-size1);\n  color: var(--jp-content-font-color1);\n  text-align: left;\n  padding-left: 10px;\n}\n\n.type-button {\n  color: var(--jp-ui-font-color0);\n}\n\n.name-button {\n  color: var(--jp-ui-font-color1);\n}\n\n.filter-list {\n  display: flex;\n}", ""]);
             const c = i
         },
         935: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
@@ -28,16 +28,16 @@
                     var i = {};
                     if (o)
                         for (var c = 0; c < this.length; c++) {
                             var s = this[c][0];
                             null != s && (i[s] = !0)
                         }
                     for (var l = 0; l < n.length; l++) {
-                        var u = [].concat(n[l]);
-                        o && i[u[0]] || (void 0 !== a && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = a), t && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = t) : u[2] = t), r && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = r) : u[4] = "".concat(r)), e.push(u))
+                        var p = [].concat(n[l]);
+                        o && i[p[0]] || (void 0 !== a && (void 0 === p[5] || (p[1] = "@layer".concat(p[5].length > 0 ? " ".concat(p[5]) : "", " {").concat(p[1], "}")), p[5] = a), t && (p[2] ? (p[1] = "@media ".concat(p[2], " {").concat(p[1], "}"), p[2] = t) : p[2] = t), r && (p[4] ? (p[1] = "@supports (".concat(p[4], ") {").concat(p[1], "}"), p[4] = r) : p[4] = "".concat(r)), e.push(p))
                     }
                 }, e
             }
         },
         6758: n => {
             n.exports = function(n) {
                 return n[1]
@@ -54,35 +54,35 @@
                     } return t
             }
 
             function o(n, o) {
                 for (var a = {}, i = [], c = 0; c < n.length; c++) {
                     var s = n[c],
                         l = o.base ? s[0] + o.base : s[0],
-                        u = a[l] || 0,
-                        p = "".concat(l, " ").concat(u);
-                    a[l] = u + 1;
-                    var f = t(p),
+                        p = a[l] || 0,
+                        u = "".concat(l, " ").concat(p);
+                    a[l] = p + 1;
+                    var f = t(u),
                         d = {
                             css: s[1],
                             media: s[2],
                             sourceMap: s[3],
                             supports: s[4],
                             layer: s[5]
                         };
                     if (-1 !== f) e[f].references++, e[f].updater(d);
                     else {
                         var m = r(d, o);
                         o.byIndex = c, e.splice(c, 0, {
-                            identifier: p,
+                            identifier: u,
                             updater: m,
                             references: 1
                         })
                     }
-                    i.push(p)
+                    i.push(u)
                 }
                 return i
             }
 
             function r(n, e) {
                 var t = e.domAPI(e);
                 return t.update(n),
@@ -98,16 +98,16 @@
                 return function(n) {
                     n = n || [];
                     for (var i = 0; i < a.length; i++) {
                         var c = t(a[i]);
                         e[c].references--
                     }
                     for (var s = o(n, r), l = 0; l < a.length; l++) {
-                        var u = t(a[l]);
-                        0 === e[u].references && (e[u].updater(), e.splice(u, 1))
+                        var p = t(a[l]);
+                        0 === e[p].references && (e[p].updater(), e.splice(p, 1))
                     }
                     a = s
                 }
             }
         },
         8128: n => {
             var e = {};
@@ -181,18 +181,18 @@
             var o = t(2591),
                 r = t.n(o),
                 a = t(1740),
                 i = t.n(a),
                 c = t(8128),
                 s = t.n(c),
                 l = t(855),
-                u = t.n(l),
-                p = t(3051),
-                f = t.n(p),
+                p = t.n(l),
+                u = t(3051),
+                f = t.n(u),
                 d = t(3656),
                 m = t.n(d),
                 v = t(4296),
                 h = {};
-            h.styleTagTransform = m(), h.setAttributes = u(), h.insert = s().bind(null, "head"), h.domAPI = i(), h.insertStyleElement = f(), r()(v.A, h), v.A && v.A.locals && v.A.locals
+            h.styleTagTransform = m(), h.setAttributes = p(), h.insert = s().bind(null, "head"), h.domAPI = i(), h.insertStyleElement = f(), r()(v.A, h), v.A && v.A.locals && v.A.locals
         }
     }
 ]);
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/684.c971d4662ee41caa2dda.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,35 +1,35 @@
 "use strict";
 (self.webpackChunk_amphi_pipeline_log_console = self.webpackChunk_amphi_pipeline_log_console || []).push([
     [684], {
-        684: (e, t, n) => {
-            n.r(t), n.d(t, {
-                default: () => H
+        684: (e, t, s) => {
+            s.r(t), s.d(t, {
+                default: () => I
             });
-            var s = n(5923),
-                o = n(9626),
-                i = n(4236),
-                r = n(1527),
-                a = n(5881),
-                l = n(4602);
+            var n = s(5923),
+                o = s(9626),
+                i = s(4236),
+                r = s(1527),
+                l = s(5881),
+                a = s(4602);
             class c {
                 constructor(e) {
-                    this._isDisposed = !1, this._disposed = new l.Signal(this), this._rendermime = null, this._connector = e
+                    this._isDisposed = !1, this._disposed = new a.Signal(this), this._rendermime = null, this._connector = e
                 }
                 get disposed() {
                     return this._disposed
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get rendermime() {
                     return this._rendermime
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, this._disposed.emit(), l.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, this._disposed.emit(), a.Signal.clearData(this))
                 }
             }
             class d extends c {
                 constructor(e) {
                     var t;
                     super(e.connector), this._id = e.id, this._rendermime = null !== (t = e.rendermime) && void 0 !== t ? t : null, this._ready = this._connector.ready, this._connector.kernelRestarted.connect(((e, t) => {
                         this._ready = this._connector.ready
@@ -40,17 +40,18 @@
                 }
                 get ready() {
                     return this._ready
                 }
             }
             class h {
                 constructor(e) {
-                    this._kernelRestarted = new l.Signal(this), this._session = e.session, this._session.statusChanged.connect(((e, t) => {
+                    this._kernelRestarted = new a.Signal(this), this._session = e.session, this._session.statusChanged.connect(((e, t) => {
                         switch (t) {
                             case "restarting":
+                                this._kernelRestarted.emit(this._session.ready);
                             case "autorestarting":
                                 this._kernelRestarted.emit(this._session.ready)
                         }
                     }))
                 }
                 get kernelRestarted() {
                     return this._kernelRestarted
@@ -64,162 +65,154 @@
                 }
                 get ready() {
                     return this._session.ready
                 }
                 get iopubMessage() {
                     return this._session.iopubMessage
                 }
+                execute(e) {
+                    var t;
+                    if (!(null === (t = this._session.session) || void 0 === t ? void 0 : t.kernel)) throw new Error("No session available.");
+                    return this._session.session.kernel.requestExecute(e)
+                }
             }
-            var p = n(5256),
-                u = n(3345),
-                m = n.n(u),
-                _ = n(7628),
-                g = n.n(_),
-                y = n(931),
-                v = n(5180);
+            var p = s(5256),
+                u = s(3345),
+                m = s.n(u),
+                _ = s(7628),
+                g = s.n(_),
+                y = s(931),
+                v = s(1047);
             const C = ({
                 htmlData: e
             }) => {
-                const [t, n] = (0, u.useState)([]), [s, o] = (0, u.useState)([]);
+                const [t, s] = (0, u.useState)([]), [n, o] = (0, u.useState)([]);
                 return (0, u.useEffect)((() => {
+                    console.log("DATA %o", e);
                     const {
                         data: t,
-                        headers: s
+                        headers: n
                     } = function(e) {
                         const t = (new DOMParser).parseFromString(e, "text/html");
-                        let n = Array.from(t.querySelectorAll("table thead th")).map((e => {
-                            var t, n;
-                            return null !== (n = null === (t = e.textContent) || void 0 === t ? void 0 : t.trim()) && void 0 !== n ? n : ""
+                        let s = Array.from(t.querySelectorAll("table thead th")).map((e => {
+                            var t, s;
+                            return null !== (s = null === (t = e.textContent) || void 0 === t ? void 0 : t.trim()) && void 0 !== s ? s : ""
                         }));
-                        const s = t.querySelectorAll("table tbody tr");
+                        const n = t.querySelectorAll("table tbody tr");
                         return {
-                            data: Array.from(s, ((e, t) => {
-                                const s = e.querySelectorAll("th, td"),
+                            data: Array.from(n, ((e, t) => {
+                                const n = e.querySelectorAll("th, td"),
                                     o = {
                                         index: t.toString()
                                     };
-                                if (s.length === n.length) s.forEach(((e, t) => {
-                                    var s, i;
-                                    o[n[t]] = null !== (i = null === (s = e.textContent) || void 0 === s ? void 0 : s.trim()) && void 0 !== i ? i : ""
-                                }));
-                                else if (s.length === n.length + 1)["", ...n].forEach(((e, t) => {
+                                if (n.length === s.length) n.forEach(((e, t) => {
                                     var n, i;
-                                    o[e] = null !== (i = null === (n = s[t].textContent) || void 0 === n ? void 0 : n.trim()) && void 0 !== i ? i : ""
+                                    o[s[t]] = null !== (i = null === (n = e.textContent) || void 0 === n ? void 0 : n.trim()) && void 0 !== i ? i : ""
+                                }));
+                                else if (n.length === s.length + 1)["", ...s].forEach(((e, t) => {
+                                    var s, i;
+                                    o[e] = null !== (i = null === (s = n[t].textContent) || void 0 === s ? void 0 : s.trim()) && void 0 !== i ? i : ""
                                 }));
                                 else {
                                     const t = e.querySelectorAll("td");
-                                    n.forEach(((e, n) => {
-                                        var s, i, r;
-                                        o[e] = null !== (r = null === (i = null === (s = t[n]) || void 0 === s ? void 0 : s.textContent) || void 0 === i ? void 0 : i.trim()) && void 0 !== r ? r : ""
+                                    s.forEach(((e, s) => {
+                                        var n, i, r;
+                                        o[e] = null !== (r = null === (i = null === (n = t[s]) || void 0 === n ? void 0 : n.textContent) || void 0 === i ? void 0 : i.trim()) && void 0 !== r ? r : ""
                                     }))
                                 }
                                 return o
                             })),
-                            headers: n
+                            headers: s
                         }
                     }(e);
-                    n(t), o(s.map((e => ({
+                    s(t), o(n.map((e => ({
                         title: e,
                         dataIndex: e,
                         key: e
                     }))))
                 }), [e]), m().createElement(v.A, {
                     dataSource: t,
-                    columns: s,
+                    columns: n,
                     pagination: !1,
                     size: "small"
                 })
             };
-            var f = n(4363),
-                S = n(7516),
-                w = n(3361),
-                x = n(5025),
-                b = n(6198);
+            var f = s(4363),
+                w = s(7516),
+                x = s(3361),
+                S = s(6198);
             const {
-                Text: E
+                Text: k
             } = f.A;
-            class k extends p.Widget {
+            class b extends p.Widget {
                 constructor() {
-                    super(), this._source = null, this.addClass("amphi-Console"), this._title = T.createTitle(), this._title.className = "amphi-Console-title", this._console = T.createConsole(), this._console.className = "amphi-Console-table", this.node.appendChild(this._title), this.node.appendChild(this._console)
+                    super(), this._source = null, this.addClass("amphi-Console"), this._title = E.createTitle(), this._title.className = "amphi-Console-title", this._console = E.createConsole(), this._console.className = "amphi-Console-table", this.node.appendChild(this._title), this.node.appendChild(this._console)
                 }
                 get source() {
                     return this._source
                 }
                 set source(e) {
                     this._source !== e && (this._source && this._source.disposed.disconnect(this.onSourceDisposed, this), this._source = e, this._source && this._source.disposed.connect(this.onSourceDisposed, this))
                 }
                 dispose() {
                     this.isDisposed || (this.source = null, super.dispose())
                 }
-                onNewLog(e, t, n) {
+                onNewLog(e, t, s) {
                     if (!this.isAttached) return;
                     this._console.tFoot || (this._console.createTFoot(), this._console.tFoot.className = "amphi-Console-content");
-                    let s = this._console.tFoot.insertRow(0);
-                    s.className = "amphi-Console-table-row fade-background-transition";
-                    let o, i = s.insertCell(0);
-                    i.innerHTML = `\n    <span>\n      ${y.renderToString(m().createElement(S.A,null,m().createElement(E,null,e)))}\n    </span>\n  `, i.style.padding = "5px", i.className = "amphi-Console-date";
-                    const r = m().createElement(b.A, {
-                        style: {
-                            fontSize: 24
-                        },
-                        spin: !0
-                    });
-                    switch (t) {
-                        case "busy":
-                            i = s.insertCell(1), i.style.padding = "5px", o = document.createElement("div"), i.appendChild(o), g().render(m().createElement(w.A, {
-                                showIcon: !0,
-                                description: m().createElement("div", null, m().createElement(x.A, {
-                                    indicator: r
-                                }), m().createElement("span", {
-                                    dangerouslySetInnerHTML: {
-                                        __html: "Execution in progress..."
-                                    }
-                                })),
-                                type: "info"
-                            }), o);
-                            break;
+                    let n = this._console.tFoot.insertRow(0);
+                    n.className = "amphi-Console-table-row";
+                    let o, i = n.insertCell(0);
+                    switch (i.innerHTML = `\n    <span>\n      ${y.renderToString(m().createElement(w.A,null,m().createElement(k,null,e)))}\n    </span>\n  `, i.style.padding = "5px", i.className = "amphi-Console-date", m().createElement(S.A, {
+                            style: {
+                                fontSize: 24
+                            },
+                            spin: !0
+                        }), t) {
                         case "info":
-                            i = s.insertCell(1), i.style.padding = "5px", o = document.createElement("div"), i.appendChild(o);
-                            let e = /SUCCESS/i.test(n) ? "success" : /ERROR|WARNING/i.test(n) ? "warning" : "info";
-                            g().render(m().createElement(w.A, {
+                            i = n.insertCell(1), i.style.padding = "5px", o = document.createElement("div"), i.appendChild(o);
+                            let e = /SUCCESS/i.test(s) ? "success" : /ERROR|WARNING/i.test(s) ? "warning" : "info";
+                            g().render(m().createElement(x.A, {
                                 showIcon: !0,
-                                description: m().createElement("div", {
+                                message: m().createElement("div", {
                                     dangerouslySetInnerHTML: {
-                                        __html: n
+                                        __html: s
                                     }
                                 }),
                                 type: e
                             }), o);
                             break;
                         case "error":
-                            i = s.insertCell(1), i.style.padding = "5px", o = document.createElement("div"), i.appendChild(o), g().render(m().createElement(w.A, {
+                            i = n.insertCell(1), i.style.padding = "5px", o = document.createElement("div"), i.appendChild(o), g().render(m().createElement(x.A, {
                                 message: "Error",
                                 showIcon: !0,
                                 description: m().createElement("div", {
                                     dangerouslySetInnerHTML: {
-                                        __html: n
+                                        __html: s
                                     }
                                 }),
                                 type: "error"
                             }), o);
                             break;
                         case "data":
-                            i = s.insertCell(1), i.style.padding = "0", o = document.createElement("div"), i.appendChild(o), g().render(m().createElement(C, {
-                                htmlData: n
+                            i = n.insertCell(1), i.style.padding = "5", o = document.createElement("div"), i.appendChild(o), g().render(m().createElement(C, {
+                                htmlData: s
                             }), o)
                     }
-                    this._console.parentElement.scrollTop = 0, setTimeout((() => {
-                        s.style.backgroundColor = ""
-                    }), 3e3)
+                    this._console.parentElement.scrollTop = 0
+                }
+                clearLogs() {
+                    if (this._console.tFoot)
+                        for (; this._console.tFoot.rows.length > 0;) this._console.tFoot.deleteRow(0)
                 }
                 onSourceDisposed(e, t) {
                     this.source = null
                 }
             }
-            var T;
+            var E;
             ! function(e) {
                 const t = new Map(Object.entries({
                     "&": "&amp;",
                     "<": "&lt;",
                     ">": "&gt;",
                     '"': "&quot;",
                     "'": "&#39;",
@@ -229,15 +222,15 @@
                     return String(e).replace(/[&<>"'/]/g, (e => t.get(e)))
                 }, e.createConsole = function() {
                     return document.createElement("table")
                 }, e.createTitle = function(e = "") {
                     const t = document.createElement("p");
                     return t.innerHTML = e, t
                 }
-            }(T || (T = {}));
+            }(E || (E = {}));
             class D {
                 constructor() {
                     this._source = null, this._panel = null, this._handlers = {}
                 }
                 hasHandler(e) {
                     return !!this._handlers[e]
                 }
@@ -259,138 +252,150 @@
                 set source(e) {
                     this._source !== e && (this._source && this._source.disposed.disconnect(this._onSourceDisposed, this), this._source = e, this._panel && !this._panel.isDisposed && (this._panel.source = this._source), this._source && this._source.disposed.connect(this._onSourceDisposed, this))
                 }
                 _onSourceDisposed() {
                     this._source = null
                 }
             }
-            var A = n(7262);
-            const I = new A.Token("jupyterlab_extension/logconsole:IPipelineConsoleManager");
+            var T = s(7262);
+            const A = new T.Token("jupyterlab_extension/logconsole:IPipelineConsoleManager");
             var L;
-            new A.Token("jupyterlab_extension/logconsole:IPipelineConsole"),
+            new T.Token("jupyterlab_extension/logconsole:IPipelineConsole"),
                 function(e) {
                     e.open = "pipeline-console:open"
                 }(L || (L = {}));
-            const H = [{
+            const I = [{
                 id: "@amphi/pipeline-log-console",
-                requires: [s.ICommandPalette, o.ILayoutRestorer, o.ILabShell],
-                provides: I,
+                requires: [n.ICommandPalette, o.ILayoutRestorer, o.ILabShell],
+                provides: A,
                 autoStart: !0,
-                activate: (e, t, n, o) => {
+                activate: (e, t, s, o) => {
                     const i = new D,
-                        a = L.open,
-                        l = new s.WidgetTracker({
+                        l = L.open,
+                        a = new n.WidgetTracker({
                             namespace: "pipeline-console"
                         });
-                    return n.restore(l, {
-                        command: a,
+                    return s.restore(a, {
+                        command: l,
                         args: () => ({}),
                         name: () => "amphi-logConsole"
-                    }), e.commands.addCommand(a, {
+                    }), e.commands.addCommand(l, {
                         label: "Pipeline Console",
                         execute: () => {
                             let t = null;
-                            for (const n of e.shell.widgets("main"))
-                                if ("amphi-metadataPanel" === n.id) {
-                                    t = n;
+                            for (const s of e.shell.widgets("main"))
+                                if ("amphi-metadataPanel" === s.id) {
+                                    t = s;
                                     break
                                 } i.panel && !i.panel.isDisposed || (i.panel = function() {
-                                const e = new k;
+                                const e = new b;
                                 return e.id = "amphi-logConsole", e.title.label = "Pipeline Console", e.title.icon = r.listIcon, e.title.closable = !0, e.disposed.connect((() => {
                                     i.panel === e && (i.panel = null)
-                                })), l.add(e), e
+                                })), a.add(e), e
                             }()), t && t.isAttached ? i.panel.isAttached || e.shell.add(i.panel, "main", {
                                 ref: t.id,
                                 mode: "tab-after"
                             }) : i.panel.isAttached || e.shell.add(i.panel, "main", {
                                 mode: "split-bottom"
                             }), e.shell.activateById(i.panel.id)
                         }
                     }), t.addItem({
-                        command: a,
+                        command: l,
                         category: "Pipeline Console"
+                    }), e.commands.addCommand("pipeline-console:clear", {
+                        execute: () => {
+                            i.panel.clearLogs()
+                        },
+                        label: "Clear Console"
+                    }), e.commands.addCommand("pipeline-console:settings", {
+                        execute: () => {},
+                        label: "Console Settings"
+                    }), e.contextMenu.addItem({
+                        command: "pipeline-console:clear",
+                        selector: ".amphi-Console",
+                        rank: 1
                     }), console.log("JupyterLab extension @amphi/pipeline-log-console is activated!"), i
                 }
             }, {
                 id: "@amphi/pipeline-log-console:pipelines",
-                requires: [I, a.IPipelineTracker, o.ILabShell],
+                requires: [A, l.IPipelineTracker, o.ILabShell],
                 autoStart: !0,
-                activate: (e, t, n, o) => {
+                activate: (e, t, s, o) => {
                     const r = {};
 
-                    function a(e) {
+                    function l(e) {
                         const t = new Date(e);
                         return `${t.toLocaleDateString()}\n${t.toLocaleTimeString()}`
                     }
-                    n.widgetAdded.connect(((e, n) => {
-                        t.hasHandler(n.context.sessionContext.path) ? r[n.id] = new Promise(((e, s) => {
-                            e(t.getHandler(n.context.sessionContext.path))
-                        })) : r[n.id] = new Promise(((e, o) => {
-                            const l = n.context.sessionContext,
+                    s.widgetAdded.connect(((e, s) => {
+                        t.hasHandler(s.context.sessionContext.path) ? r[s.id] = new Promise(((e, n) => {
+                            e(t.getHandler(s.context.sessionContext.path))
+                        })) : r[s.id] = new Promise(((e, o) => {
+                            const a = s.context.sessionContext,
                                 c = new h({
-                                    session: l
+                                    session: a
                                 }),
                                 p = {
                                     connector: c,
-                                    id: l.path
+                                    id: a.path
                                 },
                                 u = new d(p);
-                            t.addHandler(u), n.disposed.connect((() => {
-                                delete r[n.id], u.dispose()
+                            t.addHandler(u), s.disposed.connect((() => {
+                                delete r[s.id], u.dispose()
                             })), u.ready.then((() => {
                                 e(u), c.ready.then((async () => {
-                                    l.session.kernel.anyMessage.connect(((e, n) => {
-                                        if (t.panel && "recv" === n.direction)
-                                            if ("execute_result" === n.msg.header.msg_type || "display_data" === n.msg.header.msg_type) {
-                                                const e = n.msg.content;
-                                                e.data["text/html"] && t.panel.onNewLog(a(n.msg.header.date), "data", e.data["text/html"])
-                                            } else if ("stream" === n.msg.header.msg_type) {
-                                            const e = n.msg;
+                                    a.session.kernel.anyMessage.connect(((e, s) => {
+                                        if (t.panel && "recv" === s.direction)
+                                            if ("execute_result" === s.msg.header.msg_type || "display_data" === s.msg.header.msg_type) {
+                                                const e = s.msg.content;
+                                                e.data["text/html"] && t.panel.onNewLog(l(s.msg.header.date), "data", e.data["text/html"])
+                                            } else if ("stream" === s.msg.header.msg_type) {
+                                            const e = s.msg;
                                             if (e.content.text && "\n" !== e.content.text) {
                                                 const o = document.createElement("div"),
                                                     r = {
                                                         host: o,
                                                         source: e.content.text,
-                                                        sanitizer: new s.Sanitizer
+                                                        sanitizer: new n.Sanitizer
                                                     };
                                                 (0, i.renderText)(r).then((() => {
                                                     const e = o.outerHTML;
-                                                    t.panel.onNewLog(a(n.msg.header.date), "info", e)
+                                                    t.panel.onNewLog(l(s.msg.header.date), "info", e)
                                                 }))
                                             }
-                                        } else if ("error" === n.msg.header.msg_type) {
-                                            const e = n.msg,
+                                        } else if ("error" === s.msg.header.msg_type) {
+                                            const e = s.msg,
                                                 o = e.content.traceback.join("\n"),
                                                 r = `traceback-${Date.now()}`,
-                                                l = document.createElement("div"),
+                                                a = document.createElement("div"),
                                                 c = `${e.content.evalue}`;
-                                            l.innerHTML = `<pre><span>${c}</span><br><a href="#" style="text-decoration: underline; color: grey;" id="link-${r}" onClick="document.getElementById('${r}').style.display = document.getElementById('${r}').style.display === 'none' ? 'block' : 'none'; return false;">Show Traceback</a></pre>`;
+                                            a.innerHTML = `<pre><span>${c}</span><br><a href="#" style="text-decoration: underline; color: grey;" id="link-${r}" onClick="document.getElementById('${r}').style.display = document.getElementById('${r}').style.display === 'none' ? 'block' : 'none'; return false;">Show Traceback</a></pre>`;
                                             const d = document.createElement("pre");
-                                            d.id = r, d.style.display = "none", l.appendChild(d);
+                                            d.id = r, d.style.display = "none", a.appendChild(d);
                                             const h = {
                                                 host: d,
                                                 source: o,
-                                                sanitizer: new s.Sanitizer
+                                                sanitizer: new n.Sanitizer
                                             };
                                             (0, i.renderText)(h).then((() => {
-                                                const n = l.outerHTML;
-                                                t.panel.onNewLog(a(e.header.date), "error", n)
+                                                const s = a.outerHTML;
+                                                t.panel.onNewLog(l(e.header.date), "error", s)
                                             }))
                                         }
                                     }))
                                 }))
                             }))
-                        })), l(o)
+                        })), a(o)
                     }));
-                    const l = (e, s) => {
+                    const a = (e, n) => {
                         var o;
-                        const i = null !== (o = null == s ? void 0 : s.newValue) && void 0 !== o ? o : e.currentWidget;
-                        i && n.has(i) && r[i.id].then((e => {
+                        const i = null !== (o = null == n ? void 0 : n.newValue) && void 0 !== o ? o : e.currentWidget;
+                        i && s.has(i) && r[i.id].then((e => {
                             e && (t.source = e)
                         }))
                     };
-                    l(o), o.currentChanged.connect(l)
+                    a(o), o.currentChanged.connect(a)
                 }
             }]
         }
     }
 ]);
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/818.9952ec63ac4e7e5b37d1.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/595.853e8b63deafdcf653a9.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
-/*! For license information please see 818.9952ec63ac4e7e5b37d1.js.LICENSE.txt */
+/*! For license information please see 595.853e8b63deafdcf653a9.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_log_console = self.webpackChunk_amphi_pipeline_log_console || []).push([
-    [818], {
+    [595], {
         588: (e, t, n) => {
             "use strict";
             n.d(t, {
                 z1: () => C,
                 cM: () => b,
                 bK: () => A
             });
@@ -3477,23 +3477,23 @@
                         Pe = I(),
                         ze = a.useState(null),
                         je = (0, o.A)(ze, 2),
                         Te = je[0],
                         Be = je[1],
                         De = a.useRef(null),
                         Fe = (0, k.A)((function(e) {
-                            De.current = e, (0, S.f)(e) && Te !== e && Be(e), null == Me || Me.registerSubPopup(Pe, e)
+                            De.current = e, (0, S.fk)(e) && Te !== e && Be(e), null == Me || Me.registerSubPopup(Pe, e)
                         })),
                         He = a.useState(null),
                         Le = (0, o.A)(He, 2),
                         _e = Le[0],
                         Ke = Le[1],
                         We = a.useRef(null),
                         Ve = (0, k.A)((function(e) {
-                            (0, S.f)(e) && _e !== e && (Ke(e), We.current = e)
+                            (0, S.fk)(e) && _e !== e && (Ke(e), We.current = e)
                         })),
                         qe = a.Children.only(s),
                         Xe = (null == qe ? void 0 : qe.props) || {},
                         Ge = {},
                         Ue = (0, k.A)((function(e) {
                             var t, n, r = _e;
                             return (null == r ? void 0 : r.contains(e)) || (null === (t = (0, E.j)(r)) || void 0 === t ? void 0 : t.host) === e || e === r || (null == Te ? void 0 : Te.contains(e)) || (null === (n = (0, E.j)(Te)) || void 0 === n ? void 0 : n.host) === e || e === Te || Object.values(Ne.current).some((function(t) {
@@ -3638,15 +3638,15 @@
                                             oe = G === J ? re : ne,
                                             ie = te ? re : oe;
                                         f.style.left = "auto", f.style.top = "auto", f.style.right = "0", f.style.bottom = "0";
                                         var ae = f.getBoundingClientRect();
                                         f.style.left = w, f.style.top = A, f.style.right = C, f.style.bottom = E, f.style.overflow = k, null === (u = f.parentElement) || void 0 === u || u.removeChild(O);
                                         var le = V(Math.round(F / parseFloat(b) * 1e3) / 1e3),
                                             ce = V(Math.round(D / parseFloat(y) * 1e3) / 1e3);
-                                        if (0 === le || 0 === ce || (0, S.f)(n) && !(0, H.A)(n)) return;
+                                        if (0 === le || 0 === ce || (0, S.fk)(n) && !(0, H.A)(n)) return;
                                         var se = $.offset,
                                             ue = $.targetOffset,
                                             de = U(N, se),
                                             fe = (0, o.A)(de, 2),
                                             pe = fe[0],
                                             me = fe[1],
                                             ge = U(d, ue),
@@ -8949,399 +8949,14 @@
                         spaceGapLargeSize: e.paddingLG
                     });
                     return [a(t), l(t), i(t)]
                 }), (() => ({})), {
                     resetStyle: !1
                 })
         },
-        5025: (e, t, n) => {
-            "use strict";
-            n.d(t, {
-                A: () => y
-            });
-            var r = n(3345),
-                o = n(9870),
-                i = n.n(o),
-                a = n(8892);
-            var l = n(7291),
-                c = n(9642),
-                s = n(6397),
-                u = n(8408),
-                d = n(4859),
-                f = n(8339);
-            const p = new s.Mo("antSpinMove", {
-                    to: {
-                        opacity: 1
-                    }
-                }),
-                m = new s.Mo("antRotate", {
-                    to: {
-                        transform: "rotate(405deg)"
-                    }
-                }),
-                g = e => {
-                    const {
-                        componentCls: t,
-                        calc: n
-                    } = e;
-                    return {
-                        [`${t}`]: Object.assign(Object.assign({}, (0, u.dF)(e)), {
-                            position: "absolute",
-                            display: "none",
-                            color: e.colorPrimary,
-                            fontSize: 0,
-                            textAlign: "center",
-                            verticalAlign: "middle",
-                            opacity: 0,
-                            transition: `transform ${e.motionDurationSlow} ${e.motionEaseInOutCirc}`,
-                            "&-spinning": {
-                                position: "static",
-                                display: "inline-block",
-                                opacity: 1
-                            },
-                            [`${t}-text`]: {
-                                fontSize: e.fontSize,
-                                paddingTop: n(n(e.dotSize).sub(e.fontSize)).div(2).add(2).equal()
-                            },
-                            "&-fullscreen": {
-                                position: "fixed",
-                                width: "100vw",
-                                height: "100vh",
-                                backgroundColor: e.colorBgMask,
-                                zIndex: e.zIndexPopupBase,
-                                inset: 0,
-                                display: "flex",
-                                alignItems: "center",
-                                flexDirection: "column",
-                                justifyContent: "center",
-                                opacity: 0,
-                                visibility: "hidden",
-                                transition: `all ${e.motionDurationMid}`,
-                                "&-show": {
-                                    opacity: 1,
-                                    visibility: "visible"
-                                },
-                                [`${t}-dot ${t}-dot-item`]: {
-                                    backgroundColor: e.colorWhite
-                                },
-                                [`${t}-text`]: {
-                                    color: e.colorTextLightSolid
-                                }
-                            },
-                            "&-nested-loading": {
-                                position: "relative",
-                                [`> div > ${t}`]: {
-                                    position: "absolute",
-                                    top: 0,
-                                    insetInlineStart: 0,
-                                    zIndex: 4,
-                                    display: "block",
-                                    width: "100%",
-                                    height: "100%",
-                                    maxHeight: e.contentHeight,
-                                    [`${t}-dot`]: {
-                                        position: "absolute",
-                                        top: "50%",
-                                        insetInlineStart: "50%",
-                                        margin: n(e.dotSize).mul(-1).div(2).equal()
-                                    },
-                                    [`${t}-text`]: {
-                                        position: "absolute",
-                                        top: "50%",
-                                        width: "100%",
-                                        textShadow: `0 1px 2px ${e.colorBgContainer}`
-                                    },
-                                    [`&${t}-show-text ${t}-dot`]: {
-                                        marginTop: n(e.dotSize).div(2).mul(-1).sub(10).equal()
-                                    },
-                                    "&-sm": {
-                                        [`${t}-dot`]: {
-                                            margin: n(e.dotSizeSM).mul(-1).div(2).equal()
-                                        },
-                                        [`${t}-text`]: {
-                                            paddingTop: n(n(e.dotSizeSM).sub(e.fontSize)).div(2).add(2).equal()
-                                        },
-                                        [`&${t}-show-text ${t}-dot`]: {
-                                            marginTop: n(e.dotSizeSM).div(2).mul(-1).sub(10).equal()
-                                        }
-                                    },
-                                    "&-lg": {
-                                        [`${t}-dot`]: {
-                                            margin: n(e.dotSizeLG).mul(-1).div(2).equal()
-                                        },
-                                        [`${t}-text`]: {
-                                            paddingTop: n(n(e.dotSizeLG).sub(e.fontSize)).div(2).add(2).equal()
-                                        },
-                                        [`&${t}-show-text ${t}-dot`]: {
-                                            marginTop: n(e.dotSizeLG).div(2).mul(-1).sub(10).equal()
-                                        }
-                                    }
-                                },
-                                [`${t}-container`]: {
-                                    position: "relative",
-                                    transition: `opacity ${e.motionDurationSlow}`,
-                                    "&::after": {
-                                        position: "absolute",
-                                        top: 0,
-                                        insetInlineEnd: 0,
-                                        bottom: 0,
-                                        insetInlineStart: 0,
-                                        zIndex: 10,
-                                        width: "100%",
-                                        height: "100%",
-                                        background: e.colorBgContainer,
-                                        opacity: 0,
-                                        transition: `all ${e.motionDurationSlow}`,
-                                        content: '""',
-                                        pointerEvents: "none"
-                                    }
-                                },
-                                [`${t}-blur`]: {
-                                    clear: "both",
-                                    opacity: .5,
-                                    userSelect: "none",
-                                    pointerEvents: "none",
-                                    "&::after": {
-                                        opacity: .4,
-                                        pointerEvents: "auto"
-                                    }
-                                }
-                            },
-                            "&-tip": {
-                                color: e.spinDotDefault
-                            },
-                            [`${t}-dot`]: {
-                                position: "relative",
-                                display: "inline-block",
-                                fontSize: e.dotSize,
-                                width: "1em",
-                                height: "1em",
-                                "&-item": {
-                                    position: "absolute",
-                                    display: "block",
-                                    width: n(e.dotSize).sub(n(e.marginXXS).div(2)).div(2).equal(),
-                                    height: n(e.dotSize).sub(n(e.marginXXS).div(2)).div(2).equal(),
-                                    backgroundColor: e.colorPrimary,
-                                    borderRadius: "100%",
-                                    transform: "scale(0.75)",
-                                    transformOrigin: "50% 50%",
-                                    opacity: .3,
-                                    animationName: p,
-                                    animationDuration: "1s",
-                                    animationIterationCount: "infinite",
-                                    animationTimingFunction: "linear",
-                                    animationDirection: "alternate",
-                                    "&:nth-child(1)": {
-                                        top: 0,
-                                        insetInlineStart: 0,
-                                        animationDelay: "0s"
-                                    },
-                                    "&:nth-child(2)": {
-                                        top: 0,
-                                        insetInlineEnd: 0,
-                                        animationDelay: "0.4s"
-                                    },
-                                    "&:nth-child(3)": {
-                                        insetInlineEnd: 0,
-                                        bottom: 0,
-                                        animationDelay: "0.8s"
-                                    },
-                                    "&:nth-child(4)": {
-                                        bottom: 0,
-                                        insetInlineStart: 0,
-                                        animationDelay: "1.2s"
-                                    }
-                                },
-                                "&-spin": {
-                                    transform: "rotate(45deg)",
-                                    animationName: m,
-                                    animationDuration: "1.2s",
-                                    animationIterationCount: "infinite",
-                                    animationTimingFunction: "linear"
-                                }
-                            },
-                            [`&-sm ${t}-dot`]: {
-                                fontSize: e.dotSizeSM,
-                                i: {
-                                    width: n(n(e.dotSizeSM).sub(n(e.marginXXS).div(2))).div(2).equal(),
-                                    height: n(n(e.dotSizeSM).sub(n(e.marginXXS).div(2))).div(2).equal()
-                                }
-                            },
-                            [`&-lg ${t}-dot`]: {
-                                fontSize: e.dotSizeLG,
-                                i: {
-                                    width: n(n(e.dotSizeLG).sub(e.marginXXS)).div(2).equal(),
-                                    height: n(n(e.dotSizeLG).sub(e.marginXXS)).div(2).equal()
-                                }
-                            },
-                            [`&${t}-show-text ${t}-text`]: {
-                                display: "block"
-                            }
-                        })
-                    }
-                },
-                h = (0, d.OF)("Spin", (e => {
-                    const t = (0, f.h1)(e, {
-                        spinDotDefault: e.colorTextDescription
-                    });
-                    return [g(t)]
-                }), (e => {
-                    const {
-                        controlHeightLG: t,
-                        controlHeight: n
-                    } = e;
-                    return {
-                        contentHeight: 400,
-                        dotSize: t / 2,
-                        dotSizeSM: .35 * t,
-                        dotSizeLG: n
-                    }
-                }));
-            let v = null;
-            const b = e => {
-                const {
-                    prefixCls: t,
-                    spinning: n = !0,
-                    delay: o = 0,
-                    className: s,
-                    rootClassName: u,
-                    size: d = "default",
-                    tip: f,
-                    wrapperClassName: p,
-                    style: m,
-                    children: g,
-                    fullscreen: b = !1
-                } = e, y = function(e, t) {
-                    var n = {};
-                    for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
-                    if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
-                        var o = 0;
-                        for (r = Object.getOwnPropertySymbols(e); o < r.length; o++) t.indexOf(r[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[o]) && (n[r[o]] = e[r[o]])
-                    }
-                    return n
-                }(e, ["prefixCls", "spinning", "delay", "className", "rootClassName", "size", "tip", "wrapperClassName", "style", "children", "fullscreen"]), {
-                    getPrefixCls: x
-                } = r.useContext(c.QO), w = x("spin", t), [A, C, S] = h(w), [E, k] = r.useState((() => n && ! function(e, t) {
-                    return !!e && !!t && !isNaN(Number(t))
-                }(n, o)));
-                r.useEffect((() => {
-                    if (n) {
-                        const e = function(e, t, n) {
-                            var r = (n || {}).atBegin;
-                            return function(e, t, n) {
-                                var r, o = n || {},
-                                    i = o.noTrailing,
-                                    a = void 0 !== i && i,
-                                    l = o.noLeading,
-                                    c = void 0 !== l && l,
-                                    s = o.debounceMode,
-                                    u = void 0 === s ? void 0 : s,
-                                    d = !1,
-                                    f = 0;
-
-                                function p() {
-                                    r && clearTimeout(r)
-                                }
-
-                                function m() {
-                                    for (var n = arguments.length, o = new Array(n), i = 0; i < n; i++) o[i] = arguments[i];
-                                    var l = this,
-                                        s = Date.now() - f;
-
-                                    function m() {
-                                        f = Date.now(), t.apply(l, o)
-                                    }
-
-                                    function g() {
-                                        r = void 0
-                                    }
-                                    d || (c || !u || r || m(), p(), void 0 === u && s > e ? c ? (f = Date.now(), a || (r = setTimeout(u ? g : m, e))) : m() : !0 !== a && (r = setTimeout(u ? g : m, void 0 === u ? e - s : e)))
-                                }
-                                return m.cancel = function(e) {
-                                    var t = (e || {}).upcomingOnly,
-                                        n = void 0 !== t && t;
-                                    p(), d = !n
-                                }, m
-                            }(e, t, {
-                                debounceMode: !1 !== (void 0 !== r && r)
-                            })
-                        }(o, (() => {
-                            k(!0)
-                        }));
-                        return e(), () => {
-                            var t;
-                            null === (t = null == e ? void 0 : e.cancel) || void 0 === t || t.call(e)
-                        }
-                    }
-                    k(!1)
-                }), [o, n]);
-                const $ = r.useMemo((() => void 0 !== g && !b), [g, b]),
-                    {
-                        direction: O,
-                        spin: I
-                    } = r.useContext(c.QO),
-                    N = i()(w, null == I ? void 0 : I.className, {
-                        [`${w}-sm`]: "small" === d,
-                        [`${w}-lg`]: "large" === d,
-                        [`${w}-spinning`]: E,
-                        [`${w}-show-text`]: !!f,
-                        [`${w}-fullscreen`]: b,
-                        [`${w}-fullscreen-show`]: b && E,
-                        [`${w}-rtl`]: "rtl" === O
-                    }, s, u, C, S),
-                    M = i()(`${w}-container`, {
-                        [`${w}-blur`]: E
-                    }),
-                    R = (0, a.A)(y, ["indicator"]),
-                    P = Object.assign(Object.assign({}, null == I ? void 0 : I.style), m),
-                    z = r.createElement("div", Object.assign({}, R, {
-                        style: P,
-                        className: N,
-                        "aria-live": "polite",
-                        "aria-busy": E
-                    }), function(e, t) {
-                        const {
-                            indicator: n
-                        } = t, o = `${e}-dot`;
-                        return null === n ? null : r.isValidElement(n) ? (0, l.Ob)(n, {
-                            className: i()(n.props.className, o)
-                        }) : r.isValidElement(v) ? (0, l.Ob)(v, {
-                            className: i()(v.props.className, o)
-                        }) : r.createElement("span", {
-                            className: i()(o, `${e}-dot-spin`)
-                        }, r.createElement("i", {
-                            className: `${e}-dot-item`,
-                            key: 1
-                        }), r.createElement("i", {
-                            className: `${e}-dot-item`,
-                            key: 2
-                        }), r.createElement("i", {
-                            className: `${e}-dot-item`,
-                            key: 3
-                        }), r.createElement("i", {
-                            className: `${e}-dot-item`,
-                            key: 4
-                        }))
-                    }(w, e), f && ($ || b) ? r.createElement("div", {
-                        className: `${w}-text`
-                    }, f) : null);
-                return A($ ? r.createElement("div", Object.assign({}, R, {
-                    className: i()(`${w}-nested-loading`, p, C, S)
-                }), E && r.createElement("div", {
-                    key: "loading"
-                }, z), r.createElement("div", {
-                    className: M,
-                    key: "container"
-                }, g)) : z)
-            };
-            b.setDefaultIndicator = e => {
-                v = e
-            };
-            const y = b
-        },
         1741: (e, t, n) => {
             "use strict";
 
             function r(e, t, n) {
                 const {
                     focusElCls: r,
                     focus: o,
@@ -9971,18 +9586,18 @@
                         boxShadow: n,
                         zIndex: 0,
                         background: "transparent"
                     }
                 }
             }
         },
-        5180: (e, t, n) => {
+        1047: (e, t, n) => {
             "use strict";
             n.d(t, {
-                A: () => Ep
+                A: () => Mp
             });
             var r = n(3345),
                 o = n.n(r),
                 i = {},
                 a = "rc-table-internal-hook",
                 l = n(4240),
                 c = n(9449),
@@ -12064,15 +11679,15 @@
 
                         function p() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
                             f();
                             var t = function() {
                                 s.current.forEach((function(e, t) {
                                     if (e && e.offsetParent) {
-                                        var n = (0, Ue.A)(e),
+                                        var n = (0, Ue.Ay)(e),
                                             r = n.offsetHeight;
                                         u.current.get(t) !== r && u.current.set(t, n.offsetHeight)
                                     }
                                 })), c((function(e) {
                                     return e + 1
                                 }))
                             };
@@ -12099,51 +11714,52 @@
                     }), [H.id, H.maps]),
                     V = K && m && (Math.max(c * m.length, W) > a || !!x),
                     q = "rtl" === y,
                     G = O()(o, (0, k.A)({}, "".concat(o, "-rtl"), q), i),
                     U = m || at,
                     Y = (0, r.useRef)(),
                     Q = (0, r.useRef)(),
-                    Z = (0, r.useState)(0),
-                    J = (0, l.A)(Z, 2),
-                    ee = J[0],
-                    te = J[1],
-                    ne = (0, r.useState)(0),
-                    re = (0, l.A)(ne, 2),
-                    oe = re[0],
-                    ie = re[1],
-                    ae = (0, r.useState)(!1),
-                    le = (0, l.A)(ae, 2),
-                    ce = le[0],
-                    se = le[1],
-                    ue = function() {
-                        se(!0)
-                    },
+                    Z = (0, r.useRef)(),
+                    J = (0, r.useState)(0),
+                    ee = (0, l.A)(J, 2),
+                    te = ee[0],
+                    ne = ee[1],
+                    re = (0, r.useState)(0),
+                    oe = (0, l.A)(re, 2),
+                    ie = oe[0],
+                    ae = oe[1],
+                    le = (0, r.useState)(!1),
+                    ce = (0, l.A)(le, 2),
+                    se = ce[0],
+                    ue = ce[1],
                     de = function() {
-                        se(!1)
+                        ue(!0)
+                    },
+                    fe = function() {
+                        ue(!1)
                     },
-                    fe = {
+                    pe = {
                         getKey: z
                     };
 
-                function pe(e) {
-                    te((function(t) {
+                function me(e) {
+                    ne((function(t) {
                         var n = function(e) {
                             var t = e;
-                            return Number.isNaN(Pe.current) || (t = Math.min(t, Pe.current)), t = Math.max(t, 0)
+                            return Number.isNaN(ze.current) || (t = Math.min(t, ze.current)), t = Math.max(t, 0)
                         }("function" == typeof e ? e(t) : e);
                         return Y.current.scrollTop = n, n
                     }))
                 }
-                var me = (0, r.useRef)({
+                var ge = (0, r.useRef)({
                         start: 0,
                         end: U.length
                     }),
-                    ge = (0, r.useRef)(),
-                    he = function(e, t, n) {
+                    he = (0, r.useRef)(),
+                    ve = function(e, t, n) {
                         var o = r.useState(e),
                             i = (0, l.A)(o, 2),
                             a = i[0],
                             c = i[1],
                             s = r.useState(null),
                             u = (0, l.A)(s, 2),
                             d = u[0],
@@ -12172,17 +11788,17 @@
                                     index: s,
                                     multiple: u
                                 }
                             }(a || [], e || [], t);
                             void 0 !== (null == r ? void 0 : r.index) && (null == n || n(r.index), f(e[r.index])), c(e)
                         }), [e]), [d]
                     }(U, z),
-                    ve = (0, l.A)(he, 1)[0];
-                ge.current = ve;
-                var be = r.useMemo((function() {
+                    be = (0, l.A)(ve, 1)[0];
+                he.current = be;
+                var ye = r.useMemo((function() {
                         if (!K) return {
                             scrollHeight: void 0,
                             start: 0,
                             end: U.length - 1,
                             offset: void 0
                         };
                         var e;
@@ -12193,84 +11809,84 @@
                             offset: void 0
                         };
                         for (var t, n, r, o = 0, i = U.length, l = 0; l < i; l += 1) {
                             var s = U[l],
                                 u = z(s),
                                 d = H.get(u),
                                 f = o + (void 0 === d ? c : d);
-                            f >= ee && void 0 === t && (t = l, n = o), f > ee + a && void 0 === r && (r = l), o = f
+                            f >= te && void 0 === t && (t = l, n = o), f > te + a && void 0 === r && (r = l), o = f
                         }
                         return void 0 === t && (t = 0, n = 0, r = Math.ceil(a / c)), void 0 === r && (r = U.length - 1), {
                             scrollHeight: o,
                             start: t,
                             end: r = Math.min(r + 1, U.length - 1),
                             offset: n
                         }
-                    }), [V, K, ee, U, _, a]),
-                    ye = be.scrollHeight,
-                    xe = be.start,
-                    we = be.end,
-                    Ae = be.offset;
-                me.current.start = xe, me.current.end = we;
-                var Ce = r.useState({
+                    }), [V, K, te, U, _, a]),
+                    xe = ye.scrollHeight,
+                    we = ye.start,
+                    Ae = ye.end,
+                    Ce = ye.offset;
+                ge.current.start = we, ge.current.end = Ae;
+                var Se = r.useState({
                         width: 0,
                         height: a
                     }),
-                    Se = (0, l.A)(Ce, 2),
-                    Ee = Se[0],
-                    ke = Se[1],
-                    $e = (0, r.useRef)(),
+                    Ee = (0, l.A)(Se, 2),
+                    ke = Ee[0],
+                    $e = Ee[1],
                     Oe = (0, r.useRef)(),
-                    Ie = r.useMemo((function() {
-                        return ot(Ee.width, x)
-                    }), [Ee.width, x]),
+                    Ie = (0, r.useRef)(),
                     Ne = r.useMemo((function() {
-                        return ot(Ee.height, ye)
-                    }), [Ee.height, ye]),
-                    Me = ye - a,
-                    Pe = (0, r.useRef)(Me);
-                Pe.current = Me;
-                var ze = ee <= 0,
-                    je = ee >= Me,
-                    Te = Ge(ze, je),
-                    Be = function() {
+                        return ot(ke.width, x)
+                    }), [ke.width, x]),
+                    Me = r.useMemo((function() {
+                        return ot(ke.height, xe)
+                    }), [ke.height, xe]),
+                    Pe = xe - a,
+                    ze = (0, r.useRef)(Pe);
+                ze.current = Pe;
+                var je = te <= 0,
+                    Te = te >= Pe,
+                    Be = Ge(je, Te),
+                    De = function() {
                         return {
-                            x: q ? -oe : oe,
-                            y: ee
+                            x: q ? -ie : ie,
+                            y: te
                         }
                     },
-                    De = (0, r.useRef)(Be()),
-                    Fe = (0, T._q)((function(e) {
+                    Fe = (0, r.useRef)(De()),
+                    He = (0, T._q)((function(e) {
                         if ($) {
-                            var t = (0, E.A)((0, E.A)({}, Be()), e);
-                            De.current.x === t.x && De.current.y === t.y || ($(t), De.current = t)
+                            var t = (0, E.A)((0, E.A)({}, De()), e);
+                            Fe.current.x === t.x && Fe.current.y === t.y || ($(t), Fe.current = t)
                         }
                     }));
 
-                function He(e, t) {
+                function Le(e, t) {
                     var n = e;
                     t ? ((0, d.flushSync)((function() {
-                        ie(n)
-                    })), Fe()) : pe(n)
+                        ae(n)
+                    })), He()) : me(n)
                 }
-                var Le = function(e) {
+                var _e = function(e) {
                         var t = e,
-                            n = x ? x - Ee.width : 0;
+                            n = x ? x - ke.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    _e = (0, T._q)((function(e, t) {
+                    Ke = (0, T._q)((function(e, t) {
                         t ? ((0, d.flushSync)((function() {
-                            ie((function(t) {
-                                return Le(t + (q ? -e : e))
+                            ae((function(t) {
+                                return _e(t + (q ? -e : e))
                             }))
-                        })), Fe()) : pe((function(t) {
+                        })), He()) : me((function(t) {
                             return t + e
                         }))
                     })),
-                    Ke = function(e, t, n, o, i) {
+                    We = function(e, t, n, o, i) {
                         var a = (0, r.useRef)(0),
                             l = (0, r.useRef)(null),
                             c = (0, r.useRef)(null),
                             s = (0, r.useRef)(!1),
                             u = Ge(t, n),
                             d = (0, r.useRef)(null),
                             f = (0, r.useRef)(null);
@@ -12295,18 +11911,18 @@
                                 }(t, g) : function(e, t) {
                                     i(t, !0), Xe || e.preventDefault()
                                 }(t, m)
                             }
                         }, function(t) {
                             e && (s.current = t.detail === c.current)
                         }]
-                    }(K, ze, je, !!x, _e),
-                    We = (0, l.A)(Ke, 2),
-                    Ye = We[0],
-                    Qe = We[1];
+                    }(K, je, Te, !!x, Ke),
+                    Ye = (0, l.A)(We, 2),
+                    Qe = Ye[0],
+                    et = Ye[1];
                 ! function(e, t, n) {
                     var o, i = (0, r.useRef)(!1),
                         a = (0, r.useRef)(0),
                         l = (0, r.useRef)(null),
                         c = (0, r.useRef)(null),
                         u = function(e) {
                             if (i.current) {
@@ -12329,40 +11945,40 @@
                         return e && t.current.addEventListener("touchstart", f),
                             function() {
                                 var e;
                                 null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", f), o(), clearInterval(c.current)
                             }
                     }), [e])
                 }(K, Y, (function(e, t) {
-                    return !Te(e, t) && (Ye({
+                    return !Be(e, t) && (Qe({
                         preventDefault: function() {},
                         deltaY: e
                     }), !0)
                 })), (0, s.A)((function() {
                     function e(e) {
                         K && e.preventDefault()
                     }
                     var t = Y.current;
-                    return t.addEventListener("wheel", Ye), t.addEventListener("DOMMouseScroll", Qe), t.addEventListener("MozMousePixelScroll", e),
+                    return t.addEventListener("wheel", Qe), t.addEventListener("DOMMouseScroll", et), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", Ye), t.removeEventListener("DOMMouseScroll", Qe), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", Qe), t.removeEventListener("DOMMouseScroll", et), t.removeEventListener("MozMousePixelScroll", e)
                         }
                 }), [K]), (0, s.A)((function() {
                     if (x) {
-                        var e = Le(oe);
-                        ie(e), Fe({
+                        var e = _e(ie);
+                        ae(e), He({
                             x: e
                         })
                     }
-                }), [Ee.width, x]);
-                var et = function() {
+                }), [ke.width, x]);
+                var tt = function() {
                         var e, t;
-                        null === (e = $e.current) || void 0 === e || e.delayHidden(), null === (t = Oe.current) || void 0 === t || t.delayHidden()
+                        null === (e = Oe.current) || void 0 === e || e.delayHidden(), null === (t = Ie.current) || void 0 === t || t.delayHidden()
                     },
-                    tt = function(e, t, n, o, i, a, c, u) {
+                    rt = function(e, t, n, o, i, a, c, u) {
                         var d = r.useRef(),
                             f = r.useState(null),
                             p = (0, l.A)(f, 2),
                             m = p[0],
                             g = p[1];
                         return (0, s.A)((function() {
                                 if (m && m.times < 10) {
@@ -12430,30 +12046,31 @@
                                             originAlign: r
                                         })
                                     }
                                 } else u()
                             }
                     }(Y, U, H, c, z, (function() {
                         return F(!0)
-                    }), pe, et);
+                    }), me, tt);
                 r.useImperativeHandle(t, (function() {
                     return {
-                        getScrollInfo: Be,
+                        nativeElement: Z.current,
+                        getScrollInfo: De,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === (0, S.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ie(Le(e.left)), tt(e.top)) : tt(e)
+                            (t = e) && "object" === (0, S.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ae(_e(e.left)), rt(e.top)) : rt(e)
                         }
                     }
                 })), (0, s.A)((function() {
                     if (I) {
-                        var e = U.slice(xe, we + 1);
+                        var e = U.slice(we, Ae + 1);
                         I(e, U)
                     }
-                }), [xe, we, U]);
-                var rt = function(e, t, n, o) {
+                }), [we, Ae, U]);
+                var ct = function(e, t, n, o) {
                         var i = r.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, o]),
                             a = (0, l.A)(i, 2),
                             c = a[0],
                             s = a[1];
                         return function(r) {
@@ -12470,99 +12087,101 @@
                                 }
                             return {
                                 top: s[a - 1] || 0,
                                 bottom: s[l]
                             }
                         }
                     }(U, z, H, c),
-                    ct = null == M ? void 0 : M({
-                        start: xe,
-                        end: we,
+                    st = null == M ? void 0 : M({
+                        start: we,
+                        end: Ae,
                         virtual: V,
-                        offsetX: oe,
-                        offsetY: Ae,
+                        offsetX: ie,
+                        offsetY: Ce,
                         rtl: q,
-                        getSize: rt
+                        getSize: ct
                     }),
-                    st = function(e, t, n, o, i, a, l) {
-                        var c = l.getKey;
+                    ut = function(e, t, n, o, i, a, l, c) {
+                        var s = c.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
-                            var l = a(e, t + n, {
+                            var c = l(e, t + n, {
                                     style: {
                                         width: o
-                                    }
+                                    },
+                                    offsetX: i
                                 }),
-                                s = c(e);
+                                u = s(e);
                             return r.createElement(qe, {
-                                key: s,
+                                key: u,
                                 setRef: function(t) {
-                                    return i(e, t)
+                                    return a(e, t)
                                 }
-                            }, l)
+                            }, c)
                         }))
-                    }(U, xe, we, x, D, h, fe),
-                    ut = null;
-                a && (ut = (0, E.A)((0, k.A)({}, f ? "height" : "maxHeight", a), lt), K && (ut.overflowY = "hidden", x && (ut.overflowX = "hidden"), ce && (ut.pointerEvents = "none")));
-                var dt = {};
-                return q && (dt.dir = "rtl"), r.createElement("div", (0, g.A)({
+                    }(U, we, Ae, x, ie, D, h, pe),
+                    dt = null;
+                a && (dt = (0, E.A)((0, k.A)({}, f ? "height" : "maxHeight", a), lt), K && (dt.overflowY = "hidden", x && (dt.overflowX = "hidden"), se && (dt.pointerEvents = "none")));
+                var ft = {};
+                return q && (ft.dir = "rtl"), r.createElement("div", (0, g.A)({
+                    ref: Z,
                     style: (0, E.A)((0, E.A)({}, p), {}, {
                         position: "relative"
                     }),
                     className: G
-                }, dt, P), r.createElement(X.A, {
+                }, ft, P), r.createElement(X.A, {
                     onResize: function(e) {
-                        ke({
+                        $e({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, r.createElement(A, {
                     className: "".concat(o, "-holder"),
-                    style: ut,
+                    style: dt,
                     ref: Y,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== ee && pe(t), null == C || C(e), Fe()
+                        t !== te && me(t), null == C || C(e), He()
                     },
-                    onMouseEnter: et
+                    onMouseEnter: tt
                 }, r.createElement(Ve, {
                     prefixCls: o,
-                    height: ye,
-                    offsetX: oe,
-                    offsetY: Ae,
+                    height: xe,
+                    offsetX: ie,
+                    offsetY: Ce,
                     scrollWidth: x,
                     onInnerResize: F,
                     ref: Q,
                     innerProps: N,
                     rtl: q,
-                    extra: ct
-                }, st))), V && ye > a && r.createElement(nt, {
-                    ref: $e,
+                    extra: st
+                }, ut))), V && xe > a && r.createElement(nt, {
+                    ref: Oe,
                     prefixCls: o,
-                    scrollOffset: ee,
-                    scrollRange: ye,
+                    scrollOffset: te,
+                    scrollRange: xe,
                     rtl: q,
-                    onScroll: He,
-                    onStartMove: ue,
-                    onStopMove: de,
-                    spinSize: Ne,
-                    containerSize: Ee.height,
+                    onScroll: Le,
+                    onStartMove: de,
+                    onStopMove: fe,
+                    spinSize: Me,
+                    containerSize: ke.height,
                     style: null == R ? void 0 : R.verticalScrollBar,
                     thumbStyle: null == R ? void 0 : R.verticalScrollBarThumb
-                }), V && x > Ee.width && r.createElement(nt, {
-                    ref: Oe,
+                }), V && x > ke.width && r.createElement(nt, {
+                    ref: Ie,
                     prefixCls: o,
-                    scrollOffset: oe,
+                    scrollOffset: ie,
                     scrollRange: x,
                     rtl: q,
-                    onScroll: He,
-                    onStartMove: ue,
-                    onStopMove: de,
-                    spinSize: Ie,
-                    containerSize: Ee.width,
+                    onScroll: Le,
+                    onStartMove: de,
+                    onStopMove: fe,
+                    spinSize: Ne,
+                    containerSize: ke.width,
                     horizontal: !0,
                     style: null == R ? void 0 : R.horizontalScrollBar,
                     thumbStyle: null == R ? void 0 : R.horizontalScrollBarThumb
                 }))
             }
             var st = r.forwardRef(ct);
             st.displayName = "List";
@@ -24207,28 +23826,396 @@
                     selectPrefixCls: I,
                     className: N,
                     selectComponentClass: s || ($ ? Au : Cu),
                     locale: E,
                     showSizeChanger: A
                 }))))
             };
-            var Hu = n(5025);
+            const Hu = new Wn.Mo("antSpinMove", {
+                    to: {
+                        opacity: 1
+                    }
+                }),
+                Lu = new Wn.Mo("antRotate", {
+                    to: {
+                        transform: "rotate(405deg)"
+                    }
+                }),
+                _u = e => {
+                    const {
+                        componentCls: t,
+                        calc: n
+                    } = e;
+                    return {
+                        [`${t}`]: Object.assign(Object.assign({}, (0, Vn.dF)(e)), {
+                            position: "absolute",
+                            display: "none",
+                            color: e.colorPrimary,
+                            fontSize: 0,
+                            textAlign: "center",
+                            verticalAlign: "middle",
+                            opacity: 0,
+                            transition: `transform ${e.motionDurationSlow} ${e.motionEaseInOutCirc}`,
+                            "&-spinning": {
+                                position: "static",
+                                display: "inline-block",
+                                opacity: 1
+                            },
+                            [`${t}-text`]: {
+                                fontSize: e.fontSize,
+                                paddingTop: n(n(e.dotSize).sub(e.fontSize)).div(2).add(2).equal()
+                            },
+                            "&-fullscreen": {
+                                position: "fixed",
+                                width: "100vw",
+                                height: "100vh",
+                                backgroundColor: e.colorBgMask,
+                                zIndex: e.zIndexPopupBase,
+                                inset: 0,
+                                display: "flex",
+                                alignItems: "center",
+                                flexDirection: "column",
+                                justifyContent: "center",
+                                opacity: 0,
+                                visibility: "hidden",
+                                transition: `all ${e.motionDurationMid}`,
+                                "&-show": {
+                                    opacity: 1,
+                                    visibility: "visible"
+                                },
+                                [`${t}-dot ${t}-dot-item`]: {
+                                    backgroundColor: e.colorWhite
+                                },
+                                [`${t}-text`]: {
+                                    color: e.colorTextLightSolid
+                                }
+                            },
+                            "&-nested-loading": {
+                                position: "relative",
+                                [`> div > ${t}`]: {
+                                    position: "absolute",
+                                    top: 0,
+                                    insetInlineStart: 0,
+                                    zIndex: 4,
+                                    display: "block",
+                                    width: "100%",
+                                    height: "100%",
+                                    maxHeight: e.contentHeight,
+                                    [`${t}-dot`]: {
+                                        position: "absolute",
+                                        top: "50%",
+                                        insetInlineStart: "50%",
+                                        margin: n(e.dotSize).mul(-1).div(2).equal()
+                                    },
+                                    [`${t}-text`]: {
+                                        position: "absolute",
+                                        top: "50%",
+                                        width: "100%",
+                                        textShadow: `0 1px 2px ${e.colorBgContainer}`
+                                    },
+                                    [`&${t}-show-text ${t}-dot`]: {
+                                        marginTop: n(e.dotSize).div(2).mul(-1).sub(10).equal()
+                                    },
+                                    "&-sm": {
+                                        [`${t}-dot`]: {
+                                            margin: n(e.dotSizeSM).mul(-1).div(2).equal()
+                                        },
+                                        [`${t}-text`]: {
+                                            paddingTop: n(n(e.dotSizeSM).sub(e.fontSize)).div(2).add(2).equal()
+                                        },
+                                        [`&${t}-show-text ${t}-dot`]: {
+                                            marginTop: n(e.dotSizeSM).div(2).mul(-1).sub(10).equal()
+                                        }
+                                    },
+                                    "&-lg": {
+                                        [`${t}-dot`]: {
+                                            margin: n(e.dotSizeLG).mul(-1).div(2).equal()
+                                        },
+                                        [`${t}-text`]: {
+                                            paddingTop: n(n(e.dotSizeLG).sub(e.fontSize)).div(2).add(2).equal()
+                                        },
+                                        [`&${t}-show-text ${t}-dot`]: {
+                                            marginTop: n(e.dotSizeLG).div(2).mul(-1).sub(10).equal()
+                                        }
+                                    }
+                                },
+                                [`${t}-container`]: {
+                                    position: "relative",
+                                    transition: `opacity ${e.motionDurationSlow}`,
+                                    "&::after": {
+                                        position: "absolute",
+                                        top: 0,
+                                        insetInlineEnd: 0,
+                                        bottom: 0,
+                                        insetInlineStart: 0,
+                                        zIndex: 10,
+                                        width: "100%",
+                                        height: "100%",
+                                        background: e.colorBgContainer,
+                                        opacity: 0,
+                                        transition: `all ${e.motionDurationSlow}`,
+                                        content: '""',
+                                        pointerEvents: "none"
+                                    }
+                                },
+                                [`${t}-blur`]: {
+                                    clear: "both",
+                                    opacity: .5,
+                                    userSelect: "none",
+                                    pointerEvents: "none",
+                                    "&::after": {
+                                        opacity: .4,
+                                        pointerEvents: "auto"
+                                    }
+                                }
+                            },
+                            "&-tip": {
+                                color: e.spinDotDefault
+                            },
+                            [`${t}-dot`]: {
+                                position: "relative",
+                                display: "inline-block",
+                                fontSize: e.dotSize,
+                                width: "1em",
+                                height: "1em",
+                                "&-item": {
+                                    position: "absolute",
+                                    display: "block",
+                                    width: n(e.dotSize).sub(n(e.marginXXS).div(2)).div(2).equal(),
+                                    height: n(e.dotSize).sub(n(e.marginXXS).div(2)).div(2).equal(),
+                                    backgroundColor: e.colorPrimary,
+                                    borderRadius: "100%",
+                                    transform: "scale(0.75)",
+                                    transformOrigin: "50% 50%",
+                                    opacity: .3,
+                                    animationName: Hu,
+                                    animationDuration: "1s",
+                                    animationIterationCount: "infinite",
+                                    animationTimingFunction: "linear",
+                                    animationDirection: "alternate",
+                                    "&:nth-child(1)": {
+                                        top: 0,
+                                        insetInlineStart: 0,
+                                        animationDelay: "0s"
+                                    },
+                                    "&:nth-child(2)": {
+                                        top: 0,
+                                        insetInlineEnd: 0,
+                                        animationDelay: "0.4s"
+                                    },
+                                    "&:nth-child(3)": {
+                                        insetInlineEnd: 0,
+                                        bottom: 0,
+                                        animationDelay: "0.8s"
+                                    },
+                                    "&:nth-child(4)": {
+                                        bottom: 0,
+                                        insetInlineStart: 0,
+                                        animationDelay: "1.2s"
+                                    }
+                                },
+                                "&-spin": {
+                                    transform: "rotate(45deg)",
+                                    animationName: Lu,
+                                    animationDuration: "1.2s",
+                                    animationIterationCount: "infinite",
+                                    animationTimingFunction: "linear"
+                                }
+                            },
+                            [`&-sm ${t}-dot`]: {
+                                fontSize: e.dotSizeSM,
+                                i: {
+                                    width: n(n(e.dotSizeSM).sub(n(e.marginXXS).div(2))).div(2).equal(),
+                                    height: n(n(e.dotSizeSM).sub(n(e.marginXXS).div(2))).div(2).equal()
+                                }
+                            },
+                            [`&-lg ${t}-dot`]: {
+                                fontSize: e.dotSizeLG,
+                                i: {
+                                    width: n(n(e.dotSizeLG).sub(e.marginXXS)).div(2).equal(),
+                                    height: n(n(e.dotSizeLG).sub(e.marginXXS)).div(2).equal()
+                                }
+                            },
+                            [`&${t}-show-text ${t}-text`]: {
+                                display: "block"
+                            }
+                        })
+                    }
+                },
+                Ku = (0, hn.OF)("Spin", (e => {
+                    const t = (0, qn.h1)(e, {
+                        spinDotDefault: e.colorTextDescription
+                    });
+                    return [_u(t)]
+                }), (e => {
+                    const {
+                        controlHeightLG: t,
+                        controlHeight: n
+                    } = e;
+                    return {
+                        contentHeight: 400,
+                        dotSize: t / 2,
+                        dotSizeSM: .35 * t,
+                        dotSizeLG: n
+                    }
+                }));
+            let Wu = null;
+            const Vu = e => {
+                const {
+                    prefixCls: t,
+                    spinning: n = !0,
+                    delay: o = 0,
+                    className: i,
+                    rootClassName: a,
+                    size: l = "default",
+                    tip: c,
+                    wrapperClassName: s,
+                    style: u,
+                    children: d,
+                    fullscreen: f = !1
+                } = e, p = function(e, t) {
+                    var n = {};
+                    for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
+                    if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
+                        var o = 0;
+                        for (r = Object.getOwnPropertySymbols(e); o < r.length; o++) t.indexOf(r[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[o]) && (n[r[o]] = e[r[o]])
+                    }
+                    return n
+                }(e, ["prefixCls", "spinning", "delay", "className", "rootClassName", "size", "tip", "wrapperClassName", "style", "children", "fullscreen"]), {
+                    getPrefixCls: m
+                } = r.useContext(mn.QO), g = m("spin", t), [h, v, b] = Ku(g), [y, x] = r.useState((() => n && ! function(e, t) {
+                    return !!e && !!t && !isNaN(Number(t))
+                }(n, o)));
+                r.useEffect((() => {
+                    if (n) {
+                        const e = function(e, t, n) {
+                            var r = (n || {}).atBegin;
+                            return function(e, t, n) {
+                                var r, o = n || {},
+                                    i = o.noTrailing,
+                                    a = void 0 !== i && i,
+                                    l = o.noLeading,
+                                    c = void 0 !== l && l,
+                                    s = o.debounceMode,
+                                    u = void 0 === s ? void 0 : s,
+                                    d = !1,
+                                    f = 0;
+
+                                function p() {
+                                    r && clearTimeout(r)
+                                }
+
+                                function m() {
+                                    for (var n = arguments.length, o = new Array(n), i = 0; i < n; i++) o[i] = arguments[i];
+                                    var l = this,
+                                        s = Date.now() - f;
+
+                                    function m() {
+                                        f = Date.now(), t.apply(l, o)
+                                    }
+
+                                    function g() {
+                                        r = void 0
+                                    }
+                                    d || (c || !u || r || m(), p(), void 0 === u && s > e ? c ? (f = Date.now(), a || (r = setTimeout(u ? g : m, e))) : m() : !0 !== a && (r = setTimeout(u ? g : m, void 0 === u ? e - s : e)))
+                                }
+                                return m.cancel = function(e) {
+                                    var t = (e || {}).upcomingOnly,
+                                        n = void 0 !== t && t;
+                                    p(), d = !n
+                                }, m
+                            }(e, t, {
+                                debounceMode: !1 !== (void 0 !== r && r)
+                            })
+                        }(o, (() => {
+                            x(!0)
+                        }));
+                        return e(), () => {
+                            var t;
+                            null === (t = null == e ? void 0 : e.cancel) || void 0 === t || t.call(e)
+                        }
+                    }
+                    x(!1)
+                }), [o, n]);
+                const w = r.useMemo((() => void 0 !== d && !f), [d, f]),
+                    {
+                        direction: A,
+                        spin: C
+                    } = r.useContext(mn.QO),
+                    S = O()(g, null == C ? void 0 : C.className, {
+                        [`${g}-sm`]: "small" === l,
+                        [`${g}-lg`]: "large" === l,
+                        [`${g}-spinning`]: y,
+                        [`${g}-show-text`]: !!c,
+                        [`${g}-fullscreen`]: f,
+                        [`${g}-fullscreen-show`]: f && y,
+                        [`${g}-rtl`]: "rtl" === A
+                    }, i, a, v, b),
+                    E = O()(`${g}-container`, {
+                        [`${g}-blur`]: y
+                    }),
+                    k = (0, zt.A)(p, ["indicator"]),
+                    $ = Object.assign(Object.assign({}, null == C ? void 0 : C.style), u),
+                    I = r.createElement("div", Object.assign({}, k, {
+                        style: $,
+                        className: S,
+                        "aria-live": "polite",
+                        "aria-busy": y
+                    }), function(e, t) {
+                        const {
+                            indicator: n
+                        } = t, o = `${e}-dot`;
+                        return null === n ? null : r.isValidElement(n) ? (0, gn.Ob)(n, {
+                            className: O()(n.props.className, o)
+                        }) : r.isValidElement(Wu) ? (0, gn.Ob)(Wu, {
+                            className: O()(Wu.props.className, o)
+                        }) : r.createElement("span", {
+                            className: O()(o, `${e}-dot-spin`)
+                        }, r.createElement("i", {
+                            className: `${e}-dot-item`,
+                            key: 1
+                        }), r.createElement("i", {
+                            className: `${e}-dot-item`,
+                            key: 2
+                        }), r.createElement("i", {
+                            className: `${e}-dot-item`,
+                            key: 3
+                        }), r.createElement("i", {
+                            className: `${e}-dot-item`,
+                            key: 4
+                        }))
+                    }(g, e), c && (w || f) ? r.createElement("div", {
+                        className: `${g}-text`
+                    }, c) : null);
+                return h(w ? r.createElement("div", Object.assign({}, k, {
+                    className: O()(`${g}-nested-loading`, s, v, b)
+                }), y && r.createElement("div", {
+                    key: "loading"
+                }, I), r.createElement("div", {
+                    className: E,
+                    key: "container"
+                }, d)) : I)
+            };
+            Vu.setDefaultIndicator = e => {
+                Wu = e
+            };
+            const qu = Vu;
 
-            function Lu(e, t) {
+            function Xu(e, t) {
                 return "key" in e && void 0 !== e.key && null !== e.key ? e.key : e.dataIndex ? Array.isArray(e.dataIndex) ? e.dataIndex.join(".") : e.dataIndex : t
             }
 
-            function _u(e, t) {
+            function Gu(e, t) {
                 return t ? `${t}-${e}` : `${e}`
             }
 
-            function Ku(e, t) {
+            function Uu(e, t) {
                 return "function" == typeof e ? e(t) : e
             }
-            const Wu = {
+            const Yu = {
                 icon: {
                     tag: "svg",
                     attrs: {
                         viewBox: "64 64 896 896",
                         focusable: "false"
                     },
                     children: [{
@@ -24237,37 +24224,37 @@
                             d: "M349 838c0 17.7 14.2 32 31.8 32h262.4c17.6 0 31.8-14.3 31.8-32V642H349v196zm531.1-684H143.9c-24.5 0-39.8 26.7-27.5 48l221.3 376h348.8l221.3-376c12.1-21.3-3.2-48-27.7-48z"
                         }
                     }]
                 },
                 name: "filter",
                 theme: "filled"
             };
-            var Vu = function(e, t) {
+            var Qu = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: Wu
+                    icon: Yu
                 }))
             };
-            const qu = r.forwardRef(Vu);
+            const Zu = r.forwardRef(Qu);
 
-            function Xu(e) {
+            function Ju(e) {
                 if (null == e) throw new TypeError("Cannot destructure " + e)
             }
-            var Gu = ["className", "style", "motion", "motionNodes", "motionType", "onMotionStart", "onMotionEnd", "active", "treeNodeRequiredProps"],
-                Uu = function(e, t) {
+            var ed = ["className", "style", "motion", "motionNodes", "motionType", "onMotionStart", "onMotionEnd", "active", "treeNodeRequiredProps"],
+                td = function(e, t) {
                     var n = e.className,
                         o = e.style,
                         i = e.motion,
                         a = e.motionNodes,
                         c = e.motionType,
                         u = e.onMotionStart,
                         d = e.onMotionEnd,
                         f = e.active,
                         p = e.treeNodeRequiredProps,
-                        m = (0, L.A)(e, Gu),
+                        m = (0, L.A)(e, ed),
                         h = r.useState(!0),
                         v = (0, l.A)(h, 2),
                         b = v[0],
                         y = v[1],
                         x = r.useContext(Nt).prefixCls,
                         w = a && "hide" !== c;
                     (0, s.A)((function() {
@@ -24305,15 +24292,15 @@
                         var n = e.className,
                             o = e.style;
                         return r.createElement("div", {
                             ref: t,
                             className: O()("".concat(x, "-treenode-motion"), n),
                             style: o
                         }, a.map((function(e) {
-                            var t = Object.assign({}, (Xu(e.data), e.data)),
+                            var t = Object.assign({}, (Ju(e.data), e.data)),
                                 n = e.title,
                                 o = e.key,
                                 i = e.isStart,
                                 a = e.isEnd;
                             delete t.children;
                             var l = _t(o, p);
                             return r.createElement(Ut, (0, g.A)({}, t, l, {
@@ -24329,18 +24316,18 @@
                         domRef: t,
                         className: n,
                         style: o
                     }, m, {
                         active: f
                     }))
                 };
-            Uu.displayName = "MotionTreeNode";
-            const Yu = r.forwardRef(Uu);
+            td.displayName = "MotionTreeNode";
+            const nd = r.forwardRef(td);
 
-            function Qu(e, t, n) {
+            function rd(e, t, n) {
                 var r = e.findIndex((function(e) {
                         return e.key === n
                     })),
                     o = e[r + 1],
                     i = t.findIndex((function(e) {
                         return e.key === n
                     }));
@@ -24348,57 +24335,57 @@
                     var a = t.findIndex((function(e) {
                         return e.key === o.key
                     }));
                     return t.slice(i + 1, a)
                 }
                 return t.slice(i + 1)
             }
-            var Zu = ["prefixCls", "data", "selectable", "checkable", "expandedKeys", "selectedKeys", "checkedKeys", "loadedKeys", "loadingKeys", "halfCheckedKeys", "keyEntities", "disabled", "dragging", "dragOverNodeKey", "dropPosition", "motion", "height", "itemHeight", "virtual", "focusable", "activeItem", "focused", "tabIndex", "onKeyDown", "onFocus", "onBlur", "onActiveChange", "onListChangeStart", "onListChangeEnd"],
-                Ju = {
+            var od = ["prefixCls", "data", "selectable", "checkable", "expandedKeys", "selectedKeys", "checkedKeys", "loadedKeys", "loadingKeys", "halfCheckedKeys", "keyEntities", "disabled", "dragging", "dragOverNodeKey", "dropPosition", "motion", "height", "itemHeight", "virtual", "focusable", "activeItem", "focused", "tabIndex", "onKeyDown", "onFocus", "onBlur", "onActiveChange", "onListChangeStart", "onListChangeEnd"],
+                id = {
                     width: 0,
                     height: 0,
                     display: "flex",
                     overflow: "hidden",
                     opacity: 0,
                     border: 0,
                     padding: 0,
                     margin: 0
                 },
-                ed = function() {},
-                td = "RC_TREE_MOTION_".concat(Math.random()),
-                nd = {
-                    key: td
+                ad = function() {},
+                ld = "RC_TREE_MOTION_".concat(Math.random()),
+                cd = {
+                    key: ld
                 },
-                rd = {
-                    key: td,
+                sd = {
+                    key: ld,
                     level: 0,
                     index: 0,
                     pos: "0",
-                    node: nd,
-                    nodes: [nd]
+                    node: cd,
+                    nodes: [cd]
                 },
-                od = {
+                ud = {
                     parent: null,
                     children: [],
-                    pos: rd.pos,
-                    data: nd,
+                    pos: sd.pos,
+                    data: cd,
                     title: null,
-                    key: td,
+                    key: ld,
                     isStart: [],
                     isEnd: []
                 };
 
-            function id(e, t, n, r) {
+            function dd(e, t, n, r) {
                 return !1 !== t && n ? e.slice(0, Math.ceil(n / r) + 1) : e
             }
 
-            function ad(e) {
+            function fd(e) {
                 return Bt(e.key, e.pos)
             }
-            var ld = r.forwardRef((function(e, t) {
+            var pd = r.forwardRef((function(e, t) {
                 var n = e.prefixCls,
                     o = e.data,
                     i = (e.selectable, e.checkable, e.expandedKeys),
                     a = e.selectedKeys,
                     c = e.checkedKeys,
                     u = e.loadedKeys,
                     d = e.loadingKeys,
@@ -24418,15 +24405,15 @@
                     k = e.tabIndex,
                     $ = e.onKeyDown,
                     O = e.onFocus,
                     I = e.onBlur,
                     N = e.onActiveChange,
                     M = e.onListChangeStart,
                     R = e.onListChangeEnd,
-                    P = (0, L.A)(e, Zu),
+                    P = (0, L.A)(e, od),
                     z = r.useRef(null),
                     j = r.useRef(null);
                 r.useImperativeHandle(t, (function() {
                     return {
                         scrollTo: function(e) {
                             z.current.scrollTo(e)
                         },
@@ -24492,24 +24479,24 @@
                         }
                     }(D, i);
                     if (null !== e.key)
                         if (e.add) {
                             var t = K.findIndex((function(t) {
                                     return t.key === e.key
                                 })),
-                                n = id(Qu(K, o, e.key), A, x, w),
+                                n = dd(rd(K, o, e.key), A, x, w),
                                 r = K.slice();
-                            r.splice(t + 1, 0, od), G(r), Z(n), ne("show")
+                            r.splice(t + 1, 0, ud), G(r), Z(n), ne("show")
                         } else {
                             var a = o.findIndex((function(t) {
                                     return t.key === e.key
                                 })),
-                                l = id(Qu(o, K, e.key), A, x, w),
+                                l = dd(rd(o, K, e.key), A, x, w),
                                 c = o.slice();
-                            c.splice(a + 1, 0, od), G(c), Z(l), ne("hide")
+                            c.splice(a + 1, 0, ud), G(c), Z(l), ne("hide")
                         }
                     else K !== o && (W(o), G(o))
                 }), [i, o]), r.useEffect((function() {
                     h || oe()
                 }), [h]);
                 var ie = y ? X : o,
                     ae = {
@@ -24520,28 +24507,28 @@
                         checkedKeys: c,
                         halfCheckedKeys: f,
                         dragOverNodeKey: v,
                         dropPosition: b,
                         keyEntities: p
                     };
                 return r.createElement(r.Fragment, null, E && S && r.createElement("span", {
-                    style: Ju,
+                    style: id,
                     "aria-live": "assertive"
                 }, function(e) {
                     for (var t = String(e.data.key), n = e; n.parent;) n = n.parent, t = "".concat(n.data.key, " > ").concat(t);
                     return t
                 }(S)), r.createElement("div", null, r.createElement("input", {
-                    style: Ju,
+                    style: id,
                     disabled: !1 === C || m,
                     tabIndex: !1 !== C ? k : null,
                     onKeyDown: $,
                     onFocus: O,
                     onBlur: I,
                     value: "",
-                    onChange: ed,
+                    onChange: ad,
                     "aria-label": "for screen reader"
                 })), r.createElement("div", {
                     className: "".concat(n, "-treenode"),
                     "aria-hidden": !0,
                     style: {
                         position: "absolute",
                         pointerEvents: "none",
@@ -24554,61 +24541,61 @@
                 }, r.createElement("div", {
                     className: "".concat(n, "-indent")
                 }, r.createElement("div", {
                     ref: j,
                     className: "".concat(n, "-indent-unit")
                 }))), r.createElement(ut, (0, g.A)({}, P, {
                     data: ie,
-                    itemKey: ad,
+                    itemKey: fd,
                     height: x,
                     fullHeight: !1,
                     virtual: A,
                     itemHeight: w,
                     prefixCls: "".concat(n, "-list"),
                     ref: z,
                     onVisibleChange: function(e, t) {
                         var n = new Set(e);
                         t.filter((function(e) {
                             return !n.has(e)
                         })).some((function(e) {
-                            return ad(e) === td
+                            return fd(e) === ld
                         })) && oe()
                     }
                 }), (function(e) {
                     var t = e.pos,
-                        n = Object.assign({}, (Xu(e.data), e.data)),
+                        n = Object.assign({}, (Ju(e.data), e.data)),
                         o = e.title,
                         i = e.key,
                         a = e.isStart,
                         l = e.isEnd,
                         c = Bt(i, t);
                     delete n.key, delete n.children;
                     var s = _t(c, ae);
-                    return r.createElement(Yu, (0, g.A)({}, n, s, {
+                    return r.createElement(nd, (0, g.A)({}, n, s, {
                         title: o,
                         active: !!S && i === S.key,
                         pos: t,
                         data: e.data,
                         isStart: a,
                         isEnd: l,
                         motion: y,
-                        motionNodes: i === td ? Q : null,
+                        motionNodes: i === ld ? Q : null,
                         motionType: te,
                         onMotionStart: M,
                         onMotionEnd: oe,
                         treeNodeRequiredProps: ae,
                         onMouseMove: function() {
                             N(null)
                         }
                     }))
                 })))
             }));
-            ld.displayName = "NodeList";
-            const cd = ld;
-            var sd = function(e) {
+            pd.displayName = "NodeList";
+            const md = pd;
+            var gd = function(e) {
                 (0, Ot.A)(n, e);
                 var t = (0, It.A)(n);
 
                 function n() {
                     var e;
                     (0, Ye.A)(this, n);
                     for (var o = arguments.length, i = new Array(o), a = 0; a < o; a++) i[a] = arguments[a];
@@ -25256,15 +25243,15 @@
                                 onNodeDragEnd: this.onNodeDragEnd,
                                 onNodeDrop: this.onNodeDrop
                             }
                         }, r.createElement("div", {
                             role: "tree",
                             className: O()(h, v, V, (0, k.A)((0, k.A)((0, k.A)({}, "".concat(h, "-show-line"), y), "".concat(h, "-focused"), n), "".concat(h, "-active-focused"), null !== l)),
                             style: q
-                        }, r.createElement(cd, (0, g.A)({
+                        }, r.createElement(md, (0, g.A)({
                             ref: this.listRef,
                             prefixCls: h,
                             style: b,
                             data: o,
                             disabled: P,
                             selectable: C,
                             checkable: !!M,
@@ -25300,21 +25287,21 @@
                         }
                         var a = t.fieldNames;
                         if (i("fieldNames") && (a = Dt(e.fieldNames), o.fieldNames = a), i("treeData") ? n = e.treeData : i("children") && ((0, M.Ay)(!1, "`children` of Tree is deprecated. Please use `treeData` instead."), n = Ft(e.children)), n) {
                             o.treeData = n;
                             var l = Lt(n, {
                                 fieldNames: a
                             });
-                            o.keyEntities = (0, E.A)((0, k.A)({}, td, rd), l.keyEntities)
+                            o.keyEntities = (0, E.A)((0, k.A)({}, ld, sd), l.keyEntities)
                         }
                         var c, s = o.keyEntities || t.keyEntities;
                         if (i("expandedKeys") || r && i("autoExpandParent")) o.expandedKeys = e.autoExpandParent || !r && e.defaultExpandParent ? on(e.expandedKeys, s) : e.expandedKeys;
                         else if (!r && e.defaultExpandAll) {
                             var u = (0, E.A)({}, s);
-                            delete u[td], o.expandedKeys = Object.keys(u).map((function(e) {
+                            delete u[ld], o.expandedKeys = Object.keys(u).map((function(e) {
                                 return u[e].key
                             }))
                         } else !r && e.defaultExpandedKeys && (o.expandedKeys = e.autoExpandParent || e.defaultExpandParent ? on(e.defaultExpandedKeys, s) : e.defaultExpandedKeys);
                         if (o.expandedKeys || delete o.expandedKeys, n || o.expandedKeys) {
                             var d = Ht(n || t.treeData, o.expandedKeys || t.expandedKeys, a);
                             o.flattenNodes = d
                         }
@@ -25333,15 +25320,15 @@
                             }
                             o.checkedKeys = m, o.halfCheckedKeys = h
                         }
                         return i("loadedKeys") && (o.loadedKeys = e.loadedKeys), o
                     }
                 }]), n
             }(r.Component);
-            (0, k.A)(sd, "defaultProps", {
+            (0, k.A)(gd, "defaultProps", {
                 prefixCls: "rc-tree",
                 showLine: !1,
                 showIcon: !0,
                 selectable: !0,
                 multiple: !1,
                 checkable: !1,
                 disabled: !1,
@@ -25378,17 +25365,17 @@
                         style: i
                     })
                 },
                 allowDrop: function() {
                     return !0
                 },
                 expandAction: !1
-            }), (0, k.A)(sd, "TreeNode", Ut);
-            const ud = sd,
-                dd = {
+            }), (0, k.A)(gd, "TreeNode", Ut);
+            const hd = gd,
+                vd = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "64 64 896 896",
                             focusable: "false"
                         },
                         children: [{
@@ -25397,22 +25384,22 @@
                                 d: "M854.6 288.6L639.4 73.4c-6-6-14.1-9.4-22.6-9.4H192c-17.7 0-32 14.3-32 32v832c0 17.7 14.3 32 32 32h640c17.7 0 32-14.3 32-32V311.3c0-8.5-3.4-16.7-9.4-22.7zM790.2 326H602V137.8L790.2 326zm1.8 562H232V136h302v216a42 42 0 0042 42h216v494z"
                             }
                         }]
                     },
                     name: "file",
                     theme: "outlined"
                 };
-            var fd = function(e, t) {
+            var bd = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: dd
+                    icon: vd
                 }))
             };
-            const pd = r.forwardRef(fd),
-                md = {
+            const yd = r.forwardRef(bd),
+                xd = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "64 64 896 896",
                             focusable: "false"
                         },
                         children: [{
@@ -25421,22 +25408,22 @@
                                 d: "M928 444H820V330.4c0-17.7-14.3-32-32-32H473L355.7 186.2a8.15 8.15 0 00-5.5-2.2H96c-17.7 0-32 14.3-32 32v592c0 17.7 14.3 32 32 32h698c13 0 24.8-7.9 29.7-20l134-332c1.5-3.8 2.3-7.9 2.3-12 0-17.7-14.3-32-32-32zM136 256h188.5l119.6 114.4H748V444H238c-13 0-24.8 7.9-29.7 20L136 643.2V256zm635.3 512H159l103.3-256h612.4L771.3 768z"
                             }
                         }]
                     },
                     name: "folder-open",
                     theme: "outlined"
                 };
-            var gd = function(e, t) {
+            var wd = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: md
+                    icon: xd
                 }))
             };
-            const hd = r.forwardRef(gd),
-                vd = {
+            const Ad = r.forwardRef(wd),
+                Cd = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "64 64 896 896",
                             focusable: "false"
                         },
                         children: [{
@@ -25445,22 +25432,22 @@
                                 d: "M880 298.4H521L403.7 186.2a8.15 8.15 0 00-5.5-2.2H144c-17.7 0-32 14.3-32 32v592c0 17.7 14.3 32 32 32h736c17.7 0 32-14.3 32-32V330.4c0-17.7-14.3-32-32-32zM840 768H184V256h188.5l119.6 114.4H840V768z"
                             }
                         }]
                     },
                     name: "folder",
                     theme: "outlined"
                 };
-            var bd = function(e, t) {
+            var Sd = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: vd
+                    icon: Cd
                 }))
             };
-            const yd = r.forwardRef(bd),
-                xd = {
+            const Ed = r.forwardRef(Sd),
+                kd = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "64 64 896 896",
                             focusable: "false"
                         },
                         children: [{
@@ -25469,40 +25456,40 @@
                                 d: "M300 276.5a56 56 0 1056-97 56 56 0 00-56 97zm0 284a56 56 0 1056-97 56 56 0 00-56 97zM640 228a56 56 0 10112 0 56 56 0 00-112 0zm0 284a56 56 0 10112 0 56 56 0 00-112 0zM300 844.5a56 56 0 1056-97 56 56 0 00-56 97zM640 796a56 56 0 10112 0 56 56 0 00-112 0z"
                             }
                         }]
                     },
                     name: "holder",
                     theme: "outlined"
                 };
-            var wd = function(e, t) {
+            var $d = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: xd
+                    icon: kd
                 }))
             };
-            const Ad = r.forwardRef(wd),
-                Cd = new Wn.Mo("ant-tree-node-fx-do-not-use", {
+            const Od = r.forwardRef($d),
+                Id = new Wn.Mo("ant-tree-node-fx-do-not-use", {
                     "0%": {
                         opacity: 0
                     },
                     "100%": {
                         opacity: 1
                     }
                 }),
-                Sd = (e, t) => ({
+                Nd = (e, t) => ({
                     [`.${e}-switcher-icon`]: {
                         display: "inline-block",
                         fontSize: 10,
                         verticalAlign: "baseline",
                         svg: {
                             transition: `transform ${t.motionDurationSlow}`
                         }
                     }
                 }),
-                Ed = (e, t) => ({
+                Md = (e, t) => ({
                     [`.${e}-drop-indicator`]: {
                         position: "absolute",
                         zIndex: 1,
                         height: 2,
                         backgroundColor: t.colorPrimary,
                         borderRadius: 1,
                         pointerEvents: "none",
@@ -25515,15 +25502,15 @@
                             backgroundColor: "transparent",
                             border: `${(0,Wn.zA)(t.lineWidthBold)} solid ${t.colorPrimary}`,
                             borderRadius: "50%",
                             content: '""'
                         }
                     }
                 }),
-                kd = (e, t) => {
+                Rd = (e, t) => {
                     const {
                         treeCls: n,
                         treeNodeCls: r,
                         treeNodePadding: o,
                         titleHeight: i,
                         nodeSelectedBg: a,
                         nodeHoverBg: l
@@ -25560,15 +25547,15 @@
                                             position: "absolute",
                                             top: 0,
                                             insetInlineEnd: 0,
                                             bottom: o,
                                             insetInlineStart: 0,
                                             border: `1px solid ${t.colorPrimary}`,
                                             opacity: 0,
-                                            animationName: Cd,
+                                            animationName: Id,
                                             animationDuration: t.motionDurationSlow,
                                             animationPlayState: "running",
                                             animationFillMode: "forwards",
                                             content: '""',
                                             pointerEvents: "none"
                                         }
                                     }
@@ -25627,15 +25614,15 @@
                                     display: "inline-block",
                                     width: i
                                 }
                             },
                             [`${n}-draggable-icon`]: {
                                 visibility: "hidden"
                             },
-                            [`${n}-switcher`]: Object.assign(Object.assign({}, Sd(e, t)), {
+                            [`${n}-switcher`]: Object.assign(Object.assign({}, Nd(e, t)), {
                                 position: "relative",
                                 flex: "none",
                                 alignSelf: "stretch",
                                 width: i,
                                 margin: 0,
                                 lineHeight: `${(0,Wn.zA)(i)}`,
                                 textAlign: "center",
@@ -25721,15 +25708,15 @@
                             },
                             [`${n}-unselectable ${n}-node-content-wrapper:hover`]: {
                                 backgroundColor: "transparent"
                             },
                             [`${n}-node-content-wrapper`]: Object.assign({
                                 lineHeight: `${(0,Wn.zA)(i)}`,
                                 userSelect: "none"
-                            }, Ed(e, t)),
+                            }, Md(e, t)),
                             [`${r}.drop-container`]: {
                                 "> [draggable]": {
                                     boxShadow: `0 0 0 2px ${t.colorPrimary}`
                                 }
                             },
                             "&-show-line": {
                                 [`${n}-indent`]: {
@@ -25768,15 +25755,15 @@
                                         }
                                     }
                                 }
                             }
                         })
                     }
                 },
-                $d = e => {
+                Pd = e => {
                     const {
                         treeCls: t,
                         treeNodeCls: n,
                         treeNodePadding: r,
                         directoryNodeSelectedBg: o,
                         directoryNodeSelectedColor: i
                     } = e;
@@ -25828,32 +25815,32 @@
                                         background: "transparent"
                                     }
                                 }
                             }
                         }
                     }
                 },
-                Od = (e, t) => {
+                zd = (e, t) => {
                     const n = `.${e}`,
                         r = `${n}-treenode`,
                         o = t.calc(t.paddingXS).div(2).equal(),
                         i = (0, qn.h1)(t, {
                             treeCls: n,
                             treeNodeCls: r,
                             treeNodePadding: o
                         });
-                    return [kd(e, i), $d(i)]
+                    return [Rd(e, i), Pd(i)]
                 },
-                Id = (0, hn.OF)("Tree", ((e, t) => {
+                jd = (0, hn.OF)("Tree", ((e, t) => {
                     let {
                         prefixCls: n
                     } = t;
                     return [{
                         [e.componentCls]: Gn(`${n}-checkbox`, e)
-                    }, Od(n, e), Ji(e)]
+                    }, zd(n, e), Ji(e)]
                 }), (e => {
                     const {
                         colorTextLightSolid: t,
                         colorPrimary: n
                     } = e;
                     return Object.assign(Object.assign({}, (e => {
                         const {
@@ -25866,15 +25853,15 @@
                         }
                     })(e)), {
                         directoryNodeSelectedColor: t,
                         directoryNodeSelectedBg: n
                     })
                 }));
 
-            function Nd(e) {
+            function Td(e) {
                 const {
                     dropPosition: t,
                     dropLevelOffset: n,
                     prefixCls: r,
                     indent: i,
                     direction: a = "ltr"
                 } = e, l = "ltr" === a ? "left" : "right", c = "ltr" === a ? "right" : "left", s = {
@@ -25892,15 +25879,15 @@
                         s.bottom = -3, s[l] = i + 4
                 }
                 return o().createElement("div", {
                     style: s,
                     className: `${r}-drop-indicator`
                 })
             }
-            const Md = {
+            const Bd = {
                 icon: {
                     tag: "svg",
                     attrs: {
                         viewBox: "0 0 1024 1024",
                         focusable: "false"
                     },
                     children: [{
@@ -25909,22 +25896,22 @@
                             d: "M840.4 300H183.6c-19.7 0-30.7 20.8-18.5 35l328.4 380.8c9.4 10.9 27.5 10.9 37 0L858.9 335c12.2-14.2 1.2-35-18.5-35z"
                         }
                     }]
                 },
                 name: "caret-down",
                 theme: "filled"
             };
-            var Rd = function(e, t) {
+            var Dd = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: Md
+                    icon: Bd
                 }))
             };
-            const Pd = r.forwardRef(Rd),
-                zd = {
+            const Fd = r.forwardRef(Dd),
+                Hd = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "64 64 896 896",
                             focusable: "false"
                         },
                         children: [{
@@ -25938,22 +25925,22 @@
                                 d: "M880 112H144c-17.7 0-32 14.3-32 32v736c0 17.7 14.3 32 32 32h736c17.7 0 32-14.3 32-32V144c0-17.7-14.3-32-32-32zm-40 728H184V184h656v656z"
                             }
                         }]
                     },
                     name: "minus-square",
                     theme: "outlined"
                 };
-            var jd = function(e, t) {
+            var Ld = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: zd
+                    icon: Hd
                 }))
             };
-            const Td = r.forwardRef(jd),
-                Bd = {
+            const _d = r.forwardRef(Ld),
+                Kd = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "64 64 896 896",
                             focusable: "false"
                         },
                         children: [{
@@ -25967,22 +25954,22 @@
                                 d: "M880 112H144c-17.7 0-32 14.3-32 32v736c0 17.7 14.3 32 32 32h736c17.7 0 32-14.3 32-32V144c0-17.7-14.3-32-32-32zm-40 728H184V184h656v656z"
                             }
                         }]
                     },
                     name: "plus-square",
                     theme: "outlined"
                 };
-            var Dd = function(e, t) {
+            var Wd = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: Bd
+                    icon: Kd
                 }))
             };
-            const Fd = r.forwardRef(Dd),
-                Hd = e => {
+            const Vd = r.forwardRef(Wd),
+                qd = e => {
                     const {
                         prefixCls: t,
                         switcherIcon: n,
                         treeNodeProps: o,
                         showLine: i
                     } = e, {
                         isLeaf: a,
@@ -25998,33 +25985,33 @@
                         if ("boolean" != typeof s && s) {
                             const e = "function" == typeof s ? s(o) : s,
                                 n = `${t}-switcher-line-custom-icon`;
                             return r.isValidElement(e) ? (0, gn.Ob)(e, {
                                 className: O()(e.props.className || "", n)
                             }) : e
                         }
-                        return s ? r.createElement(pd, {
+                        return s ? r.createElement(yd, {
                             className: `${t}-switcher-line-icon`
                         }) : r.createElement("span", {
                             className: `${t}-switcher-leaf-line`
                         })
                     }
                     const u = `${t}-switcher-icon`,
                         d = "function" == typeof n ? n(o) : n;
                     return r.isValidElement(d) ? (0, gn.Ob)(d, {
                         className: O()(d.props.className || "", u)
-                    }) : void 0 !== d ? d : i ? l ? r.createElement(Td, {
+                    }) : void 0 !== d ? d : i ? l ? r.createElement(_d, {
                         className: `${t}-switcher-line-icon`
-                    }) : r.createElement(Fd, {
+                    }) : r.createElement(Vd, {
                         className: `${t}-switcher-line-icon`
-                    }) : r.createElement(Pd, {
+                    }) : r.createElement(Fd, {
                         className: u
                     })
                 },
-                Ld = o().forwardRef(((e, t) => {
+                Xd = o().forwardRef(((e, t) => {
                     var n;
                     const {
                         getPrefixCls: r,
                         direction: i,
                         virtual: a,
                         tree: l
                     } = o().useContext(mn.QO), {
@@ -26045,28 +26032,28 @@
                     }), C = Object.assign(Object.assign({}, e), {
                         checkable: g,
                         selectable: h,
                         showIcon: u,
                         motion: A,
                         blockNode: p,
                         showLine: Boolean(d),
-                        dropIndicatorRender: Nd
-                    }), [S, E, k] = Id(x), [, $] = (0, yn.Ay)(), I = $.paddingXS / 2 + ((null === (n = $.Tree) || void 0 === n ? void 0 : n.titleHeight) || $.controlHeightSM), N = o().useMemo((() => {
+                        dropIndicatorRender: Td
+                    }), [S, E, k] = jd(x), [, $] = (0, yn.Ay)(), I = $.paddingXS / 2 + ((null === (n = $.Tree) || void 0 === n ? void 0 : n.titleHeight) || $.controlHeightSM), N = o().useMemo((() => {
                         if (!v) return !1;
                         let e = {};
                         switch (typeof v) {
                             case "function":
                                 e.nodeDraggable = v;
                                 break;
                             case "object":
                                 e = Object.assign({}, v)
                         }
-                        return !1 !== e.icon && (e.icon = e.icon || o().createElement(Ad, null)), e
+                        return !1 !== e.icon && (e.icon = e.icon || o().createElement(Od, null)), e
                     }), [v]);
-                    return S(o().createElement(ud, Object.assign({
+                    return S(o().createElement(hd, Object.assign({
                         itemHeight: I,
                         ref: t,
                         virtual: a
                     }, C, {
                         style: Object.assign(Object.assign({}, null == l ? void 0 : l.style), y),
                         prefixCls: x,
                         className: O()({
@@ -26076,83 +26063,83 @@
                             [`${x}-rtl`]: "rtl" === i
                         }, null == l ? void 0 : l.className, s, E, k),
                         direction: i,
                         checkable: g ? o().createElement("span", {
                             className: `${x}-checkbox-inner`
                         }) : g,
                         selectable: h,
-                        switcherIcon: e => o().createElement(Hd, {
+                        switcherIcon: e => o().createElement(qd, {
                             prefixCls: x,
                             switcherIcon: f,
                             treeNodeProps: e,
                             showLine: d
                         }),
                         draggable: N
                     }), m))
                 })),
-                _d = Ld;
+                Gd = Xd;
 
-            function Kd(e, t, n) {
+            function Ud(e, t, n) {
                 const {
                     key: r,
                     children: o
                 } = n;
                 e.forEach((function(e) {
                     const i = e[r],
                         a = e[o];
-                    !1 !== t(i, e) && Kd(a || [], t, n)
+                    !1 !== t(i, e) && Ud(a || [], t, n)
                 }))
             }
 
-            function Wd(e, t, n) {
+            function Yd(e, t, n) {
                 const r = (0, de.A)(t),
                     o = [];
-                return Kd(e, ((e, t) => {
+                return Ud(e, ((e, t) => {
                     const n = r.indexOf(e);
                     return -1 !== n && (o.push(t), r.splice(n, 1)), !!r.length
                 }), Dt(n)), o
             }
-            var Vd = function(e, t) {
+            var Qd = function(e, t) {
                 var n = {};
                 for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
                 if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                     var o = 0;
                     for (r = Object.getOwnPropertySymbols(e); o < r.length; o++) t.indexOf(r[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[o]) && (n[r[o]] = e[r[o]])
                 }
                 return n
             };
 
-            function qd(e) {
+            function Zd(e) {
                 const {
                     isLeaf: t,
                     expanded: n
                 } = e;
-                return t ? r.createElement(pd, null) : n ? r.createElement(hd, null) : r.createElement(yd, null)
+                return t ? r.createElement(yd, null) : n ? r.createElement(Ad, null) : r.createElement(Ed, null)
             }
 
-            function Xd(e) {
+            function Jd(e) {
                 let {
                     treeData: t,
                     children: n
                 } = e;
                 return t || Ft(n)
             }
-            const Gd = (e, t) => {
+            const ef = (e, t) => {
                     var {
                         defaultExpandAll: n,
                         defaultExpandParent: o,
                         defaultExpandedKeys: i
-                    } = e, a = Vd(e, ["defaultExpandAll", "defaultExpandParent", "defaultExpandedKeys"]);
+                    } = e, a = Qd(e, ["defaultExpandAll", "defaultExpandParent", "defaultExpandedKeys"]);
                     const l = r.useRef(),
                         c = r.useRef(),
                         [s, u] = r.useState(a.selectedKeys || a.defaultSelectedKeys || []),
                         [d, f] = r.useState((() => (() => {
                             const {
                                 keyEntities: e
-                            } = Lt(Xd(a));
+                            } = Lt(Jd(a));
                             let t;
                             return t = n ? Object.keys(e) : o ? on(a.expandedKeys || i || [], e) : a.expandedKeys || i || [], t
                         })()));
                     r.useEffect((() => {
                         "selectedKeys" in a && u(a.selectedKeys)
                     }), [a.selectedKeys]), r.useEffect((() => {
                         "expandedKeys" in a && f(a.expandedKeys)
@@ -26161,19 +26148,19 @@
                         getPrefixCls: p,
                         direction: m
                     } = r.useContext(mn.QO), {
                         prefixCls: g,
                         className: h,
                         showIcon: v = !0,
                         expandAction: b = "click"
-                    } = a, y = Vd(a, ["prefixCls", "className", "showIcon", "expandAction"]), x = p("tree", g), w = O()(`${x}-directory`, {
+                    } = a, y = Qd(a, ["prefixCls", "className", "showIcon", "expandAction"]), x = p("tree", g), w = O()(`${x}-directory`, {
                         [`${x}-directory-rtl`]: "rtl" === m
                     }, h);
-                    return r.createElement(_d, Object.assign({
-                        icon: qd,
+                    return r.createElement(Gd, Object.assign({
+                        icon: Zd,
                         ref: t,
                         blockNode: !0
                     }, y, {
                         showIcon: v,
                         expandAction: b,
                         prefixCls: x,
                         className: w,
@@ -26185,29 +26172,29 @@
                                 multiple: r,
                                 fieldNames: o
                             } = a, {
                                 node: i,
                                 nativeEvent: s
                             } = t, {
                                 key: f = ""
-                            } = i, p = Xd(a), m = Object.assign(Object.assign({}, t), {
+                            } = i, p = Jd(a), m = Object.assign(Object.assign({}, t), {
                                 selected: !0
                             }), g = (null == s ? void 0 : s.ctrlKey) || (null == s ? void 0 : s.metaKey), h = null == s ? void 0 : s.shiftKey;
                             let v;
-                            r && g ? (v = e, l.current = f, c.current = v, m.selectedNodes = Wd(p, v, o)) : r && h ? (v = Array.from(new Set([].concat((0, de.A)(c.current || []), (0, de.A)(function(e) {
+                            r && g ? (v = e, l.current = f, c.current = v, m.selectedNodes = Yd(p, v, o)) : r && h ? (v = Array.from(new Set([].concat((0, de.A)(c.current || []), (0, de.A)(function(e) {
                                 let {
                                     treeData: t,
                                     expandedKeys: n,
                                     startKey: r,
                                     endKey: o,
                                     fieldNames: i
                                 } = e;
                                 const a = [];
                                 let l = 0;
-                                return r && r === o ? [r] : r && o ? (Kd(t, (e => {
+                                return r && r === o ? [r] : r && o ? (Ud(t, (e => {
                                     if (2 === l) return !1;
                                     if (function(e) {
                                             return e === r || e === o
                                         }(e)) {
                                         if (a.push(e), 0 === l) l = 1;
                                         else if (1 === l) return l = 2, !1
                                     } else 1 === l && a.push(e);
@@ -26215,28 +26202,28 @@
                                 }), Dt(i)), a) : []
                             }({
                                 treeData: p,
                                 expandedKeys: d,
                                 startKey: f,
                                 endKey: l.current,
                                 fieldNames: o
-                            }))))), m.selectedNodes = Wd(p, v, o)) : (v = [f], l.current = f, c.current = v, m.selectedNodes = Wd(p, v, o)), null === (n = a.onSelect) || void 0 === n || n.call(a, v, m), "selectedKeys" in a || u(v)
+                            }))))), m.selectedNodes = Yd(p, v, o)) : (v = [f], l.current = f, c.current = v, m.selectedNodes = Yd(p, v, o)), null === (n = a.onSelect) || void 0 === n || n.call(a, v, m), "selectedKeys" in a || u(v)
                         },
                         onExpand: (e, t) => {
                             var n;
                             return "expandedKeys" in a || f(e), null === (n = a.onExpand) || void 0 === n ? void 0 : n.call(a, e, t)
                         }
                     }))
                 },
-                Ud = r.forwardRef(Gd),
-                Yd = _d;
-            Yd.DirectoryTree = Ud, Yd.TreeNode = Ut;
-            const Qd = Yd;
-            var Zd = n(4117);
-            const Jd = e => {
+                tf = r.forwardRef(ef),
+                nf = Gd;
+            nf.DirectoryTree = tf, nf.TreeNode = Ut;
+            const rf = nf;
+            var of = n(4117);
+            const af = e => {
                     const {
                         componentCls: t,
                         paddingXS: n
                     } = e;
                     return {
                         [`${t}`]: {
                             display: "inline-flex",
@@ -26255,19 +26242,19 @@
                             },
                             [`&${t}-lg ${t}-input`]: {
                                 paddingInline: e.paddingXS
                             }
                         }
                     }
                 },
-                ef = (0, hn.OF)(["Input", "OTP"], (e => {
+                lf = (0, hn.OF)(["Input", "OTP"], (e => {
                     const t = (0, qn.h1)(e, (0, Eu.C)(e));
-                    return [Jd(t)]
+                    return [af(t)]
                 }), Eu.b);
-            const tf = r.forwardRef(((e, t) => {
+            const cf = r.forwardRef(((e, t) => {
                 const {
                     value: n,
                     onChange: o,
                     onActiveChange: i,
                     index: a
                 } = e, l = function(e, t) {
                     var n = {};
@@ -26282,15 +26269,15 @@
                 const s = () => {
                     (0, Re.A)((() => {
                         var e;
                         const t = null === (e = c.current) || void 0 === e ? void 0 : e.input;
                         document.activeElement === t && t && t.select()
                     }))
                 };
-                return r.createElement(Zd.A, Object.assign({}, l, {
+                return r.createElement(of.A, Object.assign({}, l, {
                     ref: c,
                     value: n,
                     onInput: e => {
                         o(a, e.target.value)
                     },
                     onFocus: s,
                     onKeyDown: e => {
@@ -26303,18 +26290,18 @@
                         "Backspace" !== e.key || n || i(a - 1), s()
                     },
                     onMouseDown: s,
                     onMouseUp: s
                 }))
             }));
 
-            function nf(e) {
+            function sf(e) {
                 return (e || "").split("")
             }
-            const rf = r.forwardRef(((e, t) => {
+            const uf = r.forwardRef(((e, t) => {
                     const {
                         prefixCls: n,
                         length: o = 6,
                         size: i,
                         defaultValue: a,
                         value: l,
                         onChange: c,
@@ -26334,15 +26321,15 @@
                     }(e, ["prefixCls", "length", "size", "defaultValue", "value", "onChange", "formatter", "variant", "disabled", "status", "autoFocus"]), {
                         getPrefixCls: g,
                         direction: h
                     } = r.useContext(mn.QO), v = g("otp", n), b = (0, Q.A)(m, {
                         aria: !0,
                         data: !0,
                         attr: !0
-                    }), y = (0, Ln.A)(v), [x, w, A] = ef(v, y), C = (0, Wa.A)((e => null != i ? i : e)), S = r.useContext(_n.$W), E = (0, Ls.v)(S.status, f), k = r.useMemo((() => Object.assign(Object.assign({}, S), {
+                    }), y = (0, Ln.A)(v), [x, w, A] = lf(v, y), C = (0, Wa.A)((e => null != i ? i : e)), S = r.useContext(_n.$W), E = (0, Ls.v)(S.status, f), k = r.useMemo((() => Object.assign(Object.assign({}, S), {
                         status: E,
                         hasFeedback: !1,
                         feedbackIcon: null
                     })), [S, E]), $ = r.useRef(null), I = r.useRef({});
                     r.useImperativeHandle(t, (() => ({
                         focus: () => {
                             var e;
@@ -26351,28 +26338,28 @@
                         blur: () => {
                             var e;
                             for (let t = 0; t < o; t += 1) null === (e = I.current[t]) || void 0 === e || e.blur()
                         },
                         nativeElement: $.current
                     })));
                     const N = e => s ? s(e) : e,
-                        [M, R] = r.useState(nf(N(a || "")));
+                        [M, R] = r.useState(sf(N(a || "")));
                     r.useEffect((() => {
-                        void 0 !== l && R(nf(l))
+                        void 0 !== l && R(sf(l))
                     }), [l]);
                     const P = (0, T._q)((e => {
                             R(e), c && e.length === o && e.every((e => e)) && e.some(((e, t) => M[t] !== e)) && c(e.join(""))
                         })),
                         z = (0, T._q)(((e, t) => {
                             let n = (0, de.A)(M);
                             for (let t = 0; t < e; t += 1) n[t] || (n[t] = "");
-                            t.length <= 1 ? n[e] = t : n = n.slice(0, e).concat(nf(t)), n = n.slice(0, o);
+                            t.length <= 1 ? n[e] = t : n = n.slice(0, e).concat(sf(t)), n = n.slice(0, o);
                             for (let e = n.length - 1; e >= 0 && !n[e]; e -= 1) n.pop();
                             const r = N(n.map((e => e || " ")).join(""));
-                            return n = nf(r).map(((e, t) => " " !== e || n[t] ? e : n[t])), n
+                            return n = sf(r).map(((e, t) => " " !== e || n[t] ? e : n[t])), n
                         })),
                         j = (e, t) => {
                             var n;
                             const r = z(e, t),
                                 i = Math.min(e + t.length, o - 1);
                             i !== e && (null === (n = I.current[i]) || void 0 === n || n.focus()), P(r)
                         },
@@ -26393,15 +26380,15 @@
                             [`${v}-rtl`]: "rtl" === h
                         }, A, w)
                     }), r.createElement(_n.$W.Provider, {
                         value: k
                     }, new Array(o).fill(0).map(((e, t) => {
                         const n = `otp-${t}`,
                             o = M[t] || "";
-                        return r.createElement(tf, Object.assign({
+                        return r.createElement(cf, Object.assign({
                             ref: e => {
                                 I.current[t] = e
                             },
                             key: n,
                             index: t,
                             size: C,
                             htmlSize: 1,
@@ -26409,15 +26396,15 @@
                             onChange: j,
                             value: o,
                             onActiveChange: B,
                             autoFocus: 0 === t && p
                         }, D))
                     })))))
                 })),
-                of = {
+                df = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "64 64 896 896",
                             focusable: "false"
                         },
                         children: [{
@@ -26431,22 +26418,22 @@
                                 d: "M508 624c-3.46 0-6.87-.16-10.25-.47l-52.82 52.82a176.09 176.09 0 00227.42-227.42l-52.82 52.82c.31 3.38.47 6.79.47 10.25a111.94 111.94 0 01-112 112z"
                             }
                         }]
                     },
                     name: "eye-invisible",
                     theme: "outlined"
                 };
-            var af = function(e, t) {
+            var ff = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: of
+                    icon: df
                 }))
             };
-            const lf = r.forwardRef(af),
-                cf = {
+            const pf = r.forwardRef(ff),
+                mf = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "64 64 896 896",
                             focusable: "false"
                         },
                         children: [{
@@ -26455,35 +26442,35 @@
                                 d: "M942.2 486.2C847.4 286.5 704.1 186 512 186c-192.2 0-335.4 100.5-430.2 300.3a60.3 60.3 0 000 51.5C176.6 737.5 319.9 838 512 838c192.2 0 335.4-100.5 430.2-300.3 7.7-16.2 7.7-35 0-51.5zM512 766c-161.3 0-279.4-81.8-362.7-254C232.6 339.8 350.7 258 512 258c161.3 0 279.4 81.8 362.7 254C791.5 684.2 673.4 766 512 766zm-4-430c-97.2 0-176 78.8-176 176s78.8 176 176 176 176-78.8 176-176-78.8-176-176-176zm0 288c-61.9 0-112-50.1-112-112s50.1-112 112-112 112 50.1 112 112-50.1 112-112 112z"
                             }
                         }]
                     },
                     name: "eye",
                     theme: "outlined"
                 };
-            var sf = function(e, t) {
+            var gf = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: cf
+                    icon: mf
                 }))
             };
-            const uf = r.forwardRef(sf);
-            var df = n(4353);
-            const ff = e => e ? r.createElement(uf, null) : r.createElement(lf, null),
-                pf = {
+            const hf = r.forwardRef(gf);
+            var vf = n(4353);
+            const bf = e => e ? r.createElement(hf, null) : r.createElement(pf, null),
+                yf = {
                     click: "onClick",
                     hover: "onMouseOver"
                 },
-                mf = r.forwardRef(((e, t) => {
+                xf = r.forwardRef(((e, t) => {
                     const {
                         visibilityToggle: n = !0
                     } = e, o = "object" == typeof n && void 0 !== n.visible, [i, a] = (0, r.useState)((() => !!o && n.visible)), l = (0, r.useRef)(null);
                     r.useEffect((() => {
                         o && a(n.visible)
                     }), [o, n]);
-                    const c = (0, df.A)(l),
+                    const c = (0, vf.A)(l),
                         s = () => {
                             const {
                                 disabled: t
                             } = e;
                             t || (i && c(), a((e => {
                                 var t;
                                 const r = !e;
@@ -26509,16 +26496,16 @@
                             getPrefixCls: g
                         } = r.useContext(mn.QO),
                         v = g("input", f),
                         b = g("input-password", d),
                         y = n && (t => {
                             const {
                                 action: n = "click",
-                                iconRender: o = ff
-                            } = e, a = pf[n] || "", l = o(i), c = {
+                                iconRender: o = bf
+                            } = e, a = yf[n] || "", l = o(i), c = {
                                 [a]: s,
                                 className: `${t}-icon`,
                                 key: "passwordIcon",
                                 onMouseDown: e => {
                                     e.preventDefault()
                                 },
                                 onMouseUp: e => {
@@ -26532,20 +26519,20 @@
                         }),
                         w = Object.assign(Object.assign({}, (0, zt.A)(m, ["suffix", "iconRender", "visibilityToggle"])), {
                             type: i ? "text" : "password",
                             className: x,
                             prefixCls: v,
                             suffix: y
                         });
-                    return p && (w.size = p), r.createElement(Zd.A, Object.assign({
+                    return p && (w.size = p), r.createElement(of.A, Object.assign({
                         ref: (0, h.K4)(t, l)
                     }, w))
                 })),
-                gf = mf;
-            const hf = r.forwardRef(((e, t) => {
+                wf = xf;
+            const Af = r.forwardRef(((e, t) => {
                     const {
                         prefixCls: n,
                         inputPrefixCls: o,
                         className: i,
                         size: a,
                         suffix: l,
                         enterButton: c = !1,
@@ -26608,15 +26595,15 @@
                         key: "addonAfter"
                     })]);
                     const z = O()(w, {
                         [`${w}-rtl`]: "rtl" === y,
                         [`${w}-${S}`]: !!S,
                         [`${w}-with-button`]: !!c
                     }, i);
-                    return r.createElement(Zd.A, Object.assign({
+                    return r.createElement(of.A, Object.assign({
                         ref: (0, h.K4)(E, t),
                         onPressEnter: e => {
                             x.current || u || $(e)
                         }
                     }, v, {
                         size: S,
                         onCompositionStart: e => {
@@ -26633,18 +26620,18 @@
                                 source: "clear"
                             }), p && p(e)
                         },
                         className: z,
                         disabled: d
                     }))
                 })),
-                vf = hf;
-            var bf = n(1809);
-            const yf = Zd.A;
-            yf.Group = e => {
+                Cf = Af;
+            var Sf = n(1809);
+            const Ef = of.A;
+            Ef.Group = e => {
                 const {
                     getPrefixCls: t,
                     direction: n
                 } = (0, r.useContext)(mn.QO), {
                     prefixCls: o,
                     className: i
                 } = e, a = t("input-group", o), l = t("input"), [c, s] = (0, Su.Ay)(l), u = O()(a, {
@@ -26661,79 +26648,79 @@
                     onMouseEnter: e.onMouseEnter,
                     onMouseLeave: e.onMouseLeave,
                     onFocus: e.onFocus,
                     onBlur: e.onBlur
                 }, r.createElement(_n.$W.Provider, {
                     value: f
                 }, e.children)))
-            }, yf.Search = vf, yf.TextArea = bf.A, yf.Password = gf, yf.OTP = rf;
-            const xf = yf,
-                wf = function(e) {
+            }, Ef.Search = Cf, Ef.TextArea = Sf.A, Ef.Password = wf, Ef.OTP = uf;
+            const kf = Ef,
+                $f = function(e) {
                     let {
                         value: t,
                         onChange: n,
                         filterSearch: o,
                         tablePrefixCls: i,
                         locale: a
                     } = e;
                     return o ? r.createElement("div", {
                         className: `${i}-filter-dropdown-search`
-                    }, r.createElement(xf, {
+                    }, r.createElement(kf, {
                         prefix: r.createElement(hu, null),
                         placeholder: a.filterSearchPlaceholder,
                         onChange: n,
                         value: t,
                         htmlSize: 1,
                         className: `${i}-filter-dropdown-search-input`
                     })) : null
                 },
-                Af = e => {
+                Of = e => {
                     const {
                         keyCode: t
                     } = e;
                     t === ar.A.ENTER && e.stopPropagation()
                 },
-                Cf = r.forwardRef(((e, t) => r.createElement("div", {
+                If = r.forwardRef(((e, t) => r.createElement("div", {
                     className: e.className,
                     onClick: e => e.stopPropagation(),
-                    onKeyDown: Af,
+                    onKeyDown: Of,
                     ref: t
                 }, e.children)));
 
-            function Sf(e) {
+            function Nf(e) {
                 let t = [];
                 return (e || []).forEach((e => {
                     let {
                         value: n,
                         children: r
                     } = e;
-                    t.push(n), r && (t = [].concat((0, de.A)(t), (0, de.A)(Sf(r))))
+                    t.push(n), r && (t = [].concat((0, de.A)(t), (0, de.A)(Nf(r))))
                 })), t
             }
 
-            function Ef(e, t) {
+            function Mf(e, t) {
                 return ("string" == typeof t || "number" == typeof t) && (null == t ? void 0 : t.toString().toLowerCase().includes(e.trim().toLowerCase()))
             }
 
-            function kf(e) {
+            function Rf(e) {
                 let {
                     filters: t,
                     prefixCls: n,
                     filteredKeys: o,
                     filterMultiple: i,
                     searchValue: a,
                     filterSearch: l
                 } = e;
                 return t.map(((e, t) => {
                     const c = String(e.value);
                     if (e.children) return {
                         key: c || t,
                         label: e.text,
                         popupClassName: `${n}-dropdown-submenu`,
-                        children: kf({
+                        children: Rf({
                             filters: e.children,
                             prefixCls: n,
                             filteredKeys: o,
                             filterMultiple: i,
                             searchValue: a,
                             filterSearch: l
                         })
@@ -26741,22 +26728,22 @@
                     const s = i ? tr : rc,
                         u = {
                             key: void 0 !== e.value ? c : t,
                             label: r.createElement(r.Fragment, null, r.createElement(s, {
                                 checked: o.includes(c)
                             }), r.createElement("span", null, e.text))
                         };
-                    return a.trim() ? "function" == typeof l ? l(a, e) ? u : null : Ef(a, e.text) ? u : null : u
+                    return a.trim() ? "function" == typeof l ? l(a, e) ? u : null : Mf(a, e.text) ? u : null : u
                 }))
             }
 
-            function $f(e) {
+            function Pf(e) {
                 return e || []
             }
-            const Of = function(e) {
+            const zf = function(e) {
                 var t, n;
                 const {
                     tablePrefixCls: o,
                     prefixCls: i,
                     column: a,
                     dropdownPrefixCls: l,
                     columnKey: c,
@@ -26781,15 +26768,15 @@
                     $(e), null == w || w(e), null == E || E(e)
                 }, M = null !== (n = null != x ? x : S) && void 0 !== n ? n : k, R = null == m ? void 0 : m.filteredKeys, [P, z] = function(e) {
                     const t = r.useRef(e),
                         n = wc();
                     return [() => t.current, e => {
                         t.current = e, n()
                     }]
-                }($f(R)), j = e => {
+                }(Pf(R)), j = e => {
                     let {
                         selectedKeys: t
                     } = e;
                     z(t)
                 }, T = (e, t) => {
                     let {
                         node: n,
@@ -26799,15 +26786,15 @@
                         selectedKeys: e
                     } : {
                         selectedKeys: r && n.key ? [n.key] : []
                     })
                 };
                 r.useEffect((() => {
                     k && j({
-                        selectedKeys: $f(R)
+                        selectedKeys: Pf(R)
                     })
                 }), [R]);
                 const [B, D] = r.useState([]), F = e => {
                     D(e)
                 }, [H, L] = r.useState(""), _ = e => {
                     const {
                         value: t
@@ -26845,15 +26832,15 @@
                             } = e;
                             return t
                         })))
                     });
                 var X;
                 const G = e => {
                         if (e.target.checked) {
-                            const e = Sf(null == a ? void 0 : a.filters).map((e => String(e)));
+                            const e = Nf(null == a ? void 0 : a.filters).map((e => String(e)));
                             z(e)
                         } else z([])
                     },
                     U = e => {
                         let {
                             filters: t
                         } = e;
@@ -26910,28 +26897,28 @@
                                 },
                                 style: {
                                     margin: 0,
                                     padding: "16px 0"
                                 }
                             });
                             if (0 === (a.filters || []).length) return t;
-                            if ("tree" === f) return r.createElement(r.Fragment, null, r.createElement(wf, {
+                            if ("tree" === f) return r.createElement(r.Fragment, null, r.createElement($f, {
                                 filterSearch: p,
                                 value: H,
                                 onChange: _,
                                 tablePrefixCls: o,
                                 locale: h
                             }), r.createElement("div", {
                                 className: `${o}-filter-dropdown-tree`
                             }, d ? r.createElement(tr, {
-                                checked: e.length === Sf(a.filters).length,
-                                indeterminate: e.length > 0 && e.length < Sf(a.filters).length,
+                                checked: e.length === Nf(a.filters).length,
+                                indeterminate: e.length > 0 && e.length < Nf(a.filters).length,
                                 className: `${o}-filter-dropdown-checkall`,
                                 onChange: G
-                            }, h.filterCheckall) : null, r.createElement(Qd, {
+                            }, h.filterCheckall) : null, r.createElement(rf, {
                                 checkable: !0,
                                 selectable: !1,
                                 blockNode: !0,
                                 multiple: d,
                                 checkStrictly: !d,
                                 className: `${l}-menu`,
                                 onCheck: T,
@@ -26939,26 +26926,26 @@
                                 selectedKeys: e,
                                 showIcon: !1,
                                 treeData: U({
                                     filters: a.filters
                                 }),
                                 autoExpandParent: !0,
                                 defaultExpandAll: !0,
-                                filterTreeNode: H.trim() ? e => "function" == typeof p ? p(H, Y(e)) : Ef(H, e.title) : void 0
+                                filterTreeNode: H.trim() ? e => "function" == typeof p ? p(H, Y(e)) : Mf(H, e.title) : void 0
                             })));
-                            const n = kf({
+                            const n = Rf({
                                     filters: a.filters || [],
                                     filterSearch: p,
                                     prefixCls: i,
                                     filteredKeys: P(),
                                     filterMultiple: d,
                                     searchValue: H
                                 }),
                                 c = n.every((e => null === e));
-                            return r.createElement(r.Fragment, null, r.createElement(wf, {
+                            return r.createElement(r.Fragment, null, r.createElement($f, {
                                 filterSearch: p,
                                 value: H,
                                 onChange: _,
                                 tablePrefixCls: o,
                                 locale: h
                             }), c ? t : r.createElement($a, {
                                 selectable: !0,
@@ -26986,30 +26973,30 @@
                         type: "primary",
                         size: "small",
                         onClick: W
                     }, h.filterConfirm)))
                 }
                 a.filterDropdown && (Q = r.createElement(Qi, {
                     selectable: void 0
-                }, Q)), Z = "function" == typeof a.filterIcon ? a.filterIcon(I) : a.filterIcon ? a.filterIcon : r.createElement(qu, null);
+                }, Q)), Z = "function" == typeof a.filterIcon ? a.filterIcon(I) : a.filterIcon ? a.filterIcon : r.createElement(Zu, null);
                 const {
                     direction: J
                 } = r.useContext(mn.QO);
                 return r.createElement("div", {
                     className: `${i}-column`
                 }, r.createElement("span", {
                     className: `${o}-column-title`
                 }, v), r.createElement(Hl, {
-                    dropdownRender: () => r.createElement(Cf, {
+                    dropdownRender: () => r.createElement(If, {
                         className: `${i}-dropdown`
                     }, Q),
                     trigger: ["click"],
                     open: M,
                     onOpenChange: (e, t) => {
-                        "trigger" === t.source && (e && void 0 !== R && z($f(R)), N(e), e || a.filterDropdown || !s || W())
+                        "trigger" === t.source && (e && void 0 !== R && z(Pf(R)), N(e), e || a.filterDropdown || !s || W())
                     },
                     getPopupContainer: b,
                     placement: "rtl" === J ? "bottomLeft" : "bottomRight",
                     rootClassName: y
                 }, r.createElement("span", {
                     role: "button",
                     tabIndex: -1,
@@ -27018,145 +27005,145 @@
                     }),
                     onClick: e => {
                         e.stopPropagation()
                     }
                 }, Z)))
             };
 
-            function If(e, t, n) {
+            function jf(e, t, n) {
                 let r = [];
                 return (e || []).forEach(((e, o) => {
                     var i;
-                    const a = _u(o, n);
+                    const a = Gu(o, n);
                     if (e.filters || "filterDropdown" in e || "onFilter" in e)
                         if ("filteredValue" in e) {
                             let t = e.filteredValue;
                             "filterDropdown" in e || (t = null !== (i = null == t ? void 0 : t.map(String)) && void 0 !== i ? i : t), r.push({
                                 column: e,
-                                key: Lu(e, a),
+                                key: Xu(e, a),
                                 filteredKeys: t,
                                 forceFiltered: e.filtered
                             })
                         } else r.push({
                             column: e,
-                            key: Lu(e, a),
+                            key: Xu(e, a),
                             filteredKeys: t && e.defaultFilteredValue ? e.defaultFilteredValue : void 0,
                             forceFiltered: e.filtered
                         });
-                    "children" in e && (r = [].concat((0, de.A)(r), (0, de.A)(If(e.children, t, a))))
+                    "children" in e && (r = [].concat((0, de.A)(r), (0, de.A)(jf(e.children, t, a))))
                 })), r
             }
 
-            function Nf(e, t, n, o, i, a, l, c, s) {
+            function Tf(e, t, n, o, i, a, l, c, s) {
                 return n.map(((n, u) => {
-                    const d = _u(u, c),
+                    const d = Gu(u, c),
                         {
                             filterOnClose: f = !0,
                             filterMultiple: p = !0,
                             filterMode: m,
                             filterSearch: g
                         } = n;
                     let h = n;
                     if (h.filters || h.filterDropdown) {
-                        const c = Lu(h, d),
+                        const c = Xu(h, d),
                             u = o.find((e => {
                                 let {
                                     key: t
                                 } = e;
                                 return c === t
                             }));
                         h = Object.assign(Object.assign({}, h), {
-                            title: o => r.createElement(Of, {
+                            title: o => r.createElement(zf, {
                                 tablePrefixCls: e,
                                 prefixCls: `${e}-filter`,
                                 dropdownPrefixCls: t,
                                 column: h,
                                 columnKey: c,
                                 filterState: u,
                                 filterOnClose: f,
                                 filterMultiple: p,
                                 filterMode: m,
                                 filterSearch: g,
                                 triggerFilter: a,
                                 locale: i,
                                 getPopupContainer: l,
                                 rootClassName: s
-                            }, Ku(n.title, o))
+                            }, Uu(n.title, o))
                         })
                     }
                     return "children" in h && (h = Object.assign(Object.assign({}, h), {
-                        children: Nf(e, t, h.children, o, i, a, l, d, s)
+                        children: Tf(e, t, h.children, o, i, a, l, d, s)
                     })), h
                 }))
             }
 
-            function Mf(e) {
+            function Bf(e) {
                 const t = {};
                 return e.forEach((e => {
                     let {
                         key: n,
                         filteredKeys: r,
                         column: o
                     } = e;
                     const i = n,
                         {
                             filters: a,
                             filterDropdown: l
                         } = o;
                     if (l) t[i] = r || null;
                     else if (Array.isArray(r)) {
-                        const e = Sf(a);
+                        const e = Nf(a);
                         t[i] = e.filter((e => r.includes(String(e))))
                     } else t[i] = null
                 })), t
             }
 
-            function Rf(e, t, n) {
+            function Df(e, t, n) {
                 return t.reduce(((e, r) => {
                     const {
                         column: {
                             onFilter: o,
                             filters: i
                         },
                         filteredKeys: a
                     } = r;
                     return o && a && a.length ? e.map((e => Object.assign({}, e))).filter((e => a.some((r => {
-                        const a = Sf(i),
+                        const a = Nf(i),
                             l = a.findIndex((e => String(e) === String(r))),
                             c = -1 !== l ? a[l] : r;
-                        return e[n] && (e[n] = Rf(e[n], t, n)), o(c, e)
+                        return e[n] && (e[n] = Df(e[n], t, n)), o(c, e)
                     })))) : e
                 }), e)
             }
-            const Pf = e => e.flatMap((e => "children" in e ? [e].concat((0, de.A)(Pf(e.children || []))) : [e])),
-                zf = function(e) {
+            const Ff = e => e.flatMap((e => "children" in e ? [e].concat((0, de.A)(Ff(e.children || []))) : [e])),
+                Hf = function(e) {
                     let {
                         prefixCls: t,
                         dropdownPrefixCls: n,
                         mergedColumns: o,
                         onFilterChange: i,
                         getPopupContainer: a,
                         locale: l,
                         rootClassName: c
                     } = e;
                     (0, un.rJ)("Table");
-                    const s = r.useMemo((() => Pf(o || [])), [o]),
-                        [u, d] = r.useState((() => If(s, !0))),
+                    const s = r.useMemo((() => Ff(o || [])), [o]),
+                        [u, d] = r.useState((() => jf(s, !0))),
                         f = r.useMemo((() => {
-                            const e = If(s, !1);
+                            const e = jf(s, !1);
                             if (0 === e.length) return e;
                             let t = !0,
                                 n = !0;
                             if (e.forEach((e => {
                                     let {
                                         filteredKeys: r
                                     } = e;
                                     void 0 !== r ? t = !1 : n = !1
                                 })), t) {
-                                const e = (s || []).map(((e, t) => Lu(e, _u(t))));
+                                const e = (s || []).map(((e, t) => Xu(e, Gu(t))));
                                 return u.filter((t => {
                                     let {
                                         key: n
                                     } = t;
                                     return e.includes(n)
                                 })).map((t => {
                                     const n = s[e.findIndex((e => e === t.key))];
@@ -27164,28 +27151,28 @@
                                         column: Object.assign(Object.assign({}, t.column), n),
                                         forceFiltered: n.filtered
                                     })
                                 }))
                             }
                             return e
                         }), [s, u]),
-                        p = r.useMemo((() => Mf(f)), [f]),
+                        p = r.useMemo((() => Bf(f)), [f]),
                         m = e => {
                             const t = f.filter((t => {
                                 let {
                                     key: n
                                 } = t;
                                 return n !== e.key
                             }));
-                            t.push(e), d(t), i(Mf(t), t)
+                            t.push(e), d(t), i(Bf(t), t)
                         };
-                    return [e => Nf(t, n, e, f, l, m, a, void 0, c), f, p]
+                    return [e => Tf(t, n, e, f, l, m, a, void 0, c), f, p]
                 };
-            const jf = 10,
-                Tf = function(e, t, n) {
+            const Lf = 10,
+                _f = function(e, t, n) {
                     const o = n && "object" == typeof n ? n : {},
                         {
                             total: i = 0
                         } = o,
                         a = function(e, t) {
                             var n = {};
                             for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
@@ -27193,15 +27180,15 @@
                                 var o = 0;
                                 for (r = Object.getOwnPropertySymbols(e); o < r.length; o++) t.indexOf(r[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[o]) && (n[r[o]] = e[r[o]])
                             }
                             return n
                         }(o, ["total"]),
                         [l, c] = (0, r.useState)((() => ({
                             current: "defaultCurrent" in a ? a.defaultCurrent : 1,
-                            pageSize: "defaultPageSize" in a ? a.defaultPageSize : jf
+                            pageSize: "defaultPageSize" in a ? a.defaultPageSize : Lf
                         }))),
                         s = function() {
                             const e = Object.assign({}, arguments.length <= 0 ? void 0 : arguments[0]);
                             for (let t = 1; t < arguments.length; t++) {
                                 const n = t < 0 || arguments.length <= t ? void 0 : arguments[t];
                                 n && Object.keys(n).forEach((t => {
                                     const r = n[t];
@@ -27223,15 +27210,15 @@
                     return !1 === n ? [{}, () => {}] : [Object.assign(Object.assign({}, s), {
                         onChange: (e, r) => {
                             var o;
                             n && (null === (o = n.onChange) || void 0 === o || o.call(n, e, r)), d(e, r), t(e, r || (null == s ? void 0 : s.pageSize))
                         }
                     }), d]
                 },
-                Bf = {
+                Kf = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "0 0 1024 1024",
                             focusable: "false"
                         },
                         children: [{
@@ -27240,22 +27227,22 @@
                                 d: "M840.4 300H183.6c-19.7 0-30.7 20.8-18.5 35l328.4 380.8c9.4 10.9 27.5 10.9 37 0L858.9 335c12.2-14.2 1.2-35-18.5-35z"
                             }
                         }]
                     },
                     name: "caret-down",
                     theme: "outlined"
                 };
-            var Df = function(e, t) {
+            var Wf = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: Bf
+                    icon: Kf
                 }))
             };
-            const Ff = r.forwardRef(Df),
-                Hf = {
+            const Vf = r.forwardRef(Wf),
+                qf = {
                     icon: {
                         tag: "svg",
                         attrs: {
                             viewBox: "0 0 1024 1024",
                             focusable: "false"
                         },
                         children: [{
@@ -27264,62 +27251,62 @@
                                 d: "M858.9 689L530.5 308.2c-9.4-10.9-27.5-10.9-37 0L165.1 689c-12.2 14.2-1.2 35 18.5 35h656.8c19.7 0 30.7-20.8 18.5-35z"
                             }
                         }]
                     },
                     name: "caret-up",
                     theme: "outlined"
                 };
-            var Lf = function(e, t) {
+            var Xf = function(e, t) {
                 return r.createElement(St.A, (0, g.A)({}, e, {
                     ref: t,
-                    icon: Hf
+                    icon: qf
                 }))
             };
-            const _f = r.forwardRef(Lf),
-                Kf = "ascend",
-                Wf = "descend";
+            const Gf = r.forwardRef(Xf),
+                Uf = "ascend",
+                Yf = "descend";
 
-            function Vf(e) {
+            function Qf(e) {
                 return "object" == typeof e.sorter && "number" == typeof e.sorter.multiple && e.sorter.multiple
             }
 
-            function qf(e) {
+            function Zf(e) {
                 return "function" == typeof e ? e : !(!e || "object" != typeof e || !e.compare) && e.compare
             }
 
-            function Xf(e, t, n) {
+            function Jf(e, t, n) {
                 let r = [];
 
                 function o(e, t) {
                     r.push({
                         column: e,
-                        key: Lu(e, t),
-                        multiplePriority: Vf(e),
+                        key: Xu(e, t),
+                        multiplePriority: Qf(e),
                         sortOrder: e.sortOrder
                     })
                 }
                 return (e || []).forEach(((e, i) => {
-                    const a = _u(i, n);
-                    e.children ? ("sortOrder" in e && o(e, a), r = [].concat((0, de.A)(r), (0, de.A)(Xf(e.children, t, a)))) : e.sorter && ("sortOrder" in e ? o(e, a) : t && e.defaultSortOrder && r.push({
+                    const a = Gu(i, n);
+                    e.children ? ("sortOrder" in e && o(e, a), r = [].concat((0, de.A)(r), (0, de.A)(Jf(e.children, t, a)))) : e.sorter && ("sortOrder" in e ? o(e, a) : t && e.defaultSortOrder && r.push({
                         column: e,
-                        key: Lu(e, a),
-                        multiplePriority: Vf(e),
+                        key: Xu(e, a),
+                        multiplePriority: Qf(e),
                         sortOrder: e.defaultSortOrder
                     }))
                 })), r
             }
 
-            function Gf(e, t, n, o, i, a, l, c) {
+            function ep(e, t, n, o, i, a, l, c) {
                 return (t || []).map(((t, s) => {
-                    const u = _u(s, c);
+                    const u = Gu(s, c);
                     let d = t;
                     if (d.sorter) {
                         const c = d.sortDirections || i,
                             s = void 0 === d.showSorterTooltip ? l : d.showSorterTooltip,
-                            f = Lu(d, u),
+                            f = Xu(d, u),
                             p = n.find((e => {
                                 let {
                                     key: t
                                 } = e;
                                 return t === f
                             })),
                             m = p ? p.sortOrder : null,
@@ -27327,22 +27314,22 @@
                                 return t ? e[e.indexOf(t) + 1] : e[0]
                             }(c, m);
                         let h;
                         if (t.sortIcon) h = t.sortIcon({
                             sortOrder: m
                         });
                         else {
-                            const t = c.includes(Kf) && r.createElement(_f, {
+                            const t = c.includes(Uf) && r.createElement(Gf, {
                                     className: O()(`${e}-column-sorter-up`, {
-                                        active: m === Kf
+                                        active: m === Uf
                                     })
                                 }),
-                                n = c.includes(Wf) && r.createElement(Ff, {
+                                n = c.includes(Yf) && r.createElement(Vf, {
                                     className: O()(`${e}-column-sorter-down`, {
-                                        active: m === Wf
+                                        active: m === Yf
                                     })
                                 });
                             h = r.createElement("span", {
                                 className: O()(`${e}-column-sorter`, {
                                     [`${e}-column-sorter-full`]: !(!t || !n)
                                 })
                             }, r.createElement("span", {
@@ -27352,29 +27339,29 @@
                         }
                         const {
                             cancelSort: v,
                             triggerAsc: b,
                             triggerDesc: y
                         } = a || {};
                         let x = v;
-                        g === Wf ? x = y : g === Kf && (x = b);
+                        g === Yf ? x = y : g === Uf && (x = b);
                         const w = "object" == typeof s ? Object.assign({
                             title: x
                         }, s) : {
                             title: x
                         };
                         d = Object.assign(Object.assign({}, d), {
                             className: O()(d.className, {
                                 [`${e}-column-sort`]: m
                             }),
                             title: n => {
                                 const o = `${e}-column-sorters`,
                                     i = r.createElement("span", {
                                         className: `${e}-column-title`
-                                    }, Ku(t.title, n)),
+                                    }, Uu(t.title, n)),
                                     a = r.createElement("div", {
                                         className: o
                                     }, i, h);
                                 return s ? "boolean" != typeof s && "sorter-icon" === (null == s ? void 0 : s.target) ? r.createElement("div", {
                                     className: `${o} ${e}-column-sorters-tooltip-target-sorter`
                                 }, i, r.createElement(_i.A, Object.assign({}, w), h)) : r.createElement(_i.A, Object.assign({}, w), a) : a
                             },
@@ -27383,129 +27370,129 @@
                                     i = r.onClick,
                                     a = r.onKeyDown;
                                 r.onClick = e => {
                                     o({
                                         column: t,
                                         key: f,
                                         sortOrder: g,
-                                        multiplePriority: Vf(t)
+                                        multiplePriority: Qf(t)
                                     }), null == i || i(e)
                                 }, r.onKeyDown = e => {
                                     e.keyCode === ar.A.ENTER && (o({
                                         column: t,
                                         key: f,
                                         sortOrder: g,
-                                        multiplePriority: Vf(t)
+                                        multiplePriority: Qf(t)
                                     }), null == a || a(e))
                                 };
                                 const l = function(e, t) {
-                                        const n = Ku(e, {});
+                                        const n = Uu(e, {});
                                         return "[object Object]" === Object.prototype.toString.call(n) ? "" : n
                                     }(t.title),
                                     c = null == l ? void 0 : l.toString();
                                 return m ? r["aria-sort"] = "ascend" === m ? "ascending" : "descending" : r["aria-label"] = c || "", r.className = O()(r.className, `${e}-column-has-sorters`), r.tabIndex = 0, t.ellipsis && (r.title = (null != l ? l : "").toString()), r
                             }
                         })
                     }
                     return "children" in d && (d = Object.assign(Object.assign({}, d), {
-                        children: Gf(e, d.children, n, o, i, a, l, u)
+                        children: ep(e, d.children, n, o, i, a, l, u)
                     })), d
                 }))
             }
-            const Uf = e => {
+            const tp = e => {
                     const {
                         column: t,
                         sortOrder: n
                     } = e;
                     return {
                         column: t,
                         order: n,
                         field: t.dataIndex,
                         columnKey: t.key
                     }
                 },
-                Yf = e => {
+                np = e => {
                     const t = e.filter((e => {
                         let {
                             sortOrder: t
                         } = e;
                         return t
-                    })).map(Uf);
+                    })).map(tp);
                     if (0 === t.length && e.length) {
                         const t = e.length - 1;
-                        return Object.assign(Object.assign({}, Uf(e[t])), {
+                        return Object.assign(Object.assign({}, tp(e[t])), {
                             column: void 0
                         })
                     }
                     return t.length <= 1 ? t[0] || {} : t
                 };
 
-            function Qf(e, t, n) {
+            function rp(e, t, n) {
                 const r = t.slice().sort(((e, t) => t.multiplePriority - e.multiplePriority)),
                     o = e.slice(),
                     i = r.filter((e => {
                         let {
                             column: {
                                 sorter: t
                             },
                             sortOrder: n
                         } = e;
-                        return qf(t) && n
+                        return Zf(t) && n
                     }));
                 return i.length ? o.sort(((e, t) => {
                     for (let n = 0; n < i.length; n += 1) {
                         const r = i[n],
                             {
                                 column: {
                                     sorter: o
                                 },
                                 sortOrder: a
                             } = r,
-                            l = qf(o);
+                            l = Zf(o);
                         if (l && a) {
                             const n = l(e, t, a);
-                            if (0 !== n) return a === Kf ? n : -n
+                            if (0 !== n) return a === Uf ? n : -n
                         }
                     }
                     return 0
                 })).map((e => {
                     const r = e[n];
                     return r ? Object.assign(Object.assign({}, e), {
-                        [n]: Qf(r, t, n)
+                        [n]: rp(r, t, n)
                     }) : e
                 })) : o
             }
 
-            function Zf(e, t) {
+            function op(e, t) {
                 return e.map((e => {
                     const n = Object.assign({}, e);
-                    return n.title = Ku(e.title, t), "children" in n && (n.children = Zf(n.children, t)), n
+                    return n.title = Uu(e.title, t), "children" in n && (n.children = op(n.children, t)), n
                 }))
             }
 
-            function Jf(e) {
-                return [r.useCallback((t => Zf(t, e)), [e])]
+            function ip(e) {
+                return [r.useCallback((t => op(t, e)), [e])]
             }
-            const ep = Le(((e, t) => {
+            const ap = Le(((e, t) => {
                     const {
                         _renderTimes: n
                     } = e, {
                         _renderTimes: r
                     } = t;
                     return n !== r
                 })),
-                tp = At(((e, t) => {
+                lp = At(((e, t) => {
                     const {
                         _renderTimes: n
                     } = e, {
                         _renderTimes: r
                     } = t;
                     return n !== r
                 })),
-                np = e => {
+                cp = e => {
                     const {
                         componentCls: t,
                         lineWidth: n,
                         lineType: r,
                         tableBorderColor: o,
                         tableHeaderBg: i,
                         tablePaddingVertical: a,
@@ -27595,15 +27582,15 @@
                             },
                             [`${t}-bordered ${t}-cell-scrollbar`]: {
                                 borderInlineEnd: s
                             }
                         }
                     }
                 },
-                rp = e => {
+                sp = e => {
                     const {
                         componentCls: t
                     } = e;
                     return {
                         [`${t}-wrapper`]: {
                             [`${t}-cell-ellipsis`]: Object.assign(Object.assign({}, Vn.L9), {
                                 wordBreak: "keep-all",
@@ -27620,15 +27607,15 @@
                                     textOverflow: "ellipsis",
                                     wordBreak: "keep-all"
                                 }
                             })
                         }
                     }
                 },
-                op = e => {
+                up = e => {
                     const {
                         componentCls: t
                     } = e;
                     return {
                         [`${t}-wrapper`]: {
                             [`${t}-tbody > tr${t}-placeholder`]: {
                                 textAlign: "center",
@@ -27636,16 +27623,16 @@
                                 "\n          &:hover > th,\n          &:hover > td,\n        ": {
                                     background: e.colorBgContainer
                                 }
                             }
                         }
                     }
                 };
-            var ip = n(3452);
-            const ap = e => {
+            var dp = n(3452);
+            const fp = e => {
                     const {
                         componentCls: t,
                         antCls: n,
                         motionDurationSlow: r,
                         lineWidth: o,
                         paddingXS: i,
                         lineType: a,
@@ -27676,15 +27663,15 @@
                                     verticalAlign: "sub"
                                 }
                             },
                             [`${t}-row-indent`]: {
                                 height: 1,
                                 float: "left"
                             },
-                            [`${t}-row-expand-icon`]: Object.assign(Object.assign({}, (0, ip.Y)(e)), {
+                            [`${t}-row-expand-icon`]: Object.assign(Object.assign({}, (0, dp.Y)(e)), {
                                 position: "relative",
                                 float: "left",
                                 boxSizing: "border-box",
                                 width: h,
                                 height: h,
                                 padding: 0,
                                 color: "inherit",
@@ -27755,15 +27742,15 @@
                                 position: "relative",
                                 margin: `${(0,Wn.zA)(y(d).mul(-1).equal())} ${(0,Wn.zA)(y(f).mul(-1).equal())}`,
                                 padding: `${(0,Wn.zA)(d)} ${(0,Wn.zA)(f)}`
                             }
                         }
                     }
                 },
-                lp = e => {
+                pp = e => {
                     const {
                         componentCls: t,
                         antCls: n,
                         iconCls: r,
                         tableFilterDropdownWidth: o,
                         tableFilterDropdownSearchWidth: i,
                         paddingXXS: a,
@@ -27891,15 +27878,15 @@
                                 maxHeight: "calc(100vh - 130px)",
                                 overflowX: "hidden",
                                 overflowY: "auto"
                             }
                         }
                     }]
                 },
-                cp = e => {
+                mp = e => {
                     const {
                         componentCls: t,
                         lineWidth: n,
                         colorSplit: r,
                         motionDurationSlow: o,
                         zIndexTableFixed: i,
                         tableBg: a,
@@ -27988,15 +27975,15 @@
                                 [`\n        ${t}-cell-fix-left-first::after,\n        ${t}-cell-fix-left-last::after,\n        ${t}-cell-fix-right-first::after,\n        ${t}-cell-fix-right-last::after\n      `]: {
                                     boxShadow: "none"
                                 }
                             }
                         }
                     }
                 },
-                sp = e => {
+                gp = e => {
                     const {
                         componentCls: t,
                         antCls: n,
                         margin: r
                     } = e;
                     return {
                         [`${t}-wrapper`]: {
@@ -28019,15 +28006,15 @@
                                 "&-right": {
                                     justifyContent: "flex-end"
                                 }
                             }
                         }
                     }
                 },
-                up = e => {
+                hp = e => {
                     const {
                         componentCls: t,
                         tableRadius: n
                     } = e;
                     return {
                         [`${t}-wrapper`]: {
                             [t]: {
@@ -28061,15 +28048,15 @@
                                 "&-footer": {
                                     borderRadius: `0 0 ${(0,Wn.zA)(n)} ${(0,Wn.zA)(n)}`
                                 }
                             }
                         }
                     }
                 },
-                dp = e => {
+                vp = e => {
                     const {
                         componentCls: t
                     } = e;
                     return {
                         [`${t}-wrapper-rtl`]: {
                             direction: "rtl",
                             table: {
@@ -28105,15 +28092,15 @@
                                 [`${t}-row-indent`]: {
                                     float: "right"
                                 }
                             }
                         }
                     }
                 },
-                fp = e => {
+                bp = e => {
                     const {
                         componentCls: t,
                         antCls: n,
                         iconCls: r,
                         fontSizeIcon: o,
                         padding: i,
                         paddingXS: a,
@@ -28190,15 +28177,15 @@
                                         background: f
                                     }
                                 }
                             }
                         }
                     }
                 },
-                pp = e => {
+                yp = e => {
                     const {
                         componentCls: t,
                         tableExpandColumnWidth: n,
                         calc: r
                     } = e, o = (e, o, i, a) => ({
                         [`${t}${t}-${e}`]: {
                             fontSize: a,
@@ -28222,15 +28209,15 @@
                             }
                         }
                     });
                     return {
                         [`${t}-wrapper`]: Object.assign(Object.assign({}, o("middle", e.tablePaddingVerticalMiddle, e.tablePaddingHorizontalMiddle, e.tableFontSizeMiddle)), o("small", e.tablePaddingVerticalSmall, e.tablePaddingHorizontalSmall, e.tableFontSizeSmall))
                     }
                 },
-                mp = e => {
+                xp = e => {
                     const {
                         componentCls: t,
                         marginXXS: n,
                         fontSizeIcon: r,
                         headerIconColor: o,
                         headerIconHoverColor: i
                     } = e;
@@ -28307,15 +28294,15 @@
                             },
                             [`${t}-column-sorters:hover ${t}-column-sorter`]: {
                                 color: i
                             }
                         }
                     }
                 },
-                gp = e => {
+                wp = e => {
                     const {
                         componentCls: t,
                         opacityLoading: n,
                         tableScrollThumbBg: r,
                         tableScrollThumbBgHover: o,
                         tableScrollThumbSize: i,
                         tableScrollBg: a,
@@ -28358,15 +28345,15 @@
                                         }
                                     }
                                 }
                             }
                         }
                     }
                 },
-                hp = e => {
+                Ap = e => {
                     const {
                         componentCls: t,
                         lineWidth: n,
                         tableBorderColor: r,
                         calc: o
                     } = e, i = `${(0,Wn.zA)(n)} ${e.lineType} ${r}`;
                     return {
@@ -28383,15 +28370,15 @@
                             },
                             [`div${t}-summary`]: {
                                 boxShadow: `0 ${(0,Wn.zA)(o(n).mul(-1).equal())} 0 ${r}`
                             }
                         }
                     }
                 },
-                vp = e => {
+                Cp = e => {
                     const {
                         componentCls: t,
                         motionDurationMid: n,
                         lineWidth: r,
                         lineType: o,
                         tableBorderColor: i,
                         calc: a
@@ -28444,15 +28431,15 @@
                                         borderBottom: l
                                     }
                                 }
                             }
                         }
                     }
                 },
-                bp = e => {
+                Sp = e => {
                     const {
                         componentCls: t,
                         fontWeightStrong: n,
                         tablePaddingVertical: r,
                         tablePaddingHorizontal: o,
                         tableExpandColumnWidth: i,
                         lineWidth: a,
@@ -28556,15 +28543,15 @@
                                 padding: `${(0,Wn.zA)(r)} ${(0,Wn.zA)(o)}`,
                                 color: h,
                                 background: v
                             }
                         })
                     }
                 },
-                yp = (0, hn.OF)("Table", (e => {
+                Ep = (0, hn.OF)("Table", (e => {
                     const {
                         colorTextHeading: t,
                         colorSplit: n,
                         colorBgContainer: r,
                         controlInteractiveSize: o,
                         headerBg: i,
                         headerColor: a,
@@ -28633,15 +28620,15 @@
                         tableFilterDropdownHeight: 264,
                         tableFilterDropdownSearchWidth: 140,
                         tableScrollThumbSize: 8,
                         tableScrollThumbBg: P,
                         tableScrollThumbBgHover: t,
                         tableScrollBg: n
                     });
-                    return [bp(j), sp(j), hp(j), mp(j), lp(j), np(j), up(j), ap(j), hp(j), op(j), fp(j), cp(j), gp(j), rp(j), pp(j), dp(j), vp(j)]
+                    return [Sp(j), gp(j), Ap(j), xp(j), pp(j), cp(j), hp(j), fp(j), Ap(j), up(j), bp(j), mp(j), wp(j), sp(j), yp(j), vp(j), Cp(j)]
                 }), (e => {
                     const {
                         colorFillAlter: t,
                         colorBgContainer: n,
                         colorTextHeading: r,
                         colorFillSecondary: o,
                         colorFillContent: i,
@@ -28703,16 +28690,16 @@
                         expandIconScale: A / I
                     }
                 }), {
                     unitless: {
                         expandIconScale: !0
                     }
                 }),
-                xp = [],
-                wp = (e, t) => {
+                kp = [],
+                $p = (e, t) => {
                     var n, o;
                     const {
                         prefixCls: i,
                         className: l,
                         rootClassName: c,
                         style: s,
                         size: u,
@@ -28757,20 +28744,20 @@
                             table: _,
                             renderEmpty: K,
                             getPrefixCls: W,
                             getPopupContainer: V
                         } = r.useContext(mn.QO),
                         q = (0, Wa.A)(u),
                         X = Object.assign(Object.assign({}, H.Table), R),
-                        G = p || xp,
+                        G = p || kp,
                         U = W("table", i),
                         Y = W("dropdown", f),
                         [, Q] = (0, yn.Ay)(),
                         Z = (0, Ln.A)(U),
-                        [J, ee, te] = yp(U, Z),
+                        [J, ee, te] = Ep(U, Z),
                         ne = Object.assign(Object.assign({
                             childrenColumnName: x,
                             expandIconColumnIndex: $
                         }, E), {
                             expandIcon: null !== (n = null == E ? void 0 : E.expandIcon) && void 0 !== n ? n : null === (o = null == _ ? void 0 : _.expandable) || void 0 === o ? void 0 : o.expandIcon
                         }),
                         {
@@ -28860,30 +28847,30 @@
                                         }(t > o ? o : t, a, e, o);
                                     uc(i) ? i.scrollTo(window.pageXOffset, n) : i instanceof Document || "HTMLDocument" === i.constructor.name ? i.documentElement.scrollTop = n : i.scrollTop = n, t < o ? (0, Re.A)(c) : "function" == typeof r && r()
                                 };
                                 (0, Re.A)(c)
                             }(0, {
                                 getContainer: () => ie.body.current
                             }), null == w || w(a.pagination, a.filters, a.sorter, {
-                                currentDataSource: Rf(Qf(G, a.sorterStates, re), a.filterStates, re),
+                                currentDataSource: Df(rp(G, a.sorterStates, re), a.filterStates, re),
                                 action: t
                             })
                         },
                         [ge, he, ve, be] = function(e) {
                             let {
                                 prefixCls: t,
                                 mergedColumns: n,
                                 onSorterChange: o,
                                 sortDirections: i,
                                 tableLocale: a,
                                 showSorterTooltip: l
                             } = e;
-                            const [c, s] = r.useState(Xf(n, !0)), u = r.useMemo((() => {
+                            const [c, s] = r.useState(Jf(n, !0)), u = r.useMemo((() => {
                                 let e = !0;
-                                const t = Xf(n, !1);
+                                const t = Jf(n, !1);
                                 if (!t.length) return c;
                                 const r = [];
 
                                 function o(t) {
                                     e ? r.push(t) : r.push(Object.assign(Object.assign({}, t), {
                                         sortOrder: null
                                     }))
@@ -28911,57 +28898,57 @@
                             }), [u]), f = e => {
                                 let t;
                                 t = !1 !== e.multiplePriority && u.length && !1 !== u[0].multiplePriority ? [].concat((0, de.A)(u.filter((t => {
                                     let {
                                         key: n
                                     } = t;
                                     return n !== e.key
-                                }))), [e]) : [e], s(t), o(Yf(t), t)
+                                }))), [e]) : [e], s(t), o(np(t), t)
                             };
-                            return [e => Gf(t, e, u, f, i, a, l), u, d, () => Yf(u)]
+                            return [e => ep(t, e, u, f, i, a, l), u, d, () => np(u)]
                         }({
                             prefixCls: U,
                             mergedColumns: D,
                             onSorterChange: (e, t) => {
                                 me({
                                     sorter: e,
                                     sorterStates: t
                                 }, "sort", !1)
                             },
                             sortDirections: M || ["ascend", "descend"],
                             tableLocale: X,
                             showSorterTooltip: P
                         }),
-                        ye = r.useMemo((() => Qf(G, he, re)), [G, he]);
+                        ye = r.useMemo((() => rp(G, he, re)), [G, he]);
                     pe.sorter = be(), pe.sorterStates = he;
-                    const [xe, Ae, Ce] = zf({
+                    const [xe, Ae, Ce] = Hf({
                         prefixCls: U,
                         locale: X,
                         dropdownPrefixCls: Y,
                         mergedColumns: D,
                         onFilterChange: (e, t) => {
                             me({
                                 filters: e,
                                 filterStates: t
                             }, "filter", !0)
                         },
                         getPopupContainer: A || V,
                         rootClassName: O()(c, Z)
-                    }), Se = Rf(ye, Ae, re);
+                    }), Se = Df(ye, Ae, re);
                     pe.filters = Ce, pe.filterStates = Ae;
                     const Ee = r.useMemo((() => {
                             const e = {};
                             return Object.keys(Ce).forEach((t => {
                                 null !== Ce[t] && (e[t] = Ce[t])
                             })), Object.assign(Object.assign({}, ve), {
                                 filters: e
                             })
                         }), [ve, Ce]),
-                        [ke] = Jf(Ee),
-                        [$e, Oe] = Tf(Se.length, ((e, t) => {
+                        [ke] = ip(Ee),
+                        [$e, Oe] = _f(Se.length, ((e, t) => {
                             me({
                                 pagination: Object.assign(Object.assign({}, pe.pagination), {
                                     current: e,
                                     pageSize: t
                                 })
                             }, "paginate")
                         }), m);
@@ -28977,15 +28964,15 @@
                         })), n
                     }($e, m), pe.resetPagination = Oe;
                     const Ie = r.useMemo((() => {
                             if (!1 === m || !$e.pageSize) return Se;
                             const {
                                 current: e = 1,
                                 total: t,
-                                pageSize: n = jf
+                                pageSize: n = Lf
                             } = $e;
                             return Se.length < t ? Se.length > n ? Se.slice((e - 1) * n, e * n) : Se : Se.slice((e - 1) * n, e * n)
                         }), [!!m, Se, $e && $e.current, $e && $e.pageSize, $e && $e.total]),
                         [Ne, Me] = ((e, t) => {
                             const {
                                 preserveSelectedRowKeys: n,
                                 selectedRowKeys: o,
@@ -29388,15 +29375,15 @@
                     const Be = O()(te, Z, `${U}-wrapper`, null == _ ? void 0 : _.className, {
                             [`${U}-wrapper-rtl`]: "rtl" === L
                         }, l, c, ee),
                         De = Object.assign(Object.assign({}, null == _ ? void 0 : _.style), s),
                         Fe = R && R.emptyText || (null == K ? void 0 : K("Table")) || r.createElement(xc, {
                             componentName: "Table"
                         }),
-                        He = z ? tp : ep,
+                        He = z ? lp : ap,
                         Le = {},
                         _e = r.useMemo((() => {
                             const {
                                 fontSize: e,
                                 lineHeight: t,
                                 padding: n,
                                 paddingXS: r,
@@ -29411,15 +29398,15 @@
                                     return 2 * o + i
                             }
                         }), [Q, q]);
                     return z && (Le.listItemHeight = _e), J(r.createElement("div", {
                         ref: le,
                         className: Be,
                         style: De
-                    }, r.createElement(Hu.A, Object.assign({
+                    }, r.createElement(qu, Object.assign({
                         spinning: !1
                     }, Te), ze, r.createElement(He, Object.assign({}, Le, F, {
                         ref: se,
                         columns: D,
                         direction: L,
                         expandable: ne,
                         prefixCls: U,
@@ -29440,29 +29427,29 @@
                         emptyText: Fe,
                         internalHooks: a,
                         internalRefs: ie,
                         transformColumns: Pe,
                         getContainerWidth: ae
                     })), je)))
                 },
-                Ap = r.forwardRef(wp),
-                Cp = (e, t) => {
+                Op = r.forwardRef($p),
+                Ip = (e, t) => {
                     const n = r.useRef(0);
-                    return n.current += 1, r.createElement(Ap, Object.assign({}, e, {
+                    return n.current += 1, r.createElement(Op, Object.assign({}, e, {
                         ref: t,
                         _renderTimes: n.current
                     }))
                 },
-                Sp = r.forwardRef(Cp);
-            Sp.SELECTION_COLUMN = oc, Sp.EXPAND_COLUMN = i, Sp.SELECTION_ALL = ic, Sp.SELECTION_INVERT = ac, Sp.SELECTION_NONE = lc, Sp.Column = function(e) {
+                Np = r.forwardRef(Ip);
+            Np.SELECTION_COLUMN = oc, Np.EXPAND_COLUMN = i, Np.SELECTION_ALL = ic, Np.SELECTION_INVERT = ac, Np.SELECTION_NONE = lc, Np.Column = function(e) {
                 return null
-            }, Sp.ColumnGroup = function(e) {
+            }, Np.ColumnGroup = function(e) {
                 return null
-            }, Sp.Summary = q;
-            const Ep = Sp
+            }, Np.Summary = q;
+            const Mp = Np
         },
         6369: (e, t, n) => {
             "use strict";
             n.d(t, {
                 vG: () => h,
                 sb: () => g,
                 zQ: () => m
@@ -32586,15 +32573,15 @@
                                 se = le[1],
                                 ue = (0, d.useRef)(!1),
                                 de = (0, d.useRef)(null);
 
                             function fe() {
                                 return function() {
                                     try {
-                                        return z.current instanceof HTMLElement ? z.current : (0, s.A)(j.current)
+                                        return z.current instanceof HTMLElement ? z.current : (0, s.Ay)(j.current)
                                     } catch (e) {
                                         return null
                                     }
                                 }()
                             }
                             var pe = (0, d.useRef)(!1);
 
@@ -33262,15 +33249,15 @@
                         offsetHeight: -1
                     }),
                     h = !p && o.isValidElement(m) && (0, s.f3)(m),
                     v = h ? m.ref : null,
                     b = (0, s.xK)(v, i),
                     y = function() {
                         var e;
-                        return (0, c.A)(i.current) || (i.current && "object" === (0, l.A)(i.current) ? (0, c.A)(null === (e = i.current) || void 0 === e ? void 0 : e.nativeElement) : null) || (0, c.A)(d.current)
+                        return (0, c.Ay)(i.current) || (i.current && "object" === (0, l.A)(i.current) ? (0, c.Ay)(null === (e = i.current) || void 0 === e ? void 0 : e.nativeElement) : null) || (0, c.Ay)(d.current)
                     };
                 o.useImperativeHandle(t, (function() {
                     return y()
                 }));
                 var x = o.useRef(e);
                 x.current = e;
                 var w = o.useCallback((function(e) {
@@ -33479,29 +33466,32 @@
                 var v = f(e, a);
                 return v.setAttribute(s(a), t), v
             }
         },
         8299: (e, t, n) => {
             "use strict";
             n.d(t, {
-                A: () => s,
-                f: () => c
+                Ay: () => s,
+                fk: () => c
             });
             var r = n(4086),
                 o = n(3345),
                 i = n.n(o),
                 a = n(7628),
                 l = n.n(a);
 
             function c(e) {
                 return e instanceof HTMLElement || e instanceof SVGElement
             }
 
             function s(e) {
-                return e && "object" === (0, r.A)(e) && c(e.nativeElement) ? e.nativeElement : c(e) ? e : e instanceof i().Component ? l().findDOMNode(e) : null
+                var t, n = function(e) {
+                    return e && "object" === (0, r.A)(e) && c(e.nativeElement) ? e.nativeElement : c(e) ? e : null
+                }(e);
+                return n || (e instanceof i().Component ? null === (t = l().findDOMNode) || void 0 === t ? void 0 : t.call(l(), e) : null)
             }
         },
         3700: (e, t, n) => {
             "use strict";
             n.d(t, {
                 A: () => r
             });
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/818.9952ec63ac4e7e5b37d1.js.LICENSE.txt` & `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/595.853e8b63deafdcf653a9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/remoteEntry.5034e9c3d84820fce19f.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/remoteEntry.871deda2d395cf3ebdb5.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, l, u, s, p, f, d, c, h, v, m, g = {
+    var e, r, t, n, o, i, a, l, u, f, s, p, d, c, h, v, m, g = {
             8383: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(818), t.e(684)]).then((() => () => t(684))),
-                        "./extension": () => Promise.all([t.e(818), t.e(684)]).then((() => () => t(684))),
+                        "./index": () => Promise.all([t.e(595), t.e(684)]).then((() => () => t(684))),
+                        "./extension": () => Promise.all([t.e(595), t.e(684)]).then((() => () => t(684))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     i = (e, r) => {
                         if (t.S) {
@@ -43,51 +43,51 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        432: "4a34574395b64c0ecb2a",
-        684: "c971d4662ee41caa2dda",
-        818: "9952ec63ac4e7e5b37d1"
+        432: "75a351a33d4e17e2f8f8",
+        595: "853e8b63deafdcf653a9",
+        684: "06766aa445a023bc4adf"
     } [e] + ".js?v=" + {
-        432: "4a34574395b64c0ecb2a",
-        684: "c971d4662ee41caa2dda",
-        818: "9952ec63ac4e7e5b37d1"
+        432: "75a351a33d4e17e2f8f8",
+        595: "853e8b63deafdcf653a9",
+        684: "06766aa445a023bc4adf"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-log-console:", y.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
             var a, l;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var p = u[s];
-                    if (p.getAttribute("src") == t || p.getAttribute("data-webpack") == r + o) {
-                        a = p;
+                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
+                    var s = u[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        a = s;
                         break
                     }
                 }
             a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, y.nc && a.setAttribute("nonce", y.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
-            var f = (r, n) => {
+            var p = (r, n) => {
                     a.onerror = a.onload = null, clearTimeout(d);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(f.bind(null, void 0, {
+                d = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), l && document.head.appendChild(a)
+            a.onerror = p.bind(null, a.onerror), a.onload = p.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -104,19 +104,19 @@
                 var i = y.S[t],
                     a = "@amphi/pipeline-log-console",
                     l = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = i[e] = i[e] || {},
                         l = o[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (o[r] = {
-                        get: () => Promise.all([y.e(818), y.e(684)]).then((() => () => y(684))),
+                        get: () => Promise.all([y.e(595), y.e(684)]).then((() => () => y(684))),
                         from: a,
                         eager: !1
                     })
-                })("@amphi/pipeline-log-console", "0.3.2"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-log-console", "0.3.3"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -166,33 +166,33 @@
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var a = 0, l = 1, u = !0;; l++, a++) {
-                var s, p, f = l < e.length ? (typeof e[l])[0] : "";
-                if (a >= r.length || "o" == (p = (typeof(s = r[a]))[0])) return !u || ("u" == f ? l > n && !o : "" == f != o);
-                if ("u" == p) {
-                    if (!u || "u" != f) return !1
+                var f, s, p = l < e.length ? (typeof e[l])[0] : "";
+                if (a >= r.length || "o" == (s = (typeof(f = r[a]))[0])) return !u || ("u" == p ? l > n && !o : "" == p != o);
+                if ("u" == s) {
+                    if (!u || "u" != p) return !1
                 } else if (u)
-                    if (f == p)
+                    if (p == s)
                         if (l <= n) {
-                            if (s != e[l]) return !1
+                            if (f != e[l]) return !1
                         } else {
-                            if (o ? s > e[l] : s < e[l]) return !1;
-                            s != e[l] && (u = !1)
+                            if (o ? f > e[l] : f < e[l]) return !1;
+                            f != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != p && "n" != p) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || p < f != o) return !1;
+                    if (l <= n || s < p != o) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != p && "n" != p && (u = !1, l--)
             }
         }
         var d = [],
             c = d.pop.bind(d);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
             d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
@@ -201,23 +201,23 @@
     }, a = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = l(e, t);
-        return i(n, o) || p(u(e, t, o, n)), f(e[t][o])
-    }, p = e => {
+        return i(n, o) || s(u(e, t, o, n)), p(e[t][o])
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var i = y.I(r);
         return i && i.then ? i.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), c = {}, h = {
+    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), c = {}, h = {
         1527: () => d("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
         3345: () => d("default", "react", [1, 18, 2, 0]),
         4236: () => d("default", "@jupyterlab/rendermime", [1, 4, 2, 0]),
         4602: () => d("default", "@lumino/signaling", [1, 2, 0, 0]),
         5256: () => d("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         5881: () => d("default", "@amphi/pipeline-editor", [0]),
         5923: () => d("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-log-console/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969512195121951%*

 * *Differences: {"'packages'": "{32: {'versionInfo': '5.41.0'}, 33: {'versionInfo': '3.14.0'}}"}*

```diff
@@ -192,21 +192,21 @@
             "name": "rc-tree",
             "versionInfo": "5.8.7"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014-present yiminghe\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-util",
-            "versionInfo": "5.40.1"
+            "versionInfo": "5.41.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.12.0"
+            "versionInfo": "3.14.0"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react-dom",
             "versionInfo": "18.3.1"
         },
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/package.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9bc842b6cc0c70b4b0c3.js'}}",*

 * * "'version'": "'0.3.3'"}*

```diff
@@ -51,15 +51,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.16d4e872755a30ebdc97.js",
+            "load": "static/remoteEntry.9bc842b6cc0c70b4b0c3.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-metadata-panel",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -95,9 +95,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.3.3"
 }
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/static/remoteEntry.16d4e872755a30ebdc97.js` & `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/remoteEntry.9bc842b6cc0c70b4b0c3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var a = i[e] = i[e] || {},
                         l = a[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : o > l.from)) && (a[r] = {
                         get: () => y.e(732).then((() => () => y(732))),
                         from: o,
                         eager: !1
                     })
-                })("@amphi/pipeline-metadata-panel", "0.3.2"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-metadata-panel", "0.3.3"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_amphi-0.3.3/amphi/pipeline-metadata-panel/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.3.4'"}*

```diff
@@ -94,9 +94,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.3.4"
 }
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/tsconfig.json` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/BrowseFileDialog.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/CodeGenerator.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/CodeGenerator.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     // Add all pipeline nodes to nodeMap, except annotations and loggers
     flow.nodes.forEach(node => {
       const type = componentService.getComponent(node.type)._type;
       if (type !== 'annotation') {
         if (type === 'logger') {
           loggersMap.set(node.id, node);
-        } else if (type === 'env_variables') {
+        } else if (type === 'env_variables' || type === 'env_file') {
           envVariablesMap.set(node.id, node);
         } else {
           nodesMap.set(node.id, node);
         }
       }
     });
 
@@ -371,14 +371,14 @@
       while ((matchResult = envVarRegex.exec(group)) !== null) {
         const [fullMatch, envVar] = matchResult;
         replacedGroup = replacedGroup.replace(fullMatch, `{os.environ['${envVar}']}`);
       }
       return replacedGroup.includes("{os.environ") ? `f"${replacedGroup}"` : `"${replacedGroup}"`;
     });
   }
-  
+
 
 
 };
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/CustomHandle.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/CustomHandle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/DndProviderWrapper.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/DndProviderWrapper.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/PipelineComponent.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/PipelineComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/PipelineService.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/PipelineService.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -213,19 +213,24 @@
   
     return lastUpdatedList;
   }
 
 
   static getEnvironmentVariables(pipelineJson: string): any[] {
     const flow = PipelineService.filterPipeline(pipelineJson);
-    const envVariablesNodes = flow.nodes.filter(node => node.type === 'envVariables');
+    const envVariablesNodes = flow.nodes.filter(node => node.type === 'envVariables' );
 
     const variablesList = envVariablesNodes.reduce((acc, node) => {
       return acc.concat(node.data.variables || []);
     }, []);
+
+
+    // const envFileNodes = flow.nodes.filter(node => node.type === 'envFile' );
+
+
   
     return variablesList;
   }
 
 }
 
 export interface Node {
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/RequestService.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/RequestService.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -100,36 +100,47 @@
     }
 
 
   };
 
   static retrieveTableColumns(
     event: React.MouseEvent<HTMLElement>,
+    imports: string[],
     connectionString: string,
+    schemaName: string,
     tableName: string,
     query: string,
     context: any,
     commands: any,
     componentService: any,
     setDataSource: any,
     setLoadings: any,
     nodeId: any,
     ): any {
     setLoadings(true);
+    const importString = imports.join(', ');
 
-    const code = `
-!pip install --quiet pymysql --disable-pip-version-check
+    let escapedQuery = query.replace(/"/g, '\\"');
+    escapedQuery = escapedQuery.replace(/{{schema}}/g, schemaName).replace(/{{table}}/g, tableName);
+    
+    let code = `
+!pip install --quiet ${importString} --disable-pip-version-check
 import pandas as pd
 from sqlalchemy import create_engine
-schema = pd.read_sql("${query}", con = create_engine("${connectionString}"))
+query = """
+${escapedQuery}
+"""
+schema = pd.read_sql(query, con = create_engine("${connectionString}"))
 column_info = schema[["Field", "Type"]]
 formatted_output = ", ".join([f"{row['Field']} ({row['Type']})" for _, row in column_info.iterrows()])
 print(formatted_output)
 `;
 
+code = CodeGenerator.convertToFString(code);
+
 console.log("code: " + code);
 
       const future = context.sessionContext.session.kernel!.requestExecute({ code: code });
 
       future.onReply = reply => {
         if (reply.content.status == "ok") {
           console.log("OK")
@@ -183,9 +194,8 @@
           const errorOutput = errorMsg.content;
           console.error(`Received error: ${errorOutput.ename}: ${errorOutput.evalue}`);
         }
       };
 
   };
 
-
 }
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/configUtils.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/configUtils.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -368,17 +368,17 @@
                 <Form.Item label={field.label} {...(field.required ? { required: field.required } : {})} {...(field.tooltip ? { tooltip: field.tooltip } : {})}>
                   <DataMapping data={data} field={field} handleChange={handleChange} defaultValue={values} context={context} componentService={componentService} commands={commands} nodeId={nodeId} inDialog={advanced} />
                 </Form.Item>
               );
               case "info":
                 const { Paragraph } = Typography;
                 return (
-                  <Paragraph>
-                  {field.text}
-                </Paragraph>
+                  <Paragraph style={{ padding: '5px' }}>
+                    {field.text}
+                  </Paragraph>
                 );
           default:
             return null;
         }
       })}
     </>
   );
@@ -503,14 +503,16 @@
   height?: number;
   rows?: number;
   outputType?: string;
   drivers?: string;
   typeOptions?: any;
   inputType?: 'password';
   text?: string;
+  imports?: string[];
+  query?: string;
 }
 
 interface ConfigModalProps {
   name: string;
   nodeId: string;
   form: object;
   data: object;
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/connectionUtils.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/connectionUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/generatorUtils.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/generatorUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/icons.ts` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/index.ts` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/rendererUtils.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/rendererUtils.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
 export const renderComponentUI: React.FC<UIComponentProps> = ({ id, data, context, manager, commands, name, ConfigForm, Icon, showContent, handle, deleteNode, setViewport }) => {
 
   const handleDoubleClick = () => {
     // Example: Zoom in 1.2 times the current zoom level
     setViewport({ zoom: 1.2, duration: 500 });
   };
+  
 
   return (
     <>
       <div className="component" onDoubleClick={handleDoubleClick}>
         <div className="component__header">
           {name}
           <Popconfirm title="Sure to delete?" placement="right" onConfirm={() => deleteNode()} icon={<QuestionCircleOutlined style={{ color: 'red' }} />}>
@@ -109,15 +110,14 @@
               <div className="placeholder">
                 <Icon.react top="8px" height="32px" width="32px;" color="#5A8F7B" verticalAlign="middle" />
               </div>
             )}
           </form>
         </div>
         {handle}
-
       </div>
     </>
   );
 };
 
 export interface UIComponentProps {
   id: string;
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/InputRegular.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/InputRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/connectionSelector.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/connectionSelector.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/dataMapping.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/dataMapping.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -267,17 +267,19 @@
             type="primary"
             size="small"
             style={{ marginBottom: 16 }}
             onClick={(event) => {
               setDataSource([]);
               RequestService.retrieveTableColumns(
                 event,
+                field.imports,
                 `${field.drivers}://${data.dbOptions.username}:${data.dbOptions.password}@${data.dbOptions.host}:${data.dbOptions.port}/${data.dbOptions.databaseName}`,
+                `${data.dbOptions.schema ?? 'public'}`,
                 `${data.dbOptions.tableName}`,
-                `DESCRIBE ${data.dbOptions.tableName}`,
+                `${field.query}`,
                 context,
                 commands,
                 componentService,
                 setDataSource,
                 setLoadingsOutput,
                 nodeId
               );
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/keyValueForm.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectColumn.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectColumn.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectColumns.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectMultiple.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectMultiple.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectRegular.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/selectTokenization.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectTokenization.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/transferData.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/transferData.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 export const TransferData: React.FC<TransferDataProps> = ({
   field, handleChange, defaultValue, context, componentService, commands, nodeId, inDialog
 }) => {
 
   type TransferItem = GetProp<TransferProps, 'dataSource'>[number];
   type TableRowSelection<T extends object> = TableProps<T>['rowSelection'];
-  
+
 
   interface RecordType {
     key: string;
     value: string;
     title: string;
     disabled: boolean;
     type: string;
@@ -143,62 +143,62 @@
             />
           );
         } else {
 
           const rowDrop = (dragIndex, hoverIndex) => {
             console.log("dragIndex:", dragIndex);
             console.log("hoverIndex:", hoverIndex);
-          
+
             // Ensure the indices are valid
             if (dragIndex === undefined || hoverIndex === undefined) {
               console.error("Invalid drag or hover index");
               return;
             }
-          
+
             // Create a copy of the target keys with all properties intact
             let newKeys = [...targetKeys];
-          
+
             console.log("Initial newKeys:", newKeys);
-          
+
             // Extract the dragged item and re-insert at the hover index
             const dragRow = newKeys.splice(dragIndex, 1)[0]; // Ensure correct extraction
             newKeys.splice(hoverIndex, 0, dragRow); // Insert at the correct position
-          
+
             console.log("Updated newKeys:", newKeys);
-          
+
             setTargetKeys(newKeys);
             const savedSchema = { sourceData: sourceData, targetKeys: newKeys }
             handleChange(savedSchema, field.id);
           };
 
           return (
             <DndProviderWrapper>
               <Table
-                  rowSelection={rowSelection}
-                  columns={columns}
-                  dataSource={filteredItems}
-                  components={{
-                    body: {
-                      row: DragableBodyRow,
-                    },
-                  }}
-                  size="small"
-                  style={{ pointerEvents: listDisabled ? 'none' : undefined }}
-                  onRow={(record, idx) => ({
-                    index: idx, // Pass the correct index to the row
-                    rowDrop,
-                    onClick: () => {
-                      if (record.disabled) {
-                        return;
-                      }
-                      onItemSelect(record.key, !listSelectedKeys.includes(record.key)); // Toggle selection
-                    },
-                  })}
-                />
-              </DndProviderWrapper>
+                rowSelection={rowSelection}
+                columns={columns}
+                dataSource={filteredItems}
+                components={{
+                  body: {
+                    row: DragableBodyRow,
+                  },
+                }}
+                size="small"
+                style={{ pointerEvents: listDisabled ? 'none' : undefined }}
+                onRow={(record, idx) => ({
+                  index: idx, // Pass the correct index to the row
+                  rowDrop,
+                  onClick: () => {
+                    if (record.disabled) {
+                      return;
+                    }
+                    onItemSelect(record.key, !listSelectedKeys.includes(record.key)); // Toggle selection
+                  },
+                })}
+              />
+            </DndProviderWrapper>
           );
         }
 
       }}
     </Transfer>
   );
 
@@ -207,17 +207,17 @@
   const [targetKeys, setTargetKeys] = useState<TransferProps['targetKeys']>([]);
   const [loadings, setLoadings] = useState<boolean>();
 
   useEffect(() => {
     console.log("Transfer Data, items %o", items)
 
     setSourceData(items.map(item => ({
-        ...item,
-        key: item.value,
-        title: item.value
+      ...item,
+      key: item.value,
+      title: item.value
     })));
   }, [items]);
 
 
   useEffect(() => {
     if (defaultValue && defaultValue.sourceData && defaultValue.targetKeys) {
       setSourceData(defaultValue.sourceData);
@@ -248,26 +248,33 @@
     const savedSchema = { sourceData: sourceData, targetKeys: nextTargetKeys }
     handleChange(savedSchema, field.id);
   };
 
   const renderFooter: TransferProps['footer'] = (_, info) => {
     if (info?.direction === 'left') {
       return (
-        <Button type="primary" size="small" style={{ float: 'left', margin: 5 }} onClick={(event) => RequestService.retrieveDataframeColumns(
-          event,
-          context,
-          commands,
-          componentService,
-          setItems,
-          setLoadings,
-          nodeId,
-          0,
-          true
-        )}
-        loading={loadings}>
+        <Button
+          type="primary"
+          size="small"
+          style={{ float: 'left', margin: 5 }}
+          onClick={(event) => {
+            setItems([]);
+            RequestService.retrieveDataframeColumns(
+              event,
+              context,
+              commands,
+              componentService,
+              setItems,
+              setLoadings,
+              nodeId,
+              0,
+              true
+            );
+          }}
+          loading={loadings}>
           Retrieve columns
         </Button>
       );
     }
     return;
   };
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/src/forms/valuesListForm.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/valuesListForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/settings-16.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/settings-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/settings-24.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/settings-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/trash-16.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/trash-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/trash-24.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/trash-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-components-manager/style/icons/x-square-16.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/x-square-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940476190476191%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.bfb171550404534afb06.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}"}*

```diff
@@ -45,14 +45,19 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.bfb171550404534afb06.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
                 "singleton": true
             },
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/pipeline-16.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/pipeline-24.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/tsconfig.json` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/schema/plugin copy.json` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/plugin copy.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/schema/plugin.json` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/Dropzone.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/PipelineEditorWidget.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/PipelineEditorWidget.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,14 @@
       </div>
     );
   }
 
   function Sidebar() {
 
     const [sidebarOpen, setSideBarOpen] = useState(false);
-
     const sidebarClass = sidebarOpen ? "" : "open";
 
     const onDragStart = (event, nodeType, config) => {
       event.dataTransfer.setData('application/reactflow', nodeType);
       // Here, you can add more data as needed
       event.dataTransfer.setData('additionalData', config);
       event.dataTransfer.effectAllowed = 'move';
```

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/customEdge.tsx` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/customEdge.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/icons.ts` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/src/index.ts` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/canvas.css` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/canvas.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/output.css` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/output.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/pipeline-category-icon.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/pipeline-category-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/react-icon.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/react-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/api-24.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/api-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/file-plus-24.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/file-plus-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/file-text-24.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/file-text-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/pipeline-brand-16.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/pipeline-brand-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/packages/pipeline-editor/style/icons/pipeline-brand-24.svg` & `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/pipeline-brand-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/LICENSE` & `jupyterlab_amphi-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/README.md` & `jupyterlab_amphi-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/pyproject.toml` & `jupyterlab_amphi-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.3/PKG-INFO` & `jupyterlab_amphi-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-amphi
-Version: 0.3.3
+Version: 0.3.4
 Dynamic: Keywords
 Summary: Amphi is a micro ETL for Jupyterlab.
 Project-URL: Homepage, https://amphi.ai
 Project-URL: Bug Tracker, https://github.com/amphi-ai/jupyterlab-amphi/issues
 Project-URL: Repository, https://github.com/amphi-ai/jupyterlab-amphi.git
 Author-email: Thibaut Gourdel <tgourdel@amphi.ai>
 License: Elastic License 2.0 \(ELv2\)
```

