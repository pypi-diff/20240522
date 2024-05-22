# Comparing `tmp/PyFusion-1.1.0.dev1.tar.gz` & `tmp/pyfusion-1.1.0.dev3.tar.gz`

## Comparing `PyFusion-1.1.0.dev1.tar` & `pyfusion-1.1.0.dev3.tar`

### file list

```diff
@@ -1,43 +1,47 @@
--rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 PyFusion-1.1.0.dev1/Cargo.toml
--rw-r--r--   0     1001      127      326 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0     1001      127     9838 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.github/workflows/dev.yml
--rw-r--r--   0     1001      127     4939 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1328 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.gitignore
--rw-r--r--   0     1001      127      668 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      235 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/BUILD.md
--rw-r--r--   0     1001      127     2559 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/CHANGELOG.md
--rw-r--r--   0     1001      127      575 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/LICENSE
--rw-r--r--   0     1001      127     1386 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/README.md
--rw-r--r--   0     1001      127       35 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/api.md
--rw-r--r--   0     1001      127       43 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/changelog.md
--rw-r--r--   0     1001      127     3532 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/contributing.md
--rw-r--r--   0     1001      127    86597 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/get_started.ipynb
--rw-r--r--   0     1001      127       42 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/index.md
--rw-r--r--   0     1001      127      930 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/installation.md
--rw-r--r--   0     1001      127      106 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/usage.md
--rw-r--r--   0     1001      127      373 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/__init__.py
--rw-r--r--   0     1001      127     1597 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/__main__.py
--rw-r--r--   0     1001      127    25755 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/authentication.py
--rw-r--r--   0     1001      127      910 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/exceptions.py
--rw-r--r--   0     1001      127    13730 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/fs_sync.py
--rw-r--r--   0     1001      127    53307 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/fusion.py
--rw-r--r--   0     1001      127    24428 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/fusion_filesystem.py
--rw-r--r--   0     1001      127        0 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/test_fusion_filesystem.py
--rw-r--r--   0     1001      127      163 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/types.py
--rw-r--r--   0     1001      127    35946 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/utils.py
--rw-r--r--   0     1001      127      473 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/makefile
--rw-r--r--   0     1001      127     1783 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/mkdocs.yml
--rw-r--r--   0     1001      127       36 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/__init__.py
--rw-r--r--   0     1001      127     5857 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/conftest.py
--rw-r--r--   0     1001      127    25811 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_authentication.py
--rw-r--r--   0     1001      127     4258 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_filesystem.py
--rw-r--r--   0     1001      127      525 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_fsync.py
--rw-r--r--   0     1001      127    28808 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_fusion.py
--rw-r--r--   0     1001      127    38800 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_utils.py
--rw-r--r--   0     1001      127    16095 2024-05-14 19:28:45.000000 PyFusion-1.1.0.dev1/requirements-dev.lock
--rw-r--r--   0     1001      127    12643 2024-05-14 19:28:37.000000 PyFusion-1.1.0.dev1/requirements.lock
--rw-r--r--   0     1001      127     1042 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/src/lib.rs
--rw-r--r--   0     1001      127     1201 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/tox.ini
--rw-r--r--   0     1001      127     8095 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/Cargo.lock
--rw-r--r--   0     1001      127     5677 2024-05-14 19:28:21.000000 PyFusion-1.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     3450 1970-01-01 00:00:00.000000 PyFusion-1.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 pyfusion-1.1.0.dev3/Cargo.toml
+-rw-r--r--   0     1001      127      326 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0     1001      127    20251 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/.github/workflows/dev.yml
+-rw-r--r--   0     1001      127     5098 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1328 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/.gitignore
+-rw-r--r--   0     1001      127      668 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      235 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/BUILD.md
+-rw-r--r--   0     1001      127     2616 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/CHANGELOG.md
+-rw-r--r--   0     1001      127      575 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/LICENSE
+-rw-r--r--   0     1001      127     1386 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/README.md
+-rw-r--r--   0     1001      127       35 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/docs/api.md
+-rw-r--r--   0     1001      127       43 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/docs/changelog.md
+-rw-r--r--   0     1001      127     3532 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/docs/contributing.md
+-rw-r--r--   0     1001      127    86597 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/docs/get_started.ipynb
+-rw-r--r--   0     1001      127       42 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/docs/index.md
+-rw-r--r--   0     1001      127      930 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/docs/installation.md
+-rw-r--r--   0     1001      127      106 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/docs/usage.md
+-rw-r--r--   0     1001      127      373 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/__init__.py
+-rw-r--r--   0     1001      127     1597 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/__main__.py
+-rw-r--r--   0     1001      127    26995 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/authentication.py
+-rw-r--r--   0     1001      127      910 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/exceptions.py
+-rw-r--r--   0     1001      127    13730 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/fs_sync.py
+-rw-r--r--   0     1001      127    53307 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/fusion.py
+-rw-r--r--   0     1001      127    24428 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/fusion_filesystem.py
+-rw-r--r--   0     1001      127        0 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/test_fusion_filesystem.py
+-rw-r--r--   0     1001      127      163 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/types.py
+-rw-r--r--   0     1001      127    35946 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/fusion/utils.py
+-rw-r--r--   0     1001      127      473 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/makefile
+-rw-r--r--   0     1001      127     1783 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/mkdocs.yml
+-rw-r--r--   0     1001      127       37 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_integ/__init__.py
+-rw-r--r--   0     1001      127      583 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_integ/conftest.py
+-rw-r--r--   0     1001      127      111 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_integ/pytest.ini
+-rw-r--r--   0     1001      127     2304 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_integ/test_integ.py
+-rw-r--r--   0     1001      127       36 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_tests/__init__.py
+-rw-r--r--   0     1001      127     6849 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_tests/conftest.py
+-rw-r--r--   0     1001      127    27171 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_tests/test_authentication.py
+-rw-r--r--   0     1001      127     4258 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_tests/test_filesystem.py
+-rw-r--r--   0     1001      127      525 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_tests/test_fsync.py
+-rw-r--r--   0     1001      127    28808 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_tests/test_fusion.py
+-rw-r--r--   0     1001      127    38800 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/py_tests/test_utils.py
+-rw-r--r--   0     1001      127    15819 2024-05-22 12:05:10.000000 pyfusion-1.1.0.dev3/requirements-dev.lock
+-rw-r--r--   0     1001      127    12403 2024-05-22 12:05:03.000000 pyfusion-1.1.0.dev3/requirements.lock
+-rw-r--r--   0     1001      127     1042 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/src/lib.rs
+-rw-r--r--   0     1001      127     1337 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/tox.ini
+-rw-r--r--   0     1001      127     8095 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/Cargo.lock
+-rw-r--r--   0     1001      127     5430 2024-05-22 12:02:49.000000 pyfusion-1.1.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     3450 1970-01-01 00:00:00.000000 pyfusion-1.1.0.dev3/PKG-INFO
```

