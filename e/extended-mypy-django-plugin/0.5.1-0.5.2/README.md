# Comparing `tmp/extended_mypy_django_plugin-0.5.1.tar.gz` & `tmp/extended_mypy_django_plugin-0.5.2.tar.gz`

## Comparing `extended_mypy_django_plugin-0.5.1.tar` & `extended_mypy_django_plugin-0.5.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.readthedocs.yaml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/DEVELOPMENT.rst
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/find
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/format
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/lint
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/mypy.ini
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/pytest.ini
--rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/run.sh
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/test.sh
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tox.ini
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/types
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/ciold.yml
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/lintold.yml
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/release.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/.gitignore
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/README.rst
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/conf.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/index.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/_static/css/extra.css
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/changelog.rst
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/installation.rst
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/primer.rst
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/tracking-changes.rst
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/usage.rst
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/actions.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/config.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/dependencies.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/hook.rst
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/index.rst
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/plugin.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/reports.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/store.rst
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/manage.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/mypy.ini
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/asgi.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/settings.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/urls.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/version.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/views.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/apps.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp2/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp2/apps.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp2/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp2/migrations/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/__init__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/annotations.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/entry.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/py.typed
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/version.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/__init__.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_config.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_debug.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_dependencies.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_hook.py
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_plugin.py
--rw-r--r--   0        0        0    15489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_reports.py
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_store.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/__init__.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_type_analyze.py
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_type_checker.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/determine_django_state.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/find_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/make_old.patch
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/py.typed
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/test_settings.py
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/tests_extension_hook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp/apps.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp2/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp2/apps.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp2/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tests/test_concrete_annotation.yml
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tests/test_works.yml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/.gitignore
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/bootstrap_venvstarter.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/devtools.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/requirements.dev.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/requirements.docs.txt
--rwxr-xr-x   0        0        0     1108 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/venv
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/LICENSE
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/README.rst
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/DEVELOPMENT.rst
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/find
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/format
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/lint
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/mypy.ini
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/pytest.ini
+-rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/run.sh
+-rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/test.sh
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tox.ini
+-rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/types
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/ciold.yml
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/lintold.yml
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/.gitignore
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/README.rst
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/conf.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/index.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/_static/css/extra.css
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/changelog.rst
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/installation.rst
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/primer.rst
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/tracking-changes.rst
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/usage.rst
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/actions.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/config.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/dependencies.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/hook.rst
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/index.rst
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/plugin.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/reports.rst
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/store.rst
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/manage.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/mypy.ini
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/asgi.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/settings.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/urls.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/version.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/views.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/apps.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp2/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp2/apps.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp2/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp2/migrations/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/__init__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/annotations.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/entry.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/py.typed
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/version.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/__init__.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_config.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_debug.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_dependencies.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_hook.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_plugin.py
+-rw-r--r--   0        0        0    15489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_reports.py
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_store.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/__init__.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_type_analyze.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_type_checker.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/determine_django_state.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/find_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/make_old.patch
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/py.typed
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/test_settings.py
+-rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/tests_extension_hook.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp/apps.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp2/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp2/apps.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp2/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tests/test_concrete_annotation.yml
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tests/test_works.yml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/.gitignore
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/bootstrap_venvstarter.py
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/devtools.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/requirements.dev.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/requirements.docs.txt
+-rwxr-xr-x   0        0        0     1108 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/venv
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/README.rst
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/PKG-INFO
```

### Comparing `extended_mypy_django_plugin-0.5.1/DEVELOPMENT.rst` & `extended_mypy_django_plugin-0.5.2/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/run.sh` & `extended_mypy_django_plugin-0.5.2/run.sh`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/.github/workflows/ci.yml` & `extended_mypy_django_plugin-0.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/.github/workflows/ciold.yml` & `extended_mypy_django_plugin-0.5.2/.github/workflows/ciold.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/.github/workflows/lint.yml` & `extended_mypy_django_plugin-0.5.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/.github/workflows/lintold.yml` & `extended_mypy_django_plugin-0.5.2/.github/workflows/lintold.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/.github/workflows/release.yml` & `extended_mypy_django_plugin-0.5.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/docs/conf.py` & `extended_mypy_django_plugin-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/docs/api/changelog.rst` & `extended_mypy_django_plugin-0.5.2/docs/api/changelog.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. _changelog:
 
 Changelog
 ---------
 
+.. _release-0.5.2:
+
+0.5.2 - 22 May 2024
+    * Add more confidence get_function_hook doesn't steal from django-stubs
+
 .. _release-0.5.1:
 
 0.5.1 - 21 May 2024
     * Providing a return code of 2 from the installed_apps script will make dmypy not
       change version to cause a restart.
     * Changed the ``get_installed_apps`` setting to be ``determine_django_state``
     * Changed the name in pyproject.toml to use dashes instead of underscores
```

