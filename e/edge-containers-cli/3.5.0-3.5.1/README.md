# Comparing `tmp/edge_containers_cli-3.5.0.tar.gz` & `tmp/edge_containers_cli-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_containers_cli-3.5.0.tar", last modified: Tue May 21 11:20:39 2024, max compression
+gzip compressed data, was "edge_containers_cli-3.5.1.tar", last modified: Wed May 22 12:41:17 2024, max compression
```

## Comparing `edge_containers_cli-3.5.0.tar` & `edge_containers_cli-3.5.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.006164 edge_containers_cli-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.982164 edge_containers_cli-3.5.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2753 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_sys_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    99678 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:20:39.006164 edge_containers_cli-3.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.998164 edge_containers_cli-3.5.0/src/edge_containers_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/autocomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.998164 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/k8s_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/local_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8601 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/monitor.tcss
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.998164 edge_containers_cli-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.998164 edge_containers_cli-3.5.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/autocomplete.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1253 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.github/workflows/ci_verify.sh
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.github/workflows/verify.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1874 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/environment.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/tests/data/bl01t/helm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/Chart.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/tests/data/bl01t/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/templates/configmap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/tests/data/bl01t/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/pretend_helm.tgz
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/values.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/update-helm
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.144475 edge_containers_cli-3.5.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.148475 edge_containers_cli-3.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.140475 edge_containers_cli-3.5.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.148475 edge_containers_cli-3.5.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.148475 edge_containers_cli-3.5.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2753 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.148475 edge_containers_cli-3.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/workflows/_sys_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.148475 edge_containers_cli-3.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.148475 edge_containers_cli-3.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.148475 edge_containers_cli-3.5.1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.148475 edge_containers_cli-3.5.1/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.148475 edge_containers_cli-3.5.1/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    99678 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.144475 edge_containers_cli-3.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.152475 edge_containers_cli-3.5.1/src/edge_containers_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 12:41:17.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/autocomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.156475 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/k8s_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/local_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15429 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/monitor.tcss
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/src/edge_containers_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/src/edge_containers_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-22 12:41:17.000000 edge_containers_cli-3.5.1/src/edge_containers_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-22 12:41:17.000000 edge_containers_cli-3.5.1/src/edge_containers_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:41:17.000000 edge_containers_cli-3.5.1/src/edge_containers_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 12:41:17.000000 edge_containers_cli-3.5.1/src/edge_containers_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 12:41:17.000000 edge_containers_cli-3.5.1/src/edge_containers_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 12:41:17.000000 edge_containers_cli-3.5.1/src/edge_containers_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.156475 edge_containers_cli-3.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.156475 edge_containers_cli-3.5.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/autocomplete.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/tests/data/bl01t/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/tests/data/bl01t/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/tests/data/bl01t/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1253 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/.github/workflows/ci_verify.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/.github/workflows/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1874 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/environment.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.144475 edge_containers_cli-3.5.1/tests/data/bl01t/helm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/tests/data/bl01t/helm/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/helm/shared/Chart.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/helm/shared/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/helm/shared/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.144475 edge_containers_cli-3.5.1/tests/data/bl01t/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/tests/data/bl01t/include/iocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/include/iocs/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/tests/data/bl01t/include/iocs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/include/iocs/templates/configmap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.144475 edge_containers_cli-3.5.1/tests/data/bl01t/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:17.160475 edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/pretend_helm.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/values.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/bl01t/update-helm
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/data/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/test_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/test_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-22 12:41:12.000000 edge_containers_cli-3.5.1/tests/test_system.py
```

### Comparing `edge_containers_cli-3.5.0/.devcontainer/devcontainer.json` & `edge_containers_cli-3.5.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/CONTRIBUTING.md` & `edge_containers_cli-3.5.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/actions/install_requirements/action.yml` & `edge_containers_cli-3.5.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/dependabot.yml` & `edge_containers_cli-3.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/pages/make_switcher.py` & `edge_containers_cli-3.5.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/workflows/_check.yml` & `edge_containers_cli-3.5.1/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/workflows/_dist.yml` & `edge_containers_cli-3.5.1/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/workflows/_release.yml` & `edge_containers_cli-3.5.1/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/workflows/_sys_test.yml` & `edge_containers_cli-3.5.1/.github/workflows/_sys_test.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/workflows/_test.yml` & `edge_containers_cli-3.5.1/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.github/workflows/ci.yml` & `edge_containers_cli-3.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.gitignore` & `edge_containers_cli-3.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.pre-commit-config.yaml` & `edge_containers_cli-3.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/.vscode/launch.json` & `edge_containers_cli-3.5.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/LICENSE` & `edge_containers_cli-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/PKG-INFO` & `edge_containers_cli-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-containers-cli
-Version: 3.5.0
+Version: 3.5.1
 Summary: CLI for deploying and managing epics containers IOCs and services
 Author-email: Giles Knap <giles.knap@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `edge_containers_cli-3.5.0/README.md` & `edge_containers_cli-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/conf.py` & `edge_containers_cli-3.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `edge_containers_cli-3.5.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/explanations/decisions.rst` & `edge_containers_cli-3.5.1/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/how-to/build-docs.rst` & `edge_containers_cli-3.5.1/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/how-to/lint.rst` & `edge_containers_cli-3.5.1/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/how-to/make-release.rst` & `edge_containers_cli-3.5.1/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/how-to/pin-requirements.rst` & `edge_containers_cli-3.5.1/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/how-to/test-container.rst` & `edge_containers_cli-3.5.1/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/how-to/update-tools.rst` & `edge_containers_cli-3.5.1/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/index.rst` & `edge_containers_cli-3.5.1/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/reference/standards.rst` & `edge_containers_cli-3.5.1/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/developer/tutorials/dev-install.rst` & `edge_containers_cli-3.5.1/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/images/dls-favicon.ico` & `edge_containers_cli-3.5.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/images/dls-logo.svg` & `edge_containers_cli-3.5.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/index.rst` & `edge_containers_cli-3.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/user/explanations/docs-structure.rst` & `edge_containers_cli-3.5.1/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/user/index.rst` & `edge_containers_cli-3.5.1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/docs/user/tutorials/installation.rst` & `edge_containers_cli-3.5.1/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/pyproject.toml` & `edge_containers_cli-3.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -71,19 +71,23 @@
     "ignore:'autocompletion' is renamed to 'shell_complete'. The old name is deprecated and will be removed in Click 8.1. See the docs about 'Parameter' for information about new behavior.:DeprecationWarning:typer",
 ]
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "src tests"
 
 [tool.coverage.run]
 data_file = "/tmp/edge_containers_cli.coverage"
