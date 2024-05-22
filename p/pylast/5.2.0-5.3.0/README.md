# Comparing `tmp/pylast-5.2.0.tar.gz` & `tmp/pylast-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jun  6 16:24:16 2023, max compression
+gzip compressed data, last modified: Wed May 22 19:50:30 2024, max compression
```

## Comparing `pylast-5.2.0.tar` & `pylast-5.3.0.tar`

### file list

```diff
@@ -1,41 +1,39 @@
--rw-r--r--   0        0        0      240 2023-06-06 16:24:16.000000 pylast-5.2.0/.codecov.yml
--rw-r--r--   0        0        0      313 2023-06-06 16:24:16.000000 pylast-5.2.0/.editorconfig
--rw-r--r--   0        0        0       30 2023-06-06 16:24:16.000000 pylast-5.2.0/.flake8
--rw-r--r--   0        0        0     1454 2023-06-06 16:24:16.000000 pylast-5.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      164 2023-06-06 16:24:16.000000 pylast-5.2.0/.scrutinizer.yml
--rw-r--r--   0        0        0     4762 2023-06-06 16:24:16.000000 pylast-5.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      817 2023-06-06 16:24:16.000000 pylast-5.2.0/RELEASING.md
--rw-r--r--   0        0        0      138 2023-06-06 16:24:16.000000 pylast-5.2.0/example_test_pylast.yaml
--rw-r--r--   0        0        0      110 2023-06-06 16:24:16.000000 pylast-5.2.0/pytest.ini
--rw-r--r--   0        0        0      568 2023-06-06 16:24:16.000000 pylast-5.2.0/tox.ini
--rw-r--r--   0        0        0       15 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      442 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0       61 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     2631 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/labels.yml
--rw-r--r--   0        0        0      892 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      255 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/renovate.json
--rw-r--r--   0        0        0     1755 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      298 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      490 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1414 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0    88620 2023-06-06 16:24:16.000000 pylast-5.2.0/src/pylast/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/__init__.py
--rwxr-xr-x   0        0        0     3029 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_album.py
--rwxr-xr-x   0        0        0     7947 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_artist.py
--rwxr-xr-x   0        0        0      895 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_country.py
--rwxr-xr-x   0        0        0     1406 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_library.py
--rwxr-xr-x   0        0        0     1103 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_librefm.py
--rwxr-xr-x   0        0        0    12849 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_network.py
--rwxr-xr-x   0        0        0     3951 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_pylast.py
--rwxr-xr-x   0        0        0     1436 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_tag.py
--rwxr-xr-x   0        0        0     6546 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_track.py
--rwxr-xr-x   0        0        0    14387 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_user.py
--rw-r--r--   0        0        0     1866 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/unicode_test.py
--rw-r--r--   0        0        0      840 2023-06-06 16:24:16.000000 pylast-5.2.0/.gitignore
--rw-r--r--   0        0        0     9115 2023-06-06 16:24:16.000000 pylast-5.2.0/COPYING
--rw-r--r--   0        0        0    11359 2023-06-06 16:24:16.000000 pylast-5.2.0/LICENSE.txt
--rw-r--r--   0        0        0     5723 2023-06-06 16:24:16.000000 pylast-5.2.0/README.md
--rw-r--r--   0        0        0     1641 2023-06-06 16:24:16.000000 pylast-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     7323 2023-06-06 16:24:16.000000 pylast-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0      240 2024-05-22 19:50:30.000000 pylast-5.3.0/.codecov.yml
+-rw-r--r--   0        0        0      313 2024-05-22 19:50:30.000000 pylast-5.3.0/.editorconfig
+-rw-r--r--   0        0        0     1851 2024-05-22 19:50:30.000000 pylast-5.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4771 2024-05-22 19:50:30.000000 pylast-5.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      823 2024-05-22 19:50:30.000000 pylast-5.3.0/RELEASING.md
+-rw-r--r--   0        0        0      134 2024-05-22 19:50:30.000000 pylast-5.3.0/example_test_pylast.yaml
+-rw-r--r--   0        0        0      110 2024-05-22 19:50:30.000000 pylast-5.3.0/pytest.ini
+-rw-r--r--   0        0        0      662 2024-05-22 19:50:30.000000 pylast-5.3.0/tox.ini
+-rw-r--r--   0        0        0       15 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      442 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0       61 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2631 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/labels.yml
+-rw-r--r--   0        0        0      892 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      350 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/renovate.json
+-rw-r--r--   0        0        0     1725 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      389 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      377 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      517 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1379 2024-05-22 19:50:30.000000 pylast-5.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0    88823 2024-05-22 19:50:30.000000 pylast-5.3.0/src/pylast/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/__init__.py
+-rwxr-xr-x   0        0        0     3065 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_album.py
+-rwxr-xr-x   0        0        0     7983 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_artist.py
+-rwxr-xr-x   0        0        0      931 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_country.py
+-rwxr-xr-x   0        0        0     1442 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_library.py
+-rwxr-xr-x   0        0        0     1139 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_librefm.py
+-rwxr-xr-x   0        0        0    12886 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_network.py
+-rwxr-xr-x   0        0        0     3987 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_pylast.py
+-rwxr-xr-x   0        0        0     1472 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_tag.py
+-rwxr-xr-x   0        0        0     6511 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_track.py
+-rwxr-xr-x   0        0        0    14423 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/test_user.py
+-rw-r--r--   0        0        0     1906 2024-05-22 19:50:30.000000 pylast-5.3.0/tests/unicode_test.py
+-rw-r--r--   0        0        0      840 2024-05-22 19:50:30.000000 pylast-5.3.0/.gitignore
+-rw-r--r--   0        0        0     9112 2024-05-22 19:50:30.000000 pylast-5.3.0/COPYING
+-rw-r--r--   0        0        0    11359 2024-05-22 19:50:30.000000 pylast-5.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     5797 2024-05-22 19:50:30.000000 pylast-5.3.0/README.md
+-rw-r--r--   0        0        0     2303 2024-05-22 19:50:30.000000 pylast-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7400 2024-05-22 19:50:30.000000 pylast-5.3.0/PKG-INFO
```

### Comparing `pylast-5.2.0/.pre-commit-config.yaml` & `pylast-5.3.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,75 @@
 repos:
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.4
     hooks:
