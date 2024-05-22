# Comparing `tmp/jupyverse-0.5.4.tar.gz` & `tmp/jupyverse-0.6.0.tar.gz`

## Comparing `jupyverse-0.5.4.tar` & `jupyverse-0.6.0.tar`

### file list

```diff
@@ -1,252 +1,252 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyverse-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    79989 2020-02-02 00:00:00.000000 jupyverse-0.5.4/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.5.4/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.5.4/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.5.4/config.yaml
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 jupyverse-0.5.4/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.5.4/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.5.4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.5.4/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.5.4/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 jupyverse-0.5.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.5.4/binder/environment.yml
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyverse-0.5.4/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.5.4/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.5.4/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/index.md
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/kernels.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/notebook.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/plugins/yjs.md
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/tutorials/jupyterhub_jupyverse_deployment.md
--rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/tutorials/standalone_jupyverse_deployment.md
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/usage/microservices.md
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 jupyverse-0.5.4/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/README.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/cli.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/notebook/__init__.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.5.4/jupyverse_api/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.5.4/notebooks/admin_users.ipynb
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.5.4/notebooks/admin_users.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/COPYING.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/README.md
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/pyproject.toml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/config.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/launch.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/models.py
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/lab/README.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/lab/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/noauth/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/notebook/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/notebook/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/notebook/README.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/notebook/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/notebook/fps_notebook/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/notebook/fps_notebook/main.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/notebook/fps_notebook/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/terminals/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/webdav/COPYING.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/webdav/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/webdav/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/webdav/fps_webdav/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/webdav/fps_webdav/config.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/webdav/fps_webdav/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/webdav/fps_webdav/py.typed
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/webdav/fps_webdav/routes.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/webdav/tests/test_webdav.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/README.md
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/utils.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/ybasedoc.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/yblob.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/yfile.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/ynotebook.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/yunicode.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/awareness.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/websocket.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py
--rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/yroom.py
--rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/ystore.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/yutils.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywidgets/__init__.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyverse-0.5.4/plugins/yjs/fps_yjs/ywidgets/widgets.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/conftest.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/test_app.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/test_contents.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/test_execute.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/test_kernels.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/test_server.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.5.4/tests/data/notebook1.ipynb
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse-0.5.4/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.4/COPYING.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyverse-0.5.4/README.md
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 jupyverse-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyverse-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyverse-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    80603 2020-02-02 00:00:00.000000 jupyverse-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.6.0/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.6.0/config.yaml
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 jupyverse-0.6.0/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.6.0/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.6.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.6.0/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.6.0/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 jupyverse-0.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.6.0/binder/environment.yml
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyverse-0.6.0/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.6.0/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.6.0/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/index.md
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/notebook.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/tutorials/jupyterhub_jupyverse_deployment.md
+-rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/tutorials/standalone_jupyverse_deployment.md
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 jupyverse-0.6.0/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/notebook/__init__.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.6.0/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.6.0/notebooks/admin_users.ipynb
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.6.0/notebooks/admin_users.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/COPYING.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/README.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/pyproject.toml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/config.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/launch.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/models.py
+-rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/lab/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/noauth/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/notebook/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/notebook/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/notebook/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/notebook/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/notebook/fps_notebook/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/notebook/fps_notebook/main.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/notebook/fps_notebook/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/terminals/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/webdav/COPYING.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/webdav/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/webdav/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/webdav/fps_webdav/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/webdav/fps_webdav/config.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/webdav/fps_webdav/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/webdav/fps_webdav/py.typed
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/webdav/fps_webdav/routes.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/webdav/tests/test_webdav.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/utils.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/ybasedoc.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/yblob.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/yfile.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/ynotebook.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/yunicode.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/awareness.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/websocket.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py
+-rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/yroom.py
+-rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/ystore.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/yutils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywidgets/__init__.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyverse-0.6.0/plugins/yjs/fps_yjs/ywidgets/widgets.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/test_app.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/test_contents.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/test_execute.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/test_kernels.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/test_server.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.6.0/tests/data/notebook1.ipynb
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse-0.6.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.6.0/COPYING.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyverse-0.6.0/README.md
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 jupyverse-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyverse-0.6.0/PKG-INFO
```