### Comparing `PyFusion-1.1.0.dev1/.github/workflows/release.yml` & `pyfusion-1.1.0.dev3/.github/workflows/release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,35 @@
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 permissions:
   contents: write
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 env:
   UV_HTTP_TIMEOUT: 300
   PIP_DISABLE_PIP_VERSION_CHECK: 1
+  DOCS_PY_VERSION: 3.12
+
 
 jobs:
   check-build:
     runs-on: ubuntu-latest
     outputs:
       build-successful: ${{ steps.check-build-success.outputs.successful }}
       run_id: ${{ steps.check-build-success.outputs.run_id }}
 
     steps:
       - name: Check latest build status
         id: check-build-success
-        uses: actions/github-script@v6
+        uses: actions/github-script@v7
         with:
           script: |
             const { owner, repo } = context.repo;
             const tagSha = context.sha;
             console.log('current run sha = ' + tagSha)
             dev_workflow = 'dev.yml'
             const runs = await github.rest.actions.listWorkflowRuns({
@@ -44,15 +50,15 @@
               head_sha: tagSha
             });
 
             const successfulRun = runs.data.workflow_runs.find(run => run.head_sha === tagSha);
             if (successfulRun) {
               core.setOutput('successful', 'true');
               core.setOutput('run_id', successfulRun.id);
-              console.log('Found Successful build run #' + successfulRun.run_number + ', run_id=' + successfulRun.id + ', it was started at' + successfulRun.created_at)
+              console.log('Found Successful build run #' + successfulRun.run_number + ', run_id=' + successfulRun.id + ', it was started at ' + successfulRun.created_at)
 
             } else {
               core.setOutput('successful', 'false');
               core.setFailed('No successful build for this commit/tag');
             }
 
   publish:
@@ -79,15 +85,15 @@
       uses: mindsers/changelog-reader-action@v2
       with:
         version: ${{ steps.tag_name.outputs.current_version }}
         path: CHANGELOG.md
 
     - uses: actions/setup-python@v5
       with:
-        python-version: '3.12'
+        python-version: ${{ env.DOCS_PY_VERSION }}
 
     - name: Set up rye
       run: curl -sSf https://rye-up.com/get | RYE_INSTALL_OPTION="--yes" bash
 
     - name: Add Rye to PATH
       run: |
         echo "$HOME/.rye/env" >> $GITHUB_PATH