-      - id: pyupgrade
-        args: [--py38-plus]
+      - id: ruff
+        args: [--exit-non-zero-on-fix]
 
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
+  - repo: https://github.com/psf/black-pre-commit-mirror
+    rev: 24.4.2
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.16.0
     hooks:
       - id: blacken-docs
         args: [--target-version=py38]
-        additional_dependencies: [black==23.3.0]
-
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
-    hooks:
-      - id: flake8
-        additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
-
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.10.0
-    hooks:
-      - id: python-check-blanket-noqa
-      - id: python-no-log-warn
+        additional_dependencies: [black]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
+      - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-json
       - id: check-toml
       - id: check-yaml
+      - id: debug-statements
       - id: end-of-file-fixer
-      - id: requirements-txt-fixer
+      - id: forbid-submodules
+      - id: trailing-whitespace
+        exclude: .github/(ISSUE_TEMPLATE|PULL_REQUEST_TEMPLATE).md
+
+  - repo: https://github.com/python-jsonschema/check-jsonschema
+    rev: 0.28.4
+    hooks:
+      - id: check-github-workflows
+      - id: check-renovate
+
+  - repo: https://github.com/rhysd/actionlint
+    rev: v1.7.0
+    hooks:
+      - id: actionlint
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.10.0
+    rev: 1.7.0
     hooks:
       - id: pyproject-fmt