### Comparing `jupyverse-0.5.4/.pre-commit-config.yaml` & `jupyverse-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/CHANGELOG.md` & `jupyverse-0.6.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.6.0
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.5.4...74a20c5aba350ae2dac605ff303d4e75f72eff40))
+
+### Merged PRs
+
+- Fix terminals [#414](https://github.com/jupyter-server/jupyverse/pull/414) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2024-05-14&to=2024-05-22&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2024-05-14..2024-05-22&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.5.4
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.5.3...9f208a6e2e13396f6723a80e23bef688285611e5))
 
 ### Merged PRs
 
 - Improve terminals [#413](https://github.com/jupyter-server/jupyverse/pull/413) ([@davidbrochart](https://github.com/davidbrochart))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2024-05-13&to=2024-05-14&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2024-05-13..2024-05-14&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2024-05-13..2024-05-14&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.5.3
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.5.2...d5a5b178b93172a9bb8b90459d45ed20a1b734c5))
 
 ### Merged PRs
 
 - Remove asyncio reader when quitting terminal [#411](https://github.com/jupyter-server/jupyverse/pull/411) ([@davidbrochart](https://github.com/davidbrochart))
```

### Comparing `jupyverse-0.5.4/CONTRIBUTING.md` & `jupyverse-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/config.yaml` & `jupyverse-0.6.0/config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/mkdocs.yml` & `jupyverse-0.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/.devcontainer/devcontainer.json` & `jupyverse-0.6.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/.github/workflows/check-release.yml` & `jupyverse-0.6.0/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/.github/workflows/test.yml` & `jupyverse-0.6.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/binder/jupyter_notebook_config.py` & `jupyverse-0.6.0/binder/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/docs/index.md` & `jupyverse-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/docs/install.md` & `jupyverse-0.6.0/docs/install.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/docs/jupyter.svg` & `jupyverse-0.6.0/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/docs/plugins/auth.md` & `jupyverse-0.6.0/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/docs/tutorials/jupyterhub_jupyverse_deployment.md` & `jupyverse-0.6.0/docs/tutorials/jupyterhub_jupyverse_deployment.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/docs/tutorials/standalone_jupyverse_deployment.md` & `jupyverse-0.6.0/docs/tutorials/standalone_jupyverse_deployment.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/docs/usage/microservices.md` & `jupyverse-0.6.0/docs/usage/microservices.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/docs/usage/multi_user.md` & `jupyverse-0.6.0/docs/usage/multi_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/docs/usage/single_user.md` & `jupyverse-0.6.0/docs/usage/single_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/COPYING.md` & `jupyverse-0.6.0/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/pyproject.toml` & `jupyverse-0.6.0/jupyverse_api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 
 from pydantic import BaseModel
 
 from .app import App
 
-__version__ = "0.5.4"
+__version__ = "0.6.0"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/cli.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/contents/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/contents/models.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/jupyterlab/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/kernels/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/lab/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/nbconvert/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/notebook/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/resource_usage/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/terminals/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/terminals/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,9 +79,9 @@
 
 class TerminalServer(ABC):
     @abstractmethod
     async def serve(self, websocket, permissions):
         ...
 
     @abstractmethod
-    def quit(self, websocket):
+    async def exit(self):
         ...
```

### Comparing `jupyverse-0.5.4/jupyverse_api/jupyverse_api/yjs/__init__.py` & `jupyverse-0.6.0/jupyverse_api/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/notebooks/admin_users.ipynb` & `jupyverse-0.6.0/notebooks/admin_users.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/notebooks/admin_users.py` & `jupyverse-0.6.0/notebooks/admin_users.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth/COPYING.md` & `jupyverse-0.6.0/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth/pyproject.toml` & `jupyverse-0.6.0/plugins/auth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth/fps_auth/backends.py` & `jupyverse-0.6.0/plugins/auth/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth/fps_auth/config.py` & `jupyverse-0.6.0/plugins/auth/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth/fps_auth/db.py` & `jupyverse-0.6.0/plugins/auth/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth/fps_auth/main.py` & `jupyverse-0.6.0/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth/fps_auth/routes.py` & `jupyverse-0.6.0/plugins/auth/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_fief/COPYING.md` & `jupyverse-0.6.0/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_fief/pyproject.toml` & `jupyverse-0.6.0/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.6.0/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_fief/fps_auth_fief/config.py` & `jupyverse-0.6.0/plugins/auth_fief/fps_auth_fief/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.6.0/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.6.0/plugins/auth_fief/fps_auth_fief/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_jupyterhub/COPYING.md` & `jupyverse-0.6.0/plugins/auth_jupyterhub/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_jupyterhub/pyproject.toml` & `jupyverse-0.6.0/plugins/auth_jupyterhub/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py` & `jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py` & `jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py` & `jupyverse-0.6.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/contents/COPYING.md` & `jupyverse-0.6.0/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/contents/pyproject.toml` & `jupyverse-0.6.0/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.6.0/plugins/contents/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/contents/fps_contents/routes.py` & `jupyverse-0.6.0/plugins/contents/fps_contents/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/frontend/COPYING.md` & `jupyverse-0.6.0/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/frontend/pyproject.toml` & `jupyverse-0.6.0/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/jupyterlab/COPYING.md` & `jupyverse-0.6.0/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.6.0/plugins/jupyterlab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.6.0/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.6.0/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.6.0/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/COPYING.md` & `jupyverse-0.6.0/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/pyproject.toml` & `jupyverse-0.6.0/plugins/kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.6.0/plugins/kernels/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.6.0/plugins/kernels/fps_kernels/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.6.0/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/lab/COPYING.md` & `jupyverse-0.6.0/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/lab/pyproject.toml` & `jupyverse-0.6.0/plugins/lab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/lab/fps_lab/main.py` & `jupyverse-0.6.0/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/lab/fps_lab/routes.py` & `jupyverse-0.6.0/plugins/lab/fps_lab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/lab/fps_lab/static/favicon.ico` & `jupyverse-0.6.0/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/COPYING.md` & `jupyverse-0.6.0/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/pyproject.toml` & `jupyverse-0.6.0/plugins/login/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/routes.py` & `jupyverse-0.6.0/plugins/login/fps_login/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/index.html` & `jupyverse-0.6.0/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.6.0/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.6.0/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.6.0/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.6.0/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/nbconvert/COPYING.md` & `jupyverse-0.6.0/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/nbconvert/pyproject.toml` & `jupyverse-0.6.0/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.6.0/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/noauth/COPYING.md` & `jupyverse-0.6.0/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/noauth/pyproject.toml` & `jupyverse-0.6.0/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.6.0/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/notebook/COPYING.md` & `jupyverse-0.6.0/plugins/notebook/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/notebook/pyproject.toml` & `jupyverse-0.6.0/plugins/notebook/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/notebook/fps_notebook/main.py` & `jupyverse-0.6.0/plugins/notebook/fps_notebook/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/notebook/fps_notebook/routes.py` & `jupyverse-0.6.0/plugins/notebook/fps_notebook/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/resource_usage/COPYING.md` & `jupyverse-0.6.0/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/resource_usage/pyproject.toml` & `jupyverse-0.6.0/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.6.0/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.6.0/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/terminals/COPYING.md` & `jupyverse-0.6.0/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/terminals/pyproject.toml` & `jupyverse-0.6.0/plugins/terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.6.0/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/terminals/fps_terminals/routes.py` & `jupyverse-0.6.0/plugins/terminals/fps_terminals/routes.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,26 +41,20 @@
         return terminal
 
     async def delete_terminal(
         self,
         name: str,
         user: User,
     ):
-        for websocket in TERMINALS[name]["server"].websockets:
-            TERMINALS[name]["server"].quit(websocket)
-        del TERMINALS[name]
+        await TERMINALS[name]["server"].exit(TERMINALS, name)
         return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
     async def terminal_websocket(
         self,
         name,
         websocket_permissions,
     ):
         if websocket_permissions is None:
             return
         websocket, permissions = websocket_permissions
         await websocket.accept()
-        await TERMINALS[name]["server"].serve(websocket, permissions)
-        if name in TERMINALS:
-            TERMINALS[name]["server"].quit(websocket)
-            if not TERMINALS[name]["server"].websockets:
-                del TERMINALS[name]
+        await TERMINALS[name]["server"].serve(websocket, permissions, TERMINALS, name)
```

### Comparing `jupyverse-0.5.4/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.6.0/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/webdav/COPYING.md` & `jupyverse-0.6.0/plugins/webdav/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/webdav/pyproject.toml` & `jupyverse-0.6.0/plugins/webdav/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/webdav/fps_webdav/routes.py` & `jupyverse-0.6.0/plugins/webdav/fps_webdav/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/webdav/tests/test_webdav.py` & `jupyverse-0.6.0/plugins/webdav/tests/test_webdav.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/COPYING.md` & `jupyverse-0.6.0/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/pyproject.toml` & `jupyverse-0.6.0/plugins/yjs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/utils.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/ybasedoc.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/ybasedoc.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/yblob.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/yblob.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/ynotebook.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/ynotebook.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ydocs/yunicode.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ydocs/yunicode.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/awareness.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/awareness.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/websocket.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/websocket.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/yroom.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/yroom.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/ystore.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/ystore.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywebsocket/yutils.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywebsocket/yutils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/plugins/yjs/fps_yjs/ywidgets/widgets.py` & `jupyverse-0.6.0/plugins/yjs/fps_yjs/ywidgets/widgets.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/conftest.py` & `jupyverse-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/test_app.py` & `jupyverse-0.6.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/test_auth.py` & `jupyverse-0.6.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/test_contents.py` & `jupyverse-0.6.0/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/test_execute.py` & `jupyverse-0.6.0/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/test_kernels.py` & `jupyverse-0.6.0/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/test_server.py` & `jupyverse-0.6.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/test_settings.py` & `jupyverse-0.6.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/utils.py` & `jupyverse-0.6.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/data/notebook0.ipynb` & `jupyverse-0.6.0/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/tests/data/notebook1.ipynb` & `jupyverse-0.6.0/tests/data/notebook1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/.gitignore` & `jupyverse-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/COPYING.md` & `jupyverse-0.6.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/README.md` & `jupyverse-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/pyproject.toml` & `jupyverse-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.4/PKG-INFO` & `jupyverse-0.6.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyverse
-Version: 0.5.4
+Version: 0.6.0
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