@@ -99,15 +105,15 @@
 
     - name: Verify Rye Installation
       run: rye --version
       shell: bash
 
     - name: Sync dependencies using rye
       run: |
-        rye pin 3.12
+        rye pin ${{ env.DOCS_PY_VERSION }}
         rye sync --all-features
 
     - name: Setup main repo deploy git user
       run: |
         git config --local user.email "github-actions[bot]@users.noreply.github.com"
         git config --local user.name "github-actions[bot]"
```

### Comparing `PyFusion-1.1.0.dev1/.gitignore` & `pyfusion-1.1.0.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/.pre-commit-config.yaml` & `pyfusion-1.1.0.dev3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/CHANGELOG.md` & `pyfusion-1.1.0.dev3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.1.0-dev3] - 2024-05-22
+
+* Internal build updates
+
+
 ## [1.1.0-dev1] - 2024-05-14
 
 * Internal build updates
 
 
 ## [1.0.23] - 2024-04-12
```

### Comparing `PyFusion-1.1.0.dev1/LICENSE` & `pyfusion-1.1.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/README.md` & `pyfusion-1.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/docs/contributing.md` & `pyfusion-1.1.0.dev3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/docs/get_started.ipynb` & `pyfusion-1.1.0.dev3/docs/get_started.ipynb`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/docs/installation.md` & `pyfusion-1.1.0.dev3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/fusion/__main__.py` & `pyfusion-1.1.0.dev3/fusion/__main__.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/fusion/authentication.py` & `pyfusion-1.1.0.dev3/fusion/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,49 @@
 from . import __version__ as version
 from .exceptions import CredentialError
 
 logger = logging.getLogger(__name__)
 VERBOSE_LVL = 25
 
 
+def try_get_env_var(var_name: str, default: Optional[str] = None) -> Optional[str]:
+    """Get the value of an environment variable or return a default value.
+
+    Args:
+        var_name (str): The name of the environment variable.
+        default (str, optional): The default value to return if the environment variable is not set. Defaults to None.
+
+    Returns:
+        Optional[str]: The value of the environment variable or the default value.
+    """
+    return os.environ.get(var_name, default)
+
+
+def try_get_client_id(client_id: Optional[str]) -> Optional[str]:
+    """Get the client ID from the environment variable or return None.
+
+    Returns:
+        Optional[str]: The client ID or None.
+    """
+    if client_id:
+        return client_id
+    return try_get_env_var("FUSION_CLIENT_ID")
+
+
+def try_get_client_secret(client_secret: Optional[str]) -> Optional[str]:
+    """Get the client secret from the environment variable or return None.
+
+    Returns:
+        Optional[str]: The client secret or None.
+    """
+    if client_secret:
+        return client_secret
+    return try_get_env_var("FUSION_CLIENT_SECRET")
+
+
 def _res_plural(ref_int: int, pluraliser: str = "s") -> str:
     """Private function to return the plural form when the number is more than one.
 
     Args:
         ref_int (int): The reference integer that determines whether to return a plural suffix.
         pluraliser (str, optional): The plural suffix. Defaults to "s".
 
@@ -119,16 +154,16 @@
             is_bearer_token_expirable (bool, optional): Is bearer token expirable. Defaults to None.
             proxies (dict, optional): Any proxy servers required to route HTTP and HTTPS requests to the internet.
             grant_type (str, optional): Allows the grant type to be changed to support different credential types.
                 Defaults to client_credentials.
         """
         if proxies is None:
             proxies = {}
-        self.client_id = client_id
-        self.client_secret = client_secret
+        self.client_id = try_get_client_id(client_id)
+        self.client_secret = try_get_client_secret(client_secret)
         self.username = username
         self.password = password
         self.resource = resource
         self.auth_url = auth_url
         self.proxies = proxies
         self.grant_type = grant_type
         self.bearer_token = bearer_token
@@ -271,16 +306,16 @@
         """
         if not credentials or not isinstance(credentials, dict):
             raise CredentialError("A valid credentials dictionary is required")
 
         grant_type = credentials.get("grant_type", "client_credentials")
         try:
             if grant_type == "client_credentials":
-                client_id = credentials["client_id"]
-                client_secret = credentials["client_secret"]
+                client_id = try_get_client_id(credentials.get("client_id"))
+                client_secret = try_get_client_secret(credentials.get("client_secret"))
                 username = None
                 password = None
                 bearer_token = None
                 bearer_token_expiry = datetime.now(tz=timezone.utc)
                 is_bearer_token_expirable = True
                 resource = credentials["resource"]
                 auth_url = credentials["auth_url"]
@@ -299,15 +334,15 @@
                 if isinstance(bearer_token_expirable, str):
                     bearer_token_expirable = bearer_token_expirable.lower()
 
                 is_bearer_token_expirable = bearer_token_expirable not in ["false"] if bearer_token_expirable else True
                 resource = None
                 auth_url = None
             elif grant_type == "password":
-                client_id = credentials["client_id"]
+                client_id = try_get_client_id(credentials.get("client_id"))
                 client_secret = None
                 username = credentials["username"]
                 password = credentials["password"]
                 bearer_token = None
                 bearer_token_expiry = datetime.now(tz=timezone.utc)
                 is_bearer_token_expirable = True
                 resource = credentials["resource"]
```

