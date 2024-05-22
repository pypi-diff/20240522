# Comparing `tmp/pvi-0.8.1.tar.gz` & `tmp/pvi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvi-0.8.1.tar", last modified: Thu Mar 28 17:17:47 2024, max compression
+gzip compressed data, was "pvi-0.9.0.tar", last modified: Wed May 22 13:39:58 2024, max compression
```

## Comparing `pvi-0.8.1.tar` & `pvi-0.9.0.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.403223 pvi-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.375223 pvi-0.8.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-28 17:17:42.000000 pvi-0.8.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.379223 pvi-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-28 17:17:42.000000 pvi-0.8.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.371223 pvi-0.8.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.379223 pvi-0.8.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-28 17:17:42.000000 pvi-0.8.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-28 17:17:42.000000 pvi-0.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.379223 pvi-0.8.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-28 17:17:42.000000 pvi-0.8.1/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     3043 2024-03-28 17:17:42.000000 pvi-0.8.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.379223 pvi-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-03-28 17:17:42.000000 pvi-0.8.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-28 17:17:42.000000 pvi-0.8.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-28 17:17:42.000000 pvi-0.8.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-28 17:17:42.000000 pvi-0.8.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-28 17:17:42.000000 pvi-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-28 17:17:42.000000 pvi-0.8.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-28 17:17:42.000000 pvi-0.8.1/.gitremotes
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-28 17:17:42.000000 pvi-0.8.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.379223 pvi-0.8.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-28 17:17:42.000000 pvi-0.8.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)    15559 2024-03-28 17:17:42.000000 pvi-0.8.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-28 17:17:42.000000 pvi-0.8.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-28 17:17:42.000000 pvi-0.8.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-28 17:17:42.000000 pvi-0.8.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-28 17:17:42.000000 pvi-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-03-28 17:17:47.403223 pvi-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-28 17:17:42.000000 pvi-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.379223 pvi-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.379223 pvi-0.8.1/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.379223 pvi-0.8.1/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.379223 pvi-0.8.1/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/explanations/original-design.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.383223 pvi-0.8.1/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/how-to/write-a-formatter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.383223 pvi-0.8.1/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.383223 pvi-0.8.1/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.383223 pvi-0.8.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    99678 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    55895 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/images/pilatus_edl.png
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/images/pvi-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    17571 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/images/pvi-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.391223 pvi-0.8.1/docs/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/snippets/pilatusDetector.pvi.producer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    32481 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/snippets/pilatusDetectorParamSet.h
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/snippets/pilatusDetectorParameters.template
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/snippets/pilatusParameters.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/snippets/static_table.pvi.producer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.391223 pvi-0.8.1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.391223 pvi-0.8.1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.391223 pvi-0.8.1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.391223 pvi-0.8.1/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.391223 pvi-0.8.1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-28 17:17:42.000000 pvi-0.8.1/docs/user/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.391223 pvi-0.8.1/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-28 17:17:42.000000 pvi-0.8.1/formatters/aps.pvi.formatter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-28 17:17:42.000000 pvi-0.8.1/formatters/dls.bob.pvi.formatter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-28 17:17:42.000000 pvi-0.8.1/formatters/dls.edl.pvi.formatter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-28 17:17:42.000000 pvi-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.391223 pvi-0.8.1/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    23963 2024-03-28 17:17:42.000000 pvi-0.8.1/schemas/pvi.device.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-03-28 17:17:42.000000 pvi-0.8.1/schemas/pvi.formatter.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:17:47.403223 pvi-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.375223 pvi-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.391223 pvi-0.8.1/src/pvi/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.395223 pvi-0.8.1/src/pvi/_convert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_convert/_asyn_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_convert/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_convert/_template_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_convert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.395223 pvi-0.8.1/src/pvi/_format/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/adl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/aps.adl
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/aps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/bob.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/dls.bob
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/dls.edl
--rw-r--r--   0 runner    (1001) docker     (127)    14971 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/dls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/edl.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/pvi.template.jinja
--rw-r--r--   0 runner    (1001) docker     (127)    21332 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_format/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_pv_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 17:17:47.000000 pvi-0.8.1/src/pvi/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/typed_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-28 17:17:42.000000 pvi-0.8.1/src/pvi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.403223 pvi-0.8.1/src/pvi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-03-28 17:17:47.000000 pvi-0.8.1/src/pvi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-03-28 17:17:47.000000 pvi-0.8.1/src/pvi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:17:47.000000 pvi-0.8.1/src/pvi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 17:17:47.000000 pvi-0.8.1/src/pvi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-28 17:17:47.000000 pvi-0.8.1/src/pvi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-28 17:17:47.000000 pvi-0.8.1/src/pvi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.395223 pvi-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/bad.pvi.device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.375223 pvi-0.8.1/tests/convert/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.399223 pvi-0.8.1/tests/convert/input/
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/convert/input/simDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/convert/input/simDetector.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.399223 pvi-0.8.1/tests/convert/output/
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/convert/output/simDetector.pvi.device.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.375223 pvi-0.8.1/tests/format/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.399223 pvi-0.8.1/tests/format/input/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/input/aps.adl.pvi.formatter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/input/asynNDArrayDriver.pvi.device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/input/dls.bob.pvi.formatter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/input/dls.edl.pvi.formatter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/input/mixedWidgets.pvi.device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/input/signal_default_widgets.pvi.device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/input/static_table.pvi.device.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:17:47.403223 pvi-0.8.1/tests/format/output/
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/button.bob
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/combo_box.bob
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/device_ref.bob
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/index.bob
--rw-r--r--   0 runner    (1001) docker     (127)    18120 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/mixedWidgets.adl
--rw-r--r--   0 runner    (1001) docker     (127)    28876 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/mixedWidgets.bob
--rw-r--r--   0 runner    (1001) docker     (127)    29504 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/mixedWidgets.edl
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/pva_table.bob
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/pva_table_panda.bob
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/pvi.template
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/signal_default_widgets.bob
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/static_table.adl
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/static_table.bob
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/static_table.edl
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/static_table_BigTable.adl
--rw-r--r--   0 runner    (1001) docker     (127)     9253 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/static_table_BigTable.bob
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/static_table_BigTable.edl
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/static_table_BigTableA.adl
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/static_table_BigTableA.bob
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/static_table_BigTableA.edl
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/sub_screen.bob
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/sub_screen_Group1.bob
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/sub_screen_Group4.bob
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/text_format.adl
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/text_format.bob
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/format/output/text_format.edl
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/regenerate_test_output.sh
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/test.pvi.device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-28 17:17:42.000000 pvi-0.8.1/tests/test_device_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.659524 pvi-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.635524 pvi-0.9.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-22 13:39:55.000000 pvi-0.9.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.635524 pvi-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-22 13:39:55.000000 pvi-0.9.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.627524 pvi-0.9.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.635524 pvi-0.9.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-22 13:39:55.000000 pvi-0.9.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-22 13:39:55.000000 pvi-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.635524 pvi-0.9.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-22 13:39:55.000000 pvi-0.9.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3043 2024-05-22 13:39:55.000000 pvi-0.9.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.635524 pvi-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-22 13:39:55.000000 pvi-0.9.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-22 13:39:55.000000 pvi-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-22 13:39:55.000000 pvi-0.9.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 13:39:55.000000 pvi-0.9.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-22 13:39:55.000000 pvi-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-22 13:39:55.000000 pvi-0.9.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 13:39:55.000000 pvi-0.9.0/.gitremotes
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-22 13:39:55.000000 pvi-0.9.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.635524 pvi-0.9.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-22 13:39:55.000000 pvi-0.9.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15559 2024-05-22 13:39:55.000000 pvi-0.9.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-22 13:39:55.000000 pvi-0.9.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 13:39:55.000000 pvi-0.9.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-22 13:39:55.000000 pvi-0.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 13:39:55.000000 pvi-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16336 2024-05-22 13:39:58.659524 pvi-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-22 13:39:55.000000 pvi-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.635524 pvi-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.635524 pvi-0.9.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.635524 pvi-0.9.0/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.639524 pvi-0.9.0/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/explanations/original-design.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.639524 pvi-0.9.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/how-to/write-a-formatter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.639524 pvi-0.9.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.639524 pvi-0.9.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.639524 pvi-0.9.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    99678 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    55895 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/images/pilatus_edl.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/images/pvi-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    17571 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/images/pvi-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.643524 pvi-0.9.0/docs/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/snippets/pilatusDetector.pvi.producer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    32481 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/snippets/pilatusDetectorParamSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/snippets/pilatusDetectorParameters.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/snippets/pilatusParameters.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/snippets/static_table.pvi.producer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.643524 pvi-0.9.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.643524 pvi-0.9.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.643524 pvi-0.9.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.643524 pvi-0.9.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.643524 pvi-0.9.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-22 13:39:55.000000 pvi-0.9.0/docs/user/tutorials/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.643524 pvi-0.9.0/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-22 13:39:55.000000 pvi-0.9.0/formatters/aps.pvi.formatter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-22 13:39:55.000000 pvi-0.9.0/formatters/dls.bob.pvi.formatter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 13:39:55.000000 pvi-0.9.0/formatters/dls.edl.pvi.formatter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-22 13:39:55.000000 pvi-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.643524 pvi-0.9.0/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    28645 2024-05-22 13:39:55.000000 pvi-0.9.0/schemas/pvi.device.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-22 13:39:55.000000 pvi-0.9.0/schemas/pvi.formatter.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:39:58.659524 pvi-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.631523 pvi-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.643524 pvi-0.9.0/src/pvi/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.647523 pvi-0.9.0/src/pvi/_convert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_convert/_asyn_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_convert/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_convert/_template_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_convert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.647523 pvi-0.9.0/src/pvi/_format/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/adl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/aps.adl
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/aps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/bob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/dls.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/dls.edl
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/dls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/edl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/pvi.template.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)    22089 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_format/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_pv_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 13:39:58.000000 pvi-0.9.0/src/pvi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/typed_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-22 13:39:55.000000 pvi-0.9.0/src/pvi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.655524 pvi-0.9.0/src/pvi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16336 2024-05-22 13:39:58.000000 pvi-0.9.0/src/pvi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-22 13:39:58.000000 pvi-0.9.0/src/pvi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:39:58.000000 pvi-0.9.0/src/pvi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 13:39:58.000000 pvi-0.9.0/src/pvi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-22 13:39:58.000000 pvi-0.9.0/src/pvi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 13:39:58.000000 pvi-0.9.0/src/pvi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.651524 pvi-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/bad.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.631523 pvi-0.9.0/tests/convert/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.651524 pvi-0.9.0/tests/convert/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/convert/input/simDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/convert/input/simDetector.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.651524 pvi-0.9.0/tests/convert/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/convert/output/simDetector.pvi.device.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.631523 pvi-0.9.0/tests/format/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.651524 pvi-0.9.0/tests/format/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/input/aps.adl.pvi.formatter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/input/asynNDArrayDriver.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/input/dls.bob.pvi.formatter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/input/dls.edl.pvi.formatter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/input/mixedWidgets.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/input/signal_default_widgets.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/input/static_table.pvi.device.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:39:58.655524 pvi-0.9.0/tests/format/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/button.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/combo_box.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/device_ref.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/index.bob
+-rw-r--r--   0 runner    (1001) docker     (127)    18120 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/mixedWidgets.adl
+-rw-r--r--   0 runner    (1001) docker     (127)    30579 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/mixedWidgets.bob
+-rw-r--r--   0 runner    (1001) docker     (127)    29504 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/mixedWidgets.edl
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/pva_table.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/pva_table_panda.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/pvi.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/signal_default_widgets.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/static_table.adl
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/static_table.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/static_table.edl
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/static_table_BigTable.adl
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/static_table_BigTable.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/static_table_BigTable.edl
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/static_table_BigTableA.adl
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/static_table_BigTableA.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/static_table_BigTableA.edl
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/sub_screen.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/sub_screen_Group1.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/sub_screen_Group4.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/text_format.adl
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/text_format.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/format/output/text_format.edl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/regenerate_test_output.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/test.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-22 13:39:55.000000 pvi-0.9.0/tests/test_device_serialization.py
```

### Comparing `pvi-0.8.1/.devcontainer/devcontainer.json` & `pvi-0.9.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.github/CONTRIBUTING.rst` & `pvi-0.9.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.github/actions/install_requirements/action.yml` & `pvi-0.9.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.github/dependabot.yml` & `pvi-0.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.github/pages/make_switcher.py` & `pvi-0.9.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.github/workflows/code.yml` & `pvi-0.9.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.github/workflows/docs.yml` & `pvi-0.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.github/workflows/docs_clean.yml` & `pvi-0.9.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.github/workflows/linkcheck.yml` & `pvi-0.9.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.gitignore` & `pvi-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.gitmodules` & `pvi-0.9.0/.gitmodules`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.vscode/launch.json` & `pvi-0.9.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/.vscode/settings.json` & `pvi-0.9.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/Dockerfile` & `pvi-0.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/LICENSE` & `pvi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/PKG-INFO` & `pvi-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvi
-Version: 0.8.1
+Version: 0.9.0
 Summary: One line description of your module
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>, Gary Yendell <gary.yendell@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: pydantic
+Requires-Dist: pydantic>=2.7
 Requires-Dist: lxml
 Requires-Dist: ruamel.yaml
 Requires-Dist: typer
 Requires-Dist: jinja2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `pvi-0.8.1/README.rst` & `pvi-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/conf.py` & `pvi-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `pvi-0.9.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/explanations/decisions.rst` & `pvi-0.9.0/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/explanations/original-design.rst` & `pvi-0.9.0/docs/developer/explanations/original-design.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/how-to/build-docs.rst` & `pvi-0.9.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/how-to/lint.rst` & `pvi-0.9.0/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/how-to/make-release.rst` & `pvi-0.9.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/how-to/pin-requirements.rst` & `pvi-0.9.0/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/how-to/test-container.rst` & `pvi-0.9.0/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/how-to/update-tools.rst` & `pvi-0.9.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/how-to/write-a-formatter.rst` & `pvi-0.9.0/docs/developer/how-to/write-a-formatter.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/index.rst` & `pvi-0.9.0/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/reference/standards.rst` & `pvi-0.9.0/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/developer/tutorials/dev-install.rst` & `pvi-0.9.0/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/images/dls-favicon.ico` & `pvi-0.9.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/images/dls-logo.svg` & `pvi-0.9.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/images/pilatus_edl.png` & `pvi-0.9.0/docs/images/pilatus_edl.png`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/images/pvi-favicon.ico` & `pvi-0.9.0/docs/images/pvi-favicon.ico`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/images/pvi-logo.svg` & `pvi-0.9.0/docs/images/pvi-logo.svg`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/index.rst` & `pvi-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/snippets/pilatusDetector.pvi.producer.yaml` & `pvi-0.9.0/docs/snippets/pilatusDetector.pvi.producer.yaml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/snippets/pilatusDetectorParamSet.h` & `pvi-0.9.0/docs/snippets/pilatusDetectorParamSet.h`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/snippets/pilatusDetectorParameters.template` & `pvi-0.9.0/docs/snippets/pilatusDetectorParameters.template`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/snippets/pilatusParameters.csv` & `pvi-0.9.0/docs/snippets/pilatusParameters.csv`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/snippets/static_table.pvi.producer.yaml` & `pvi-0.9.0/docs/snippets/static_table.pvi.producer.yaml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/user/explanations/docs-structure.rst` & `pvi-0.9.0/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/user/index.rst` & `pvi-0.9.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/docs/user/tutorials/installation.rst` & `pvi-0.9.0/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/pyproject.toml` & `pvi-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "One line description of your module"
 dependencies = [
-    "pydantic",
+    "pydantic>=2.7",
     "lxml",
     "ruamel.yaml",
     "typer",
     "jinja2",
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
```

