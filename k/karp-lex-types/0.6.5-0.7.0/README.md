# Comparing `tmp/karp_lex_types-0.6.5.tar.gz` & `tmp/karp_lex_types-0.7.0.tar.gz`

## Comparing `karp_lex_types-0.6.5.tar` & `karp_lex_types-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/.bumpversion.toml
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/CHANGELOG.md
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/Makefile
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/cliff.toml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/mypy.ini
--rw-r--r--   0        0        0    38432 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/pdm.lock
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/ruff.toml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/alias_generators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/py.typed
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/commands/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/commands/base.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/commands/entry_commands.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/commands/entry_repo_commands.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/commands/resource_commands.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/dtos/__init__.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/dtos/entry_dto.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/value_objects/__init__.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/src/karp_lex_types/value_objects/unique_id.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/tests/conftest.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/tests/entry_dto_unit_test.py
--rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/tests/requirements-testing.lock
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/tests/test_entry_commands.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/tests/test_entry_repo_commands.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/tests/test_resource_commands.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/tests/test_unique_id.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/LICENSE
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/README.md
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 karp_lex_types-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/.bumpversion.toml
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/Makefile
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/cliff.toml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/mypy.ini
+-rw-r--r--   0        0        0    38495 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/pdm.lock
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/ruff.toml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/alias_generators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/py.typed
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/base.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/entry_commands.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/entry_repo_commands.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/resource_commands.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/dtos/__init__.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/dtos/entry_dto.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/value_objects/__init__.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/value_objects/unique_id.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/entry_dto_unit_test.py
+-rw-r--r--   0        0        0    15784 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/requirements-testing.lock
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/test_entry_commands.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/test_entry_repo_commands.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/test_resource_commands.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/test_unique_id.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/README.md
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/PKG-INFO
```

### Comparing `karp_lex_types-0.6.5/.bumpversion.toml` & `karp_lex_types-0.7.0/.bumpversion.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.bumpversion]
-current_version = "0.6.5"
+current_version = "0.7.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 commit = true
 tag = true
 sign_tag = true
 allow_dirty = false
 message = "chore(release): Bump version: {current_version} → {new_version}"
```

### Comparing `karp_lex_types-0.6.5/CHANGELOG.md` & `karp_lex_types-0.7.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.7.0] - 2024-05-22
+
+### Fixed
+
+- Serialize UniuqeId as str
+
 ## [0.6.5] - 2024-05-15
 
 ### Documentation
 
 - Update readme
 
 ## [0.6.3] - 2024-05-14
```

### Comparing `karp_lex_types-0.6.5/Makefile` & `karp_lex_types-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/cliff.toml` & `karp_lex_types-0.7.0/cliff.toml`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/pdm.lock` & `karp_lex_types-0.7.0/pdm.lock`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 groups = ["default", "dev"]
 strategy = ["cross_platform", "inherit_metadata"]
 lock_version = "4.4.1"
 content_hash = "sha256:e40ce2d2f35abe5e0aff464f3cd12f3843d3017fb9b4ec4e84845112a0a2ee5b"
 
 [[package]]
 name = "annotated-types"
-version = "0.6.0"
+version = "0.7.0"
 requires_python = ">=3.8"
 summary = "Reusable constraint types to use with typing.Annotated"
 groups = ["default", "dev"]
 files = [
-    {file = "annotated_types-0.6.0-py3-none-any.whl", hash = "sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43"},
-    {file = "annotated_types-0.6.0.tar.gz", hash = "sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d"},
+    {file = "annotated_types-0.7.0-py3-none-any.whl", hash = "sha256:1f02e8b43a8fbbc3f3e0d4f0f4bfc8131bcb4eebe8849b8e5c773f3a1c582a53"},
+    {file = "annotated_types-0.7.0.tar.gz", hash = "sha256:aff07c09a53a08bc8cfccb9c85b05f1aa9a2a6f23728d790723543408344ce89"},
 ]
 
 [[package]]
 name = "bracex"
 version = "2.4"
 requires_python = ">=3.8"
 summary = "Bash style brace expander."
@@ -27,31 +27,31 @@
 files = [
     {file = "bracex-2.4-py3-none-any.whl", hash = "sha256:efdc71eff95eaff5e0f8cfebe7d01adf2c8637c8c92edaf63ef348c241a82418"},
     {file = "bracex-2.4.tar.gz", hash = "sha256:a27eaf1df42cf561fed58b7a8f3fdf129d1ea16a81e1fadd1d17989bc6384beb"},
 ]
 
 [[package]]
 name = "bump-my-version"
-version = "0.21.0"
+version = "0.21.1"
 requires_python = ">=3.8"
 summary = "Version bump your Python project"
 groups = ["dev"]
 dependencies = [
     "click",
     "pydantic-settings",
     "pydantic>=2.0.0",
     "questionary",
     "rich",
     "rich-click",
     "tomlkit",
     "wcmatch>=8.5.1",
 ]
 files = [
-    {file = "bump_my_version-0.21.0-py3-none-any.whl", hash = "sha256:a614d8176b5ac0e644239c9a8a246b696d316f68406fd78b8486a9e13fc93266"},
-    {file = "bump_my_version-0.21.0.tar.gz", hash = "sha256:c3f1a31e32345679b517cbba99a0875457ee45d7ba6189fcd2a74d3ddae41515"},
+    {file = "bump_my_version-0.21.1-py3-none-any.whl", hash = "sha256:946a7edcf30c5a8574c579684df983136ea395f70c184e4db32eb3e307584c14"},
+    {file = "bump_my_version-0.21.1.tar.gz", hash = "sha256:ec612474e9e790c3fbbfed153a10b356f84fc15096ceff181b399d5e985bfacc"},
 ]
 
 [[package]]
 name = "click"
 version = "8.1.7"
 requires_python = ">=3.7"
 summary = "Composable command line interface toolkit"