### Comparing `PyFusion-1.1.0.dev1/fusion/exceptions.py` & `pyfusion-1.1.0.dev3/fusion/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/fusion/fs_sync.py` & `pyfusion-1.1.0.dev3/fusion/fs_sync.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/fusion/fusion.py` & `pyfusion-1.1.0.dev3/fusion/fusion.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/fusion/fusion_filesystem.py` & `pyfusion-1.1.0.dev3/fusion/fusion_filesystem.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/fusion/utils.py` & `pyfusion-1.1.0.dev3/fusion/utils.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/mkdocs.yml` & `pyfusion-1.1.0.dev3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/py_tests/conftest.py` & `pyfusion-1.1.0.dev3/py_tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -87,14 +87,33 @@
             "http": "http://myproxy.com:8080",
             "https": "http://myproxy.com:8081",
         },
     }
 
 
 @pytest.fixture()
+def example_creds_dict_from_env(
+    monkeypatch: pytest.MonkeyPatch, example_client_id: str, example_client_secret: str
+) -> dict[str, Any]:
+    # Mocked creds info
+
+    monkeypatch.setenv("FUSION_CLIENT_ID", example_client_id)
+    monkeypatch.setenv("FUSION_CLIENT_SECRET", example_client_secret)
+
+    return {
+        "resource": "JPMC:URI:RS-97834-Fusion-PROD",
+        "auth_url": "https://authe.mysite.com/as/token.oauth2",
+        "proxies": {
+            "http": "http://myproxy.com:8080",
+            "https": "http://myproxy.com:8081",
+        },
+    }
+
+
+@pytest.fixture()
 def example_creds_dict_https_pxy(example_client_id: str, example_client_secret: str) -> dict[str, Any]:
     # Mocked creds info
     return {
         "client_id": example_client_id,
         "client_secret": example_client_secret,
         "resource": "JPMC:URI:RS-97834-Fusion-PROD",
         "auth_url": "https://authe.mysite.com/as/token.oauth2",
@@ -113,14 +132,28 @@
 @pytest.fixture()
 def example_creds_dict_empty_pxy(example_creds_dict: dict[str, Any]) -> dict[str, Any]:
     example_creds_dict["proxies"].pop("http")
     example_creds_dict["proxies"].pop("https")
     return example_creds_dict
 
 
+@pytest.fixture(
+    params=[
+        "example_creds_dict",
+        "example_creds_dict_from_env",
+        "example_creds_dict_https_pxy",
+        "example_creds_dict_no_pxy",
+        "example_creds_dict_empty_pxy",
+    ]
+)
+def creds_dict(request: pytest.FixtureRequest) -> Any:
+    """Parameterized fixture to return credentials from different sources."""
+    return request.getfixturevalue(request.param)
+
+
 @pytest.fixture()
 def good_json() -> str:
     return """{
         "client_id": "vf3tdjK0jdp7MdY3",
         "client_secret": "vswag2iet7Merdkdwe64YcI9gxbemjMsh5jgimrwpcghsqc2mnj4w4qQffrfhtKz0ba3u48tqJrbp1y",
         "resource": "JPMC:URI:RS-97834-Fusion-PROD",
         "auth_url": "https://authe.mysite.com/as/token.oauth2",
```

### Comparing `PyFusion-1.1.0.dev1/py_tests/test_authentication.py` & `pyfusion-1.1.0.dev3/py_tests/test_authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from freezegun import freeze_time
 
 from fusion.authentication import (
     FusionAiohttpSession,
     FusionCredentials,
     FusionOAuthAdapter,
     get_default_fs,
+    try_get_client_id,
+    try_get_client_secret,
 )
 from fusion.exceptions import CredentialError
 from fusion.fusion import Fusion
 from fusion.utils import distribution_to_url
 
 from .conftest import change_dir
 
@@ -497,17 +499,17 @@
         fusion_oauth_adapter._refresh_token_data()
 
 
 def test_refresh_fusion_token_data(
     fusion_oauth_adapter: FusionOAuthAdapter,
     fusion_oauth_adapter_from_obj: FusionOAuthAdapter,
     requests_mock: requests_mock.Mocker,
-    example_creds_dict: dict[str, Any],
+    creds_dict: dict[str, Any],
 ) -> None:
-    creds = FusionCredentials.from_dict(example_creds_dict)
+    creds = FusionCredentials.from_dict(creds_dict)
     fusion_obj = Fusion(credentials=creds)
     catalog = "my_catalog"
     dataset = "my_dataset"
     datasetseries = "2020-04-04"
     file_format = "csv"
     url = distribution_to_url(fusion_obj.root_url, catalog, dataset, datasetseries, file_format)
     token_auth_url = f"{fusion_obj.root_url}catalogs/csv/datasets/{catalog}/authorize/token"
@@ -525,17 +527,17 @@
     )
     fusion_oauth_adapter_from_obj._refresh_fusion_token_data(prep_req)
 
 
 def test_refresh_fusion_token_data_refresh(
     fusion_oauth_adapter: FusionOAuthAdapter,
     requests_mock: requests_mock.Mocker,
-    example_creds_dict: dict[str, Any],
+    creds_dict: dict[str, Any],
 ) -> None:
-    creds = FusionCredentials.from_dict(example_creds_dict)
+    creds = FusionCredentials.from_dict(creds_dict)
     fusion_obj = Fusion(credentials=creds)
     catalog = "my_catalog"
     dataset = "my_dataset"
     datasetseries = "2020-04-04"
     file_format = "csv"
     fusion_token_key = catalog + "_" + dataset
     fusion_oauth_adapter.fusion_token_dict[fusion_token_key] = "prev_token"
@@ -556,17 +558,17 @@
 
     fusion_oauth_adapter.send(prep_req)
 
 
 def test_fusion_oauth_adapter_send(
     fusion_oauth_adapter: FusionOAuthAdapter,
     requests_mock: requests_mock.Mocker,
-    example_creds_dict: dict[str, Any],
+    creds_dict: dict[str, Any],
 ) -> None:
-    creds = FusionCredentials.from_dict(example_creds_dict)
+    creds = FusionCredentials.from_dict(creds_dict)
     fusion_obj = Fusion(credentials=creds)
     catalog = "my_catalog"
     dataset = "my_dataset"
     datasetseries = "2020-04-04"
     file_format = "csv"
     fusion_token_key = catalog + "_" + dataset
 
@@ -713,7 +715,41 @@
 
 def test_async_session() -> None:
     session = FusionAiohttpSession()
     assert session
 
     session.post_init()
     assert session
+
+
+@pytest.mark.parametrize(
+    ("client_id", "expected", "env_var_value"),
+    [
+        (None, "12345", "12345"),  # Test fetching from environment variable
+        ("abcde", "abcde", "12345"),  # Test returning provided client_id
+        (None, None, None),  # Test with no environment variable set
+    ],
+)
+def test_try_get_client_id(monkeypatch: pytest.MonkeyPatch, client_id: str, expected: str, env_var_value: str) -> None:
+    if env_var_value is not None:
+        monkeypatch.setenv("FUSION_CLIENT_ID", env_var_value)
+    else:
+        monkeypatch.delenv("FUSION_CLIENT_ID", raising=False)
+    assert try_get_client_id(client_id) == expected
+
+
+@pytest.mark.parametrize(
+    ("client_secret", "expected", "env_var_value"),
+    [
+        (None, "secret123", "secret123"),  # Test fetching from environment variable
+        ("mysecret", "mysecret", "secret123"),  # Test returning provided client_secret
+        (None, None, None),  # Test with no environment variable set
+    ],
+)
+def test_try_get_client_secret(
+    monkeypatch: pytest.MonkeyPatch, client_secret: str, expected: str, env_var_value: str
+) -> None:
+    if env_var_value is not None:
+        monkeypatch.setenv("FUSION_CLIENT_SECRET", env_var_value)
+    else:
+        monkeypatch.delenv("FUSION_CLIENT_SECRET", raising=False)
+    assert try_get_client_secret(client_secret) == expected
```

### Comparing `PyFusion-1.1.0.dev1/py_tests/test_filesystem.py` & `pyfusion-1.1.0.dev3/py_tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/py_tests/test_fsync.py` & `pyfusion-1.1.0.dev3/py_tests/test_fsync.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/py_tests/test_fusion.py` & `pyfusion-1.1.0.dev3/py_tests/test_fusion.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/py_tests/test_utils.py` & `pyfusion-1.1.0.dev3/py_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/requirements-dev.lock` & `pyfusion-1.1.0.dev3/requirements-dev.lock`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # use `rye lock` or `rye sync` to update this lockfile
 #
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: true
 #   with-sources: false
+#   generate-hashes: false
 
 -e file:.
 adlfs==2024.4.1
     # via pyfusion
 aiobotocore==2.12.3
     # via s3fs
 aiohttp==3.9.5
@@ -38,16 +39,14 @@
     # via notebook
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 asttokens==2.4.1
     # via stack-data
-astunparse==1.6.3
-    # via griffe
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via aiohttp
     # via aiohttp-sse-client
     # via jsonschema
     # via referencing
@@ -60,16 +59,14 @@
     # via adlfs
 azure-identity==1.16.0
     # via adlfs
 azure-storage-blob==12.19.1
     # via adlfs
 babel==2.14.0
     # via mkdocs-material
-backcall==0.2.0
-    # via ipython
 backports-tarfile==1.1.1
     # via jaraco-context
 beautifulsoup4==4.12.3
     # via nbconvert
 bleach==6.1.0
     # via nbconvert
 boto3==1.34.69
@@ -120,21 +117,22 @@
 decorator==5.1.1
     # via gcsfs
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
 distlib==0.3.8
     # via virtualenv
-docutils==0.20.1
+docutils==0.21.2
     # via pyfusion
     # via readme-renderer
 entrypoints==0.4
     # via jupyter-client
 exceptiongroup==1.2.1
     # via anyio
+    # via ipython
     # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
 filelock==3.13.4
     # via tox
@@ -193,25 +191,22 @@
     # via mike
     # via mkdocs
     # via mkdocs-get-deps
     # via mkdocstrings
     # via nbconvert
     # via twine
 importlib-resources==6.4.0
-    # via jsonschema
-    # via jsonschema-specifications
-    # via keyring
     # via mike
 iniconfig==2.0.0
     # via pytest
 ipykernel==6.29.4
     # via mkdocs-jupyter
     # via nbclassic
     # via notebook
-ipython==8.12.3
+ipython==8.18.1
     # via ipykernel
 ipython-genutils==0.2.0
     # via jupyter-contrib-nbextensions
     # via nbclassic
     # via notebook
 isodate==0.6.1
     # via azure-storage-blob
@@ -399,16 +394,17 @@
 notebook==6.5.7
     # via jupyter-contrib-core
     # via jupyter-contrib-nbextensions
     # via jupyter-nbextensions-configurator
     # via pyfusion
 notebook-shim==0.2.4
     # via nbclassic
-numpy==1.24.4
+numpy==1.26.4
     # via pandas
+    # via pandas-stubs
     # via pyarrow
 oauthlib==3.2.2
     # via requests-oauthlib
 overrides==7.7.0
     # via jupyter-server
 packaging==24.0
     # via auditwheel
@@ -420,33 +416,29 @@
     # via nbconvert
     # via pyproject-api
     # via pytest
     # via tox
     # via tox-uv
 paginate==0.5.6
     # via mkdocs-material
-pandas==2.0.3
+pandas==2.2.2
     # via pyfusion
-pandas-stubs==2.0.3.230814
+pandas-stubs==2.2.1.240316
 pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.4
     # via jedi
 patchelf==0.17.2.1
 pathspec==0.12.1
     # via mkdocs
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
 pip==24.0
 pkginfo==1.10.0
     # via twine
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 platformdirs==4.2.1
     # via jupyter-core
     # via mkdocs-get-deps
     # via mkdocstrings
     # via tox
     # via virtualenv
 pluggy==1.5.0
@@ -533,15 +525,14 @@
     # via moto
     # via pandas
 python-dotenv==1.0.1
     # via pydantic-settings
 python-json-logger==2.0.7
     # via jupyter-events
 pytz==2024.1
-    # via babel
     # via pandas
 pyyaml==6.0.1
     # via jupyter-events
     # via jupyter-nbextensions-configurator
     # via jupytext
     # via mike
     # via mkdocs
@@ -621,15 +612,14 @@
     # via jupyter-server
     # via nbclassic
     # via notebook
 setuptools==69.5.1
     # via jupyter-contrib-core
 six==1.16.0
     # via asttokens
-    # via astunparse
     # via azure-core
     # via bleach
     # via isodate
     # via python-dateutil
     # via rfc3339-validator
     # via sseclient
 smmap==5.0.1
@@ -704,24 +694,22 @@
 types-requests==2.31.0.6
 types-tabulate==0.9.0.20240106
 types-tqdm==4.66.0.20240417
 types-urllib3==1.26.25.14
     # via types-requests
 typing-extensions==4.11.0
     # via aioitertools
-    # via annotated-types
     # via anyio
     # via azure-core
     # via azure-storage-blob
     # via ipython
     # via mkdocstrings
     # via mypy
     # via pydantic
     # via pydantic-core
-    # via rich
     # via rich-click
 tzdata==2024.1
     # via pandas
 uri-template==1.3.0
     # via jsonschema
 urllib3==1.26.18
     # via botocore
@@ -746,16 +734,14 @@
 webencodings==0.5.1
     # via bleach
     # via tinycss2
 websocket-client==1.8.0
     # via jupyter-server
 werkzeug==3.0.2
     # via moto
-wheel==0.43.0
-    # via astunparse
 wrapt==1.16.0
     # via aiobotocore
 xmltodict==0.13.0
     # via moto
 yarl==1.9.4
     # via aiohttp
     # via aiohttp-sse-client
```

### Comparing `PyFusion-1.1.0.dev1/requirements.lock` & `pyfusion-1.1.0.dev3/requirements.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # use `rye lock` or `rye sync` to update this lockfile
 #
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: true
 #   with-sources: false
+#   generate-hashes: false
 
 -e file:.
 adlfs==2024.4.1
     # via pyfusion
 aiobotocore==2.12.3
     # via s3fs
 aiohttp==3.9.5
@@ -33,16 +34,14 @@
     # via notebook
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 asttokens==2.4.1
     # via stack-data
-astunparse==1.6.3
-    # via griffe
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via aiohttp
     # via aiohttp-sse-client
     # via jsonschema
     # via referencing
@@ -54,16 +53,14 @@
     # via adlfs
 azure-identity==1.16.0
     # via adlfs
 azure-storage-blob==12.19.1
     # via adlfs
 babel==2.14.0
     # via mkdocs-material
-backcall==0.2.0
-    # via ipython
 beautifulsoup4==4.12.3
     # via nbconvert
 bleach==6.1.0
     # via nbconvert
 botocore==1.34.69
     # via aiobotocore
 bracex==2.4
@@ -94,20 +91,21 @@
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via gcsfs
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
-docutils==0.20.1
+docutils==0.21.2
     # via pyfusion
 entrypoints==0.4
     # via jupyter-client
 exceptiongroup==1.2.1
     # via anyio
+    # via ipython
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
 fqdn==1.5.1
     # via jsonschema
 frozenlist==1.4.1
@@ -159,22 +157,20 @@
     # via markdown
     # via mike
     # via mkdocs
     # via mkdocs-get-deps
     # via mkdocstrings
     # via nbconvert
 importlib-resources==6.4.0
-    # via jsonschema
-    # via jsonschema-specifications
     # via mike
 ipykernel==6.29.4
     # via mkdocs-jupyter
     # via nbclassic
     # via notebook
-ipython==8.12.3
+ipython==8.18.1
     # via ipykernel
 ipython-genutils==0.2.0
     # via jupyter-contrib-nbextensions
     # via nbclassic
     # via notebook
 isodate==0.6.1
     # via azure-storage-blob
@@ -337,15 +333,15 @@
 notebook==6.5.6
     # via jupyter-contrib-core
     # via jupyter-contrib-nbextensions
     # via jupyter-nbextensions-configurator
     # via pyfusion
 notebook-shim==0.2.4
     # via nbclassic
-numpy==1.24.4
+numpy==1.26.4
     # via pandas
     # via pyarrow
 oauthlib==3.2.2
     # via requests-oauthlib
 overrides==7.7.0
     # via jupyter-server
 packaging==24.0
@@ -353,28 +349,24 @@
     # via jupyter-server
     # via jupytext
     # via mkdocs
     # via msal-extensions
     # via nbconvert
 paginate==0.5.6
     # via mkdocs-material
-pandas==2.0.3
+pandas==2.2.2
     # via pyfusion
 pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.4
     # via jedi
 pathspec==0.12.1
     # via mkdocs
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 platformdirs==4.2.1
     # via jupyter-core
     # via mkdocs-get-deps
     # via mkdocstrings
 polars==0.20.22
     # via pyfusion
 portalocker==2.8.2
@@ -424,15 +416,14 @@
     # via botocore
     # via ghp-import
     # via jupyter-client
     # via pandas
 python-json-logger==2.0.7
     # via jupyter-events
 pytz==2024.1
-    # via babel
     # via pandas
 pyyaml==6.0.1
     # via jupyter-events
     # via jupyter-nbextensions-configurator
     # via jupytext
     # via mike
     # via mkdocs
@@ -483,15 +474,14 @@
     # via jupyter-server
     # via nbclassic
     # via notebook
 setuptools==69.5.1
     # via jupyter-contrib-core
 six==1.16.0
     # via asttokens
-    # via astunparse
     # via azure-core
     # via bleach
     # via isodate
     # via python-dateutil
     # via rfc3339-validator
     # via sseclient
 smmap==5.0.1
@@ -571,16 +561,14 @@
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via bleach
     # via tinycss2
 websocket-client==1.8.0
     # via jupyter-server
-wheel==0.43.0
-    # via astunparse
 wrapt==1.16.0
     # via aiobotocore
 yarl==1.9.4
     # via aiohttp
     # via aiohttp-sse-client
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `PyFusion-1.1.0.dev1/src/lib.rs` & `pyfusion-1.1.0.dev3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `PyFusion-1.1.0.dev1/tox.ini` & `pyfusion-1.1.0.dev3/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -43,8 +43,13 @@
 
 [testenv:build]
 allowlist_externals = rye
 
 commands =
     rye sync
     rye build
-    rye run twine check dist/*
+    rye run twine check dist/*
+
+[testenv:clean]
+allowlist_externals = rm # for cleanup
+commands =
+    rm -rf {toxinidir}/dist {toxinidir}/target {toxinidir}/downloads
```

### Comparing `PyFusion-1.1.0.dev1/Cargo.lock` & `pyfusion-1.1.0.dev3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "PyFusion"
-version = "1.1.0-dev1"
-dependencies = [
- "pyo3",
-]
-
-[[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
@@ -105,14 +98,21 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "pyfusion"
+version = "1.1.0-dev3"
+dependencies = [
+ "pyo3",
+]
+
+[[package]]
 name = "pyo3"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
```

### Comparing `PyFusion-1.1.0.dev1/pyproject.toml` & `pyfusion-1.1.0.dev3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "PyFusion"
-version = "1.1.0-dev1"
+name = "pyfusion"
+version = "1.1.0-dev3"
 
 homepage = "https://github.com/jpmorganchase/fusion"
 description = "JPMC Fusion Developer Tools"
 authors = [
     { name = "FusionDevs", email = "fusion_developers@jpmorgan.com" }
 ]
 readme = "README.md"
@@ -20,15 +20,15 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
     'Typing :: Typed',
 ]
 
-requires-python = ">= 3.8"
+requires-python = ">= 3.9"
 
 dependencies = [
     "requests >= 2",
     "pandas >= 1.1",
     "joblib >= 1.1",
     "tabulate >= 0.8",
     "tqdm >= 4",
@@ -203,45 +203,40 @@
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
 report.fail_under = 60
 run.parallel = true
 
 [tool.bumpversion]
-current_version = "1.1.0-dev1-dev1"
-parse = """(?x)
-    (?P<major>0|[1-9]\\d*)\\.
-    (?P<minor>0|[1-9]\\d*)\\.
-    (?P<patch>0|[1-9]\\d*)
-    (?:
-        -                             # dash separator for pre-release section
-        (?P<pre_l>[a-zA-Z-]+)         # pre-release label
-        (?P<pre_n>0|[1-9]\\d*)        # pre-release version number
-    )?                                # pre-release section is optional
-"""
+current_version = "1.1.0-dev3"
+parse = '(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[a-z]+)(?P<candidate>\d+))?'
 serialize = [
-    "{major}.{minor}.{patch}-{pre_l}{pre_n}",
-    "{major}.{minor}.{patch}",
+    '{major}.{minor}.{patch}-{release}{candidate}',
+	'{major}.{minor}.{patch}'
 ]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = false
 sign_tags = false
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 commit = false
 message = "Bump version: {current_version} → {new_version}"
 commit_args = ""
 
-[tool.bumpversion.parts.pre_l]
-values = ["dev"]
-optional_value = "dev"
+[tool.bumpversion.parts.release]
+first_value = 'dev'
+optional_value = 'release'
+values = [
+    'dev',
+    'release'
+]
 
 [[tool.bumpversion.files]]
 filename = "Cargo.toml"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
```

### Comparing `PyFusion-1.1.0.dev1/PKG-INFO` & `pyfusion-1.1.0.dev3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
-Name: PyFusion
-Version: 1.1.0.dev1
+Name: pyfusion
+Version: 1.1.0.dev3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -45,15 +45,15 @@
 Provides-Extra: azr
 Provides-Extra: polars
 Provides-Extra: events
 License-File: LICENSE
 Summary: JPMC Fusion Developer Tools
 Author-email: FusionDevs <fusion_developers@jpmorgan.com>
 License: Apache-2.0
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI version](https://badge.fury.io/py/PyFusion.svg)](https://badge.fury.io/py/PyFusion)
 [![Python Versions](https://img.shields.io/pypi/pyversions/PyFusion)](https://pypi.org/project/PyFusion/)
 [![dev workflow](https://github.com/jpmorganchase/fusion/actions/workflows/dev.yml/badge.svg?branch=master)](https://github.com/jpmorganchase/fusion/actions/workflows/dev.yml)
 # PyFusion #
```