+        additional_dependencies: [tox]
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.13
+    rev: v0.18
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: 1.3.0
+    rev: 1.3.1
     hooks:
       - id: tox-ini-fmt
 
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v4.0.0-alpha.8
+    hooks:
+      - id: prettier
+        args: [--prose-wrap=always, --print-width=88]
+        exclude: .github/(ISSUE_TEMPLATE|PULL_REQUEST_TEMPLATE).md
+
+  - repo: meta
+    hooks:
+      - id: check-hooks-apply
+      - id: check-useless-excludes
+
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `pylast-5.2.0/CHANGELOG.md` & `pylast-5.3.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,125 +8,133 @@
 
 - https://github.com/pylast/pylast/releases
 
 ## [4.2.0] - 2021-03-14
 
 ## Changed
 
-* Fix unsafe creation of temp file for caching, and improve exception raising (#356) @kvanzuijlen
-* [pre-commit.ci] pre-commit autoupdate (#362) @pre-commit-ci
-
+- Fix unsafe creation of temp file for caching, and improve exception raising (#356)
+  @kvanzuijlen
+- [pre-commit.ci] pre-commit autoupdate (#362) @pre-commit-ci
 
 ## [4.1.0] - 2021-01-04
+
 ## Added
 
-* Add support for streaming (#336) @kvanzuijlen
-* Add Python 3.9 final to Travis CI (#350) @sheetalsingala
+- Add support for streaming (#336) @kvanzuijlen
+- Add Python 3.9 final to Travis CI (#350) @sheetalsingala
 
 ## Changed
 
-* Update copyright year (#360) @hugovk
-* Replace Travis CI with GitHub Actions (#352) @hugovk
-* [pre-commit.ci] pre-commit autoupdate (#359) @pre-commit-ci
+- Update copyright year (#360) @hugovk
+- Replace Travis CI with GitHub Actions (#352) @hugovk
+- [pre-commit.ci] pre-commit autoupdate (#359) @pre-commit-ci
 
 ## Fixed
 
-* Set limit to 50 by default, not 1 (#355) @hugovk
-
+- Set limit to 50 by default, not 1 (#355) @hugovk
 
 ## [4.0.0] - 2020-10-07
+
 ## Added
 
-* Add support for Python 3.9 (#347) @hugovk
+- Add support for Python 3.9 (#347) @hugovk
 
 ## Removed
 
-* Remove deprecated `Artist.get_cover_image`, `User.get_artist_tracks` and `STATUS_TOKEN_ERROR` (#348) @hugovk
-* Drop support for EOL Python 3.5 (#346) @hugovk
-
+- Remove deprecated `Artist.get_cover_image`, `User.get_artist_tracks` and
+  `STATUS_TOKEN_ERROR` (#348) @hugovk
+- Drop support for EOL Python 3.5 (#346) @hugovk
 
 ## [3.3.0] - 2020-06-25
+
 ### Added
 
-* `User.get_now_playing`: Add album and cover image to info (#330) @hugovk
+- `User.get_now_playing`: Add album and cover image to info (#330) @hugovk
 
 ### Changed
 
-* Improve handling of error responses from the API (#327) @spiritualized
+- Improve handling of error responses from the API (#327) @spiritualized
 
 ### Deprecated
 
-* Deprecate `Artist.get_cover_image`, they're no longer available from Last.fm (#332) @hugovk
+- Deprecate `Artist.get_cover_image`, they're no longer available from Last.fm (#332)
+  @hugovk
 
 ### Fixed
 
-* Fix `artist.get_bio_content()` to return `None` if bio is empty (#326) @hugovk
-
+- Fix `artist.get_bio_content()` to return `None` if bio is empty (#326) @hugovk
 
 ## [3.2.1] - 2020-03-05
+
 ### Fixed
 
-* Only Python 3 is supported: don't create universal wheel (#318) @hugovk
-* Fix regression calling `get_recent_tracks` with `limit=None` (#320) @hugovk
-* Fix `DeprecationWarning`: Please use `assertRegex` instead (#323) @hugovk
+- Only Python 3 is supported: don't create universal wheel (#318) @hugovk
+- Fix regression calling `get_recent_tracks` with `limit=None` (#320) @hugovk
+- Fix `DeprecationWarning`: Please use `assertRegex` instead (#323) @hugovk
 
 ## [3.2.0] - 2020-01-03
+
 ### Added
 
-* Support for Python 3.8
-* Store album art URLs when you call `GetTopAlbums` ([#307])
-* Retry paging through results on exception ([#297])
-* More error status codes from https://last.fm/api/errorcodes ([#297])
+- Support for Python 3.8
+- Store album art URLs when you call `GetTopAlbums` ([#307])
+- Retry paging through results on exception ([#297])
+- More error status codes from https://last.fm/api/errorcodes ([#297])
 
 ### Changed
 
-* Respect `get_recent_tracks`' limit when there's a now playing track ([#310])
-* Move installable code to `src/` ([#301])
-* Update `get_weekly_artist_charts` docstring: only for `User` ([#311])
-* Remove Python 2 warnings, `python_requires` should be enough ([#312])
-* Use setuptools_scm to simplify versioning during release ([#316])
-* Various lint and test updates
+- Respect `get_recent_tracks`' limit when there's a now playing track ([#310])
+- Move installable code to `src/` ([#301])
+- Update `get_weekly_artist_charts` docstring: only for `User` ([#311])
+- Remove Python 2 warnings, `python_requires` should be enough ([#312])
+- Use setuptools_scm to simplify versioning during release ([#316])
+- Various lint and test updates
 
 ### Deprecated
 
-* Last.fm's `user.getArtistTracks` has now been deprecated by Last.fm and is no longer
+- Last.fm's `user.getArtistTracks` has now been deprecated by Last.fm and is no longer
   available. Last.fm returns a "Deprecated - This type of request is no longer
   supported" error when calling it. A future version of pylast will remove its
   `User.get_artist_tracks` altogether. ([#305])
 
-* `STATUS_TOKEN_ERROR` is deprecated and will be removed in a future version.
-  Use `STATUS_OPERATION_FAILED` instead.
+- `STATUS_TOKEN_ERROR` is deprecated and will be removed in a future version. Use
+  `STATUS_OPERATION_FAILED` instead.
 
 ## [3.1.0] - 2019-03-07
+
 ### Added
 
-* Extract username from session via new
+- Extract username from session via new
   `SessionKeyGenerator.get_web_auth_session_key_username` ([#290])
-* `User.get_track_scrobbles` ([#298])
+- `User.get_track_scrobbles` ([#298])
 
 ### Deprecated
 
-*  `User.get_artist_tracks`. Use `User.get_track_scrobbles` as a partial replacement.
-   ([#298])
+- `User.get_artist_tracks`. Use `User.get_track_scrobbles` as a partial replacement.
+  ([#298])
 
 ## [3.0.0] - 2019-01-01
+
 ### Added
-* This changelog file ([#273])
+
+- This changelog file ([#273])
 
 ### Removed
 
-* Support for Python 2.7 ([#265])
+- Support for Python 2.7 ([#265])
 
-* Constants `COVER_SMALL`, `COVER_MEDIUM`, `COVER_LARGE`, `COVER_EXTRA_LARGE`
-  and `COVER_MEGA`. Use `SIZE_SMALL` etc. instead. ([#282])
+- Constants `COVER_SMALL`, `COVER_MEDIUM`, `COVER_LARGE`, `COVER_EXTRA_LARGE` and
+  `COVER_MEGA`. Use `SIZE_SMALL` etc. instead. ([#282])
 
 ## [2.4.0] - 2018-08-08
+
 ### Deprecated
 
-* Support for Python 2.7 ([#265])
+- Support for Python 2.7 ([#265])
 
 [4.2.0]: https://github.com/pylast/pylast/compare/4.1.0...4.2.0
 [4.1.0]: https://github.com/pylast/pylast/compare/4.0.0...4.1.0
 [4.0.0]: https://github.com/pylast/pylast/compare/3.3.0...4.0.0
 [3.3.0]: https://github.com/pylast/pylast/compare/3.2.1...3.3.0
 [3.2.1]: https://github.com/pylast/pylast/compare/3.2.0...3.2.1
 [3.2.0]: https://github.com/pylast/pylast/compare/3.1.0...3.2.0
```

### Comparing `pylast-5.2.0/RELEASING.md` & `pylast-5.3.0/RELEASING.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Release Checklist
 
 - [ ] Get `main` to the appropriate code release state.