+omit = ["src/edge_containers_cli/cmds/monitor.py"]
 
 [tool.coverage.paths]
 # Tests are run from installed location, map back to the src directory
 source = ["src", "**/site-packages/"]
 
+[tool.coverage.report]
+omit = ["src/edge_containers_cli/cmds/monitor.py"]
+
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skipsdist=True
```

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/__main__.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/autocomplete.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/cli.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,35 +44,35 @@
 
     return commands
 
 
 @cli.command()
 def ps(
     ctx: typer.Context,
-    all: bool = typer.Option(
-        False, "-a", "--all", help="list stopped IOCs/services as well as running ones"
+    running_only: bool = typer.Option(
+        False, "-r", "--running-only", help="list only IOCs/services that are running"
     ),
     wide: bool = typer.Option(
         False, "--wide", "-w", help="use a wide format with additional fields"
     ),
 ):
     """List the IOCs/services running in the current namespace"""
-    commands(ctx).ps(all, wide)
+    commands(ctx).ps(running_only, wide)
 
 
 @cli.command()
 def monitor(
     ctx: typer.Context,
-    all: bool = typer.Option(
-        False, "-a", "--all", help="list stopped IOCs/services as well as running ones"
+    running_only: bool = typer.Option(
+        False, "-r", "--running-only", help="list only IOCs/services that are running"
     ),
 ):
     """Open IOC monitor TUI."""
     cmds = commands(ctx)
-    app = MonitorApp(EC_K8S_NAMESPACE, cmds, all)
+    app = MonitorApp(EC_K8S_NAMESPACE, cmds, running_only)
     app.run()
 
 
 @cli.command()
 def env(
     ctx: typer.Context,
     verbose: bool = typer.Option(
```

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/commands.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,31 +38,31 @@
 
     def deploy(self, service_name: str, version: str, args: str):
         raise NotImplementedError
 
     def exec(self, service_name: str):
         raise NotImplementedError
 