### Comparing `pvi-0.8.1/schemas/pvi.device.schema.json` & `pvi-0.9.0/schemas/pvi.device.schema.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955977625425171%*

 * *Differences: {"'$defs'": "{'ArrayTrace': {'properties': {'type': {'enum': ['ArrayTrace'], 'type': 'string'}}}, "*

 * *            "'ArrayWrite': {'properties': {'type': {'enum': ['ArrayWrite'], 'type': 'string'}}}, "*

 * *            "'BitField': {'properties': {'type': {'enum': ['BitField'], 'type': 'string'}}}, "*

 * *            "'ButtonPanel': {'properties': {'type': {'enum': ['ButtonPanel'], 'type': 'string'}}}, "*

 * *            "'CheckBox': {'properties': {'type': {'enum': ['CheckBox'], 'type': 'string'}}}, "*

 * *            "'ComboBox […]*

```diff
@@ -8,15 +8,19 @@
                     "description": "Traces with same axis name will appear on same axis, plotted against 'x' trace if it exists, or indexes if not. Only one traces with axis='x' allowed.",
                     "title": "Axis",
                     "type": "string"
                 },
                 "type": {
                     "const": "ArrayTrace",
                     "default": "ArrayTrace",
-                    "title": "Type"
+                    "enum": [
+                        "ArrayTrace"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "required": [
                 "axis"
             ],
             "title": "ArrayTrace",
             "type": "object"
@@ -24,15 +28,19 @@
         "ArrayWrite": {
             "additionalProperties": false,
             "description": "Control of an array PV",
             "properties": {
                 "type": {
                     "const": "ArrayWrite",
                     "default": "ArrayWrite",
-                    "title": "Type"
+                    "enum": [
+                        "ArrayWrite"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 },
                 "widget": {
                     "description": "What widget should be used for each item",
                     "oneOf": [
                         {
                             "$ref": "#/$defs/ButtonPanel"
                         },
@@ -81,15 +89,19 @@
                     "exclusiveMinimum": 0,
                     "title": "Number Of Bits",
                     "type": "integer"
                 },
                 "type": {
                     "const": "BitField",
                     "default": "BitField",
-                    "title": "Type"
+                    "enum": [
+                        "BitField"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "BitField",
             "type": "object"
         },
         "ButtonPanel": {
             "additionalProperties": false,
@@ -107,28 +119,36 @@
                     },
                     "title": "Actions",
                     "type": "object"
                 },
                 "type": {
                     "const": "ButtonPanel",
                     "default": "ButtonPanel",
-                    "title": "Type"
+                    "enum": [
+                        "ButtonPanel"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "ButtonPanel",
             "type": "object"
         },
         "CheckBox": {
             "additionalProperties": false,
             "description": "Checkable control of a boolean PV.\n\nThis is compact replacement for a `ToggleButton` to be used in rows and tables.",
             "properties": {
                 "type": {
                     "const": "CheckBox",
                     "default": "CheckBox",
-                    "title": "Type"
+                    "enum": [
+                        "CheckBox"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "CheckBox",
             "type": "object"
         },
         "ComboBox": {
             "additionalProperties": false,
@@ -142,34 +162,52 @@
                     },
                     "title": "Choices",
                     "type": "array"
                 },
                 "type": {
                     "const": "ComboBox",
                     "default": "ComboBox",
-                    "title": "Type"
+                    "enum": [
+                        "ComboBox"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "ComboBox",
             "type": "object"
         },
         "DeviceRef": {
             "additionalProperties": false,
             "description": "Reference to another Device.",
             "properties": {
+                "description": {
+                    "anyOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
+                    "description": "Description for label tooltip",
+                    "title": "Description"
+                },
                 "label": {
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": null,
+                    "description": "Label for component",
                     "title": "Label"
                 },
                 "macros": {
                     "additionalProperties": {
                         "type": "string"
                     },
                     "default": {},
@@ -187,15 +225,19 @@
                     "description": "Child device PVI PV",
                     "title": "Pv",
                     "type": "string"
                 },
                 "type": {
                     "const": "DeviceRef",
                     "default": "DeviceRef",
-                    "title": "Type"
+                    "enum": [
+                        "DeviceRef"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 },
                 "ui": {
                     "description": "UI file to open for referenced Device",
                     "title": "Ui",
                     "type": "string"
                 }
             },
@@ -216,15 +258,19 @@
                     "description": "If True use names of children as labels",
                     "title": "Labelled",
                     "type": "boolean"
                 },
                 "type": {
                     "const": "Grid",
                     "default": "Grid",
-                    "title": "Type"
+                    "enum": [
+                        "Grid"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "Grid",
             "type": "object"
         },
         "Group": {
             "additionalProperties": false,
@@ -256,24 +302,38 @@
                                 "$ref": "#/$defs/DeviceRef"
                             }
                         ]
                     },
                     "title": "Children",
                     "type": "array"
                 },
+                "description": {
+                    "anyOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
+                    "description": "Description for label tooltip",
+                    "title": "Description"
+                },
                 "label": {
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": null,
+                    "description": "Label for component",
                     "title": "Label"
                 },
                 "layout": {
                     "description": "How to layout children on screen",
                     "oneOf": [
                         {
                             "$ref": "#/$defs/Plot"
@@ -295,15 +355,19 @@
                     "pattern": "^([A-Z][a-z0-9]*)*$",
                     "title": "Name",
                     "type": "string"
                 },
                 "type": {
                     "const": "Group",
                     "default": "Group",
-                    "title": "Type"
+                    "enum": [
+                        "Group"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "required": [
                 "name",
                 "layout",
                 "children"
             ],
@@ -313,54 +377,70 @@
         "ImageRead": {
             "additionalProperties": false,
             "description": "2D Image view of an NTNDArray",
             "properties": {
                 "type": {
                     "const": "ImageRead",
                     "default": "ImageRead",
-                    "title": "Type"
+                    "enum": [
+                        "ImageRead"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "ImageRead",
             "type": "object"
         },
         "LED": {
             "additionalProperties": false,
             "description": "LED display of a boolean PV",
             "properties": {
                 "type": {
                     "const": "LED",
                     "default": "LED",
-                    "title": "Type"
+                    "enum": [
+                        "LED"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "LED",
             "type": "object"
         },
         "Plot": {
             "additionalProperties": false,
             "description": "Children are traces of the plot",
             "properties": {
                 "type": {
                     "const": "Plot",
                     "default": "Plot",
-                    "title": "Type"
+                    "enum": [
+                        "Plot"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "Plot",
             "type": "object"
         },
         "ProgressBar": {
             "additionalProperties": false,
             "description": "Progress bar from lower to upper limit of a float PV",
             "properties": {
                 "type": {
                     "const": "ProgressBar",
                     "default": "ProgressBar",
-                    "title": "Type"
+                    "enum": [
+                        "ProgressBar"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "ProgressBar",
             "type": "object"
         },
         "Row": {
             "additionalProperties": false,
@@ -381,34 +461,52 @@
                     "default": null,
                     "description": "Labels for the items in the row",
                     "title": "Header"
                 },
                 "type": {
                     "const": "Row",
                     "default": "Row",
-                    "title": "Type"
+                    "enum": [
+                        "Row"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "Row",
             "type": "object"
         },
         "SignalR": {
             "additionalProperties": false,
             "description": "Read-only `Signal` backed by a single PV.",
             "properties": {
+                "description": {
+                    "anyOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
+                    "description": "Description for label tooltip",
+                    "title": "Description"
+                },
                 "label": {
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": null,
+                    "description": "Label for component",
                     "title": "Label"
                 },
                 "name": {
                     "description": "PascalCase name to uniquely identify",
                     "pattern": "^([A-Z][a-z0-9]*)*$",
                     "title": "Name",
                     "type": "string"
@@ -445,38 +543,56 @@
                         }
                     ],
                     "title": "Read Widget"
                 },
                 "type": {
                     "const": "SignalR",
                     "default": "SignalR",
-                    "title": "Type"
+                    "enum": [
+                        "SignalR"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "required": [
                 "name",
                 "read_pv"
             ],
             "title": "SignalR",
             "type": "object"
         },
         "SignalRW": {
             "additionalProperties": false,
             "description": "Read/write `Signal` backed by a demand PV and a readback PV.\n\nOne PV can be used as both a demand and a readback by leaving `read_pv` unset. In\nthis case no readback widget will be displayed unless `read_widget` is set.\n\nIf `read_pv` is set and `read_widget` is not, a `TextRead` widget will be used.",
             "properties": {
+                "description": {
+                    "anyOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
+                    "description": "Description for label tooltip",
+                    "title": "Description"
+                },
                 "label": {
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": null,
+                    "description": "Label for component",
                     "title": "Label"
                 },
                 "name": {
                     "description": "PascalCase name to uniquely identify",
                     "pattern": "^([A-Z][a-z0-9]*)*$",
                     "title": "Name",
                     "type": "string"
@@ -514,15 +630,19 @@
                         }
                     ],
                     "title": "Read Widget"
                 },
                 "type": {
                     "const": "SignalRW",
                     "default": "SignalRW",
-                    "title": "Type"
+                    "enum": [
+                        "SignalRW"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 },
                 "write_pv": {
                     "description": "PV to use for demand",
                     "title": "Write Pv",
                     "type": "string"
                 },
                 "write_widget": {
@@ -560,70 +680,106 @@
             "title": "SignalRW",
             "type": "object"
         },
         "SignalRef": {
             "additionalProperties": false,
             "description": "Reference to another Signal with the same name in this Device.",
             "properties": {
+                "description": {
+                    "anyOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
+                    "description": "Description for label tooltip",
+                    "title": "Description"
+                },
                 "label": {
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": null,
+                    "description": "Label for component",
                     "title": "Label"
                 },
                 "name": {
                     "description": "PascalCase name to uniquely identify",
                     "pattern": "^([A-Z][a-z0-9]*)*$",
                     "title": "Name",
                     "type": "string"
                 },
                 "type": {
                     "const": "SignalRef",
                     "default": "SignalRef",
-                    "title": "Type"
+                    "enum": [
+                        "SignalRef"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "required": [
                 "name"
             ],
             "title": "SignalRef",
             "type": "object"
         },
         "SignalW": {
             "additionalProperties": false,
             "description": "Write-only `Signal` backed by a single PV.",
             "properties": {
+                "description": {
+                    "anyOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
+                    "description": "Description for label tooltip",
+                    "title": "Description"
+                },
                 "label": {
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": null,
+                    "description": "Label for component",
                     "title": "Label"
                 },
                 "name": {
                     "description": "PascalCase name to uniquely identify",
                     "pattern": "^([A-Z][a-z0-9]*)*$",
                     "title": "Name",
                     "type": "string"
                 },
                 "type": {
                     "const": "SignalW",
                     "default": "SignalW",
-                    "title": "Type"
+                    "enum": [
+                        "SignalW"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 },
                 "write_pv": {
                     "description": "PV to use for demand",
                     "title": "Write Pv",
                     "type": "string"
                 },
                 "write_widget": {
@@ -661,36 +817,54 @@
             "title": "SignalW",
             "type": "object"
         },
         "SignalX": {
             "additionalProperties": false,
             "description": "`SignalW` that can be triggered to write a fixed value to a PV.",
             "properties": {
+                "description": {
+                    "anyOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
+                    "description": "Description for label tooltip",
+                    "title": "Description"
+                },
                 "label": {
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": null,
+                    "description": "Label for component",
                     "title": "Label"
                 },
                 "name": {
                     "description": "PascalCase name to uniquely identify",
                     "pattern": "^([A-Z][a-z0-9]*)*$",
                     "title": "Name",
                     "type": "string"
                 },
                 "type": {
                     "const": "SignalX",
                     "default": "SignalX",
-                    "title": "Type"
+                    "enum": [
+                        "SignalX"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 },
                 "value": {
                     "default": null,
                     "description": "Value to write. None means zero",
                     "title": "Value",
                     "type": "string"
                 },
@@ -724,28 +898,36 @@
                     "description": "Display labels for components",
                     "title": "Labelled",
                     "type": "boolean"
                 },
                 "type": {
                     "const": "SubScreen",
                     "default": "SubScreen",
-                    "title": "Type"
+                    "enum": [
+                        "SubScreen"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "SubScreen",
             "type": "object"
         },
         "TableRead": {
             "additionalProperties": false,
             "description": "A read-only tabular view of an NTTable.",
             "properties": {
                 "type": {
                     "const": "TableRead",
                     "default": "TableRead",
-                    "title": "Type"
+                    "enum": [
+                        "TableRead"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 },
                 "widgets": {
                     "default": [],
                     "description": "For each column, what widget should be repeated for every row",
                     "items": {
                         "oneOf": [
                             {
@@ -772,15 +954,19 @@
         "TableWrite": {
             "additionalProperties": false,
             "description": "A writeable tabular view of an NTTable.",
             "properties": {
                 "type": {
                     "const": "TableWrite",
                     "default": "TableWrite",
-                    "title": "Type"
+                    "enum": [
+                        "TableWrite"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 },
                 "widgets": {
                     "default": [],
                     "description": "For each column, what widget should be repeated for every row",
                     "items": {
                         "oneOf": [
                             {
@@ -803,22 +989,22 @@
             },
             "title": "TableWrite",
             "type": "object"
         },
         "TextFormat": {
             "description": "Format to use for display of Text{Read,Write} widgets on a UI",
             "enum": [
-                0,
-                1,
-                2,
-                3,
-                4
+                "decimal",
+                "hexadecimal",
+                "engineer",
+                "exponential",
+                "string"
             ],
             "title": "TextFormat",
-            "type": "integer"
+            "type": "string"
         },
         "TextRead": {
             "additionalProperties": false,
             "description": "Text view of any PV",
             "properties": {
                 "format": {
                     "anyOf": [
@@ -844,15 +1030,19 @@
                     "default": null,
                     "description": "Number of lines to display",
                     "title": "Lines"
                 },
                 "type": {
                     "const": "TextRead",
                     "default": "TextRead",
-                    "title": "Type"
+                    "enum": [
+                        "TextRead"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "TextRead",
             "type": "object"
         },
         "TextWrite": {
             "additionalProperties": false,
@@ -882,28 +1072,36 @@
                     "default": null,
                     "description": "Number of lines to display",
                     "title": "Lines"
                 },
                 "type": {
                     "const": "TextWrite",
                     "default": "TextWrite",
-                    "title": "Type"
+                    "enum": [
+                        "TextWrite"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "TextWrite",
             "type": "object"
         },
         "ToggleButton": {
             "additionalProperties": false,
             "description": "A pair of buttons to select between two mutually exclusive states.",
             "properties": {
                 "type": {
                     "const": "ToggleButton",
                     "default": "ToggleButton",
-                    "title": "Type"
+                    "enum": [
+                        "ToggleButton"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 }
             },
             "title": "ToggleButton",
             "type": "object"
         }
     },
     "additionalProperties": false,
@@ -956,15 +1154,19 @@
             ],
             "default": null,
             "title": "Parent"
         },
         "type": {
             "const": "Device",
             "default": "Device",
-            "title": "Type"
+            "enum": [
+                "Device"
+            ],
+            "title": "Type",
+            "type": "string"
         }
     },
     "required": [
         "label"
     ],
     "title": "Device",
     "type": "object"
```

### Comparing `pvi-0.8.1/schemas/pvi.formatter.schema.json` & `pvi-0.9.0/schemas/pvi.formatter.schema.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995535714285715%*

 * *Differences: {"'$defs'": "{'APSFormatter': {'properties': {'type': {'enum': ['APSFormatter'], 'type': "*

 * *            "'string'}}}, 'DLSFormatter': {'properties': {'type': {'enum': ['DLSFormatter'], "*

 * *            "'type': 'string'}}}}"}*

```diff
@@ -26,15 +26,19 @@
                     "description": "Height of screen title bar",
                     "title": "Title Height",
                     "type": "integer"
                 },
                 "type": {
                     "const": "APSFormatter",
                     "default": "APSFormatter",
-                    "title": "Type"
+                    "enum": [
+                        "APSFormatter"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 },
                 "widget_height": {
                     "default": 20,
                     "description": "Height of the widgets",
                     "title": "Widget Height",
                     "type": "integer"
                 },
@@ -74,15 +78,19 @@
                     "description": "Height of screen title bar",
                     "title": "Title Height",
                     "type": "integer"
                 },
                 "type": {
                     "const": "DLSFormatter",
                     "default": "DLSFormatter",
-                    "title": "Type"
+                    "enum": [
+                        "DLSFormatter"
+                    ],
+                    "title": "Type",
+                    "type": "string"
                 },
                 "widget_height": {
                     "default": 20,
                     "description": "Height of the widgets",
                     "title": "Widget Height",
                     "type": "integer"
                 },
```

### Comparing `pvi-0.8.1/src/pvi/__main__.py` & `pvi-0.9.0/src/pvi/__main__.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_convert/_asyn_convert.py` & `pvi-0.9.0/src/pvi/_convert/_asyn_convert.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_convert/_parameters.py` & `pvi-0.9.0/src/pvi/_convert/_parameters.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_convert/_template_convert.py` & `pvi-0.9.0/src/pvi/_convert/_template_convert.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_convert/utils.py` & `pvi-0.9.0/src/pvi/_convert/utils.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/adl.py` & `pvi-0.9.0/src/pvi/_format/adl.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/aps.adl` & `pvi-0.9.0/src/pvi/_format/aps.adl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/aps.py` & `pvi-0.9.0/src/pvi/_format/aps.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/base.py` & `pvi-0.9.0/src/pvi/_format/base.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/bob.py` & `pvi-0.9.0/src/pvi/_format/bob.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/dls.bob` & `pvi-0.9.0/src/pvi/_format/dls.bob`

 * *Files 2% similar despite different names*

#### Comparing `pvi-0.8.1/src/pvi/_format/dls.bob` & `pvi-0.9.0/src/pvi/_format/dls.bob`

```diff
@@ -35,14 +35,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Label</text>
     <x>18</x>
     <y>58</y>
     <width>120</width>
     <height>30</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>TextWrite</pv_name>
     <x>18</x>
     <y>78</y>
     <width>120</width>
@@ -60,15 +61,15 @@
       </action>
     </actions>
     <text>SignalX</text>
     <x>18</x>
     <y>118</y>
     <width>120</width>
     <height>40</height>
-    <tooltip>$(actions)</tooltip>
+    <tooltip>$(tooltip)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>TextRead</pv_name>
     <x>18</x>
     <y>168</y>
     <width>120</width>
```

### Comparing `pvi-0.8.1/src/pvi/_format/dls.edl` & `pvi-0.9.0/src/pvi/_format/dls.edl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/dls.py` & `pvi-0.9.0/src/pvi/_format/dls.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 template,
                 search="Heading",
                 property_map={"text": "text"},
             ),
             label_formatter_cls=LabelWidgetFormatter.from_template(
                 template,
                 search="Label",
-                property_map={"text": "text"},
+                property_map={"text": "text", "tooltip": "description"},
             ),
             led_formatter_cls=PVWidgetFormatter.from_template(
                 template,
                 search="LED",
                 sized=Bounds.square,
                 property_map={"pv_name": "pv"},
             ),