-      [GitHub Actions](https://github.com/pylast/pylast/actions) should be running cleanly for
-      all merges to `main`.
+      [GitHub Actions](https://github.com/pylast/pylast/actions) should be running
+      cleanly for all merges to `main`.
       [![Test](https://github.com/pylast/pylast/workflows/Test/badge.svg)](https://github.com/pylast/pylast/actions)
 
 - [ ] Edit release draft, adjust text if needed:
       https://github.com/pylast/pylast/releases
 
 - [ ] Check next tag is correct, amend if needed
 
 - [ ] Publish release
 
-- [ ] Check the tagged [GitHub Actions build](https://github.com/pylast/pylast/actions/workflows/deploy.yml)
+- [ ] Check the tagged
+      [GitHub Actions build](https://github.com/pylast/pylast/actions/workflows/deploy.yml)
       has deployed to [PyPI](https://pypi.org/project/pylast/#history)
 
 - [ ] Check installation:
 
 ```bash
 pip3 uninstall -y pylast && pip3 install -U pylast && python3 -c "import pylast; print(pylast.__version__)"
 ```
```

### Comparing `pylast-5.2.0/.github/labels.yml` & `pylast-5.3.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pylast-5.2.0/.github/release-drafter.yml` & `pylast-5.3.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pylast-5.2.0/.github/workflows/deploy.yml` & `pylast-5.3.0/.github/workflows/deploy.yml`

 * *Files 21% similar despite different names*

```diff
@@ -17,56 +17,59 @@
 jobs:
   # Always build & lint package.
   build-package:
     name: Build & verify package
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - uses: hynek/build-and-inspect-python-package@v1
+      - uses: hynek/build-and-inspect-python-package@v2
 
   # Upload to Test PyPI on every commit on main.
   release-test-pypi:
     name: Publish in-dev package to test.pypi.org
-    if: github.event_name == 'push' && github.ref == 'refs/heads/main'
+    if: |
+      github.repository_owner == 'pylast'
+      && github.event_name == 'push'
+      && github.ref == 'refs/heads/main'
     runs-on: ubuntu-latest
     needs: build-package
 
     permissions:
-      # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
 
     steps:
       - name: Download packages built by build-and-inspect-python-package
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: Packages
           path: dist
 
       - name: Upload package to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           repository-url: https://test.pypi.org/legacy/
 
   # Upload to real PyPI on GitHub Releases.
   release-pypi:
     name: Publish released package to pypi.org
-    if: github.event.action == 'published'
+    if: |
+      github.repository_owner == 'pylast'
+      && github.event.action == 'published'
     runs-on: ubuntu-latest
     needs: build-package
 
     permissions:
-      # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
 
     steps:
       - name: Download packages built by build-and-inspect-python-package
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: Packages
           path: dist
 
       - name: Upload package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `pylast-5.2.0/.github/workflows/release-drafter.yml` & `pylast-5.3.0/.github/workflows/release-drafter.yml`

 * *Files 1% similar despite different names*

```diff
@@ -25,10 +25,10 @@
       contents: write
       # write permission is required for autolabeler
       # otherwise, read permission is required at least
       pull-requests: write
     runs-on: ubuntu-latest
     steps:
       # Drafts your next release notes as pull requests are merged into "main"
-      - uses: release-drafter/release-drafter@v5
+      - uses: release-drafter/release-drafter@v6
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `pylast-5.2.0/.github/workflows/test.yml` & `pylast-5.3.0/.github/workflows/test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy3.9", "3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["pypy3.10", "3.8", "3.9", "3.10", "3.11", "3.12", "3.13"]
         os: [ubuntu-latest]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
           cache: pip
-          cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
           python -m pip install -U tox
 
@@ -37,15 +36,15 @@
         env:
           PYLAST_API_KEY: ${{ secrets.PYLAST_API_KEY }}
           PYLAST_API_SECRET: ${{ secrets.PYLAST_API_SECRET }}
           PYLAST_PASSWORD_HASH: ${{ secrets.PYLAST_PASSWORD_HASH }}
           PYLAST_USERNAME: ${{ secrets.PYLAST_USERNAME }}
 
       - name: Upload coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v3.1.5
         with:
           flags: ${{ matrix.os }}
           name: ${{ matrix.os }} Python ${{ matrix.python-version }}
 
   success:
     needs: test
     runs-on: ubuntu-latest
```

### Comparing `pylast-5.2.0/src/pylast/__init__.py` & `pylast-5.3.0/src/pylast/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -525,33 +525,33 @@
         if duration:
             params["duration"] = duration
 
         _Request(self, "track.updateNowPlaying", params).execute()
 
     def scrobble(
         self,
-        artist,
-        title,
-        timestamp,
-        album=None,
-        album_artist=None,
-        track_number=None,
-        duration=None,
-        stream_id=None,
-        context=None,
-        mbid=None,
+        artist: str,
+        title: str,
+        timestamp: int,
+        album: str | None = None,
+        album_artist: str | None = None,
+        track_number: int | None = None,
+        duration: int | None = None,
+        stream_id: str | None = None,
+        context: str | None = None,
+        mbid: str | None = None,
     ):
         """Used to add a track-play to a user's profile.
 
         Parameters:
             artist (Required) : The artist name.
             title (Required) : The track name.
-            timestamp (Required) : The time the track started playing, in UNIX
+            timestamp (Required) : The time the track started playing, in Unix
                 timestamp format (integer number of seconds since 00:00:00,
-                January 1st 1970 UTC). This must be in the UTC time zone.
+                January 1st 1970 UTC).
             album (Optional) : The album name.
             album_artist (Optional) : The album artist - if this differs from
                 the track artist.
             context (Optional) : Sub-client version (not public, only enabled
                 for certain API keys)
             stream_id (Optional) : The stream id for this track received from
                 the radio.getPlaylist service.
@@ -624,15 +624,14 @@
         _Request(self, "track.scrobble", params).execute()
 
         if remaining_tracks:
             self.scrobble_many(remaining_tracks)
 
 
 class LastFMNetwork(_Network):
-
     """A Last.fm network object
 
     api_key: a provided API_KEY
     api_secret: a provided API_SECRET
     session_key: a generated session_key or None
     username: a username of a valid user
     password_hash: the output of pylast.md5(password) where password is the
@@ -890,27 +889,30 @@
         if self.network.limit_rate:
             self.network._delay_call()
 
         username = self.params.pop("username", None)
         username = "" if username is None else f"?username={username}"
 
         (host_name, host_subdir) = self.network.ws_server
+        timeout = httpx.Timeout(5, read=10)
 
         if self.network.is_proxy_enabled():
             client = httpx.Client(
                 verify=SSL_CONTEXT,
                 base_url=f"https://{host_name}",
                 headers=HEADERS,
                 proxies=self.network.proxy,
+                timeout=timeout,
             )
         else:
             client = httpx.Client(
                 verify=SSL_CONTEXT,
                 base_url=f"https://{host_name}",
                 headers=HEADERS,
+                timeout=timeout,
             )
 
         try:
             response = client.post(f"{host_subdir}{username}", data=self.params)
         except Exception as e:
             raise NetworkError(self.network, e) from e
 
@@ -1152,29 +1154,29 @@
 
                 yield TopItem(thing_type(artist, title, self.network), playcount)
 
         return _stream_get_things() if stream else list(_stream_get_things())
 
     def get_wiki_published_date(self):
         """
-        Returns the summary of the wiki.
+        Returns the date on which the wiki was published.
         Only for Album/Track.
         """
         return self.get_wiki("published")
 
     def get_wiki_summary(self):
         """
         Returns the summary of the wiki.
         Only for Album/Track.
         """
         return self.get_wiki("summary")
 
     def get_wiki_content(self):
         """
-        Returns the summary of the wiki.
+        Returns the content of the wiki.
         Only for Album/Track.
         """
         return self.get_wiki("content")
 
     def get_wiki(self, section):
         """
         Returns a section of the wiki.
@@ -1236,16 +1238,18 @@
 
     def get_weekly_charts(self, chart_kind, from_date=None, to_date=None):
         """
         Returns the weekly charts for the week starting from the
         from_date value to the to_date value.
         chart_kind should be one of "album", "artist" or "track"
         """
+        import sys
+
         method = ".getWeekly" + chart_kind.title() + "Chart"
-        chart_type = eval(chart_kind.title())  # string to type
+        chart_type = getattr(sys.modules[__name__], chart_kind.title())
 
         params = self._get_params()
         if from_date and to_date:
             params["from"] = from_date
             params["to"] = to_date
 
         doc = self._request(self.ws_prefix + method, True, params)
@@ -1349,19 +1353,19 @@
             old_tags.append(tag.get_name())
 
         for tag in tags:
             c_new_tags.append(tag.lower())
             new_tags.append(tag)
 
         for i in range(0, len(old_tags)):
-            if not c_old_tags[i] in c_new_tags:
+            if c_old_tags[i] not in c_new_tags:
                 to_remove.append(old_tags[i])
 
         for i in range(0, len(new_tags)):
-            if not c_new_tags[i] in c_old_tags:
+            if c_new_tags[i] not in c_old_tags:
                 to_add.append(new_tags[i])
 
         self.remove_tags(to_remove)
         self.add_tags(to_add)
 
     def get_top_tags(self, limit=None):
         """Returns a list of the most frequently used Tags on this object."""
@@ -1501,15 +1505,15 @@
         )
 
     @_string_output
     def __str__(self) -> str:
         return f"{self.get_artist().get_name()} - {self.get_title()}"
 
     def __eq__(self, other):
-        if type(self) != type(other):
+        if type(self) is not type(other):
             return False
         a = self.get_title().lower()
         b = other.get_title().lower()
         c = self.get_artist().get_name().lower()
         d = other.get_artist().get_name().lower()
         return (a == b) and (c == d)
 
@@ -1539,15 +1543,15 @@
         if "image" not in self.info:
             self.info["image"] = _extract_all(
                 self._request(self.ws_prefix + ".getInfo", cacheable=True), "image"
             )
         return self.info["image"][size]
 
     def get_title(self, properly_capitalized: bool = False):
-        """Returns the artist or track title."""
+        """Returns the album or track title."""
         if properly_capitalized:
             self.title = _extract(
                 self._request(self.ws_prefix + ".getInfo", True), "name"
             )
 
         return self.title
 
@@ -2291,33 +2295,31 @@
 
         return Track(artist, title, self.network, self.name, info=info)
 
     def get_recent_tracks(
         self,
         limit: int = 10,
         cacheable: bool = True,
-        time_from=None,
-        time_to=None,
+        time_from: int | None = None,
+        time_to: int | None = None,
         stream: bool = False,
         now_playing: bool = False,
     ):
         """
         Returns this user's played track as a sequence of PlayedTrack objects
         in reverse order of playtime, all the way back to the first track.
 
         Parameters:
         limit : If None, it will try to pull all the available data.
         from (Optional) : Beginning timestamp of a range - only display
-        scrobbles after this time, in UNIX timestamp format (integer
-        number of seconds since 00:00:00, January 1st 1970 UTC). This
-        must be in the UTC time zone.
+        scrobbles after this time, in Unix timestamp format (integer
+        number of seconds since 00:00:00, January 1st 1970 UTC).
         to (Optional) : End timestamp of a range - only display scrobbles
-        before this time, in UNIX timestamp format (integer number of
-        seconds since 00:00:00, January 1st 1970 UTC). This must be in
-        the UTC time zone.
+        before this time, in Unix timestamp format (integer number of
+        seconds since 00:00:00, January 1st 1970 UTC).
         stream: If True, it will yield tracks as soon as a page has been retrieved.
 
         This method uses caching. Enable caching only if you're pulling a
         large amount of data.
         """
 
         def _get_recent_tracks():
@@ -2378,15 +2380,15 @@
         """Returns the user's registration date."""
 
         doc = self._request(self.ws_prefix + ".getInfo", True)
 
         return _extract(doc, "registered")
 
     def get_unixtime_registered(self):
-        """Returns the user's registration date as a UNIX timestamp."""
+        """Returns the user's registration date as a Unix timestamp."""
 
         doc = self._request(self.ws_prefix + ".getInfo", True)
 
         return int(doc.getElementsByTagName("registered")[0].getAttribute("unixtime"))
 
     def get_tagged_albums(self, tag, limit=None, cacheable: bool = True):
         """Returns the albums tagged by a user."""
@@ -2773,15 +2775,16 @@
             main = doc.documentElement.childNodes[0]
 
             if main.hasAttribute("totalPages") or main.hasAttribute("totalpages"):
                 total_pages = _number(
                     main.getAttribute("totalPages") or main.getAttribute("totalpages")
                 )
             else:
-                raise PyLastError("No total pages attribute")
+                msg = "No total pages attribute"
+                raise PyLastError(msg)
 
             for node in main.childNodes:
                 if not node.nodeType == xml.dom.Node.TEXT_NODE and (
                     not limit or (node_count < limit)
                 ):
                     node_count += 1
                     yield node
```

### Comparing `pylast-5.2.0/tests/test_album.py` & `pylast-5.3.0/tests/test_album.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """
 Integration (not unit) tests for pylast.py
 """
+from __future__ import annotations
+
 import pylast
 
 from .test_pylast import TestPyLastWithLastFm
 
 
 class TestPyLastAlbum(TestPyLastWithLastFm):
     def test_album_tags_are_topitems(self) -> None:
```

### Comparing `pylast-5.2.0/tests/test_artist.py` & `pylast-5.3.0/tests/test_artist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """
 Integration (not unit) tests for pylast.py
 """
+from __future__ import annotations
+
 import pytest
 
 import pylast
 
 from .test_pylast import WRITE_TEST, TestPyLastWithLastFm
```

### Comparing `pylast-5.2.0/tests/test_country.py` & `pylast-5.3.0/tests/test_country.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """
 Integration (not unit) tests for pylast.py
 """
+from __future__ import annotations
+
 import pylast
 
 from .test_pylast import TestPyLastWithLastFm
 
 
 class TestPyLastCountry(TestPyLastWithLastFm):
     def test_country_is_hashable(self) -> None:
```

### Comparing `pylast-5.2.0/tests/test_library.py` & `pylast-5.3.0/tests/test_library.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """
 Integration (not unit) tests for pylast.py
 """
+from __future__ import annotations
+
 import pylast
 
 from .test_pylast import TestPyLastWithLastFm
 
 
 class TestPyLastLibrary(TestPyLastWithLastFm):
     def test_repr(self) -> None:
```

### Comparing `pylast-5.2.0/tests/test_librefm.py` & `pylast-5.3.0/tests/test_librefm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """
 Integration (not unit) tests for pylast.py
 """
+from __future__ import annotations
+
 from flaky import flaky
 
 import pylast
 
 from .test_pylast import load_secrets
```

### Comparing `pylast-5.2.0/tests/test_network.py` & `pylast-5.3.0/tests/test_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 Integration (not unit) tests for pylast.py
 """
+
+from __future__ import annotations
+
 import re
 import time
 
 import pytest
 
 import pylast
```

### Comparing `pylast-5.2.0/tests/test_pylast.py` & `pylast-5.3.0/tests/test_pylast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """
 Integration (not unit) tests for pylast.py
 """
+from __future__ import annotations
+
 import os
 import time
 
 import pytest
 from flaky import flaky
 
 import pylast
```

### Comparing `pylast-5.2.0/tests/test_tag.py` & `pylast-5.3.0/tests/test_tag.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """
 Integration (not unit) tests for pylast.py
 """
+from __future__ import annotations
+
 import pylast
 
 from .test_pylast import TestPyLastWithLastFm
 
 
 class TestPyLastTag(TestPyLastWithLastFm):
     def test_tag_is_hashable(self) -> None:
```

### Comparing `pylast-5.2.0/tests/test_track.py` & `pylast-5.3.0/tests/test_track.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 Integration (not unit) tests for pylast.py
 """
+
+from __future__ import annotations
+
 import time
 
 import pytest
 
 import pylast
 
 from .test_pylast import WRITE_TEST, TestPyLastWithLastFm
@@ -131,19 +134,15 @@
         # Arrange
         track = pylast.Track("Cher", "Believe", self.network)
 
         # Act
         similar = track.get_similar()
 
         # Assert
-        found = False
-        for track in similar:
-            if str(track.item) == "Madonna - Vogue":
-                found = True
-                break
+        found = any(str(track.item) == "Cher - Strong Enough" for track in similar)
         assert found
 
     def test_track_get_similar_limits(self) -> None:
         # Arrange
         track = pylast.Track("Cher", "Believe", self.network)
 
         # Act/Assert
```

### Comparing `pylast-5.2.0/tests/test_user.py` & `pylast-5.3.0/tests/test_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """
 Integration (not unit) tests for pylast.py
 """
+from __future__ import annotations
+
 import calendar
 import datetime as dt
 import inspect
 import os
 import re
 
 import pytest
```

### Comparing `pylast-5.2.0/tests/unicode_test.py` & `pylast-5.3.0/tests/unicode_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from unittest import mock
 
 import pytest
 
 import pylast
 
 
@@ -21,15 +23,15 @@
 def test_get_cache_key(artist) -> None:
     request = pylast._Request(mock_network(), "some_method", params={"artist": artist})
     request._get_cache_key()
 
 
 @pytest.mark.parametrize("obj", [pylast.Artist("B\xe9l", mock_network())])
 def test_cast_and_hash(obj) -> None:
-    assert type(str(obj)) is str
+    assert isinstance(str(obj), str)
     assert isinstance(hash(obj), int)
 
 
 @pytest.mark.parametrize(
     "test_input, expected",
     [
         (
```

### Comparing `pylast-5.2.0/.gitignore` & `pylast-5.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pylast-5.2.0/COPYING` & `pylast-5.3.0/COPYING`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 
 2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
 
 3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
 
 4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
 
-You must give any other recipients of the Work or Derivative Works a copy of this License; and 
+You must give any other recipients of the Work or Derivative Works a copy of this License; and
 
-You must cause any modified files to carry prominent notices stating that You changed the files; and 
+You must cause any modified files to carry prominent notices stating that You changed the files; and
 
-You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and 
+You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
 
 If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
 You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
 5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
 
 6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
```

### Comparing `pylast-5.2.0/LICENSE.txt` & `pylast-5.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylast-5.2.0/README.md` & `pylast-5.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,38 +31,38 @@
 
 ```txt
 -e https://github.com/pylast/pylast.git#egg=pylast
 ```
 
 Note:
 
-* pyLast 5.2+ supports Python 3.8-3.12.
-* pyLast 5.1 supports Python 3.7-3.11.
-* pyLast 5.0 supports Python 3.7-3.10.
-* pyLast 4.3 - 4.5 supports Python 3.6-3.10.
-* pyLast 4.0 - 4.2 supports Python 3.6-3.9.
-* pyLast 3.2 - 3.3 supports Python 3.5-3.8.
-* pyLast 3.0 - 3.1 supports Python 3.5-3.7.
-* pyLast 2.2 - 2.4 supports Python 2.7.10+, 3.4-3.7.
-* pyLast 2.0 - 2.1 supports Python 2.7.10+, 3.4-3.6.
-* pyLast 1.7 - 1.9 supports Python 2.7, 3.3-3.6.
-* pyLast 1.0 - 1.6 supports Python 2.7, 3.3-3.4.
-* pyLast 0.5 supports Python 2, 3.
-* pyLast < 0.5 supports Python 2.
+- pyLast 5.3+ supports Python 3.8-3.13.
+- pyLast 5.2+ supports Python 3.8-3.12.
+- pyLast 5.1 supports Python 3.7-3.11.
+- pyLast 5.0 supports Python 3.7-3.10.
+- pyLast 4.3 - 4.5 supports Python 3.6-3.10.
+- pyLast 4.0 - 4.2 supports Python 3.6-3.9.
+- pyLast 3.2 - 3.3 supports Python 3.5-3.8.
+- pyLast 3.0 - 3.1 supports Python 3.5-3.7.
+- pyLast 2.2 - 2.4 supports Python 2.7.10+, 3.4-3.7.
+- pyLast 2.0 - 2.1 supports Python 2.7.10+, 3.4-3.6.
+- pyLast 1.7 - 1.9 supports Python 2.7, 3.3-3.6.
+- pyLast 1.0 - 1.6 supports Python 2.7, 3.3-3.4.
+- pyLast 0.5 supports Python 2, 3.
+- pyLast < 0.5 supports Python 2.
 
 ## Features
 
- * Simple public interface.
- * Access to all the data exposed by the Last.fm web services.
- * Scrobbling support.
- * Full object-oriented design.
- * Proxy support.
- * Internal caching support for some web services calls (disabled by default).
- * Support for other API-compatible networks like Libre.fm.
-
+- Simple public interface.
+- Access to all the data exposed by the Last.fm web services.
+- Scrobbling support.
+- Full object-oriented design.
+- Proxy support.
+- Internal caching support for some web services calls (disabled by default).
+- Support for other API-compatible networks like Libre.fm.
 
 ## Getting started
 
 Here's some simple code example to get you started. In order to create any object from
 pyLast, you need a `Network` object which represents a social music network that is
 Last.fm or any other API-compatible one. You can obtain a pre-configured one for Last.fm
 and use it as follows:
@@ -83,16 +83,16 @@
     api_key=API_KEY,
     api_secret=API_SECRET,
     username=username,
     password_hash=password_hash,
 )
 ```
 
-Alternatively, instead of creating `network` with a username and password,
-you can authenticate with a session key:
+Alternatively, instead of creating `network` with a username and password, you can
+authenticate with a session key:
 
 ```python
 import pylast
 
 SESSION_KEY_FILE = os.path.join(os.path.expanduser("~"), ".session_key")
 network = pylast.LastFMNetwork(API_KEY, API_SECRET)
 if not os.path.exists(SESSION_KEY_FILE):
@@ -127,28 +127,28 @@
 track.love()
 track.add_tags(("awesome", "favorite"))
 
 # Type help(pylast.LastFMNetwork) or help(pylast) in a Python interpreter
 # to get more help about anything and see examples of how it works
 ```
 
-
 More examples in
 <a href="https://github.com/hugovk/lastfm-tools">hugovk/lastfm-tools</a> and
 [tests/](https://github.com/pylast/pylast/tree/main/tests).
 
 ## Testing
 
 The [tests/](https://github.com/pylast/pylast/tree/main/tests) directory contains
 integration and unit tests with Last.fm, and plenty of code examples.
 
 For integration tests you need a test account at Last.fm that will become cluttered with
 test data, and an API key and secret. Either copy
-[example_test_pylast.yaml](example_test_pylast.yaml) to test_pylast.yaml and fill out
-the credentials, or set them as environment variables like:
+[example_test_pylast.yaml](https://github.com/pylast/pylast/blob/main/example_test_pylast.yaml)
+to test_pylast.yaml and fill out the credentials, or set them as environment variables
+like:
 
 ```sh
 export PYLAST_USERNAME=TODO_ENTER_YOURS_HERE
 export PYLAST_PASSWORD_HASH=TODO_ENTER_YOURS_HERE
 export PYLAST_API_KEY=TODO_ENTER_YOURS_HERE
 export PYLAST_API_SECRET=TODO_ENTER_YOURS_HERE
 ```
```

### Comparing `pylast-5.2.0/pyproject.toml` & `pylast-5.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 license = {text = "Apache-2.0"}
 maintainers = [{name = "Hugo van Kemenade"}]
 authors = [{name = "Amr Hassan <amr.hassan@gmail.com> and Contributors", email = "amr.hassan@gmail.com"}]
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: Apache Software License",
-  "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3.13",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Internet",
   "Topic :: Multimedia :: Sound/Audio",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = [
@@ -56,9 +56,33 @@
 
 [tool.hatch]
 version.source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
-[tool.isort]
-profile = "black"
+[tool.ruff.lint]
+select = [
+  "C4", # flake8-comprehensions
+  "E", # pycodestyle errors
+  "EM", # flake8-errmsg
+  "F", # pyflakes errors
+  "I", # isort
+  "ISC", # flake8-implicit-str-concat
+  "LOG", # flake8-logging
+  "PGH", # pygrep-hooks
+  "RUF100", # unused noqa (yesqa)
+  "RUF022", # unsorted-dunder-all
+  "UP", # pyupgrade
+  "W", # pycodestyle warnings
+  "YTT", # flake8-2020
+]
+extend-ignore = [
+  "E203", # Whitespace before ':'
+  "E221", # Multiple spaces before operator
+  "E226", # Missing whitespace around arithmetic operator
+  "E241", # Multiple spaces after ','
+]
+
+[tool.ruff.lint.isort]
+known-first-party = ["pylast"]
+required-imports = ["from __future__ import annotations"]
```

### Comparing `pylast-5.2.0/PKG-INFO` & `pylast-5.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pylast
-Version: 5.2.0
+Version: 5.3.0
 Summary: A Python interface to Last.fm and Libre.fm
 Project-URL: Changelog, https://github.com/pylast/pylast/releases
 Project-URL: Homepage, https://github.com/pylast/pylast
 Project-URL: Source, https://github.com/pylast/pylast
 Author-email: "Amr Hassan <amr.hassan@gmail.com> and Contributors" <amr.hassan@gmail.com>
 Maintainer: Hugo van Kemenade
 License: Apache-2.0
 License-File: COPYING
 License-File: LICENSE.txt
 Keywords: Last.fm,music,scrobble,scrobbling
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: httpx
@@ -68,38 +68,38 @@
 
 ```txt
 -e https://github.com/pylast/pylast.git#egg=pylast
 ```
 
 Note:
 
-* pyLast 5.2+ supports Python 3.8-3.12.
-* pyLast 5.1 supports Python 3.7-3.11.
-* pyLast 5.0 supports Python 3.7-3.10.
-* pyLast 4.3 - 4.5 supports Python 3.6-3.10.
-* pyLast 4.0 - 4.2 supports Python 3.6-3.9.
-* pyLast 3.2 - 3.3 supports Python 3.5-3.8.
-* pyLast 3.0 - 3.1 supports Python 3.5-3.7.
-* pyLast 2.2 - 2.4 supports Python 2.7.10+, 3.4-3.7.
-* pyLast 2.0 - 2.1 supports Python 2.7.10+, 3.4-3.6.
-* pyLast 1.7 - 1.9 supports Python 2.7, 3.3-3.6.
-* pyLast 1.0 - 1.6 supports Python 2.7, 3.3-3.4.
-* pyLast 0.5 supports Python 2, 3.
-* pyLast < 0.5 supports Python 2.
+- pyLast 5.3+ supports Python 3.8-3.13.
+- pyLast 5.2+ supports Python 3.8-3.12.
+- pyLast 5.1 supports Python 3.7-3.11.
+- pyLast 5.0 supports Python 3.7-3.10.
+- pyLast 4.3 - 4.5 supports Python 3.6-3.10.
+- pyLast 4.0 - 4.2 supports Python 3.6-3.9.
+- pyLast 3.2 - 3.3 supports Python 3.5-3.8.
+- pyLast 3.0 - 3.1 supports Python 3.5-3.7.
+- pyLast 2.2 - 2.4 supports Python 2.7.10+, 3.4-3.7.
+- pyLast 2.0 - 2.1 supports Python 2.7.10+, 3.4-3.6.
+- pyLast 1.7 - 1.9 supports Python 2.7, 3.3-3.6.
+- pyLast 1.0 - 1.6 supports Python 2.7, 3.3-3.4.
+- pyLast 0.5 supports Python 2, 3.
+- pyLast < 0.5 supports Python 2.
 
 ## Features
 
- * Simple public interface.
- * Access to all the data exposed by the Last.fm web services.
- * Scrobbling support.
- * Full object-oriented design.
- * Proxy support.
- * Internal caching support for some web services calls (disabled by default).
- * Support for other API-compatible networks like Libre.fm.
-
+- Simple public interface.
+- Access to all the data exposed by the Last.fm web services.
+- Scrobbling support.
+- Full object-oriented design.
+- Proxy support.
+- Internal caching support for some web services calls (disabled by default).
+- Support for other API-compatible networks like Libre.fm.
 
 ## Getting started
 
 Here's some simple code example to get you started. In order to create any object from
 pyLast, you need a `Network` object which represents a social music network that is
 Last.fm or any other API-compatible one. You can obtain a pre-configured one for Last.fm
 and use it as follows:
@@ -120,16 +120,16 @@
     api_key=API_KEY,
     api_secret=API_SECRET,
     username=username,
     password_hash=password_hash,
 )
 ```
 
-Alternatively, instead of creating `network` with a username and password,
-you can authenticate with a session key:
+Alternatively, instead of creating `network` with a username and password, you can
+authenticate with a session key:
 
 ```python
 import pylast
 
 SESSION_KEY_FILE = os.path.join(os.path.expanduser("~"), ".session_key")
 network = pylast.LastFMNetwork(API_KEY, API_SECRET)
 if not os.path.exists(SESSION_KEY_FILE):
@@ -164,28 +164,28 @@
 track.love()
 track.add_tags(("awesome", "favorite"))
 
 # Type help(pylast.LastFMNetwork) or help(pylast) in a Python interpreter
 # to get more help about anything and see examples of how it works
 ```
 
-
 More examples in
 <a href="https://github.com/hugovk/lastfm-tools">hugovk/lastfm-tools</a> and
 [tests/](https://github.com/pylast/pylast/tree/main/tests).
 
 ## Testing
 
 The [tests/](https://github.com/pylast/pylast/tree/main/tests) directory contains
 integration and unit tests with Last.fm, and plenty of code examples.
 
 For integration tests you need a test account at Last.fm that will become cluttered with
 test data, and an API key and secret. Either copy
-[example_test_pylast.yaml](example_test_pylast.yaml) to test_pylast.yaml and fill out
-the credentials, or set them as environment variables like:
+[example_test_pylast.yaml](https://github.com/pylast/pylast/blob/main/example_test_pylast.yaml)
+to test_pylast.yaml and fill out the credentials, or set them as environment variables
+like:
 
 ```sh
 export PYLAST_USERNAME=TODO_ENTER_YOURS_HERE
 export PYLAST_PASSWORD_HASH=TODO_ENTER_YOURS_HERE
 export PYLAST_API_KEY=TODO_ENTER_YOURS_HERE
 export PYLAST_API_SECRET=TODO_ENTER_YOURS_HERE
 ```
```