-    def logs(self, service_name: str, prev: bool, follow: bool):
+    def logs(self, service_name: str, prev: bool, follow: bool, stdout: bool):
         raise NotImplementedError
 
     def restart(self, service_name: str):
         raise NotImplementedError
 
     def start(self, service_name: str):
         raise NotImplementedError
 
     def stop(self, service_name: str):
         raise NotImplementedError
 
-    def get_services(self, all: bool) -> polars.DataFrame:
+    def get_services(self, running_only: bool) -> polars.DataFrame:
         raise NotImplementedError
 
-    def ps(self, all: bool, wide: bool):
-        select_data = self.get_services(all)
+    def ps(self, running_only: bool, wide: bool):
+        select_data = self.get_services(running_only)
         if not wide:
             select_data.drop_in_place("image")
         print(select_data)
 
     def environment(self, verbose: bool):
         """
         declare the environment settings for ec
```

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/helm.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/helm.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/k8s_commands.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/k8s_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Relies on the Helm class for deployment aspects.
 """
 
 from datetime import datetime
 from io import StringIO
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
 import polars
 import typer
 
 import edge_containers_cli.globals as globals
 import edge_containers_cli.shell as shell
 from edge_containers_cli.cmds.commands import Commands
@@ -119,22 +119,33 @@
         )
         chart.deploy()
 
     def exec(self, service_name):
         fullname = check_service(service_name, self.namespace)
         shell.run_command(f"kubectl -it -n {self.namespace} exec {fullname} -- bash")
 
-    def logs(self, service_name: str, prev: bool, follow: bool):
+    def logs(
+        self, service_name: str, prev: bool, follow: bool, stdout: bool = False
+    ) -> Optional[Union[str, bool]]:
         fullname = check_service(service_name, self.namespace)
         previous = "-p" if prev else ""
         fol = "-f" if follow else ""
 
-        shell.run_command(
-            f"kubectl -n {self.namespace} logs {fullname} {previous} {fol}"
-        )
+        if stdout:
+            a = shell.run_command(
+                f"kubectl -n {self.namespace} logs {fullname} {previous} {fol}",
+                interactive=False,
+                show=False,
+                error_OK=True,
+            )
+            return a
+        else:
+            shell.run_command(
+                f"kubectl -n {self.namespace} logs {fullname} {previous} {fol}",
+            )
 
     def restart(self, service_name):
         check_service(service_name, self.namespace)
         pod_name = shell.run_command(
             f"kubectl get -n {self.namespace} pod -l app={service_name} -o name",
             interactive=False,
         )
@@ -145,15 +156,15 @@
         shell.run_command(f"kubectl scale -n {self.namespace} {fullname} --replicas=1")
 
     def stop(self, service_name):
         fullname = check_service(service_name, self.namespace)
         """Stop an IOC"""
         shell.run_command(f"kubectl scale -n {self.namespace} {fullname} --replicas=0 ")
 