@@ -302,15 +302,20 @@
                 template,
                 search="Table",
                 property_map={"pv_name": "pv"},
             ),
             action_formatter_cls=ActionWidgetFormatter.from_template(
                 template,
                 search="WritePV",
-                property_map={"text": "label", "pv_name": "pv", "value": "value"},
+                property_map={
+                    "text": "label",
+                    "pv_name": "pv",
+                    "value": "value",
+                    "tooltip": "tooltip",
+                },
             ),
             sub_screen_formatter_cls=SubScreenWidgetFormatter.from_template(
                 template,
                 search="OpenDisplay",
                 property_map={"file": "file_name", "text": "label", "macros": "macros"},
             ),
         )
```

### Comparing `pvi-0.8.1/src/pvi/_format/edl.py` & `pvi-0.9.0/src/pvi/_format/edl.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/screen.py` & `pvi-0.9.0/src/pvi/_format/screen.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,15 +79,16 @@
         """Create an instance of `screen_cls` populated with widgets of `components`
 
         Args:
             components: A list of components that make up a device
             title: The title of the screen
 
         Returns:
-            A constructed screen object and a list of zero or more sub screen objects
+            A `ScreenFormatter` plus a list of (file name, `ScreenFormatter`) for any
+            nested `SubScreen`s in components
 
         """
         full_w = (
             self.layout.label_width + self.layout.widget_width + 2 * self.layout.spacing
         )
         screen_bounds = Bounds(h=self.layout.max_height)
         widget_dims = {"w": full_w, "h": self.layout.widget_height}