@@ -74,109 +74,109 @@
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.4.1"
+version = "7.5.1"
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
 groups = ["dev"]
 files = [
-    {file = "coverage-7.4.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:077d366e724f24fc02dbfe9d946534357fda71af9764ff99d73c3c596001bbd7"},
-    {file = "coverage-7.4.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0193657651f5399d433c92f8ae264aff31fc1d066deee4b831549526433f3f61"},
-    {file = "coverage-7.4.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d17bbc946f52ca67adf72a5ee783cd7cd3477f8f8796f59b4974a9b59cacc9ee"},
-    {file = "coverage-7.4.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a3277f5fa7483c927fe3a7b017b39351610265308f5267ac6d4c2b64cc1d8d25"},
-    {file = "coverage-7.4.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6dceb61d40cbfcf45f51e59933c784a50846dc03211054bd76b421a713dcdf19"},
-    {file = "coverage-7.4.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:6008adeca04a445ea6ef31b2cbaf1d01d02986047606f7da266629afee982630"},
-    {file = "coverage-7.4.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:c61f66d93d712f6e03369b6a7769233bfda880b12f417eefdd4f16d1deb2fc4c"},
-    {file = "coverage-7.4.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b9bb62fac84d5f2ff523304e59e5c439955fb3b7f44e3d7b2085184db74d733b"},
-    {file = "coverage-7.4.1-cp310-cp310-win32.whl", hash = "sha256:f86f368e1c7ce897bf2457b9eb61169a44e2ef797099fb5728482b8d69f3f016"},
-    {file = "coverage-7.4.1-cp310-cp310-win_amd64.whl", hash = "sha256:869b5046d41abfea3e381dd143407b0d29b8282a904a19cb908fa24d090cc018"},
-    {file = "coverage-7.4.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:b8ffb498a83d7e0305968289441914154fb0ef5d8b3157df02a90c6695978295"},
-    {file = "coverage-7.4.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:3cacfaefe6089d477264001f90f55b7881ba615953414999c46cc9713ff93c8c"},
-    {file = "coverage-7.4.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5d6850e6e36e332d5511a48a251790ddc545e16e8beaf046c03985c69ccb2676"},
-    {file = "coverage-7.4.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:18e961aa13b6d47f758cc5879383d27b5b3f3dcd9ce8cdbfdc2571fe86feb4dd"},
-    {file = "coverage-7.4.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dfd1e1b9f0898817babf840b77ce9fe655ecbe8b1b327983df485b30df8cc011"},
-    {file = "coverage-7.4.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:6b00e21f86598b6330f0019b40fb397e705135040dbedc2ca9a93c7441178e74"},
-    {file = "coverage-7.4.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:536d609c6963c50055bab766d9951b6c394759190d03311f3e9fcf194ca909e1"},
-    {file = "coverage-7.4.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:7ac8f8eb153724f84885a1374999b7e45734bf93a87d8df1e7ce2146860edef6"},
-    {file = "coverage-7.4.1-cp311-cp311-win32.whl", hash = "sha256:f3771b23bb3675a06f5d885c3630b1d01ea6cac9e84a01aaf5508706dba546c5"},
-    {file = "coverage-7.4.1-cp311-cp311-win_amd64.whl", hash = "sha256:9d2f9d4cc2a53b38cabc2d6d80f7f9b7e3da26b2f53d48f05876fef7956b6968"},
-    {file = "coverage-7.4.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:f68ef3660677e6624c8cace943e4765545f8191313a07288a53d3da188bd8581"},
-    {file = "coverage-7.4.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:23b27b8a698e749b61809fb637eb98ebf0e505710ec46a8aa6f1be7dc0dc43a6"},
-    {file = "coverage-7.4.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3e3424c554391dc9ef4a92ad28665756566a28fecf47308f91841f6c49288e66"},
-    {file = "coverage-7.4.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e0860a348bf7004c812c8368d1fc7f77fe8e4c095d661a579196a9533778e156"},
-    {file = "coverage-7.4.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fe558371c1bdf3b8fa03e097c523fb9645b8730399c14fe7721ee9c9e2a545d3"},
-    {file = "coverage-7.4.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:3468cc8720402af37b6c6e7e2a9cdb9f6c16c728638a2ebc768ba1ef6f26c3a1"},
-    {file = "coverage-7.4.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:02f2edb575d62172aa28fe00efe821ae31f25dc3d589055b3fb64d51e52e4ab1"},
-    {file = "coverage-7.4.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:ca6e61dc52f601d1d224526360cdeab0d0712ec104a2ce6cc5ccef6ed9a233bc"},
-    {file = "coverage-7.4.1-cp312-cp312-win32.whl", hash = "sha256:ca7b26a5e456a843b9b6683eada193fc1f65c761b3a473941efe5a291f604c74"},
-    {file = "coverage-7.4.1-cp312-cp312-win_amd64.whl", hash = "sha256:85ccc5fa54c2ed64bd91ed3b4a627b9cce04646a659512a051fa82a92c04a448"},
-    {file = "coverage-7.4.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:32a8d985462e37cfdab611a6f95b09d7c091d07668fdc26e47a725ee575fe166"},
-    {file = "coverage-7.4.1.tar.gz", hash = "sha256:1ed4b95480952b1a26d863e546fa5094564aa0065e1e5f0d4d0041f293251d04"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146"},
+    {file = "coverage-7.5.1-cp310-cp310-win32.whl", hash = "sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228"},
+    {file = "coverage-7.5.1-cp310-cp310-win_amd64.whl", hash = "sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987"},
+    {file = "coverage-7.5.1-cp311-cp311-win32.whl", hash = "sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136"},
+    {file = "coverage-7.5.1-cp311-cp311-win_amd64.whl", hash = "sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7"},
+    {file = "coverage-7.5.1-cp312-cp312-win32.whl", hash = "sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19"},
+    {file = "coverage-7.5.1-cp312-cp312-win_amd64.whl", hash = "sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596"},
+    {file = "coverage-7.5.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312"},
+    {file = "coverage-7.5.1.tar.gz", hash = "sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.4.1"
+version = "7.5.1"
 extras = ["toml"]
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
 groups = ["dev"]
 dependencies = [
-    "coverage==7.4.1",
+    "coverage==7.5.1",
     "tomli; python_full_version <= \"3.11.0a6\"",
 ]
 files = [
-    {file = "coverage-7.4.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:077d366e724f24fc02dbfe9d946534357fda71af9764ff99d73c3c596001bbd7"},
-    {file = "coverage-7.4.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0193657651f5399d433c92f8ae264aff31fc1d066deee4b831549526433f3f61"},
-    {file = "coverage-7.4.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d17bbc946f52ca67adf72a5ee783cd7cd3477f8f8796f59b4974a9b59cacc9ee"},
-    {file = "coverage-7.4.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a3277f5fa7483c927fe3a7b017b39351610265308f5267ac6d4c2b64cc1d8d25"},
-    {file = "coverage-7.4.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6dceb61d40cbfcf45f51e59933c784a50846dc03211054bd76b421a713dcdf19"},
-    {file = "coverage-7.4.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:6008adeca04a445ea6ef31b2cbaf1d01d02986047606f7da266629afee982630"},
-    {file = "coverage-7.4.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:c61f66d93d712f6e03369b6a7769233bfda880b12f417eefdd4f16d1deb2fc4c"},
-    {file = "coverage-7.4.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b9bb62fac84d5f2ff523304e59e5c439955fb3b7f44e3d7b2085184db74d733b"},
-    {file = "coverage-7.4.1-cp310-cp310-win32.whl", hash = "sha256:f86f368e1c7ce897bf2457b9eb61169a44e2ef797099fb5728482b8d69f3f016"},
-    {file = "coverage-7.4.1-cp310-cp310-win_amd64.whl", hash = "sha256:869b5046d41abfea3e381dd143407b0d29b8282a904a19cb908fa24d090cc018"},
-    {file = "coverage-7.4.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:b8ffb498a83d7e0305968289441914154fb0ef5d8b3157df02a90c6695978295"},
-    {file = "coverage-7.4.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:3cacfaefe6089d477264001f90f55b7881ba615953414999c46cc9713ff93c8c"},
-    {file = "coverage-7.4.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5d6850e6e36e332d5511a48a251790ddc545e16e8beaf046c03985c69ccb2676"},
-    {file = "coverage-7.4.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:18e961aa13b6d47f758cc5879383d27b5b3f3dcd9ce8cdbfdc2571fe86feb4dd"},
-    {file = "coverage-7.4.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dfd1e1b9f0898817babf840b77ce9fe655ecbe8b1b327983df485b30df8cc011"},
-    {file = "coverage-7.4.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:6b00e21f86598b6330f0019b40fb397e705135040dbedc2ca9a93c7441178e74"},
-    {file = "coverage-7.4.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:536d609c6963c50055bab766d9951b6c394759190d03311f3e9fcf194ca909e1"},
-    {file = "coverage-7.4.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:7ac8f8eb153724f84885a1374999b7e45734bf93a87d8df1e7ce2146860edef6"},
-    {file = "coverage-7.4.1-cp311-cp311-win32.whl", hash = "sha256:f3771b23bb3675a06f5d885c3630b1d01ea6cac9e84a01aaf5508706dba546c5"},
-    {file = "coverage-7.4.1-cp311-cp311-win_amd64.whl", hash = "sha256:9d2f9d4cc2a53b38cabc2d6d80f7f9b7e3da26b2f53d48f05876fef7956b6968"},
-    {file = "coverage-7.4.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:f68ef3660677e6624c8cace943e4765545f8191313a07288a53d3da188bd8581"},
-    {file = "coverage-7.4.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:23b27b8a698e749b61809fb637eb98ebf0e505710ec46a8aa6f1be7dc0dc43a6"},
-    {file = "coverage-7.4.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3e3424c554391dc9ef4a92ad28665756566a28fecf47308f91841f6c49288e66"},
-    {file = "coverage-7.4.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e0860a348bf7004c812c8368d1fc7f77fe8e4c095d661a579196a9533778e156"},
-    {file = "coverage-7.4.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fe558371c1bdf3b8fa03e097c523fb9645b8730399c14fe7721ee9c9e2a545d3"},
-    {file = "coverage-7.4.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:3468cc8720402af37b6c6e7e2a9cdb9f6c16c728638a2ebc768ba1ef6f26c3a1"},
-    {file = "coverage-7.4.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:02f2edb575d62172aa28fe00efe821ae31f25dc3d589055b3fb64d51e52e4ab1"},
-    {file = "coverage-7.4.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:ca6e61dc52f601d1d224526360cdeab0d0712ec104a2ce6cc5ccef6ed9a233bc"},
-    {file = "coverage-7.4.1-cp312-cp312-win32.whl", hash = "sha256:ca7b26a5e456a843b9b6683eada193fc1f65c761b3a473941efe5a291f604c74"},
-    {file = "coverage-7.4.1-cp312-cp312-win_amd64.whl", hash = "sha256:85ccc5fa54c2ed64bd91ed3b4a627b9cce04646a659512a051fa82a92c04a448"},
-    {file = "coverage-7.4.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:32a8d985462e37cfdab611a6f95b09d7c091d07668fdc26e47a725ee575fe166"},
-    {file = "coverage-7.4.1.tar.gz", hash = "sha256:1ed4b95480952b1a26d863e546fa5094564aa0065e1e5f0d4d0041f293251d04"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146"},
+    {file = "coverage-7.5.1-cp310-cp310-win32.whl", hash = "sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228"},
+    {file = "coverage-7.5.1-cp310-cp310-win_amd64.whl", hash = "sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987"},
+    {file = "coverage-7.5.1-cp311-cp311-win32.whl", hash = "sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136"},
+    {file = "coverage-7.5.1-cp311-cp311-win_amd64.whl", hash = "sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7"},
+    {file = "coverage-7.5.1-cp312-cp312-win32.whl", hash = "sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19"},
+    {file = "coverage-7.5.1-cp312-cp312-win_amd64.whl", hash = "sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596"},
+    {file = "coverage-7.5.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312"},
+    {file = "coverage-7.5.1.tar.gz", hash = "sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.2.0"
+version = "1.2.1"
 requires_python = ">=3.7"
 summary = "Backport of PEP 654 (exception groups)"
 groups = ["dev"]
 marker = "python_version < \"3.11\""
 files = [
-    {file = "exceptiongroup-1.2.0-py3-none-any.whl", hash = "sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14"},
-    {file = "exceptiongroup-1.2.0.tar.gz", hash = "sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68"},
+    {file = "exceptiongroup-1.2.1-py3-none-any.whl", hash = "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad"},
+    {file = "exceptiongroup-1.2.1.tar.gz", hash = "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"},
 ]
 
 [[package]]
 name = "iniconfig"
 version = "2.0.0"
 requires_python = ">=3.7"
 summary = "brain-dead simple config-ini parsing"
@@ -251,21 +251,21 @@
 files = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "packaging"
-version = "23.2"
+version = "24.0"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
 groups = ["dev"]
 files = [
-    {file = "packaging-23.2-py3-none-any.whl", hash = "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"},
-    {file = "packaging-23.2.tar.gz", hash = "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5"},
+    {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
+    {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
 ]
 
 [[package]]
 name = "pluggy"
 version = "1.5.0"
 requires_python = ">=3.8"
 summary = "plugin and hook calling mechanisms for python"
@@ -287,93 +287,93 @@
 files = [
     {file = "prompt_toolkit-3.0.36-py3-none-any.whl", hash = "sha256:aa64ad242a462c5ff0363a7b9cfe696c20d55d9fc60c11fd8e632d064804d305"},
     {file = "prompt_toolkit-3.0.36.tar.gz", hash = "sha256:3e163f254bef5a03b146397d7c1963bd3e2812f0964bb9a24e6ec761fd28db63"},
 ]
 
 [[package]]
 name = "pydantic"
-version = "2.6.3"
+version = "2.7.1"
 requires_python = ">=3.8"
 summary = "Data validation using Python type hints"
 groups = ["default", "dev"]
 dependencies = [
     "annotated-types>=0.4.0",
-    "pydantic-core==2.16.3",
+    "pydantic-core==2.18.2",
     "typing-extensions>=4.6.1",
 ]
 files = [
-    {file = "pydantic-2.6.3-py3-none-any.whl", hash = "sha256:72c6034df47f46ccdf81869fddb81aade68056003900a8724a4f160700016a2a"},
-    {file = "pydantic-2.6.3.tar.gz", hash = "sha256:e07805c4c7f5c6826e33a1d4c9d47950d7eaf34868e2690f8594d2e30241f11f"},
+    {file = "pydantic-2.7.1-py3-none-any.whl", hash = "sha256:e029badca45266732a9a79898a15ae2e8b14840b1eabbb25844be28f0b33f3d5"},
+    {file = "pydantic-2.7.1.tar.gz", hash = "sha256:e9dbb5eada8abe4d9ae5f46b9939aead650cd2b68f249bb3a8139dbe125803cc"},
 ]
 
 [[package]]
 name = "pydantic-core"
-version = "2.16.3"
+version = "2.18.2"
 requires_python = ">=3.8"
-summary = ""
+summary = "Core functionality for Pydantic validation and serialization"
 groups = ["default", "dev"]
 dependencies = [
     "typing-extensions!=4.7.0,>=4.6.0",
 ]
 files = [
-    {file = "pydantic_core-2.16.3-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:75b81e678d1c1ede0785c7f46690621e4c6e63ccd9192af1f0bd9d504bbb6bf4"},
-    {file = "pydantic_core-2.16.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9c865a7ee6f93783bd5d781af5a4c43dadc37053a5b42f7d18dc019f8c9d2bd1"},
-    {file = "pydantic_core-2.16.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:162e498303d2b1c036b957a1278fa0899d02b2842f1ff901b6395104c5554a45"},
-    {file = "pydantic_core-2.16.3-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:2f583bd01bbfbff4eaee0868e6fc607efdfcc2b03c1c766b06a707abbc856187"},
-    {file = "pydantic_core-2.16.3-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b926dd38db1519ed3043a4de50214e0d600d404099c3392f098a7f9d75029ff8"},
-    {file = "pydantic_core-2.16.3-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:716b542728d4c742353448765aa7cdaa519a7b82f9564130e2b3f6766018c9ec"},
-    {file = "pydantic_core-2.16.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fc4ad7f7ee1a13d9cb49d8198cd7d7e3aa93e425f371a68235f784e99741561f"},
-    {file = "pydantic_core-2.16.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:bd87f48924f360e5d1c5f770d6155ce0e7d83f7b4e10c2f9ec001c73cf475c99"},
-    {file = "pydantic_core-2.16.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:0df446663464884297c793874573549229f9eca73b59360878f382a0fc085979"},
-    {file = "pydantic_core-2.16.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:4df8a199d9f6afc5ae9a65f8f95ee52cae389a8c6b20163762bde0426275b7db"},
-    {file = "pydantic_core-2.16.3-cp310-none-win32.whl", hash = "sha256:456855f57b413f077dff513a5a28ed838dbbb15082ba00f80750377eed23d132"},
-    {file = "pydantic_core-2.16.3-cp310-none-win_amd64.whl", hash = "sha256:732da3243e1b8d3eab8c6ae23ae6a58548849d2e4a4e03a1924c8ddf71a387cb"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-macosx_10_12_x86_64.whl", hash = "sha256:519ae0312616026bf4cedc0fe459e982734f3ca82ee8c7246c19b650b60a5ee4"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b3992a322a5617ded0a9f23fd06dbc1e4bd7cf39bc4ccf344b10f80af58beacd"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8d62da299c6ecb04df729e4b5c52dc0d53f4f8430b4492b93aa8de1f541c4aac"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:2acca2be4bb2f2147ada8cac612f8a98fc09f41c89f87add7256ad27332c2fda"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:1b662180108c55dfbf1280d865b2d116633d436cfc0bba82323554873967b340"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e7c6ed0dc9d8e65f24f5824291550139fe6f37fac03788d4580da0d33bc00c97"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a6b1bb0827f56654b4437955555dc3aeeebeddc47c2d7ed575477f082622c49e"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:e56f8186d6210ac7ece503193ec84104da7ceb98f68ce18c07282fcc2452e76f"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:936e5db01dd49476fa8f4383c259b8b1303d5dd5fb34c97de194560698cc2c5e"},
-    {file = "pydantic_core-2.16.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:33809aebac276089b78db106ee692bdc9044710e26f24a9a2eaa35a0f9fa70ba"},
-    {file = "pydantic_core-2.16.3-cp311-none-win32.whl", hash = "sha256:ded1c35f15c9dea16ead9bffcde9bb5c7c031bff076355dc58dcb1cb436c4721"},
-    {file = "pydantic_core-2.16.3-cp311-none-win_amd64.whl", hash = "sha256:d89ca19cdd0dd5f31606a9329e309d4fcbb3df860960acec32630297d61820df"},
-    {file = "pydantic_core-2.16.3-cp311-none-win_arm64.whl", hash = "sha256:6162f8d2dc27ba21027f261e4fa26f8bcb3cf9784b7f9499466a311ac284b5b9"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-macosx_10_12_x86_64.whl", hash = "sha256:0f56ae86b60ea987ae8bcd6654a887238fd53d1384f9b222ac457070b7ac4cff"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:c9bd22a2a639e26171068f8ebb5400ce2c1bc7d17959f60a3b753ae13c632975"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4204e773b4b408062960e65468d5346bdfe139247ee5f1ca2a378983e11388a2"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f651dd19363c632f4abe3480a7c87a9773be27cfe1341aef06e8759599454120"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:aaf09e615a0bf98d406657e0008e4a8701b11481840be7d31755dc9f97c44053"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8e47755d8152c1ab5b55928ab422a76e2e7b22b5ed8e90a7d584268dd49e9c6b"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:500960cb3a0543a724a81ba859da816e8cf01b0e6aaeedf2c3775d12ee49cade"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:cf6204fe865da605285c34cf1172879d0314ff267b1c35ff59de7154f35fdc2e"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:d33dd21f572545649f90c38c227cc8631268ba25c460b5569abebdd0ec5974ca"},
-    {file = "pydantic_core-2.16.3-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:49d5d58abd4b83fb8ce763be7794d09b2f50f10aa65c0f0c1696c677edeb7cbf"},
-    {file = "pydantic_core-2.16.3-cp312-none-win32.whl", hash = "sha256:f53aace168a2a10582e570b7736cc5bef12cae9cf21775e3eafac597e8551fbe"},
-    {file = "pydantic_core-2.16.3-cp312-none-win_amd64.whl", hash = "sha256:0d32576b1de5a30d9a97f300cc6a3f4694c428d956adbc7e6e2f9cad279e45ed"},
-    {file = "pydantic_core-2.16.3-cp312-none-win_arm64.whl", hash = "sha256:ec08be75bb268473677edb83ba71e7e74b43c008e4a7b1907c6d57e940bf34b6"},
-    {file = "pydantic_core-2.16.3-pp310-pypy310_pp73-macosx_10_12_x86_64.whl", hash = "sha256:36fa178aacbc277bc6b62a2c3da95226520da4f4e9e206fdf076484363895d2c"},
-    {file = "pydantic_core-2.16.3-pp310-pypy310_pp73-macosx_11_0_arm64.whl", hash = "sha256:dcca5d2bf65c6fb591fff92da03f94cd4f315972f97c21975398bd4bd046854a"},
-    {file = "pydantic_core-2.16.3-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2a72fb9963cba4cd5793854fd12f4cfee731e86df140f59ff52a49b3552db241"},
-    {file = "pydantic_core-2.16.3-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b60cc1a081f80a2105a59385b92d82278b15d80ebb3adb200542ae165cd7d183"},
-    {file = "pydantic_core-2.16.3-pp310-pypy310_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:cbcc558401de90a746d02ef330c528f2e668c83350f045833543cd57ecead1ad"},
-    {file = "pydantic_core-2.16.3-pp310-pypy310_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:fee427241c2d9fb7192b658190f9f5fd6dfe41e02f3c1489d2ec1e6a5ab1e04a"},
-    {file = "pydantic_core-2.16.3-pp310-pypy310_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:f4cb85f693044e0f71f394ff76c98ddc1bc0953e48c061725e540396d5c8a2e1"},
-    {file = "pydantic_core-2.16.3-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:b29eeb887aa931c2fcef5aa515d9d176d25006794610c264ddc114c053bf96fe"},
-    {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:a425479ee40ff021f8216c9d07a6a3b54b31c8267c6e17aa88b70d7ebd0e5e5b"},
-    {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-macosx_11_0_arm64.whl", hash = "sha256:5c5cbc703168d1b7a838668998308018a2718c2130595e8e190220238addc96f"},
-    {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:99b6add4c0b39a513d323d3b93bc173dac663c27b99860dd5bf491b240d26137"},
-    {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75f76ee558751746d6a38f89d60b6228fa174e5172d143886af0f85aa306fd89"},
-    {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:00ee1c97b5364b84cb0bd82e9bbf645d5e2871fb8c58059d158412fee2d33d8a"},
-    {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:287073c66748f624be4cef893ef9174e3eb88fe0b8a78dc22e88eca4bc357ca6"},
-    {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:ed25e1835c00a332cb10c683cd39da96a719ab1dfc08427d476bce41b92531fc"},
-    {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:86b3d0033580bd6bbe07590152007275bd7af95f98eaa5bd36f3da219dcd93da"},
-    {file = "pydantic_core-2.16.3.tar.gz", hash = "sha256:1cac689f80a3abab2d3c0048b29eea5751114054f032a941a32de4c852c59cad"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:9e08e867b306f525802df7cd16c44ff5ebbe747ff0ca6cf3fde7f36c05a59a81"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:f0a21cbaa69900cbe1a2e7cad2aa74ac3cf21b10c3efb0fa0b80305274c0e8a2"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0680b1f1f11fda801397de52c36ce38ef1c1dc841a0927a94f226dea29c3ae3d"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:95b9d5e72481d3780ba3442eac863eae92ae43a5f3adb5b4d0a1de89d42bb250"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:c4fcf5cd9c4b655ad666ca332b9a081112cd7a58a8b5a6ca7a3104bc950f2038"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:9b5155ff768083cb1d62f3e143b49a8a3432e6789a3abee8acd005c3c7af1c74"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:553ef617b6836fc7e4df130bb851e32fe357ce36336d897fd6646d6058d980af"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:b89ed9eb7d616ef5714e5590e6cf7f23b02d0d539767d33561e3675d6f9e3857"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:75f7e9488238e920ab6204399ded280dc4c307d034f3924cd7f90a38b1829563"},
+    {file = "pydantic_core-2.18.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:ef26c9e94a8c04a1b2924149a9cb081836913818e55681722d7f29af88fe7b38"},
+    {file = "pydantic_core-2.18.2-cp310-none-win32.whl", hash = "sha256:182245ff6b0039e82b6bb585ed55a64d7c81c560715d1bad0cbad6dfa07b4027"},
+    {file = "pydantic_core-2.18.2-cp310-none-win_amd64.whl", hash = "sha256:e23ec367a948b6d812301afc1b13f8094ab7b2c280af66ef450efc357d2ae543"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-macosx_10_12_x86_64.whl", hash = "sha256:219da3f096d50a157f33645a1cf31c0ad1fe829a92181dd1311022f986e5fbe3"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:cc1cfd88a64e012b74e94cd00bbe0f9c6df57049c97f02bb07d39e9c852e19a4"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:05b7133a6e6aeb8df37d6f413f7705a37ab4031597f64ab56384c94d98fa0e90"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:224c421235f6102e8737032483f43c1a8cfb1d2f45740c44166219599358c2cd"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b14d82cdb934e99dda6d9d60dc84a24379820176cc4a0d123f88df319ae9c150"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2728b01246a3bba6de144f9e3115b532ee44bd6cf39795194fb75491824a1413"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:470b94480bb5ee929f5acba6995251ada5e059a5ef3e0dfc63cca287283ebfa6"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:997abc4df705d1295a42f95b4eec4950a37ad8ae46d913caeee117b6b198811c"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:75250dbc5290e3f1a0f4618db35e51a165186f9034eff158f3d490b3fed9f8a0"},
+    {file = "pydantic_core-2.18.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:4456f2dca97c425231d7315737d45239b2b51a50dc2b6f0c2bb181fce6207664"},
+    {file = "pydantic_core-2.18.2-cp311-none-win32.whl", hash = "sha256:269322dcc3d8bdb69f054681edff86276b2ff972447863cf34c8b860f5188e2e"},
+    {file = "pydantic_core-2.18.2-cp311-none-win_amd64.whl", hash = "sha256:800d60565aec896f25bc3cfa56d2277d52d5182af08162f7954f938c06dc4ee3"},
+    {file = "pydantic_core-2.18.2-cp311-none-win_arm64.whl", hash = "sha256:1404c69d6a676245199767ba4f633cce5f4ad4181f9d0ccb0577e1f66cf4c46d"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl", hash = "sha256:fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d7d904828195733c183d20a54230c0df0eb46ec746ea1a666730787353e87182"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:c9bd70772c720142be1020eac55f8143a34ec9f82d75a8e7a07852023e46617f"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2b8ed04b3582771764538f7ee7001b02e1170223cf9b75dff0bc698fadb00cf3"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e6dac87ddb34aaec85f873d737e9d06a3555a1cc1a8e0c44b7f8d5daeb89d86f"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:886eec03591b7cf058467a70a87733b35f44707bd86cf64a615584fd72488b7c"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:ca7b0c1f1c983e064caa85f3792dd2fe3526b3505378874afa84baf662e12241"},
+    {file = "pydantic_core-2.18.2-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4b4356d3538c3649337df4074e81b85f0616b79731fe22dd11b99499b2ebbdf3"},
+    {file = "pydantic_core-2.18.2-cp312-none-win32.whl", hash = "sha256:8b172601454f2d7701121bbec3425dd71efcb787a027edf49724c9cefc14c038"},
+    {file = "pydantic_core-2.18.2-cp312-none-win_amd64.whl", hash = "sha256:b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438"},
+    {file = "pydantic_core-2.18.2-cp312-none-win_arm64.whl", hash = "sha256:98758d627ff397e752bc339272c14c98199c613f922d4a384ddc07526c86a2ec"},
+    {file = "pydantic_core-2.18.2-pp310-pypy310_pp73-macosx_10_12_x86_64.whl", hash = "sha256:a1874c6dd4113308bd0eb568418e6114b252afe44319ead2b4081e9b9521fe75"},
+    {file = "pydantic_core-2.18.2-pp310-pypy310_pp73-macosx_11_0_arm64.whl", hash = "sha256:ccdd111c03bfd3666bd2472b674c6899550e09e9f298954cfc896ab92b5b0e6d"},
+    {file = "pydantic_core-2.18.2-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e18609ceaa6eed63753037fc06ebb16041d17d28199ae5aba0052c51449650a9"},
+    {file = "pydantic_core-2.18.2-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6e5c584d357c4e2baf0ff7baf44f4994be121e16a2c88918a5817331fc7599d7"},
+    {file = "pydantic_core-2.18.2-pp310-pypy310_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:43f0f463cf89ace478de71a318b1b4f05ebc456a9b9300d027b4b57c1a2064fb"},
+    {file = "pydantic_core-2.18.2-pp310-pypy310_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:e1b395e58b10b73b07b7cf740d728dd4ff9365ac46c18751bf8b3d8cca8f625a"},
+    {file = "pydantic_core-2.18.2-pp310-pypy310_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:0098300eebb1c837271d3d1a2cd2911e7c11b396eac9661655ee524a7f10587b"},
+    {file = "pydantic_core-2.18.2-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:36789b70d613fbac0a25bb07ab3d9dba4d2e38af609c020cf4d888d165ee0bf3"},
+    {file = "pydantic_core-2.18.2-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:3f9a801e7c8f1ef8718da265bba008fa121243dfe37c1cea17840b0944dfd72c"},
+    {file = "pydantic_core-2.18.2-pp39-pypy39_pp73-macosx_11_0_arm64.whl", hash = "sha256:3a6515ebc6e69d85502b4951d89131ca4e036078ea35533bb76327f8424531ce"},
+    {file = "pydantic_core-2.18.2-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:20aca1e2298c56ececfd8ed159ae4dde2df0781988c97ef77d5c16ff4bd5b400"},
+    {file = "pydantic_core-2.18.2-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:223ee893d77a310a0391dca6df00f70bbc2f36a71a895cecd9a0e762dc37b349"},
+    {file = "pydantic_core-2.18.2-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:2334ce8c673ee93a1d6a65bd90327588387ba073c17e61bf19b4fd97d688d63c"},
+    {file = "pydantic_core-2.18.2-pp39-pypy39_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:cbca948f2d14b09d20268cda7b0367723d79063f26c4ffc523af9042cad95592"},
+    {file = "pydantic_core-2.18.2-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:b3ef08e20ec49e02d5c6717a91bb5af9b20f1805583cb0adfe9ba2c6b505b5ae"},
+    {file = "pydantic_core-2.18.2-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:c6fdc8627910eed0c01aed6a390a252fe3ea6d472ee70fdde56273f198938374"},
+    {file = "pydantic_core-2.18.2.tar.gz", hash = "sha256:2e29d20810dfc3043ee13ac7d9e25105799817683348823f305ab3f349b9386e"},
 ]
 
 [[package]]
 name = "pydantic-settings"
 version = "2.2.1"
 requires_python = ">=3.8"
 summary = "Settings management using Pydantic"
@@ -396,29 +396,29 @@
 files = [
     {file = "pygments-2.18.0-py3-none-any.whl", hash = "sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a"},
     {file = "pygments-2.18.0.tar.gz", hash = "sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199"},
 ]
 
 [[package]]
 name = "pytest"
-version = "8.2.0"
+version = "8.2.1"
 requires_python = ">=3.8"
 summary = "pytest: simple powerful testing with Python"
 groups = ["dev"]
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
     "pluggy<2.0,>=1.5",
     "tomli>=1; python_version < \"3.11\"",
 ]
 files = [
-    {file = "pytest-8.2.0-py3-none-any.whl", hash = "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233"},
-    {file = "pytest-8.2.0.tar.gz", hash = "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"},
+    {file = "pytest-8.2.1-py3-none-any.whl", hash = "sha256:faccc5d332b8c3719f40283d0d44aa5cf101cec36f88cde9ed8f2bc0538612b1"},
+    {file = "pytest-8.2.1.tar.gz", hash = "sha256:5046e5b46d8e4cac199c373041f26be56fdb81eb4e67dc11d4e10811fc3408fd"},
 ]
 
 [[package]]
 name = "pytest-cov"
 version = "5.0.0"
 requires_python = ">=3.8"
 summary = "Pytest plugin for measuring coverage."
@@ -470,26 +470,26 @@
 files = [
     {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
     {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
 ]
 
 [[package]]
 name = "rich-click"
-version = "1.8.1"
+version = "1.8.2"
 requires_python = ">=3.7"
 summary = "Format click help output nicely with rich"
 groups = ["dev"]
 dependencies = [
     "click>=7",
     "rich>=10.7",
     "typing-extensions",
 ]
 files = [
-    {file = "rich_click-1.8.1-py3-none-any.whl", hash = "sha256:0cf0bf84404e78379bd2722db88cb07ffd0535440e20a05943d5b02249d90f8a"},
-    {file = "rich_click-1.8.1.tar.gz", hash = "sha256:73c2ec88a66d7bf6b8c32783539d1c9c92c7c75847f14186092d27f83b206e8a"},
+    {file = "rich_click-1.8.2-py3-none-any.whl", hash = "sha256:b57856f304e4fe0394b82d7ce0784450758f8c8b4e201ccc4320501cc201806b"},
+    {file = "rich_click-1.8.2.tar.gz", hash = "sha256:8e29bdede858b59aa2859a1ab1c4ccbd39ed7ed5870262dae756fba6b5dc72e8"},
 ]
 
 [[package]]
 name = "ruff"
 version = "0.4.4"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
@@ -535,45 +535,45 @@
 files = [
     {file = "tomlkit-0.12.5-py3-none-any.whl", hash = "sha256:af914f5a9c59ed9d0762c7b64d3b5d5df007448eb9cd2edc8a46b1eafead172f"},
     {file = "tomlkit-0.12.5.tar.gz", hash = "sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.9.0"
+version = "4.11.0"
 requires_python = ">=3.8"
 summary = "Backported and Experimental Type Hints for Python 3.8+"
 groups = ["default", "dev"]
 files = [
-    {file = "typing_extensions-4.9.0-py3-none-any.whl", hash = "sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd"},
-    {file = "typing_extensions-4.9.0.tar.gz", hash = "sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783"},
+    {file = "typing_extensions-4.11.0-py3-none-any.whl", hash = "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"},
+    {file = "typing_extensions-4.11.0.tar.gz", hash = "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0"},
 ]
 
 [[package]]
 name = "ulid-py"
 version = "1.1.0"
 summary = "Universally Unique Lexicographically Sortable Identifier"
 groups = ["default"]
 files = [
     {file = "ulid-py-1.1.0.tar.gz", hash = "sha256:dc6884be91558df077c3011b9fb0c87d1097cb8fc6534b11f310161afd5738f0"},
     {file = "ulid_py-1.1.0-py2.py3-none-any.whl", hash = "sha256:b56a0f809ef90d6020b21b89a87a48edc7c03aea80e5ed5174172e82d76e3987"},
 ]
 
 [[package]]
 name = "wcmatch"
-version = "8.5.1"
+version = "8.5.2"
 requires_python = ">=3.8"
 summary = "Wildcard/glob file name matcher."
 groups = ["dev"]
 dependencies = [
     "bracex>=2.1.1",
 ]
 files = [
-    {file = "wcmatch-8.5.1-py3-none-any.whl", hash = "sha256:24c19cedc92bc9c9e27f39db4e1824d72f95bd2cea32b254a47a45b1a1b227ed"},
-    {file = "wcmatch-8.5.1.tar.gz", hash = "sha256:c0088c7f6426cf6bf27e530e2b7b734031905f7e490475fd83c7c5008ab581b3"},
+    {file = "wcmatch-8.5.2-py3-none-any.whl", hash = "sha256:17d3ad3758f9d0b5b4dedc770b65420d4dac62e680229c287bf24c9db856a478"},
+    {file = "wcmatch-8.5.2.tar.gz", hash = "sha256:a70222b86dea82fb382dd87b73278c10756c138bd6f8f714e2183128887b9eb2"},
 ]
 
 [[package]]
 name = "wcwidth"
 version = "0.2.13"
 summary = "Measures the displayed width of unicode strings in a terminal"
 groups = ["dev"]
```

### Comparing `karp_lex_types-0.6.5/ruff.toml` & `karp_lex_types-0.7.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/src/karp_lex_types/commands/__init__.py` & `karp_lex_types-0.7.0/src/karp_lex_types/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/src/karp_lex_types/commands/base.py` & `karp_lex_types-0.7.0/src/karp_lex_types/commands/base.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/src/karp_lex_types/commands/entry_commands.py` & `karp_lex_types-0.7.0/src/karp_lex_types/commands/entry_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/src/karp_lex_types/commands/entry_repo_commands.py` & `karp_lex_types-0.7.0/src/karp_lex_types/commands/entry_repo_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/src/karp_lex_types/commands/resource_commands.py` & `karp_lex_types-0.7.0/src/karp_lex_types/commands/resource_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/src/karp_lex_types/dtos/entry_dto.py` & `karp_lex_types-0.7.0/src/karp_lex_types/dtos/entry_dto.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/src/karp_lex_types/value_objects/unique_id.py` & `karp_lex_types-0.7.0/src/karp_lex_types/value_objects/unique_id.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,25 +23,31 @@
         json_schema.update(examples=["01BJQMF54D093DXEAWZ6JYRPAQ"])
         return json_schema
 
     @classmethod
     def __get_pydantic_core_schema__(  # noqa: D105, PLW3201
         cls, source: typing.Any, handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
+        def _serialize(instance: typing.Any, info: typing.Any) -> typing.Any:
+            return instance.to_string() if info.mode == "json" else instance
+
         from_any_schema = core_schema.chain_schema(
             [
                 core_schema.any_schema(),
                 core_schema.no_info_plain_validator_function(cls.validate),
             ]
         )
         return core_schema.json_or_python_schema(
             json_schema=from_any_schema,
             python_schema=core_schema.union_schema(
                 [core_schema.is_instance_schema(ulid.ULID), from_any_schema]
             ),
+            serialization=core_schema.plain_serializer_function_ser_schema(
+                _serialize, info_arg=True
+            ),
         )
 
     @classmethod
     def validate(cls, v) -> "UniqueId":  # noqa: D102
         if isinstance(v, UniqueId):
             return v  # type: ignore
         if isinstance(v, ulid.ULID):
```

### Comparing `karp_lex_types-0.6.5/tests/entry_dto_unit_test.py` & `karp_lex_types-0.7.0/tests/entry_dto_unit_test.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/tests/requirements-testing.lock` & `karp_lex_types-0.7.0/tests/requirements-testing.lock`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 # This file is @generated by PDM.
 # Please do not edit it manually.
 
-annotated-types==0.6.0 \
-    --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
-    --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
+annotated-types==0.7.0 \
+    --hash=sha256:1f02e8b43a8fbbc3f3e0d4f0f4bfc8131bcb4eebe8849b8e5c773f3a1c582a53 \
+    --hash=sha256:aff07c09a53a08bc8cfccb9c85b05f1aa9a2a6f23728d790723543408344ce89
 bracex==2.4 \
     --hash=sha256:a27eaf1df42cf561fed58b7a8f3fdf129d1ea16a81e1fadd1d17989bc6384beb \
     --hash=sha256:efdc71eff95eaff5e0f8cfebe7d01adf2c8637c8c92edaf63ef348c241a82418
-bump-my-version==0.21.0 \
-    --hash=sha256:a614d8176b5ac0e644239c9a8a246b696d316f68406fd78b8486a9e13fc93266 \
-    --hash=sha256:c3f1a31e32345679b517cbba99a0875457ee45d7ba6189fcd2a74d3ddae41515
+bump-my-version==0.21.1 \
+    --hash=sha256:946a7edcf30c5a8574c579684df983136ea395f70c184e4db32eb3e307584c14 \
+    --hash=sha256:ec612474e9e790c3fbbfed153a10b356f84fc15096ceff181b399d5e985bfacc
 click==8.1.7 \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
 colorama==0.4.6; sys_platform == "win32" or platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-coverage==7.4.1 \
-    --hash=sha256:0193657651f5399d433c92f8ae264aff31fc1d066deee4b831549526433f3f61 \
-    --hash=sha256:02f2edb575d62172aa28fe00efe821ae31f25dc3d589055b3fb64d51e52e4ab1 \
-    --hash=sha256:077d366e724f24fc02dbfe9d946534357fda71af9764ff99d73c3c596001bbd7 \
-    --hash=sha256:18e961aa13b6d47f758cc5879383d27b5b3f3dcd9ce8cdbfdc2571fe86feb4dd \
-    --hash=sha256:1ed4b95480952b1a26d863e546fa5094564aa0065e1e5f0d4d0041f293251d04 \
-    --hash=sha256:23b27b8a698e749b61809fb637eb98ebf0e505710ec46a8aa6f1be7dc0dc43a6 \
-    --hash=sha256:32a8d985462e37cfdab611a6f95b09d7c091d07668fdc26e47a725ee575fe166 \
-    --hash=sha256:3468cc8720402af37b6c6e7e2a9cdb9f6c16c728638a2ebc768ba1ef6f26c3a1 \
-    --hash=sha256:3cacfaefe6089d477264001f90f55b7881ba615953414999c46cc9713ff93c8c \
-    --hash=sha256:3e3424c554391dc9ef4a92ad28665756566a28fecf47308f91841f6c49288e66 \
-    --hash=sha256:536d609c6963c50055bab766d9951b6c394759190d03311f3e9fcf194ca909e1 \
-    --hash=sha256:5d6850e6e36e332d5511a48a251790ddc545e16e8beaf046c03985c69ccb2676 \
-    --hash=sha256:6008adeca04a445ea6ef31b2cbaf1d01d02986047606f7da266629afee982630 \
-    --hash=sha256:6b00e21f86598b6330f0019b40fb397e705135040dbedc2ca9a93c7441178e74 \
-    --hash=sha256:6dceb61d40cbfcf45f51e59933c784a50846dc03211054bd76b421a713dcdf19 \
-    --hash=sha256:7ac8f8eb153724f84885a1374999b7e45734bf93a87d8df1e7ce2146860edef6 \
-    --hash=sha256:85ccc5fa54c2ed64bd91ed3b4a627b9cce04646a659512a051fa82a92c04a448 \
-    --hash=sha256:869b5046d41abfea3e381dd143407b0d29b8282a904a19cb908fa24d090cc018 \
-    --hash=sha256:9d2f9d4cc2a53b38cabc2d6d80f7f9b7e3da26b2f53d48f05876fef7956b6968 \
-    --hash=sha256:a3277f5fa7483c927fe3a7b017b39351610265308f5267ac6d4c2b64cc1d8d25 \
-    --hash=sha256:b8ffb498a83d7e0305968289441914154fb0ef5d8b3157df02a90c6695978295 \
-    --hash=sha256:b9bb62fac84d5f2ff523304e59e5c439955fb3b7f44e3d7b2085184db74d733b \
-    --hash=sha256:c61f66d93d712f6e03369b6a7769233bfda880b12f417eefdd4f16d1deb2fc4c \
-    --hash=sha256:ca6e61dc52f601d1d224526360cdeab0d0712ec104a2ce6cc5ccef6ed9a233bc \
-    --hash=sha256:ca7b26a5e456a843b9b6683eada193fc1f65c761b3a473941efe5a291f604c74 \
-    --hash=sha256:d17bbc946f52ca67adf72a5ee783cd7cd3477f8f8796f59b4974a9b59cacc9ee \
-    --hash=sha256:dfd1e1b9f0898817babf840b77ce9fe655ecbe8b1b327983df485b30df8cc011 \
-    --hash=sha256:e0860a348bf7004c812c8368d1fc7f77fe8e4c095d661a579196a9533778e156 \
-    --hash=sha256:f3771b23bb3675a06f5d885c3630b1d01ea6cac9e84a01aaf5508706dba546c5 \
-    --hash=sha256:f68ef3660677e6624c8cace943e4765545f8191313a07288a53d3da188bd8581 \
-    --hash=sha256:f86f368e1c7ce897bf2457b9eb61169a44e2ef797099fb5728482b8d69f3f016 \
-    --hash=sha256:fe558371c1bdf3b8fa03e097c523fb9645b8730399c14fe7721ee9c9e2a545d3
-exceptiongroup==1.2.0; python_version < "3.11" \
-    --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
-    --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
+coverage==7.5.1 \
+    --hash=sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d \
+    --hash=sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2 \
+    --hash=sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34 \
+    --hash=sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f \
+    --hash=sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a \
+    --hash=sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35 \
+    --hash=sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223 \
+    --hash=sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746 \
+    --hash=sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c \
+    --hash=sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca \
+    --hash=sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596 \
+    --hash=sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd \
+    --hash=sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e \
+    --hash=sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3 \
+    --hash=sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e \
+    --hash=sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312 \
+    --hash=sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7 \
+    --hash=sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572 \
+    --hash=sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428 \
+    --hash=sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07 \
+    --hash=sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e \
+    --hash=sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136 \
+    --hash=sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8 \
+    --hash=sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228 \
+    --hash=sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206 \
+    --hash=sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa \
+    --hash=sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e \
+    --hash=sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057 \
+    --hash=sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146 \
+    --hash=sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8 \
+    --hash=sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987 \
+    --hash=sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19
+exceptiongroup==1.2.1; python_version < "3.11" \
+    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
+    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
     --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
 mdurl==0.1.2 \
@@ -78,106 +78,106 @@
     --hash=sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051 \
     --hash=sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2 \
     --hash=sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7 \
     --hash=sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
-packaging==23.2 \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
+packaging==24.0 \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
 pluggy==1.5.0 \
     --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
     --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
 prompt-toolkit==3.0.36 \
     --hash=sha256:3e163f254bef5a03b146397d7c1963bd3e2812f0964bb9a24e6ec761fd28db63 \
     --hash=sha256:aa64ad242a462c5ff0363a7b9cfe696c20d55d9fc60c11fd8e632d064804d305
-pydantic==2.6.3 \
-    --hash=sha256:72c6034df47f46ccdf81869fddb81aade68056003900a8724a4f160700016a2a \
-    --hash=sha256:e07805c4c7f5c6826e33a1d4c9d47950d7eaf34868e2690f8594d2e30241f11f
-pydantic-core==2.16.3 \
-    --hash=sha256:00ee1c97b5364b84cb0bd82e9bbf645d5e2871fb8c58059d158412fee2d33d8a \
-    --hash=sha256:0d32576b1de5a30d9a97f300cc6a3f4694c428d956adbc7e6e2f9cad279e45ed \
-    --hash=sha256:0df446663464884297c793874573549229f9eca73b59360878f382a0fc085979 \
-    --hash=sha256:0f56ae86b60ea987ae8bcd6654a887238fd53d1384f9b222ac457070b7ac4cff \
-    --hash=sha256:162e498303d2b1c036b957a1278fa0899d02b2842f1ff901b6395104c5554a45 \
-    --hash=sha256:1b662180108c55dfbf1280d865b2d116633d436cfc0bba82323554873967b340 \
-    --hash=sha256:1cac689f80a3abab2d3c0048b29eea5751114054f032a941a32de4c852c59cad \
-    --hash=sha256:287073c66748f624be4cef893ef9174e3eb88fe0b8a78dc22e88eca4bc357ca6 \
-    --hash=sha256:2a72fb9963cba4cd5793854fd12f4cfee731e86df140f59ff52a49b3552db241 \
-    --hash=sha256:2acca2be4bb2f2147ada8cac612f8a98fc09f41c89f87add7256ad27332c2fda \
-    --hash=sha256:2f583bd01bbfbff4eaee0868e6fc607efdfcc2b03c1c766b06a707abbc856187 \
-    --hash=sha256:33809aebac276089b78db106ee692bdc9044710e26f24a9a2eaa35a0f9fa70ba \
-    --hash=sha256:36fa178aacbc277bc6b62a2c3da95226520da4f4e9e206fdf076484363895d2c \
-    --hash=sha256:4204e773b4b408062960e65468d5346bdfe139247ee5f1ca2a378983e11388a2 \
-    --hash=sha256:456855f57b413f077dff513a5a28ed838dbbb15082ba00f80750377eed23d132 \
-    --hash=sha256:49d5d58abd4b83fb8ce763be7794d09b2f50f10aa65c0f0c1696c677edeb7cbf \
-    --hash=sha256:4df8a199d9f6afc5ae9a65f8f95ee52cae389a8c6b20163762bde0426275b7db \
-    --hash=sha256:500960cb3a0543a724a81ba859da816e8cf01b0e6aaeedf2c3775d12ee49cade \
-    --hash=sha256:519ae0312616026bf4cedc0fe459e982734f3ca82ee8c7246c19b650b60a5ee4 \
-    --hash=sha256:5c5cbc703168d1b7a838668998308018a2718c2130595e8e190220238addc96f \
-    --hash=sha256:6162f8d2dc27ba21027f261e4fa26f8bcb3cf9784b7f9499466a311ac284b5b9 \
-    --hash=sha256:716b542728d4c742353448765aa7cdaa519a7b82f9564130e2b3f6766018c9ec \
-    --hash=sha256:732da3243e1b8d3eab8c6ae23ae6a58548849d2e4a4e03a1924c8ddf71a387cb \
-    --hash=sha256:75b81e678d1c1ede0785c7f46690621e4c6e63ccd9192af1f0bd9d504bbb6bf4 \
-    --hash=sha256:75f76ee558751746d6a38f89d60b6228fa174e5172d143886af0f85aa306fd89 \
-    --hash=sha256:86b3d0033580bd6bbe07590152007275bd7af95f98eaa5bd36f3da219dcd93da \
-    --hash=sha256:8d62da299c6ecb04df729e4b5c52dc0d53f4f8430b4492b93aa8de1f541c4aac \
-    --hash=sha256:8e47755d8152c1ab5b55928ab422a76e2e7b22b5ed8e90a7d584268dd49e9c6b \
-    --hash=sha256:936e5db01dd49476fa8f4383c259b8b1303d5dd5fb34c97de194560698cc2c5e \
-    --hash=sha256:99b6add4c0b39a513d323d3b93bc173dac663c27b99860dd5bf491b240d26137 \
-    --hash=sha256:9c865a7ee6f93783bd5d781af5a4c43dadc37053a5b42f7d18dc019f8c9d2bd1 \
-    --hash=sha256:a425479ee40ff021f8216c9d07a6a3b54b31c8267c6e17aa88b70d7ebd0e5e5b \
-    --hash=sha256:a6b1bb0827f56654b4437955555dc3aeeebeddc47c2d7ed575477f082622c49e \
-    --hash=sha256:aaf09e615a0bf98d406657e0008e4a8701b11481840be7d31755dc9f97c44053 \
-    --hash=sha256:b29eeb887aa931c2fcef5aa515d9d176d25006794610c264ddc114c053bf96fe \
-    --hash=sha256:b3992a322a5617ded0a9f23fd06dbc1e4bd7cf39bc4ccf344b10f80af58beacd \
-    --hash=sha256:b60cc1a081f80a2105a59385b92d82278b15d80ebb3adb200542ae165cd7d183 \
-    --hash=sha256:b926dd38db1519ed3043a4de50214e0d600d404099c3392f098a7f9d75029ff8 \
-    --hash=sha256:bd87f48924f360e5d1c5f770d6155ce0e7d83f7b4e10c2f9ec001c73cf475c99 \
-    --hash=sha256:c9bd22a2a639e26171068f8ebb5400ce2c1bc7d17959f60a3b753ae13c632975 \
-    --hash=sha256:cbcc558401de90a746d02ef330c528f2e668c83350f045833543cd57ecead1ad \
-    --hash=sha256:cf6204fe865da605285c34cf1172879d0314ff267b1c35ff59de7154f35fdc2e \
-    --hash=sha256:d33dd21f572545649f90c38c227cc8631268ba25c460b5569abebdd0ec5974ca \
-    --hash=sha256:d89ca19cdd0dd5f31606a9329e309d4fcbb3df860960acec32630297d61820df \
-    --hash=sha256:dcca5d2bf65c6fb591fff92da03f94cd4f315972f97c21975398bd4bd046854a \
-    --hash=sha256:ded1c35f15c9dea16ead9bffcde9bb5c7c031bff076355dc58dcb1cb436c4721 \
-    --hash=sha256:e56f8186d6210ac7ece503193ec84104da7ceb98f68ce18c07282fcc2452e76f \
-    --hash=sha256:e7c6ed0dc9d8e65f24f5824291550139fe6f37fac03788d4580da0d33bc00c97 \
-    --hash=sha256:ec08be75bb268473677edb83ba71e7e74b43c008e4a7b1907c6d57e940bf34b6 \
-    --hash=sha256:ed25e1835c00a332cb10c683cd39da96a719ab1dfc08427d476bce41b92531fc \
-    --hash=sha256:f4cb85f693044e0f71f394ff76c98ddc1bc0953e48c061725e540396d5c8a2e1 \
-    --hash=sha256:f53aace168a2a10582e570b7736cc5bef12cae9cf21775e3eafac597e8551fbe \
-    --hash=sha256:f651dd19363c632f4abe3480a7c87a9773be27cfe1341aef06e8759599454120 \
-    --hash=sha256:fc4ad7f7ee1a13d9cb49d8198cd7d7e3aa93e425f371a68235f784e99741561f \
-    --hash=sha256:fee427241c2d9fb7192b658190f9f5fd6dfe41e02f3c1489d2ec1e6a5ab1e04a
+pydantic==2.7.1 \
+    --hash=sha256:e029badca45266732a9a79898a15ae2e8b14840b1eabbb25844be28f0b33f3d5 \
+    --hash=sha256:e9dbb5eada8abe4d9ae5f46b9939aead650cd2b68f249bb3a8139dbe125803cc
+pydantic-core==2.18.2 \
+    --hash=sha256:0098300eebb1c837271d3d1a2cd2911e7c11b396eac9661655ee524a7f10587b \
+    --hash=sha256:05b7133a6e6aeb8df37d6f413f7705a37ab4031597f64ab56384c94d98fa0e90 \
+    --hash=sha256:0680b1f1f11fda801397de52c36ce38ef1c1dc841a0927a94f226dea29c3ae3d \
+    --hash=sha256:1404c69d6a676245199767ba4f633cce5f4ad4181f9d0ccb0577e1f66cf4c46d \
+    --hash=sha256:182245ff6b0039e82b6bb585ed55a64d7c81c560715d1bad0cbad6dfa07b4027 \
+    --hash=sha256:20aca1e2298c56ececfd8ed159ae4dde2df0781988c97ef77d5c16ff4bd5b400 \
+    --hash=sha256:219da3f096d50a157f33645a1cf31c0ad1fe829a92181dd1311022f986e5fbe3 \
+    --hash=sha256:223ee893d77a310a0391dca6df00f70bbc2f36a71a895cecd9a0e762dc37b349 \
+    --hash=sha256:224c421235f6102e8737032483f43c1a8cfb1d2f45740c44166219599358c2cd \
+    --hash=sha256:2334ce8c673ee93a1d6a65bd90327588387ba073c17e61bf19b4fd97d688d63c \
+    --hash=sha256:269322dcc3d8bdb69f054681edff86276b2ff972447863cf34c8b860f5188e2e \
+    --hash=sha256:2728b01246a3bba6de144f9e3115b532ee44bd6cf39795194fb75491824a1413 \
+    --hash=sha256:2b8ed04b3582771764538f7ee7001b02e1170223cf9b75dff0bc698fadb00cf3 \
+    --hash=sha256:2e29d20810dfc3043ee13ac7d9e25105799817683348823f305ab3f349b9386e \
+    --hash=sha256:36789b70d613fbac0a25bb07ab3d9dba4d2e38af609c020cf4d888d165ee0bf3 \
+    --hash=sha256:3a6515ebc6e69d85502b4951d89131ca4e036078ea35533bb76327f8424531ce \
+    --hash=sha256:3f9a801e7c8f1ef8718da265bba008fa121243dfe37c1cea17840b0944dfd72c \
+    --hash=sha256:43f0f463cf89ace478de71a318b1b4f05ebc456a9b9300d027b4b57c1a2064fb \
+    --hash=sha256:4456f2dca97c425231d7315737d45239b2b51a50dc2b6f0c2bb181fce6207664 \
+    --hash=sha256:470b94480bb5ee929f5acba6995251ada5e059a5ef3e0dfc63cca287283ebfa6 \
+    --hash=sha256:4b4356d3538c3649337df4074e81b85f0616b79731fe22dd11b99499b2ebbdf3 \
+    --hash=sha256:553ef617b6836fc7e4df130bb851e32fe357ce36336d897fd6646d6058d980af \
+    --hash=sha256:6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043 \
+    --hash=sha256:6e5c584d357c4e2baf0ff7baf44f4994be121e16a2c88918a5817331fc7599d7 \
+    --hash=sha256:75250dbc5290e3f1a0f4618db35e51a165186f9034eff158f3d490b3fed9f8a0 \
+    --hash=sha256:75f7e9488238e920ab6204399ded280dc4c307d034f3924cd7f90a38b1829563 \
+    --hash=sha256:7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72 \
+    --hash=sha256:800d60565aec896f25bc3cfa56d2277d52d5182af08162f7954f938c06dc4ee3 \
+    --hash=sha256:886eec03591b7cf058467a70a87733b35f44707bd86cf64a615584fd72488b7c \
+    --hash=sha256:8b172601454f2d7701121bbec3425dd71efcb787a027edf49724c9cefc14c038 \
+    --hash=sha256:95b9d5e72481d3780ba3442eac863eae92ae43a5f3adb5b4d0a1de89d42bb250 \
+    --hash=sha256:98758d627ff397e752bc339272c14c98199c613f922d4a384ddc07526c86a2ec \
+    --hash=sha256:997abc4df705d1295a42f95b4eec4950a37ad8ae46d913caeee117b6b198811c \
+    --hash=sha256:9b5155ff768083cb1d62f3e143b49a8a3432e6789a3abee8acd005c3c7af1c74 \
+    --hash=sha256:9e08e867b306f525802df7cd16c44ff5ebbe747ff0ca6cf3fde7f36c05a59a81 \
+    --hash=sha256:a1874c6dd4113308bd0eb568418e6114b252afe44319ead2b4081e9b9521fe75 \
+    --hash=sha256:b14d82cdb934e99dda6d9d60dc84a24379820176cc4a0d123f88df319ae9c150 \
+    --hash=sha256:b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438 \
+    --hash=sha256:b3ef08e20ec49e02d5c6717a91bb5af9b20f1805583cb0adfe9ba2c6b505b5ae \
+    --hash=sha256:b89ed9eb7d616ef5714e5590e6cf7f23b02d0d539767d33561e3675d6f9e3857 \
+    --hash=sha256:c4fcf5cd9c4b655ad666ca332b9a081112cd7a58a8b5a6ca7a3104bc950f2038 \
+    --hash=sha256:c6fdc8627910eed0c01aed6a390a252fe3ea6d472ee70fdde56273f198938374 \
+    --hash=sha256:c9bd70772c720142be1020eac55f8143a34ec9f82d75a8e7a07852023e46617f \
+    --hash=sha256:ca7b0c1f1c983e064caa85f3792dd2fe3526b3505378874afa84baf662e12241 \
+    --hash=sha256:cbca948f2d14b09d20268cda7b0367723d79063f26c4ffc523af9042cad95592 \
+    --hash=sha256:cc1cfd88a64e012b74e94cd00bbe0f9c6df57049c97f02bb07d39e9c852e19a4 \
+    --hash=sha256:ccdd111c03bfd3666bd2472b674c6899550e09e9f298954cfc896ab92b5b0e6d \
+    --hash=sha256:d7d904828195733c183d20a54230c0df0eb46ec746ea1a666730787353e87182 \
+    --hash=sha256:e18609ceaa6eed63753037fc06ebb16041d17d28199ae5aba0052c51449650a9 \
+    --hash=sha256:e1b395e58b10b73b07b7cf740d728dd4ff9365ac46c18751bf8b3d8cca8f625a \
+    --hash=sha256:e23ec367a948b6d812301afc1b13f8094ab7b2c280af66ef450efc357d2ae543 \
+    --hash=sha256:e6dac87ddb34aaec85f873d737e9d06a3555a1cc1a8e0c44b7f8d5daeb89d86f \
+    --hash=sha256:ef26c9e94a8c04a1b2924149a9cb081836913818e55681722d7f29af88fe7b38 \
+    --hash=sha256:f0a21cbaa69900cbe1a2e7cad2aa74ac3cf21b10c3efb0fa0b80305274c0e8a2 \
+    --hash=sha256:fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
 pydantic-settings==2.2.1 \
     --hash=sha256:00b9f6a5e95553590434c0fa01ead0b216c3e10bc54ae02e37f359948643c5ed \
     --hash=sha256:0235391d26db4d2190cb9b31051c4b46882d28a51533f97440867f012d4da091
 pygments==2.18.0 \
     --hash=sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199 \
     --hash=sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
-pytest==8.2.0 \
-    --hash=sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233 \
-    --hash=sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f
+pytest==8.2.1 \
+    --hash=sha256:5046e5b46d8e4cac199c373041f26be56fdb81eb4e67dc11d4e10811fc3408fd \
+    --hash=sha256:faccc5d332b8c3719f40283d0d44aa5cf101cec36f88cde9ed8f2bc0538612b1
 pytest-cov==5.0.0 \
     --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
     --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
 python-dotenv==1.0.1 \
     --hash=sha256:e324ee90a023d808f1959c46bcbc04446a10ced277783dc6ee09987c37ec10ca \
     --hash=sha256:f7b63ef50f1b690dddf550d03497b66d609393b40b564ed0d674909a68ebf16a
 questionary==2.0.1 \
     --hash=sha256:8ab9a01d0b91b68444dff7f6652c1e754105533f083cbe27597c8110ecc230a2 \
     --hash=sha256:bcce898bf3dbb446ff62830c86c5c6fb9a22a54146f0f5597d3da43b10d8fc8b
 rich==13.7.1 \
     --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
     --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
-rich-click==1.8.1 \
-    --hash=sha256:0cf0bf84404e78379bd2722db88cb07ffd0535440e20a05943d5b02249d90f8a \
-    --hash=sha256:73c2ec88a66d7bf6b8c32783539d1c9c92c7c75847f14186092d27f83b206e8a
+rich-click==1.8.2 \
+    --hash=sha256:8e29bdede858b59aa2859a1ab1c4ccbd39ed7ed5870262dae756fba6b5dc72e8 \
+    --hash=sha256:b57856f304e4fe0394b82d7ce0784450758f8c8b4e201ccc4320501cc201806b
 ruff==0.4.4 \
     --hash=sha256:1aecced1269481ef2894cc495647392a34b0bf3e28ff53ed95a385b13aa45768 \
     --hash=sha256:29d44ef5bb6a08e235c8249294fa8d431adc1426bfda99ed493119e6f9ea1bf6 \
     --hash=sha256:39df0537b47d3b597293edbb95baf54ff5b49589eb7ff41926d8243caa995ea6 \
     --hash=sha256:424e5b72597482543b684c11def82669cc6b395aa8cc69acc1858b5ef3e5daae \
     --hash=sha256:4c8e2f1e8fc12d07ab521a9005d68a969e167b589cbcaee354cb61e9d9de9c15 \
     --hash=sha256:60ed88b636a463214905c002fa3eaab19795679ed55529f91e488db3fe8976ab \
@@ -194,19 +194,19 @@
     --hash=sha256:f87ea42d5cdebdc6a69761a9d0bc83ae9b3b30d0ad78952005ba6568d6c022af
 tomli==2.0.1; python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
 tomlkit==0.12.5 \
     --hash=sha256:af914f5a9c59ed9d0762c7b64d3b5d5df007448eb9cd2edc8a46b1eafead172f \
     --hash=sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c
-typing-extensions==4.9.0 \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
 ulid-py==1.1.0 \
     --hash=sha256:b56a0f809ef90d6020b21b89a87a48edc7c03aea80e5ed5174172e82d76e3987 \
     --hash=sha256:dc6884be91558df077c3011b9fb0c87d1097cb8fc6534b11f310161afd5738f0
-wcmatch==8.5.1 \
-    --hash=sha256:24c19cedc92bc9c9e27f39db4e1824d72f95bd2cea32b254a47a45b1a1b227ed \
-    --hash=sha256:c0088c7f6426cf6bf27e530e2b7b734031905f7e490475fd83c7c5008ab581b3
+wcmatch==8.5.2 \
+    --hash=sha256:17d3ad3758f9d0b5b4dedc770b65420d4dac62e680229c287bf24c9db856a478 \
+    --hash=sha256:a70222b86dea82fb382dd87b73278c10756c138bd6f8f714e2183128887b9eb2
 wcwidth==0.2.13 \
     --hash=sha256:3da69048e4540d84af32131829ff948f1e022c1c6bdb8d6102117aac784f6859 \
     --hash=sha256:72ea0c06399eb286d978fdedb6923a9eb47e1c486ce63e9b4e64fc18303972b5
```

### Comparing `karp_lex_types-0.6.5/tests/test_entry_commands.py` & `karp_lex_types-0.7.0/tests/test_entry_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/tests/test_resource_commands.py` & `karp_lex_types-0.7.0/tests/test_resource_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/tests/test_unique_id.py` & `karp_lex_types-0.7.0/tests/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/.gitignore` & `karp_lex_types-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/LICENSE` & `karp_lex_types-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/README.md` & `karp_lex_types-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.5/pyproject.toml` & `karp_lex_types-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 license = { text = "MIT" }
 requires-python = ">=3.10"
 dependencies = ["pydantic>=2.5.3", "ulid-py>=1.1.0"]
 name = "karp-lex-types"
-version = "0.6.5"
+version = "0.7.0"
 description = "The types of karp-lex"
 readme = "README.md"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/spraakbanken/karp-lex-types/issues"
 homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/karp-lex-types"
```

### Comparing `karp_lex_types-0.6.5/PKG-INFO` & `karp_lex_types-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: karp-lex-types
-Version: 0.6.5
+Version: 0.7.0
 Summary: The types of karp-lex
 Project-URL: Bug Tracker, https://github.com/spraakbanken/karp-lex-types/issues
 Project-URL: homepage, https://spraakbanken.gu.se
 Project-URL: repository, https://github.com/spraakbanken/karp-lex-types
 Project-URL: documentation, https://github.com/spraakbanken/karp-lex-types
 Author-email: Språkbanken Text <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
 License: MIT
```