-    def get_services(self, all: bool) -> polars.DataFrame:
+    def get_services(self, running_only: bool) -> polars.DataFrame:
         services_df = polars.DataFrame()
 
         # Gives all services (running & not running) and their image
         for resource in ["deployment", "statefulset"]:
             kubectl_res = shell.run_command(
                 f"kubectl get {resource} -n {self.namespace} {jsonpath_deploy_info}",
                 interactive=False,
@@ -184,15 +195,15 @@
                 new_columns=["name", "running", "restarts"],
             )
             services_df = services_df.join(gtpo_df, on="name", how="left")
             services_df = services_df.with_columns(
                 polars.col("running").replace({"Running": True}, default=False),
                 polars.col("restarts").fill_null(0),
             )
-        elif all:
+        elif not running_only:
             services_df = services_df.with_columns(
                 running=polars.lit(False), restarts=polars.lit(0)
             )
         else:
             print("No running services found")
             raise typer.Exit()
 
@@ -206,19 +217,19 @@
         services_df = services_df.join(helm_df, on="name", how="left")
         log.debug(services_df)
 
         # Arrange columns
         services_df = services_df.select(
             ["name", "version", "running", "restarts", "deployed", "image"]
         )
-        if not all:
+        if running_only:
             services_df = services_df.filter(polars.col("running").eq(True))
             log.debug(services_df)
         return services_df
 
-    def ps(self, all: bool, wide: bool):
+    def ps(self, running_only: bool, wide: bool):
         """List all IOCs and Services in the current namespace"""
-        services_df = self.get_services(all)
+        services_df = self.get_services(running_only)
         if not wide:
             services_df.drop_in_place("image")
             log.debug(services_df)
         print(services_df)