### Comparing `extended_mypy_django_plugin-0.5.1/docs/api/installation.rst` & `extended_mypy_django_plugin-0.5.2/docs/api/installation.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/docs/api/primer.rst` & `extended_mypy_django_plugin-0.5.2/docs/api/primer.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/docs/api/tracking-changes.rst` & `extended_mypy_django_plugin-0.5.2/docs/api/tracking-changes.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/docs/api/usage.rst` & `extended_mypy_django_plugin-0.5.2/docs/api/usage.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/docs/api/internals/actions.rst` & `extended_mypy_django_plugin-0.5.2/docs/api/internals/actions.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/example/manage.py` & `extended_mypy_django_plugin-0.5.2/example/manage.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/example/djangoexample/settings.py` & `extended_mypy_django_plugin-0.5.2/example/djangoexample/settings.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/example/djangoexample/urls.py` & `extended_mypy_django_plugin-0.5.2/example/djangoexample/urls.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/example/djangoexample/views.py` & `extended_mypy_django_plugin-0.5.2/example/djangoexample/views.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/models.py` & `extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/models.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/annotations.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/annotations.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/entry.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/entry.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_config.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_config.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_dependencies.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_dependencies.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_hook.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_hook.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_plugin.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,16 +200,16 @@
                 assert_never(name)
 
             return method(unbound_type=ctx.type)
 
     @_hook.hook
     class get_function_hook(Hook[FunctionContext, MypyType]):
         """
-        Find functions that return a ``DefaultQuerySet`` annotation and resolve
-        the annotation.
+        Find functions that return a ``DefaultQuerySet`` annotation with a type variable
+        and resolve the annotation.
         """
 
         def choose(self) -> bool:
             sym = self.plugin.lookup_fully_qualified(self.fullname)
             if not sym or not sym.node:
                 return False
 
@@ -220,20 +220,27 @@
             return call.is_generic()
 
         def run(self, ctx: FunctionContext) -> MypyType:
             assert isinstance(ctx.api, TypeChecker)
 
             type_checking = actions.TypeChecking(self.store, api=ctx.api)
 
-            return type_checking.modify_default_queryset_return_type(
+            result = type_checking.modify_default_queryset_return_type(
                 ctx,
-                super_hook=self.super_hook,
                 desired_annotation_fullname=ExtendedMypyStubs.Annotations.DEFAULT_QUERYSET.value,
             )
 
+            if result is not None:
+                return result
+
+            if self.super_hook is not None:
+                return self.super_hook(ctx)
+
+            return ctx.default_return_type
+
     @_hook.hook
     class get_attribute_hook(Hook[AttributeContext, MypyType]):
         """
         An implementation of the change found in
         https://github.com/typeddjango/django-stubs/pull/2027
         """
```

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_reports.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_reports.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_store.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_store.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_type_analyze.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_type_analyze.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_type_checker.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_type_checker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections.abc import Callable
 from typing import Protocol
 
 from mypy.checker import TypeChecker
 from mypy.nodes import CallExpr, MemberExpr, TypeInfo
 from mypy.plugin import (
     AttributeContext,
     FunctionContext,
@@ -35,42 +34,40 @@
         self.api = api
         self.store = store
 
     def modify_default_queryset_return_type(
         self,
         ctx: FunctionContext,
         *,
-        super_hook: Callable[[FunctionContext], MypyType] | None,
         desired_annotation_fullname: str,
-    ) -> MypyType:
+    ) -> MypyType | None:
         if not isinstance(ctx.default_return_type, UnboundType):
-            return ctx.default_return_type
+            return None
 
         context = ctx.context
         if not isinstance(context, CallExpr):
-            return ctx.default_return_type
+            return None
 
         if hasattr(self.api, "get_expression_type"):
             # In later mypy versions
             func = self.api.get_expression_type(context.callee)
         else:
             func = self.api.expr_checker.accept(context.callee)
 
         func = get_proper_type(func)
 
         if not isinstance(func, CallableType):
-            self.api.fail("Expected to be operating on a callable", context)
-            return AnyType(TypeOfAny.from_error)
+            return None
 
         if not isinstance(func.ret_type, UnboundType):
-            return ctx.default_return_type
+            return None
 
         as_generic_type = self.api.named_generic_type(func.ret_type.name, [func.ret_type.args[0]])
         if as_generic_type.type.fullname != desired_annotation_fullname:
-            return ctx.default_return_type
+            return None
 
         if len(func.ret_type.args) != 1:
             self.api.fail("DefaultQuerySet takes only one argument", context)
             return AnyType(TypeOfAny.from_error)
 
         found_type: MypyType | None = None
```

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/determine_django_state.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/determine_django_state.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/find_models.py` & `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/find_models.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/scripts/make_old.patch` & `extended_mypy_django_plugin-0.5.2/scripts/make_old.patch`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/scripts/tests_extension_hook.py` & `extended_mypy_django_plugin-0.5.2/scripts/tests_extension_hook.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/scripts/myapp/models.py` & `extended_mypy_django_plugin-0.5.2/scripts/myapp/models.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/tests/test_concrete_annotation.yml` & `extended_mypy_django_plugin-0.5.2/tests/test_concrete_annotation.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/tests/test_works.yml` & `extended_mypy_django_plugin-0.5.2/tests/test_works.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/tools/bootstrap_venvstarter.py` & `extended_mypy_django_plugin-0.5.2/tools/bootstrap_venvstarter.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/tools/devtools.py` & `extended_mypy_django_plugin-0.5.2/tools/devtools.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/tools/venv` & `extended_mypy_django_plugin-0.5.2/tools/venv`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/LICENSE` & `extended_mypy_django_plugin-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/README.rst` & `extended_mypy_django_plugin-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/pyproject.toml` & `extended_mypy_django_plugin-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.1/PKG-INFO` & `extended_mypy_django_plugin-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: extended-mypy-django-plugin
-Version: 0.5.1
+Version: 0.5.2
 Summary: Trying to make mypy understand .objects on abstract django models
 Author-email: Stephen Moore <stephen@delfick.com>
 License: MIT
 License-File: LICENSE
 Provides-Extra: stubs-latest
 Requires-Dist: django-stubs==5.0.0; extra == 'stubs-latest'
 Requires-Dist: mypy==1.10.0; extra == 'stubs-latest'
```

