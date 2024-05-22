# Comparing `tmp/kr8s-0.9.1.tar.gz` & `tmp/kr8s-0.9.2.tar.gz`

## Comparing `kr8s-0.9.1.tar` & `kr8s-0.9.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kr8s-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 kr8s-0.9.1/.readthedocs.yaml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 kr8s-0.9.1/codecov.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 kr8s-0.9.1/.github/labeler.yml
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 kr8s-0.9.1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 kr8s-0.9.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kr8s-0.9.1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 kr8s-0.9.1/.github/workflows/pr-labeler.yaml
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 kr8s-0.9.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 kr8s-0.9.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 kr8s-0.9.1/.github/workflows/update-kubernetes.yaml
--rw-r--r--   0        0        0   371092 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/banner.jpeg
--rw-r--r--   0        0        0    24640 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/kr8s-sticker.svg
--rw-r--r--   0        0        0   172626 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo-alt.jpeg
--rw-r--r--   0        0        0    75601 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo-alt.png
--rw-r--r--   0        0        0    23375 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo-alt.svg
--rw-r--r--   0        0        0   108080 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo-solo.png
--rw-r--r--   0        0        0   760967 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo-wide.jpeg
--rw-r--r--   0        0        0   118783 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo-wide.png
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo-wide.svg
--rw-r--r--   0        0        0   174304 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo.jpeg
--rw-r--r--   0        0        0   148638 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo.png
--rw-r--r--   0        0        0    23133 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/logo.svg
--rw-r--r--   0        0        0   536700 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/profile.jpeg
--rw-r--r--   0        0        0   125457 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/social.png
--rw-r--r--   0        0        0    53667 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/text-trimmed.png
--rw-r--r--   0        0        0    83203 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/text.jpeg
--rw-r--r--   0        0        0    27291 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/text.png
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/text.svg
--rw-r--r--   0        0        0   428882 2020-02-02 00:00:00.000000 kr8s-0.9.1/branding/vector.ai
--rwxr-xr-x   0        0        0     2254 2020-02-02 00:00:00.000000 kr8s-0.9.1/ci/update-kubernetes.py
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/alternatives.md
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/asyncio.md
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/authentication.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/branding.md
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/client.md
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/conf.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/contributing.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/history.md
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/index.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/installation.md
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/object.md
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/releasing.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/examples/creating_resources.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/examples/index.md
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/examples/inspecting_resources.md
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/examples/labelling_operator.md
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/examples/listing_resources.md
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 kr8s-0.9.1/docs/examples/modifying_resources.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/README.md
--rw-r--r--   0        0        0    77540 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/poetry.lock
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/pyproject.toml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/__init__.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_api_resources.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_create.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_delete.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_formatters.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_get.py
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_wait.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/cli.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/tests/test_create_delete.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/tests/test_formatters.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/tests/test_version.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/tests/resources/simple/nginx_pod_service.yaml
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/__init__.py
--rw-r--r--   0        0        0    14762 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/_api.py
--rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/_auth.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/_data_utils.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/_exceptions.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/_io.py
--rw-r--r--   0        0        0    40284 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/_objects.py
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/_testutils.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/_version.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/conftest.py
--rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/objects.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/portforward.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/asyncio/_helpers.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/test_io.py
--rw-r--r--   0        0        0    21208 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/resources/serviceaccount.yaml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/resources/custom/evc.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/resources/simple/nginx_pod.yaml
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/resources/simple/nginx_pod_service.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
--rwxr-xr-x   0        0        0      614 2020-02-02 00:00:00.000000 kr8s-0.9.1/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 kr8s-0.9.1/.gitignore
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 kr8s-0.9.1/LICENSE
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 kr8s-0.9.1/README.md
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 kr8s-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 kr8s-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kr8s-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 kr8s-0.9.2/.readthedocs.yaml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 kr8s-0.9.2/codecov.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 kr8s-0.9.2/.github/labeler.yml
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 kr8s-0.9.2/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 kr8s-0.9.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kr8s-0.9.2/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 kr8s-0.9.2/.github/workflows/pr-labeler.yaml
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 kr8s-0.9.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 kr8s-0.9.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 kr8s-0.9.2/.github/workflows/update-kubernetes.yaml
+-rw-r--r--   0        0        0   371092 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/banner.jpeg
+-rw-r--r--   0        0        0    24640 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/kr8s-sticker.svg
+-rw-r--r--   0        0        0   172626 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo-alt.jpeg
+-rw-r--r--   0        0        0    75601 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo-alt.png
+-rw-r--r--   0        0        0    23375 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo-alt.svg
+-rw-r--r--   0        0        0   108080 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo-solo.png
+-rw-r--r--   0        0        0   760967 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo-wide.jpeg
+-rw-r--r--   0        0        0   118783 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo-wide.png
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo-wide.svg
+-rw-r--r--   0        0        0   174304 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo.jpeg
+-rw-r--r--   0        0        0   148638 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo.png
+-rw-r--r--   0        0        0    23133 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/logo.svg
+-rw-r--r--   0        0        0   536700 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/profile.jpeg
+-rw-r--r--   0        0        0   125457 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/social.png
+-rw-r--r--   0        0        0    53667 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/text-trimmed.png
+-rw-r--r--   0        0        0    83203 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/text.jpeg
+-rw-r--r--   0        0        0    27291 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/text.png
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/text.svg
+-rw-r--r--   0        0        0   428882 2020-02-02 00:00:00.000000 kr8s-0.9.2/branding/vector.ai
+-rwxr-xr-x   0        0        0     2254 2020-02-02 00:00:00.000000 kr8s-0.9.2/ci/update-kubernetes.py
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/alternatives.md
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/asyncio.md
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/authentication.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/branding.md
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/client.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/conf.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/contributing.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/history.md
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/index.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/installation.md
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/object.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/releasing.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/examples/creating_resources.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/examples/index.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/examples/inspecting_resources.md
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/examples/labelling_operator.md
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/examples/listing_resources.md
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 kr8s-0.9.2/docs/examples/modifying_resources.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/README.md
+-rw-r--r--   0        0        0    77540 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/poetry.lock
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/pyproject.toml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/__init__.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_api_resources.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_create.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_delete.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_formatters.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_get.py
+-rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_wait.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/cli.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/tests/test_create_delete.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/tests/test_formatters.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/tests/test_version.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/tests/resources/simple/nginx_pod_service.yaml
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/__init__.py
+-rw-r--r--   0        0        0    14762 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/_api.py
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/_io.py
+-rw-r--r--   0        0        0    40312 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/_objects.py
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/_testutils.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/_version.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/conftest.py
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/portforward.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/asyncio/_helpers.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    21690 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rwxr-xr-x   0        0        0      614 2020-02-02 00:00:00.000000 kr8s-0.9.2/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 kr8s-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 kr8s-0.9.2/LICENSE
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 kr8s-0.9.2/README.md
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 kr8s-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 kr8s-0.9.2/PKG-INFO
```

### Comparing `kr8s-0.9.1/.pre-commit-config.yaml` & `kr8s-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/.github/ISSUE_TEMPLATE/bug-report.yml` & `kr8s-0.9.2/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/.github/ISSUE_TEMPLATE/feature-request.yml` & `kr8s-0.9.2/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/.github/workflows/release.yaml` & `kr8s-0.9.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/.github/workflows/test.yaml` & `kr8s-0.9.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/.github/workflows/update-kubernetes.yaml` & `kr8s-0.9.2/.github/workflows/update-kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/banner.jpeg` & `kr8s-0.9.2/branding/banner.jpeg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/kr8s-sticker.svg` & `kr8s-0.9.2/branding/kr8s-sticker.svg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo-alt.jpeg` & `kr8s-0.9.2/branding/logo-alt.jpeg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo-alt.png` & `kr8s-0.9.2/branding/logo-alt.png`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo-alt.svg` & `kr8s-0.9.2/branding/logo-alt.svg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo-solo.png` & `kr8s-0.9.2/branding/logo-solo.png`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo-wide.jpeg` & `kr8s-0.9.2/branding/logo-wide.jpeg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo-wide.png` & `kr8s-0.9.2/branding/logo-wide.png`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo-wide.svg` & `kr8s-0.9.2/branding/logo-wide.svg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo.jpeg` & `kr8s-0.9.2/branding/logo.jpeg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo.png` & `kr8s-0.9.2/branding/logo.png`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/logo.svg` & `kr8s-0.9.2/branding/logo.svg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/profile.jpeg` & `kr8s-0.9.2/branding/profile.jpeg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/social.png` & `kr8s-0.9.2/branding/social.png`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/text-trimmed.png` & `kr8s-0.9.2/branding/text-trimmed.png`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/text.jpeg` & `kr8s-0.9.2/branding/text.jpeg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/text.png` & `kr8s-0.9.2/branding/text.png`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/text.svg` & `kr8s-0.9.2/branding/text.svg`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/branding/vector.ai` & `kr8s-0.9.2/branding/vector.ai`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/ci/update-kubernetes.py` & `kr8s-0.9.2/ci/update-kubernetes.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/alternatives.md` & `kr8s-0.9.2/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/asyncio.md` & `kr8s-0.9.2/docs/asyncio.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/authentication.md` & `kr8s-0.9.2/docs/authentication.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/branding.md` & `kr8s-0.9.2/docs/branding.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/client.md` & `kr8s-0.9.2/docs/client.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/conf.py` & `kr8s-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/history.md` & `kr8s-0.9.2/docs/history.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/index.md` & `kr8s-0.9.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/object.md` & `kr8s-0.9.2/docs/object.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/examples/creating_resources.md` & `kr8s-0.9.2/docs/examples/creating_resources.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/examples/inspecting_resources.md` & `kr8s-0.9.2/docs/examples/inspecting_resources.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/examples/labelling_operator.md` & `kr8s-0.9.2/docs/examples/labelling_operator.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/examples/listing_resources.md` & `kr8s-0.9.2/docs/examples/listing_resources.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/docs/examples/modifying_resources.md` & `kr8s-0.9.2/docs/examples/modifying_resources.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/poetry.lock` & `kr8s-0.9.2/examples/kubectl-ng/poetry.lock`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/pyproject.toml` & `kr8s-0.9.2/examples/kubectl-ng/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_api_resources.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_api_resources.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_create.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_create.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_delete.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_delete.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_formatters.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_formatters.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_get.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_get.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/_wait.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/_wait.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/cli.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/cli.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/tests/test_create_delete.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/tests/test_create_delete.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/tests/test_formatters.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/examples/kubectl-ng/kubectl_ng/tests/test_version.py` & `kr8s-0.9.2/examples/kubectl-ng/kubectl_ng/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/__init__.py` & `kr8s-0.9.2/kr8s/__init__.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/_api.py` & `kr8s-0.9.2/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/_auth.py` & `kr8s-0.9.2/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/_data_utils.py` & `kr8s-0.9.2/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/_io.py` & `kr8s-0.9.2/kr8s/_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/_objects.py` & `kr8s-0.9.2/kr8s/_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     ) -> APIObject:
         """Get a Kubernetes resource by name or via selectors."""
 
         if api is None:
             if cls._asyncio:
                 api = await kr8s.asyncio.api()
             else:
-                api = kr8s.api()
+                api = await kr8s.asyncio.api(_asyncio=False)
         namespace = namespace if namespace else api.namespace
         start = time.time()
         backoff = 0.1
         while start + timeout > time.time():
             if name:
                 try:
                     resources = await api._get(
```

### Comparing `kr8s-0.9.1/kr8s/_portforward.py` & `kr8s-0.9.2/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/_testutils.py` & `kr8s-0.9.2/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/conftest.py` & `kr8s-0.9.2/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/objects.py` & `kr8s-0.9.2/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/asyncio/_api.py` & `kr8s-0.9.2/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/asyncio/_helpers.py` & `kr8s-0.9.2/kr8s/asyncio/_helpers.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/asyncio/objects.py` & `kr8s-0.9.2/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/tests/test_api.py` & `kr8s-0.9.2/kr8s/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/tests/test_auth.py` & `kr8s-0.9.2/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/tests/test_data_utils.py` & `kr8s-0.9.2/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/tests/test_io.py` & `kr8s-0.9.2/kr8s/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/tests/test_objects.py` & `kr8s-0.9.2/kr8s/tests/test_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,14 +219,29 @@
     await pod.delete()
     while await pod.exists():
         await asyncio.sleep(0.1)
     with pytest.raises(kr8s.NotFoundError):
         await pod2.delete()
 
 
+def test_pod_get_sync(example_pod_spec):
+    pod = SyncPod(example_pod_spec)
+    pod.create()
+    with pytest.raises(kr8s.NotFoundError):
+        SyncPod.get(f"{pod.name}-foo", namespace=pod.namespace, timeout=0.1)
+    pod2 = SyncPod.get(pod.name, namespace=pod.namespace)
+    assert pod2.name == pod.name
+    assert pod2.namespace == pod.namespace
+    pod.delete()
+    while pod.exists():
+        time.sleep(0.1)
+    with pytest.raises(kr8s.NotFoundError):
+        pod2.delete()
+
+
 async def test_pod_from_name(example_pod_spec):
     pod = await Pod(example_pod_spec)
     await pod.create()
     pod2 = await Pod(
         pod.name, namespace=pod.namespace
     )  # Note: Does not call the Kubernetes API
     assert pod2.name == pod.name
```

### Comparing `kr8s-0.9.1/kr8s/tests/test_testutils.py` & `kr8s-0.9.2/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/kr8s/tests/scripts/envexec.py` & `kr8s-0.9.2/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/.gitignore` & `kr8s-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/LICENSE` & `kr8s-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/README.md` & `kr8s-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/pyproject.toml` & `kr8s-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kr8s-0.9.1/PKG-INFO` & `kr8s-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Kubernetes API library
 Author-email: Jacob Tomlimson <jacob@tomlinson.email>
 License: BSD-3-Clause
 License-File: LICENSE
 Keywords: kubectl,kubernetes
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