```

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/local_commands.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/cmds/local_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,28 +137,28 @@
         )
 
         self._do_deploy(self.ioc_folder / service_name, version, args)
 
     def exec(self, service_name):
         self.docker.exec(service_name, "bash", args="-it")
 
-    def logs(self, service_name: str, prev: bool, follow: bool):
-        self.docker.logs(service_name, prev, follow)
+    def logs(self, service_name: str, prev: bool, follow: bool, stdout: bool = False):
+        self.docker.logs(service_name, prev, follow, stdout)
 
     def restart(self, service_name: str):
         shell.run_command(f"{self.docker.docker} restart {service_name}")
 
     def start(self, service_name: str):
         shell.run_command(f"{self.docker.docker} start {service_name}")
 
     def stop(self, service_name: str):
         shell.run_command(f"{self.docker.docker} stop {service_name}")
 
-    def get_services(self, all: bool) -> polars.DataFrame:
-        all_arg = " --all" if all else ""
+    def get_services(self, running_only: bool) -> polars.DataFrame:
+        all_arg = " --all" if not running_only else ""
 
         # List services
         avail_services = shell.run_command(
             f"{self.docker.docker} ps{all_arg} -q --filter label=is_IOC=true",
             interactive=False,
         )
 
@@ -197,16 +197,16 @@
                     ),
                     "image": service["Config"]["Image"],
                 }
             )
         log.debug(select_data)
         return polars.DataFrame(select_data)
 
-    def ps(self, all: bool, wide: bool):
-        select_data = self.get_services(all)
+    def ps(self, running_only: bool, wide: bool):
+        select_data = self.get_services(running_only)
         services_df = polars.DataFrame(select_data)
         if not wide:
             services_df.drop_in_place("image")
         print(services_df)
 
     def validate_instance(self, ioc_instance: Path):
         check_instance_path(ioc_instance)
```

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/docker.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/docker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Utility functions for working interacting with docker / podman CLI
 """
 
 import re
 from pathlib import Path
 from time import sleep
+from typing import Optional, Union
 
 import typer
 
 import edge_containers_cli.globals as globals
 import edge_containers_cli.shell as shell
 from edge_containers_cli.logging import log
 
@@ -100,23 +101,38 @@
         """
         attach to a container
         """
         self.is_running(container, error=True)
         # quitting the attach returns an error code so we have to ignore it
         shell.run_command(f"{self.docker} attach {container}", error_OK=True)
 
-    def logs(self, container: str, previous: bool = False, follow: bool = False):
+    def logs(
+        self,
+        container: str,
+        previous: bool = False,
+        follow: bool = False,
+        stdout: bool = False,
+    ) -> Optional[Union[str, bool]]:
         """
         show logs from a container
         """
         self.is_running(container, error=True)
         prev = " -p" if previous else ""
         fol = " -f" if follow else ""
 
-        shell.run_command(f"{self.docker} logs{prev}{fol} {container}")
+        if stdout:
+            a = shell.run_command(
+                f"{self.docker} logs{prev}{fol} {container}",
+                interactive=False,
+                show=False,
+                error_OK=True,
+            )
+            return a
+        else:
+            shell.run_command(f"{self.docker} logs{prev}{fol} {container}")
 
     def is_running(self, container: str, retry=1, error=False):
         """
         verify that a given container is up and running
         """
         for _i in range(retry):
             result = shell.run_command(
```

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/git.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/git.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/globals.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/globals.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/logging.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/logging.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/shell.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/shell.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli/utils.py` & `edge_containers_cli-3.5.1/src/edge_containers_cli/utils.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/PKG-INFO` & `edge_containers_cli-3.5.1/src/edge_containers_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-containers-cli
-Version: 3.5.0
+Version: 3.5.1
 Summary: CLI for deploying and managing epics containers IOCs and services
 Author-email: Giles Knap <giles.knap@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/SOURCES.txt` & `edge_containers_cli-3.5.1/src/edge_containers_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/conftest.py` & `edge_containers_cli-3.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/autocomplete.yaml` & `edge_containers_cli-3.5.1/tests/data/autocomplete.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/.github/workflows/ci_verify.sh` & `edge_containers_cli-3.5.1/tests/data/bl01t/.github/workflows/ci_verify.sh`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/LICENSE` & `edge_containers_cli-3.5.1/tests/data/bl01t/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/README.md` & `edge_containers_cli-3.5.1/tests/data/bl01t/README.md`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/environment.sh` & `edge_containers_cli-3.5.1/tests/data/bl01t/environment.sh`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/README.md` & `edge_containers_cli-3.5.1/tests/data/bl01t/helm/shared/README.md`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/values.yaml` & `edge_containers_cli-3.5.1/tests/data/bl01t/helm/shared/values.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/Chart.yaml` & `edge_containers_cli-3.5.1/tests/data/bl01t/include/iocs/Chart.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml` & `edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db` & `edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml` & `edge_containers_cli-3.5.1/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/ioc.yaml` & `edge_containers_cli-3.5.1/tests/data/ioc.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/data/local.yaml` & `edge_containers_cli-3.5.1/tests/data/local.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -106,19 +106,19 @@
     rsp: True
 
 stop:
   - cmd: docker stop bl01t-ea-test-01
     rsp: True
 
 ps:
-  - cmd: docker ps -q --filter label=is_IOC=true
+  - cmd: docker ps --all -q --filter label=is_IOC=true
     rsp: |
       0
       1
-  - cmd: docker inspect $(docker ps -q --filter label=is_IOC=true)
+  - cmd: docker inspect $(docker ps --all -q --filter label=is_IOC=true)
     rsp: >
       [
           {
                 "Created": "2024-03-19T11:10:53.736808252Z",
                 "State": {
                     "Running": true
                 },
```

### Comparing `edge_containers_cli-3.5.0/tests/test_autocomplete.py` & `edge_containers_cli-3.5.1/tests/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/test_ioc.py` & `edge_containers_cli-3.5.1/tests/test_ioc.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/test_local.py` & `edge_containers_cli-3.5.1/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.0/tests/test_system.py` & `edge_containers_cli-3.5.1/tests/test_system.py`

 * *Files identical despite different names*