@@ -146,57 +147,69 @@
             ),
             sub_screens,
         )
 
     def create_sub_screen_formatters(
         self, screen_widgets: List[WidgetFormatter[T]]
     ) -> List[Tuple[str, GroupFormatter[T]]]:
-        """Create and return Screens from SubScreenFactorys in screen widgets
+        """Create and return `ScreenFormatter`s for any `SubScreenWidgetFormatters`
+
+        When the root screen formatter is created it will format a button that opens a
+        screen when a `SubScreen` widget is found, with a `SubScreenWidgetFormatter`.
+        Here we search through the components of the screen for these formatters and
+        create `ScreenFormatters`s that will format the screens that those buttons will
+        open.
+
+        This will recursively call `create_screen_formatter` and
+        `create_sub_screen_formatters` until no further `SubScreenWidgetFormatters` are
+        found.
 
         Args:
-            screen_widgets: List of WidgetFormatters containing 0-or-more
-            SubScreenFactorys to be found and
+            screen_widgets: List of `WidgetFormatters` containing 0-or-more
+            `SubScreenFactory`s to be found
 
         Returns:
-            List of (file name, Screen) created from found SubScreenFactorys
+            List of (file name, `ScreenFormatter`) created from `SubScreenFactory`s
 
         """
-        sub_screen_factories = [
+        sub_screen_widget_formatters = [
             # At the root
             widget_factory
             for widget_factory in screen_widgets
             if isinstance(widget_factory, SubScreenWidgetFormatter)
         ] + [
             # Nested in a Group
             group_widget_factory
             for widget_factory in screen_widgets
             if isinstance(widget_factory, GroupFormatter)
             for group_widget_factory in widget_factory.children
             if isinstance(group_widget_factory, SubScreenWidgetFormatter)
         ]
 
         sub_screen_formatters: List[Tuple[str, GroupFormatter[T]]] = []
-        for sub_screen_factory in sub_screen_factories:
-            if sub_screen_factory.components is None:
+        for sub_screen_widget_formatter in sub_screen_widget_formatters:
+            if sub_screen_widget_formatter.components is None:
                 # This is a reference to an existing screen - don't create it
                 continue
 
             factory: ScreenFormatterFactory = ScreenFormatterFactory(
                 screen_formatter_cls=self.screen_formatter_cls,
                 group_formatter_cls=self.group_formatter_cls,
                 widget_formatter_factory=self.widget_formatter_factory,
                 layout=self.layout,
+                base_file_name=f"{sub_screen_widget_formatter.file_name}",
             )
-            screen_formatter, sub_screen_formatter = factory.create_screen_formatter(
-                [sub_screen_factory.components], sub_screen_factory.components.name
+            screen_formatter, _sub_screen_formatters = factory.create_screen_formatter(
+                [sub_screen_widget_formatter.components],
+                sub_screen_widget_formatter.components.name,
             )
-            assert not sub_screen_formatter, "Only one level of sub screens allowed"
             sub_screen_formatters.append(
-                (sub_screen_factory.file_name, screen_formatter)
+                (sub_screen_widget_formatter.file_name, screen_formatter)
             )
+            sub_screen_formatters.extend(_sub_screen_formatters)
 
         return sub_screen_formatters
 
     def create_group_formatters(
         self,
         c: Group,
         screen_bounds: Bounds,
@@ -471,15 +484,15 @@
 
         if add_label:
             # Insert label and reduce width for widget
             left, row_bounds = component_bounds.split_left(
                 self.layout.label_width, self.layout.spacing
             )
             yield self.widget_formatter_factory.label_formatter_cls(
-                bounds=left, text=c.get_label()
+                bounds=left, text=c.get_label(), description=c.description or ""
             )
         else:
             # Allow full width for widget
             row_bounds = component_bounds
 
         if isinstance(c, SignalRef):
             yield from self.generate_component_formatters(
```

### Comparing `pvi-0.8.1/src/pvi/_format/template.py` & `pvi-0.9.0/src/pvi/_format/template.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/utils.py` & `pvi-0.9.0/src/pvi/_format/utils.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_format/widget.py` & `pvi-0.9.0/src/pvi/_format/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,26 +137,31 @@
             __base__=cls,
             format=format,
         )
 
 
 class LabelWidgetFormatter(WidgetFormatter[T]):
     text: str
+    description: str = ""
 
 
 class PVWidgetFormatter(WidgetFormatter[T]):
     pv: str
     widget: WidgetUnion
 
 
 class ActionWidgetFormatter(WidgetFormatter[T]):
     label: str
     pv: str
     value: str
 
+    @property
+    def tooltip(self) -> str:
+        return f"{self.pv} = {self.value}"
+
 
 class SubScreenWidgetFormatter(WidgetFormatter[T]):
     label: str
     file_name: str
     components: Optional[Group] = None
     macros: Dict[str, str] = Field(default={})
```

### Comparing `pvi-0.8.1/src/pvi/_pv_group.py` & `pvi-0.9.0/src/pvi/_pv_group.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/_yaml_utils.py` & `pvi-0.9.0/src/pvi/_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi/device.py` & `pvi-0.9.0/src/pvi/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,19 +77,19 @@
 
 PascalStr = Annotated[str, Field(pattern="^([A-Z][a-z0-9]*)*$")]
 
 
 class TextFormat(Enum):
     """Format to use for display of Text{Read,Write} widgets on a UI"""
 
-    decimal = 0
-    hexadecimal = 1
-    engineer = 2
-    exponential = 3
-    string = 4
+    decimal = "decimal"
+    hexadecimal = "hexadecimal"
+    engineer = "engineer"
+    exponential = "exponential"
+    string = "string"
 
 
 class AccessModeMixin(BaseModel):
     _access_mode: ClassVar[str]
 
     @property
     def access_mode(self) -> str:
@@ -287,15 +287,18 @@
 class Named(TypedModel):
     name: PascalStr = Field(description="PascalCase name to uniquely identify")
 
 
 class Component(Named):
     """These make up a Device"""
 
-    label: Optional[str] = None
+    label: Annotated[str | None, Field(description="Label for component")] = None
+    description: Annotated[
+        str | None, Field(description="Description for label tooltip")
+    ] = None
 
     def get_label(self):
         return self.label or to_title_case(self.name)
 
 
 class Signal(Component, AccessModeMixin):
     """Base signal type representing one or two PVs of a `Device`."""
```

### Comparing `pvi-0.8.1/src/pvi/typed_model.py` & `pvi-0.9.0/src/pvi/typed_model.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/src/pvi.egg-info/PKG-INFO` & `pvi-0.9.0/src/pvi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvi
-Version: 0.8.1
+Version: 0.9.0
 Summary: One line description of your module
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>, Gary Yendell <gary.yendell@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: pydantic
+Requires-Dist: pydantic>=2.7
 Requires-Dist: lxml
 Requires-Dist: ruamel.yaml
 Requires-Dist: typer
 Requires-Dist: jinja2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `pvi-0.8.1/src/pvi.egg-info/SOURCES.txt` & `pvi-0.9.0/src/pvi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/conftest.py` & `pvi-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/convert/input/simDetector.h` & `pvi-0.9.0/tests/convert/input/simDetector.h`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/convert/input/simDetector.template` & `pvi-0.9.0/tests/convert/input/simDetector.template`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/convert/output/simDetector.pvi.device.yaml` & `pvi-0.9.0/tests/convert/output/simDetector.pvi.device.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       type: TextRead
 
   - type: SignalR
     name: XMLErrorMsg
     read_pv: $(P)$(R)XMLErrorMsg_RBV
     read_widget:
       type: TextRead
-      format: 4
+      format: string
 
   - type: SignalR
     name: Dimensions
     read_pv: $(P)$(R)Dimensions_RBV
     read_widget:
       type: TextRead
```

### Comparing `pvi-0.8.1/tests/format/input/asynNDArrayDriver.pvi.device.yaml` & `pvi-0.9.0/tests/format/input/asynNDArrayDriver.pvi.device.yaml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/input/mixedWidgets.pvi.device.yaml` & `pvi-0.9.0/tests/format/input/mixedWidgets.pvi.device.yaml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/input/static_table.pvi.device.yaml` & `pvi-0.9.0/tests/format/input/static_table.pvi.device.yaml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/button.bob` & `pvi-0.9.0/tests/format/output/button.bob`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Acquire Time</text>
     <x>22</x>
     <y>30</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)AcquireTime</pv_name>
     <x>146</x>
     <y>30</y>
     <width>60</width>
@@ -58,14 +59,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Acquire</text>
     <x>22</x>
     <y>54</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="action_button" version="3.0.0">
     <name>WritePV</name>
     <pv_name>$(P)Acquire</pv_name>
     <actions>
       <action type="write_pv">
         <pv_name>$(pv_name)</pv_name>
@@ -74,15 +76,15 @@
       </action>
     </actions>
     <text>Start</text>
     <x>146</x>
     <y>54</y>
     <width>60</width>
     <height>20</height>
-    <tooltip>$(actions)</tooltip>
+    <tooltip>$(P)Acquire = 1</tooltip>
   </widget>
   <widget type="action_button" version="3.0.0">
     <name>WritePV</name>
     <pv_name>$(P)Acquire</pv_name>
     <actions>
       <action type="write_pv">
         <pv_name>$(pv_name)</pv_name>
@@ -91,23 +93,24 @@
       </action>
     </actions>
     <text>Stop</text>
     <x>210</x>
     <y>54</y>
     <width>60</width>
     <height>20</height>
-    <tooltip>$(actions)</tooltip>
+    <tooltip>$(P)Acquire = 0</tooltip>
   </widget>
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Acquire With RBV</text>
     <x>22</x>
     <y>78</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="action_button" version="3.0.0">
     <name>WritePV</name>
     <pv_name>$(P)Acquire</pv_name>
     <actions>
       <action type="write_pv">
         <pv_name>$(pv_name)</pv_name>
@@ -116,15 +119,15 @@
       </action>
     </actions>
     <text>Start</text>
     <x>146</x>
     <y>78</y>
     <width>38</width>
     <height>20</height>
-    <tooltip>$(actions)</tooltip>
+    <tooltip>$(P)Acquire = 1</tooltip>
   </widget>
   <widget type="action_button" version="3.0.0">
     <name>WritePV</name>
     <pv_name>$(P)Acquire</pv_name>
     <actions>
       <action type="write_pv">
         <pv_name>$(pv_name)</pv_name>
@@ -133,15 +136,15 @@
       </action>
     </actions>
     <text>Stop</text>
     <x>188</x>
     <y>78</y>
     <width>38</width>
     <height>20</height>
-    <tooltip>$(actions)</tooltip>
+    <tooltip>$(P)Acquire = 0</tooltip>
   </widget>
   <widget type="led" version="2.0.0">
     <name>LED</name>
     <pv_name>$(P)Acquire_RBV</pv_name>
     <x>239</x>
     <y>78</y>
     <width>20</width>
```

### Comparing `pvi-0.8.1/tests/format/output/combo_box.bob` & `pvi-0.9.0/tests/format/output/combo_box.bob`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Enum</text>
     <x>22</x>
     <y>30</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="combo" version="2.0.0">
     <name>ComboBox</name>
     <pv_name>$(P)Enum</pv_name>
     <x>146</x>
     <y>30</y>
     <width>60</width>
```

### Comparing `pvi-0.8.1/tests/format/output/device_ref.bob` & `pvi-0.9.0/tests/format/output/device_ref.bob`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Combo Box</text>
     <x>22</x>
     <y>30</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="action_button" version="3.0.0">
     <name>OpenDisplay</name>
     <actions>
       <action type="open_display">
         <file>combo_box.bob</file>
         <target>tab</target>
```

### Comparing `pvi-0.8.1/tests/format/output/index.bob` & `pvi-0.9.0/tests/format/output/index.bob`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Button - $(P)</text>
     <x>23</x>
     <y>30</y>
     <width>150</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="action_button" version="3.0.0">
     <name>OpenDisplay</name>
     <actions>
       <action type="open_display">
         <file>button.bob</file>
         <target>tab</target>
@@ -55,14 +56,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>ComboBox</text>
     <x>23</x>
     <y>55</y>
     <width>150</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="action_button" version="3.0.0">
     <name>OpenDisplay</name>
     <actions>
       <action type="open_display">
         <file>combo_box.bob</file>
         <target>tab</target>
@@ -82,14 +84,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>table</text>
     <x>23</x>
     <y>80</y>
     <width>150</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="action_button" version="3.0.0">
     <name>OpenDisplay</name>
     <actions>
       <action type="open_display">
         <file>pva_table.bob</file>
         <target>tab</target>
```

### Comparing `pvi-0.8.1/tests/format/output/mixedWidgets.adl` & `pvi-0.9.0/tests/format/output/mixedWidgets.adl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/mixedWidgets.bob` & `pvi-0.9.0/tests/format/output/mixedWidgets.bob`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Reset Power</text>
       <x>0</x>
       <y>0</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="choice" version="2.0.0">
       <name>ToggleButton</name>
       <pv_name>$(P)$(R)ResetPower</pv_name>
       <x>124</x>
       <y>0</y>
       <width>124</width>
@@ -51,14 +52,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Threshold Apply</text>
       <x>0</x>
       <y>24</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="choice" version="2.0.0">
       <name>ToggleButton</name>
       <pv_name>$(P)$(R)ThresholdApply</pv_name>
       <x>124</x>
       <y>24</y>
       <width>124</width>
@@ -67,14 +69,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Image File Tmot</text>
       <x>0</x>
       <y>48</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)ImageFileTmot</pv_name>
       <x>124</x>
       <y>48</y>
       <width>124</width>
@@ -84,14 +87,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Wavelength</text>
       <x>0</x>
       <y>72</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)Wavelength</pv_name>
       <x>124</x>
       <y>72</y>
       <width>124</width>
@@ -101,14 +105,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Energy Low</text>
       <x>0</x>
       <y>96</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)EnergyLow</pv_name>
       <x>124</x>
       <y>96</y>
       <width>124</width>
@@ -118,14 +123,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Energy High</text>
       <x>0</x>
       <y>120</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)EnergyHigh</pv_name>
       <x>124</x>
       <y>120</y>
       <width>124</width>
@@ -135,14 +141,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Det Dist</text>
       <x>0</x>
       <y>144</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)DetDist</pv_name>
       <x>124</x>
       <y>144</y>
       <width>124</width>
@@ -152,14 +159,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Det V Offset</text>
       <x>0</x>
       <y>168</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)DetVOffset</pv_name>
       <x>124</x>
       <y>168</y>
       <width>124</width>
@@ -169,14 +177,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Beam X</text>
       <x>0</x>
       <y>192</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)BeamX</pv_name>
       <x>124</x>
       <y>192</y>
       <width>124</width>
@@ -186,14 +195,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Beam Y</text>
       <x>0</x>
       <y>216</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)BeamY</pv_name>
       <x>124</x>
       <y>216</y>
       <width>124</width>
@@ -203,14 +213,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Flux</text>
       <x>0</x>
       <y>240</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)Flux</pv_name>
       <x>124</x>
       <y>240</y>
       <width>124</width>
@@ -221,14 +232,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Filter Transm</text>
     <x>22</x>
     <y>328</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)FilterTransm</pv_name>
     <x>146</x>
     <y>328</y>
     <width>124</width>
@@ -238,14 +250,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Start Angle</text>
     <x>22</x>
     <y>352</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)StartAngle</pv_name>
     <x>146</x>
     <y>352</y>
     <width>124</width>
@@ -255,14 +268,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Angle Incr</text>
     <x>22</x>
     <y>376</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)AngleIncr</pv_name>
     <x>146</x>
     <y>376</y>
     <width>124</width>
@@ -272,14 +286,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Det 2theta</text>
     <x>22</x>
     <y>400</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)Det2theta</pv_name>
     <x>146</x>
     <y>400</y>
     <width>124</width>
@@ -289,14 +304,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Polarization</text>
     <x>22</x>
     <y>424</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)Polarization</pv_name>
     <x>146</x>
     <y>424</y>
     <width>124</width>
@@ -306,14 +322,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Alpha</text>
     <x>22</x>
     <y>448</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)Alpha</pv_name>
     <x>146</x>
     <y>448</y>
     <width>124</width>
@@ -323,14 +340,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Kappa</text>
     <x>22</x>
     <y>472</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)Kappa</pv_name>
     <x>146</x>
     <y>472</y>
     <width>124</width>
@@ -340,14 +358,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Phi</text>
     <x>22</x>
     <y>496</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)Phi</pv_name>
     <x>146</x>
     <y>496</y>
     <width>124</width>
@@ -357,14 +376,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Phi Incr</text>
     <x>22</x>
     <y>520</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)PhiIncr</pv_name>
     <x>146</x>
     <y>520</y>
     <width>124</width>
@@ -374,14 +394,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Chi</text>
     <x>22</x>
     <y>544</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)Chi</pv_name>
     <x>146</x>
     <y>544</y>
     <width>124</width>
@@ -391,14 +412,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Chi Incr</text>
     <x>22</x>
     <y>568</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)ChiIncr</pv_name>
     <x>146</x>
     <y>568</y>
     <width>124</width>
@@ -408,14 +430,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Omega</text>
     <x>22</x>
     <y>592</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)Omega</pv_name>
     <x>146</x>
     <y>592</y>
     <width>124</width>
@@ -425,14 +448,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Omega Incr</text>
     <x>22</x>
     <y>616</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)OmegaIncr</pv_name>
     <x>146</x>
     <y>616</y>
     <width>124</width>
@@ -442,14 +466,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Oscill Axis</text>
     <x>22</x>
     <y>640</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)OscillAxis</pv_name>
     <x>146</x>
     <y>640</y>
     <width>124</width>
@@ -459,14 +484,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Num Oscill</text>
     <x>22</x>
     <y>664</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)NumOscill</pv_name>
     <x>146</x>
     <y>664</y>
     <width>124</width>
@@ -483,14 +509,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Bad Pixel File</text>
       <x>0</x>
       <y>0</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)BadPixelFile</pv_name>
       <x>124</x>
       <y>0</y>
       <width>124</width>
@@ -500,14 +527,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Flat Field File</text>
       <x>0</x>
       <y>24</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)FlatFieldFile</pv_name>
       <x>124</x>
       <y>24</y>
       <width>124</width>
@@ -517,14 +545,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Cbf Template File</text>
       <x>0</x>
       <y>48</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)CbfTemplateFile</pv_name>
       <x>124</x>
       <y>48</y>
       <width>124</width>
@@ -534,14 +563,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Header String</text>
       <x>0</x>
       <y>72</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)HeaderString</pv_name>
       <x>124</x>
       <y>72</y>
       <width>124</width>
@@ -551,14 +581,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Armed</text>
       <x>0</x>
       <y>96</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="led" version="2.0.0">
       <name>LED</name>
       <pv_name>$(P)$(R)Armed</pv_name>
       <x>176</x>
       <y>96</y>
       <width>20</width>
@@ -567,14 +598,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Num Bad Pixels</text>
       <x>0</x>
       <y>120</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
       <pv_name>$(P)$(R)NumBadPixels</pv_name>
       <x>124</x>
       <y>120</y>
       <width>124</width>
@@ -588,14 +620,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Flat Field Valid</text>
       <x>0</x>
       <y>144</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="led" version="2.0.0">
       <name>LED</name>
       <pv_name>$(P)$(R)FlatFieldValid</pv_name>
       <x>176</x>
       <y>144</y>
       <width>20</width>
@@ -604,14 +637,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Pixel Cut Off</text>
       <x>0</x>
       <y>168</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
       <pv_name>$(P)$(R)PixelCutOff_RBV</pv_name>
       <x>124</x>
       <y>168</y>
       <width>124</width>
@@ -625,14 +659,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Temp 0</text>
       <x>0</x>
       <y>192</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
       <pv_name>$(P)$(R)Temp0_RBV</pv_name>
       <x>124</x>
       <y>192</y>
       <width>124</width>
@@ -647,14 +682,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Temp 1</text>
     <x>308</x>
     <y>280</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>$(P)$(R)Temp1_RBV</pv_name>
     <x>432</x>
     <y>280</y>
     <width>124</width>
@@ -668,14 +704,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Temp 2</text>
     <x>308</x>
     <y>304</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>$(P)$(R)Temp2_RBV</pv_name>
     <x>432</x>
     <y>304</y>
     <width>124</width>
@@ -689,14 +726,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Humid 0</text>
     <x>308</x>
     <y>328</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>$(P)$(R)Humid0_RBV</pv_name>
     <x>432</x>
     <y>328</y>
     <width>124</width>
@@ -710,14 +748,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Humid 1</text>
     <x>308</x>
     <y>352</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>$(P)$(R)Humid1_RBV</pv_name>
     <x>432</x>
     <y>352</y>
     <width>124</width>
@@ -731,14 +770,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Humid 2</text>
     <x>308</x>
     <y>376</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>$(P)$(R)Humid2_RBV</pv_name>
     <x>432</x>
     <y>376</y>
     <width>124</width>
@@ -752,14 +792,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>TVX Version</text>
     <x>308</x>
     <y>400</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>$(P)$(R)TVXVersion_RBV</pv_name>
     <x>432</x>
     <y>400</y>
     <width>124</width>
@@ -773,14 +814,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Reset Power Time</text>
     <x>308</x>
     <y>424</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)ResetPowerTime</pv_name>
     <x>432</x>
     <y>424</y>
     <width>60</width>
@@ -803,14 +845,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Delay Time</text>
     <x>308</x>
     <y>448</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)$(R)DelayTime</pv_name>
     <x>432</x>
     <y>448</y>
     <width>60</width>
@@ -840,14 +883,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Threshold Energy</text>
       <x>0</x>
       <y>0</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)ThresholdEnergy</pv_name>
       <x>124</x>
       <y>0</y>
       <width>60</width>
@@ -870,14 +914,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Threshold Auto Apply</text>
       <x>0</x>
       <y>24</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="choice" version="2.0.0">
       <name>ToggleButton</name>
       <pv_name>$(P)$(R)ThresholdAutoApply</pv_name>
       <x>124</x>
       <y>24</y>
       <width>60</width>
@@ -894,14 +939,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Energy</text>
       <x>0</x>
       <y>48</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)Energy</pv_name>
       <x>124</x>
       <y>48</y>
       <width>60</width>
@@ -924,14 +970,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Min Flat Field</text>
       <x>0</x>
       <y>72</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
       <pv_name>$(P)$(R)MinFlatField</pv_name>
       <x>124</x>
       <y>72</y>
       <width>60</width>
@@ -954,14 +1001,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Gap Fill</text>
       <x>0</x>
       <y>96</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="combo" version="2.0.0">
       <name>ComboBox</name>
       <pv_name>$(P)$(R)GapFill</pv_name>
       <x>124</x>
       <y>96</y>
       <width>60</width>
@@ -983,14 +1031,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Gap Fill No Read PV</text>
       <x>0</x>
       <y>120</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="combo" version="2.0.0">
       <name>ComboBox</name>
       <pv_name>$(P)$(R)GapFillNoReadPV</pv_name>
       <x>124</x>
       <y>120</y>
       <width>124</width>
@@ -999,14 +1048,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Progress Bar Test</text>
       <x>0</x>
       <y>144</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="progressbar" version="2.0.0">
       <name>ProgressBar</name>
       <pv_name>$(P)$(R)ProgressBarTest_RBV</pv_name>
       <x>124</x>
       <y>144</y>
       <width>124</width>
@@ -1015,14 +1065,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Byte Monitor Test</text>
       <x>0</x>
       <y>168</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="byte_monitor" version="2.0.0">
       <name>BitField</name>
       <pv_name>$(P)$(R)ByteMonitor_RBV</pv_name>
       <x>124</x>
       <y>168</y>
       <width>160</width>
@@ -1031,14 +1082,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Array Trace Test</text>
       <x>0</x>
       <y>192</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="xyplot" version="3.0.0">
       <name>ArrayTrace</name>
       <x>124</x>
       <y>192</y>
       <width>124</width>
       <height>20</height>
@@ -1065,14 +1117,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Image Read Test</text>
       <x>0</x>
       <y>216</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="image" version="2.0.0">
       <name>ImageRead</name>
       <pv_name>$(P)$(R)ImageRead_RBV</pv_name>
       <x>124</x>
       <y>216</y>
       <width>124</width>
```

### Comparing `pvi-0.8.1/tests/format/output/mixedWidgets.edl` & `pvi-0.9.0/tests/format/output/mixedWidgets.edl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/pva_table.bob` & `pvi-0.9.0/tests/format/output/pva_table.bob`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/pva_table_panda.bob` & `pvi-0.9.0/tests/format/output/pva_table_panda.bob`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/pvi.template` & `pvi-0.9.0/tests/format/output/pvi.template`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/static_table.adl` & `pvi-0.9.0/tests/format/output/static_table.adl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/static_table.bob` & `pvi-0.9.0/tests/format/output/static_table.bob`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Binary</text>
     <x>22</x>
     <y>30</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="led" version="2.0.0">
     <name>LED</name>
     <pv_name>$(P)$(R)BINARYA</pv_name>
     <x>198</x>
     <y>30</y>
     <width>20</width>
```

### Comparing `pvi-0.8.1/tests/format/output/static_table.edl` & `pvi-0.9.0/tests/format/output/static_table.edl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/static_table_BigTable.adl` & `pvi-0.9.0/tests/format/output/static_table_BigTable.adl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/static_table_BigTable.bob` & `pvi-0.9.0/tests/format/output/static_table_BigTable.bob`

 * *Files 6% similar despite different names*

```diff
@@ -116,14 +116,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Row 1</text>
     <x>22</x>
     <y>54</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="led" version="2.0.0">
     <name>LED</name>
     <pv_name>$(P)$(R)BINARY_1</pv_name>
     <x>244</x>
     <y>54</y>
     <width>20</width>
@@ -171,14 +172,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Row 2</text>
     <x>22</x>
     <y>78</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="led" version="2.0.0">
     <name>LED</name>
     <pv_name>$(P)$(R)BINARY_2</pv_name>
     <x>244</x>
     <y>78</y>
     <width>20</width>
@@ -226,14 +228,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Row 3</text>
     <x>22</x>
     <y>102</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="led" version="2.0.0">
     <name>LED</name>
     <pv_name>$(P)$(R)BINARY_3</pv_name>
     <x>244</x>
     <y>102</y>
     <width>20</width>
@@ -281,14 +284,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Row 4</text>
     <x>22</x>
     <y>126</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="led" version="2.0.0">
     <name>LED</name>
     <pv_name>$(P)$(R)BINARY_4</pv_name>
     <x>244</x>
     <y>126</y>
     <width>20</width>
```

### Comparing `pvi-0.8.1/tests/format/output/static_table_BigTable.edl` & `pvi-0.9.0/tests/format/output/static_table_BigTable.edl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/static_table_BigTableA.adl` & `pvi-0.9.0/tests/format/output/static_table_BigTableA.adl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/static_table_BigTableA.bob` & `pvi-0.9.0/tests/format/output/static_table_BigTableA.bob`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/static_table_BigTableA.edl` & `pvi-0.9.0/tests/format/output/static_table_BigTableA.edl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/sub_screen.bob` & `pvi-0.9.0/tests/format/output/sub_screen.bob`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>A</text>
     <x>22</x>
     <y>30</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>$(P)A</pv_name>
     <x>146</x>
     <y>30</y>
     <width>124</width>
@@ -72,14 +73,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Group 3 E</text>
       <x>0</x>
       <y>0</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
       <pv_name>$(P)GROUP3:E</pv_name>
       <x>124</x>
       <y>0</y>
       <width>124</width>
@@ -93,14 +95,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Group 4</text>
       <x>0</x>
       <y>24</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="action_button" version="3.0.0">
       <name>OpenDisplay</name>
       <actions>
         <action type="open_display">
           <file>sub_screen_Group4.bob</file>
           <target>tab</target>
```

### Comparing `pvi-0.8.1/tests/format/output/sub_screen_Group1.bob` & `pvi-0.9.0/tests/format/output/sub_screen_Group1.bob`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Group 1 B</text>
     <x>22</x>
     <y>30</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>$(P)GROUP1:B</pv_name>
     <x>146</x>
     <y>30</y>
     <width>124</width>
@@ -56,14 +57,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Group 2 C</text>
       <x>0</x>
       <y>0</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
       <pv_name>$(P)GROUP1:GROUP2:C</pv_name>
       <x>124</x>
       <y>0</y>
       <width>124</width>
@@ -77,14 +79,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Group 2 D</text>
       <x>0</x>
       <y>24</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
       <pv_name>$(P)GROUP1:GROUP2:D</pv_name>
       <x>124</x>
       <y>24</y>
       <width>124</width>
```

### Comparing `pvi-0.8.1/tests/format/output/sub_screen_Group4.bob` & `pvi-0.9.0/tests/format/output/sub_screen_Group4.bob`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Group 4 F</text>
     <x>22</x>
     <y>30</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textupdate" version="2.0.0">
     <name>TextUpdate</name>
     <pv_name>$(P)GROUP3:GROUP4:F</pv_name>
     <x>146</x>
     <y>30</y>
     <width>124</width>
@@ -56,14 +57,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Group 5 G</text>
       <x>0</x>
       <y>0</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
       <pv_name>$(P)GROUP3:GROUP4:GROUP5:G</pv_name>
       <x>124</x>
       <y>0</y>
       <width>124</width>
@@ -77,14 +79,15 @@
     <widget type="label" version="2.0.0">
       <name>Label</name>
       <text>Group 5 H</text>
       <x>0</x>
       <y>24</y>
       <width>120</width>
       <height>20</height>
+      <tooltip>$(text)</tooltip>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
       <pv_name>$(P)GROUP3:GROUP4:GROUP5:H</pv_name>
       <x>124</x>
       <y>24</y>
       <width>124</width>
```

### Comparing `pvi-0.8.1/tests/format/output/text_format.adl` & `pvi-0.9.0/tests/format/output/text_format.adl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/format/output/text_format.bob` & `pvi-0.9.0/tests/format/output/text_format.bob`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Decimal</text>
     <x>22</x>
     <y>30</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)Decimal</pv_name>
     <x>146</x>
     <y>30</y>
     <width>60</width>
@@ -60,14 +61,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Hexadecimal</text>
     <x>22</x>
     <y>54</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)Hexadecimal</pv_name>
     <x>146</x>
     <y>54</y>
     <width>60</width>
@@ -92,14 +94,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Engineer</text>
     <x>22</x>
     <y>78</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)Engineer</pv_name>
     <x>146</x>
     <y>78</y>
     <width>60</width>
@@ -124,14 +127,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>Exponential</text>
     <x>22</x>
     <y>102</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)Exponential</pv_name>
     <x>146</x>
     <y>102</y>
     <width>60</width>
@@ -156,14 +160,15 @@
   <widget type="label" version="2.0.0">
     <name>Label</name>
     <text>String</text>
     <x>22</x>
     <y>126</y>
     <width>120</width>
     <height>20</height>
+    <tooltip>$(text)</tooltip>
   </widget>
   <widget type="textentry" version="3.0.0">
     <name>TextEntry</name>
     <pv_name>$(P)String</pv_name>
     <x>146</x>
     <y>126</y>
     <width>60</width>
```

### Comparing `pvi-0.8.1/tests/format/output/text_format.edl` & `pvi-0.9.0/tests/format/output/text_format.edl`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/test.pvi.device.yaml` & `pvi-0.9.0/tests/test.pvi.device.yaml`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/test_api.py` & `pvi-0.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/test_cli.py` & `pvi-0.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pvi-0.8.1/tests/test_device_serialization.py` & `pvi-0.9.0/tests/test_device_serialization.py`

 * *Files identical despite different names*

