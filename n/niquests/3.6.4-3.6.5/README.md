# Comparing `tmp/niquests-3.6.4.tar.gz` & `tmp/niquests-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu May 16 05:51:35 2024, max compression
+gzip compressed data, last modified: Wed May 22 05:50:20 2024, max compression
```

## Comparing `niquests-3.6.4.tar` & `niquests-3.6.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      718 2024-05-16 05:51:35.000000 niquests-3.6.4/AUTHORS.rst
--rw-r--r--   0        0        0    86817 2024-05-16 05:51:35.000000 niquests-3.6.4/HISTORY.md
--rw-r--r--   0        0        0      377 2024-05-16 05:51:35.000000 niquests-3.6.4/Makefile
--rw-r--r--   0        0        0       38 2024-05-16 05:51:35.000000 niquests-3.6.4/NOTICE
--rw-r--r--   0        0        0      201 2024-05-16 05:51:35.000000 niquests-3.6.4/SECURITY.md
--rw-r--r--   0        0        0      233 2024-05-16 05:51:35.000000 niquests-3.6.4/requirements-dev.txt
--rw-r--r--   0        0        0        1 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/.nojekyll
--rw-r--r--   0        0        0     7664 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/Makefile
--rw-r--r--   0        0        0     5355 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/api.rst
--rw-r--r--   0        0        0    12305 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/conf.py
--rw-r--r--   0        0        0     4084 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/index.rst
--rw-r--r--   0        0        0     7253 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/make.bat
--rw-r--r--   0        0        0      185 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/requirements.txt
--rw-r--r--   0        0        0     2990 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/_static/custom.css
--rw-r--r--   0        0        0   306086 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/_static/requests-sidebar.png
--rw-r--r--   0        0        0     7360 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/faq.rst
--rw-r--r--   0        0        0     2720 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/recommended.rst
--rw-r--r--   0        0        0     1782 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/release-process.rst
--rw-r--r--   0        0        0      285 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/support.rst
--rw-r--r--   0        0        0      324 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/updates.rst
--rw-r--r--   0        0        0      945 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/community/vulnerabilities.rst
--rw-r--r--   0        0        0       48 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/dev/authors.rst
--rw-r--r--   0        0        0     5768 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/dev/contributing.rst
--rw-r--r--   0        0        0     1885 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/dev/migrate.rst
--rw-r--r--   0        0        0    52818 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/user/advanced.rst
--rw-r--r--   0        0        0     6315 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/user/authentication.rst
--rw-r--r--   0        0        0     1046 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/user/install.rst
--rw-r--r--   0        0        0    34594 2024-05-16 05:51:35.000000 niquests-3.6.4/docs/user/quickstart.rst
--rw-r--r--   0        0        0     3071 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/__init__.py
--rw-r--r--   0        0        0      534 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/__version__.py
--rw-r--r--   0        0        0    47120 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/_async.py
--rw-r--r--   0        0        0     2852 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/_compat.py
--rw-r--r--   0        0        0      480 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/_constant.py
--rw-r--r--   0        0        0     5942 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/_typing.py
--rw-r--r--   0        0        0    86896 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/adapters.py
--rw-r--r--   0        0        0    27567 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/api.py
--rw-r--r--   0        0        0     9906 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/auth.py
--rw-r--r--   0        0        0    19872 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/cookies.py
--rw-r--r--   0        0        0     4363 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/exceptions.py
--rw-r--r--   0        0        0     5248 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/help.py
--rw-r--r--   0        0        0     2776 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/hooks.py
--rw-r--r--   0        0        0    62733 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/models.py
--rw-r--r--   0        0        0        0 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/py.typed
--rw-r--r--   0        0        0    69360 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/sessions.py
--rw-r--r--   0        0        0     4284 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/status_codes.py
--rw-r--r--   0        0        0     7042 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/structures.py
--rw-r--r--   0        0        0    37300 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/utils.py
--rw-r--r--   0        0        0      119 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/extensions/__init__.py
--rw-r--r--   0        0        0    22400 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/extensions/_async_ocsp.py
--rw-r--r--   0        0        0    21160 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/extensions/_ocsp.py
--rw-r--r--   0        0        0    16942 2024-05-16 05:51:35.000000 niquests-3.6.4/src/niquests/extensions/_picotls.py
--rw-r--r--   0        0        0       80 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/__init__.py
--rw-r--r--   0        0        0     2193 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/conftest.py
--rw-r--r--   0        0        0     7540 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_async.py
--rw-r--r--   0        0        0      875 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_help.py
--rw-r--r--   0        0        0      893 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_hooks.py
--rw-r--r--   0        0        0     4022 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_live.py
--rw-r--r--   0        0        0    15985 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_lowlevel.py
--rw-r--r--   0        0        0     3722 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_multiplexed.py
--rw-r--r--   0        0        0    99906 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_requests.py
--rw-r--r--   0        0        0     2725 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_structures.py
--rw-r--r--   0        0        0     6213 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_testserver.py
--rw-r--r--   0        0        0    26728 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/test_utils.py
--rw-r--r--   0        0        0      613 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/utils.py
--rw-r--r--   0        0        0        0 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/testserver/__init__.py
--rw-r--r--   0        0        0     3882 2024-05-16 05:51:35.000000 niquests-3.6.4/tests/testserver/server.py
--rw-r--r--   0        0        0      362 2024-05-16 05:51:35.000000 niquests-3.6.4/.gitignore
--rw-r--r--   0        0        0    10142 2024-05-16 05:51:35.000000 niquests-3.6.4/LICENSE
--rw-r--r--   0        0        0    10884 2024-05-16 05:51:35.000000 niquests-3.6.4/README.md
--rw-r--r--   0        0        0     3660 2024-05-16 05:51:35.000000 niquests-3.6.4/pyproject.toml
--rw-r--r--   0        0        0    13243 2024-05-16 05:51:35.000000 niquests-3.6.4/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-05-22 05:50:20.000000 niquests-3.6.5/AUTHORS.rst
+-rw-r--r--   0        0        0    87660 2024-05-22 05:50:20.000000 niquests-3.6.5/HISTORY.md
+-rw-r--r--   0        0        0      377 2024-05-22 05:50:20.000000 niquests-3.6.5/Makefile
+-rw-r--r--   0        0        0       38 2024-05-22 05:50:20.000000 niquests-3.6.5/NOTICE
+-rw-r--r--   0        0        0      201 2024-05-22 05:50:20.000000 niquests-3.6.5/SECURITY.md
+-rw-r--r--   0        0        0      233 2024-05-22 05:50:20.000000 niquests-3.6.5/requirements-dev.txt
+-rw-r--r--   0        0        0        1 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/.nojekyll
+-rw-r--r--   0        0        0     7664 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/Makefile
+-rw-r--r--   0        0        0     5355 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/api.rst
+-rw-r--r--   0        0        0    12305 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/conf.py
+-rw-r--r--   0        0        0     4084 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/index.rst
+-rw-r--r--   0        0        0     7253 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/make.bat
+-rw-r--r--   0        0        0      185 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/requirements.txt
+-rw-r--r--   0        0        0     2990 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/_static/custom.css
+-rw-r--r--   0        0        0   306086 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/_static/requests-sidebar.png
+-rw-r--r--   0        0        0     7360 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/faq.rst
+-rw-r--r--   0        0        0     2720 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/recommended.rst
+-rw-r--r--   0        0        0     1782 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/release-process.rst
+-rw-r--r--   0        0        0      285 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/support.rst
+-rw-r--r--   0        0        0      324 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/updates.rst
+-rw-r--r--   0        0        0      945 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/vulnerabilities.rst
+-rw-r--r--   0        0        0       48 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/dev/authors.rst
+-rw-r--r--   0        0        0     5768 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/dev/contributing.rst
+-rw-r--r--   0        0        0     1885 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/dev/migrate.rst
+-rw-r--r--   0        0        0    52818 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/user/advanced.rst
+-rw-r--r--   0        0        0     6315 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/user/authentication.rst
+-rw-r--r--   0        0        0     1046 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/user/install.rst
+-rw-r--r--   0        0        0    34594 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/user/quickstart.rst
+-rw-r--r--   0        0        0     2805 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/__version__.py
+-rw-r--r--   0        0        0    47165 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/_async.py
+-rw-r--r--   0        0        0     2852 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/_compat.py
+-rw-r--r--   0        0        0      480 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/_constant.py
+-rw-r--r--   0        0        0     5942 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/_typing.py
+-rw-r--r--   0        0        0    87323 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/adapters.py
+-rw-r--r--   0        0        0    27567 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/api.py
+-rw-r--r--   0        0        0     9906 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/auth.py
+-rw-r--r--   0        0        0    20648 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/cookies.py
+-rw-r--r--   0        0        0     4363 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/exceptions.py
+-rw-r--r--   0        0        0     5248 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/help.py
+-rw-r--r--   0        0        0     2776 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/hooks.py
+-rw-r--r--   0        0        0    62733 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/models.py
+-rw-r--r--   0        0        0        0 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/py.typed
+-rw-r--r--   0        0        0    69459 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/sessions.py
+-rw-r--r--   0        0        0     4284 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/status_codes.py
+-rw-r--r--   0        0        0     7042 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/structures.py
+-rw-r--r--   0        0        0    37956 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/utils.py
+-rw-r--r--   0        0        0      119 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/extensions/__init__.py
+-rw-r--r--   0        0        0    22400 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/extensions/_async_ocsp.py
+-rw-r--r--   0        0        0    21160 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/extensions/_ocsp.py
+-rw-r--r--   0        0        0    16942 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/extensions/_picotls.py
+-rw-r--r--   0        0        0       80 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/__init__.py
+-rw-r--r--   0        0        0     2619 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/conftest.py
+-rw-r--r--   0        0        0     7540 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_async.py
+-rw-r--r--   0        0        0      875 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_help.py
+-rw-r--r--   0        0        0      893 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_hooks.py
+-rw-r--r--   0        0        0     4022 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_live.py
+-rw-r--r--   0        0        0    15985 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_lowlevel.py
+-rw-r--r--   0        0        0     3722 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_multiplexed.py
+-rw-r--r--   0        0        0   100346 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_requests.py
+-rw-r--r--   0        0        0     2725 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_structures.py
+-rw-r--r--   0        0        0     6213 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_testserver.py
+-rw-r--r--   0        0        0    26728 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_utils.py
+-rw-r--r--   0        0        0      613 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/testserver/__init__.py
+-rw-r--r--   0        0        0     3882 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/testserver/server.py
+-rw-r--r--   0        0        0      362 2024-05-22 05:50:20.000000 niquests-3.6.5/.gitignore
+-rw-r--r--   0        0        0    10142 2024-05-22 05:50:20.000000 niquests-3.6.5/LICENSE
+-rw-r--r--   0        0        0    10882 2024-05-22 05:50:20.000000 niquests-3.6.5/README.md
+-rw-r--r--   0        0        0     3660 2024-05-22 05:50:20.000000 niquests-3.6.5/pyproject.toml
+-rw-r--r--   0        0        0    13241 2024-05-22 05:50:20.000000 niquests-3.6.5/PKG-INFO
```

### Comparing `niquests-3.6.4/AUTHORS.rst` & `niquests-3.6.5/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/HISTORY.md` & `niquests-3.6.5/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 Release History
 ===============
 
+3.6.5 (2024-05-22)
+------------------
+
+**Fixed**
+- Support `localhost` as a valid domain for cookies. The standard library does not allow this special
+  domain. Researches showed that a valid domain should have at least two dots (e.g. abc.com. and xyz.tld. but not com.).
+  Public suffixes cannot be used as a cookie domain for security reasons, but as `localhost` isn't one we are explicitly
+  allowing it. Reported in https://github.com/httpie/cli/issues/602
+  `RequestsCookieJar` set a default policy that circumvent that limitation, if you specified a custom cookie policy then this
+  fix won't be applied.
+
+**Changed**
+- Lazy load the OCSP extension in order to improve the import performance.
+
+**Removed**
+- Class variable `disable_thread` in `AsyncSession` that is no longer relevant since the native asyncio implementation. (PR #122)
+
 3.6.4 (2024-05-16)
 ------------------
 
 **Changed**
 - Avoid parsing X509 peer certificate in the certificate revocation check process over and over again.
 - Avoid iterating over header items redundantly or needlessly.
```

### Comparing `niquests-3.6.4/docs/Makefile` & `niquests-3.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/api.rst` & `niquests-3.6.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/conf.py` & `niquests-3.6.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/index.rst` & `niquests-3.6.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/make.bat` & `niquests-3.6.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/_static/custom.css` & `niquests-3.6.5/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/_static/requests-sidebar.png` & `niquests-3.6.5/docs/_static/requests-sidebar.png`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/community/faq.rst` & `niquests-3.6.5/docs/community/faq.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/community/recommended.rst` & `niquests-3.6.5/docs/community/recommended.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/community/release-process.rst` & `niquests-3.6.5/docs/community/release-process.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/community/vulnerabilities.rst` & `niquests-3.6.5/docs/community/vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/dev/contributing.rst` & `niquests-3.6.5/docs/dev/contributing.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/dev/migrate.rst` & `niquests-3.6.5/docs/dev/migrate.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/user/advanced.rst` & `niquests-3.6.5/docs/user/advanced.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/user/authentication.rst` & `niquests-3.6.5/docs/user/authentication.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/user/install.rst` & `niquests-3.6.5/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/docs/user/quickstart.rst` & `niquests-3.6.5/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/__init__.py` & `niquests-3.6.5/src/niquests/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -50,18 +50,14 @@
 if HAS_LEGACY_URLLIB3 is False:
     from urllib3.exceptions import DependencyWarning
 else:
     from urllib3_future.exceptions import DependencyWarning  # type: ignore[assignment]
 
 # urllib3's DependencyWarnings should be silenced.
 warnings.simplefilter("ignore", DependencyWarning)
-# Commonly happen on Windows due to some legacy root CA in
-# their trust store. They are aware of it, we silent the warning
-# yield by Cryptography to avoid producing undesired noise to end-users.
-warnings.filterwarnings("ignore", "Parsed a negative serial number")
 
 # ruff: noqa: E402
 from . import utils
 from .__version__ import (
     __author__,
     __author_email__,
     __build__,
```

### Comparing `niquests-3.6.4/src/niquests/__version__.py` & `niquests-3.6.5/src/niquests/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 __title__: str = "niquests"
 __description__: str = "Python HTTP for Humans."
 __url__: str = "https://niquests.readthedocs.io"
 
 __version__: str
-__version__ = "3.6.4"
+__version__ = "3.6.5"
 
-__build__: int = 0x030604
+__build__: int = 0x030605
 __author__: str = "Kenneth Reitz"
 __author_email__: str = "me@kennethreitz.org"
 __license__: str = "Apache-2.0"
 __copyright__: str = "Copyright Kenneth Reitz"
 __cake__: str = "\u2728 \U0001f370 \u2728"
```

### Comparing `niquests-3.6.4/src/niquests/_async.py` & `niquests-3.6.5/src/niquests/_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,29 +68,25 @@
     default_headers,
     resolve_proxies,
     rewind_body,
     requote_uri,
     _swap_context,
     _deepcopy_ci,
     parse_scheme,
+    is_ocsp_capable,
 )
 from .cookies import (
     RequestsCookieJar,
     cookiejar_from_dict,
     extract_cookies_to_jar,
     merge_cookies,
 )
 from .structures import AsyncQuicSharedCache
 from .adapters import AsyncBaseAdapter, AsyncHTTPAdapter
 
-try:
-    from .extensions._async_ocsp import verify as ocsp_verify
-except ImportError:
-    ocsp_verify = None  # type: ignore[assignment]
-
 # Preferred clock, based on which one is more accurate on a given system.
 if sys.platform == "win32":
     preferred_clock = time.perf_counter
 else:
     preferred_clock = time.time
 
 
@@ -109,16 +105,14 @@
     Or as a context manager::
 
       >>> async with niquests.AsyncSession() as s:
       ...     await s.get('https://httpbin.org/get')
       <Response HTTP/2 [200]>
     """
 
-    disable_thread: bool = False  # no-op since v3.5
-
     def __init__(
         self,
         *,
         resolver: AsyncResolverType | None = None,
         source_address: tuple[str, int] | None = None,
         quic_cache_layer: CacheLayerAltSvcType | None = None,
         retries: RetryType = DEFAULT_RETRIES,
@@ -321,29 +315,34 @@
             """This function will be called by urllib3.future just after establishing the connection."""
             nonlocal ptr_request, request, kwargs
             ptr_request.conn_info = conn_info
 
             if (
                 ptr_request.url
                 and ptr_request.url.startswith("https://")
-                and ocsp_verify is not None
                 and kwargs["verify"]
+                and is_ocsp_capable(conn_info)
             ):
                 strict_ocsp_enabled: bool = (
                     os.environ.get("NIQUESTS_STRICT_OCSP", "0") != "0"
                 )
 
-                await ocsp_verify(
-                    ptr_request,
-                    strict_ocsp_enabled,
-                    0.2 if not strict_ocsp_enabled else 1.0,
-                    kwargs["proxies"],
-                    resolver=self.resolver,
-                    happy_eyeballs=self._happy_eyeballs,
-                )
+                try:
+                    from .extensions._async_ocsp import verify as ocsp_verify
+                except ImportError:
+                    pass
+                else:
+                    await ocsp_verify(
+                        ptr_request,
+                        strict_ocsp_enabled,
+                        0.2 if not strict_ocsp_enabled else 1.0,
+                        kwargs["proxies"],
+                        resolver=self.resolver,
+                        happy_eyeballs=self._happy_eyeballs,
+                    )
 
             # don't trigger pre_send for redirects
             if ptr_request == request:
                 await async_dispatch_hook("pre_send", hooks, ptr_request)  # type: ignore[arg-type]
 
         async def handle_upload_progress(
             total_sent: int,
```

### Comparing `niquests-3.6.4/src/niquests/_compat.py` & `niquests-3.6.5/src/niquests/_compat.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/_typing.py` & `niquests-3.6.5/src/niquests/_typing.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/adapters.py` & `niquests-3.6.5/src/niquests/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,23 +148,18 @@
     prepend_scheme_if_needed,
     select_proxy,
     urldefragauth,
     resolve_socket_family,
     _swap_context,
     _deepcopy_ci,
     parse_scheme,
+    is_ocsp_capable,
 )
 
 try:
-    from .extensions._ocsp import verify as ocsp_verify
-    from .extensions._async_ocsp import verify as async_ocsp_verify
-except ImportError:
-    ocsp_verify = None  # type: ignore[assignment]
-
-try:
     if HAS_LEGACY_URLLIB3 is False:
         from urllib3.contrib.socks import SOCKSProxyManager, AsyncSOCKSProxyManager
     else:
         from urllib3_future.contrib.socks import (  # type: ignore[assignment]
             SOCKSProxyManager,
             AsyncSOCKSProxyManager,
         )
@@ -1037,31 +1032,36 @@
 
                     assert next_request is not None
                     next_request.conn_info = conn_info
 
                     if (
                         next_request.url
                         and next_request.url.startswith("https://")
-                        and ocsp_verify is not None
                         and kwargs["verify"]
+                        and is_ocsp_capable(conn_info)
                     ):
                         strict_ocsp_enabled: bool = (
                             os.environ.get("NIQUESTS_STRICT_OCSP", "0") != "0"
                         )
 
-                        ocsp_verify(
-                            next_request,
-                            strict_ocsp_enabled,
-                            0.2 if not strict_ocsp_enabled else 1.0,
-                            kwargs["proxies"],
-                            self._resolver
-                            if isinstance(self._resolver, BaseResolver)
-                            else None,
-                            self._happy_eyeballs,
-                        )
+                        try:
+                            from .extensions._ocsp import verify as ocsp_verify
+                        except ImportError:
+                            pass
+                        else:
+                            ocsp_verify(
+                                next_request,
+                                strict_ocsp_enabled,
+                                0.2 if not strict_ocsp_enabled else 1.0,
+                                kwargs["proxies"],
+                                self._resolver
+                                if isinstance(self._resolver, BaseResolver)
+                                else None,
+                                self._happy_eyeballs,
+                            )
 
                 kwargs["on_post_connection"] = on_post_connection
 
                 next_promise = self.send(next_request, **kwargs)
 
                 # warning: next_promise could be a non-promise if the redirect location does not support
                 # multiplexing. We'll have to break the 'lazy' aspect.
@@ -2011,31 +2011,38 @@
 
                     assert next_request is not None
                     next_request.conn_info = conn_info
 
                     if (
                         next_request.url
                         and next_request.url.startswith("https://")
-                        and ocsp_verify is not None
                         and kwargs["verify"]
+                        and is_ocsp_capable(conn_info)
                     ):
-                        strict_ocsp_enabled: bool = (
-                            os.environ.get("NIQUESTS_STRICT_OCSP", "0") != "0"
-                        )
-
-                        await async_ocsp_verify(
-                            next_request,
-                            strict_ocsp_enabled,
-                            0.2 if not strict_ocsp_enabled else 1.0,
-                            kwargs["proxies"],
-                            self._resolver
-                            if isinstance(self._resolver, AsyncBaseResolver)
-                            else None,
-                            self._happy_eyeballs,
-                        )
+                        try:
+                            from .extensions._async_ocsp import (
+                                verify as async_ocsp_verify,
+                            )
+                        except ImportError:
+                            pass
+                        else:
+                            strict_ocsp_enabled: bool = (
+                                os.environ.get("NIQUESTS_STRICT_OCSP", "0") != "0"
+                            )
+
+                            await async_ocsp_verify(
+                                next_request,
+                                strict_ocsp_enabled,
+                                0.2 if not strict_ocsp_enabled else 1.0,
+                                kwargs["proxies"],
+                                self._resolver
+                                if isinstance(self._resolver, AsyncBaseResolver)
+                                else None,
+                                self._happy_eyeballs,
+                            )
 
                 kwargs["on_post_connection"] = on_post_connection
 
                 next_promise = await self.send(next_request, **kwargs)
 
                 # warning: next_promise could be a non-promise if the redirect location does not support
                 # multiplexing. We'll have to break the 'lazy' aspect.
```

### Comparing `niquests-3.6.4/src/niquests/api.py` & `niquests-3.6.5/src/niquests/api.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/auth.py` & `niquests-3.6.5/src/niquests/auth.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/cookies.py` & `niquests-3.6.5/src/niquests/cookies.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,29 @@
 else:
     from urllib3_future import BaseHTTPResponse  # type: ignore[assignment]
 
 if typing.TYPE_CHECKING:
     from .models import PreparedRequest, Request
 
 
+class CookiePolicyLocalhostBypass(cookielib.DefaultCookiePolicy):
+    """A subclass of DefaultCookiePolicy to allow cookie set for domain=localhost.
+    Credit goes to https://github.com/Pylons/webtest/blob/main/webtest/app.py#L60"""
+
+    def return_ok_domain(self, cookie, request):
+        if cookie.domain == ".localhost":
+            return True
+        return cookielib.DefaultCookiePolicy.return_ok_domain(self, cookie, request)
+
+    def set_ok_domain(self, cookie, request):
+        if cookie.domain == ".localhost":
+            return True
+        return cookielib.DefaultCookiePolicy.set_ok_domain(self, cookie, request)
+
+
 class MockRequest:
     """Wraps a `requests.Request` to mimic a `urllib2.Request`.
 
     The code in `http.cookiejar.CookieJar` expects this interface in order to correctly
     manage cookie policies, i.e., determine whether a cookie can be set, given the
     domains of the request and the cookie.
 
@@ -214,14 +229,17 @@
     ``LWPCookieJar`` and ``FileCookieJar``.
 
     Unlike a regular CookieJar, this class is pickleable.
 
     .. warning:: dictionary operations that are normally O(1) may be O(n).
     """
 
+    def __init__(self, policy: cookielib.CookiePolicy | None = None):
+        super().__init__(policy=policy or CookiePolicyLocalhostBypass())
+
     def get(self, name, default=None, domain=None, path=None):
         """Dict-like get() that also supports optional domain and path args in
         order to resolve naming collisions from using one cookie jar over
         multiple domains.
 
         .. warning:: operation is O(n), not O(1).
         """
```

### Comparing `niquests-3.6.4/src/niquests/exceptions.py` & `niquests-3.6.5/src/niquests/exceptions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/help.py` & `niquests-3.6.5/src/niquests/help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/hooks.py` & `niquests-3.6.5/src/niquests/hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/models.py` & `niquests-3.6.5/src/niquests/models.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/sessions.py` & `niquests-3.6.5/src/niquests/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,19 +64,14 @@
     ContentDecodingError,
     HTTPError,
     InvalidSchema,
     TooManyRedirects,
 )
 from .hooks import HOOKS, default_hooks, dispatch_hook
 
-try:
-    from .extensions._ocsp import verify as ocsp_verify
-except ImportError:
-    ocsp_verify = None  # type: ignore[assignment]
-
 # formerly defined here, reexposed here for backward compatibility
 from .models import (  # noqa: F401
     DEFAULT_REDIRECT_LIMIT,
     REDIRECT_STATI,
     PreparedRequest,
     Request,
     Response,
@@ -94,14 +89,15 @@
     resolve_proxies,
     rewind_body,
     should_bypass_proxies,
     to_key_val_list,
     create_resolver,
     _deepcopy_ci,
     parse_scheme,
+    is_ocsp_capable,
 )
 
 # Preferred clock, based on which one is more accurate on a given system.
 if sys.platform == "win32":
     preferred_clock = time.perf_counter
 else:
     preferred_clock = time.time
@@ -1083,29 +1079,34 @@
             """This function will be called by urllib3.future just after establishing the connection."""
             nonlocal ptr_request, request, kwargs
             ptr_request.conn_info = conn_info
 
             if (
                 ptr_request.url
                 and parse_scheme(ptr_request.url) == "https"
-                and ocsp_verify is not None
                 and kwargs["verify"]
+                and is_ocsp_capable(conn_info)
             ):
                 strict_ocsp_enabled: bool = (
                     os.environ.get("NIQUESTS_STRICT_OCSP", "0") != "0"
                 )
 
-                ocsp_verify(
-                    ptr_request,
-                    strict_ocsp_enabled,
-                    0.2 if not strict_ocsp_enabled else 1.0,
-                    kwargs["proxies"],
-                    resolver=self.resolver,
-                    happy_eyeballs=self._happy_eyeballs,
-                )
+                try:
+                    from .extensions._ocsp import verify as ocsp_verify
+                except ImportError:
+                    pass
+                else:
+                    ocsp_verify(
+                        ptr_request,
+                        strict_ocsp_enabled,
+                        0.2 if not strict_ocsp_enabled else 1.0,
+                        kwargs["proxies"],
+                        resolver=self.resolver,
+                        happy_eyeballs=self._happy_eyeballs,
+                    )
 
             # don't trigger pre_send for redirects
             if ptr_request == request:
                 dispatch_hook("pre_send", hooks, ptr_request)  # type: ignore[arg-type]
 
         def handle_upload_progress(
             total_sent: int,
```

### Comparing `niquests-3.6.4/src/niquests/status_codes.py` & `niquests-3.6.5/src/niquests/status_codes.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/structures.py` & `niquests-3.6.5/src/niquests/structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/utils.py` & `niquests-3.6.5/src/niquests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1169,7 +1169,30 @@
             return default
         raise MissingSchema(
             f"Invalid URL {url!r}: No scheme supplied. "
             f"Perhaps you meant https://{url}?"
         ) from e
 
     return scheme.lower()
+
+
+def is_ocsp_capable(conn_info: ConnectionInfo | None) -> bool:
+    # we can't do anything in that case.
+    if (
+        conn_info is None
+        or conn_info.certificate_der is None
+        or conn_info.certificate_dict is None
+    ):
+        return False
+
+    endpoints: list[str] = [  # type: ignore
+        # exclude non-HTTP endpoint. like ldap.
+        ep  # type: ignore
+        for ep in list(conn_info.certificate_dict.get("OCSP", []))  # type: ignore
+        if ep.startswith("http://")  # type: ignore
+    ]
+
+    # well... not all issued certificate have a OCSP entry. e.g. mkcert.
+    if not endpoints:
+        return False
+
+    return True
```

### Comparing `niquests-3.6.4/src/niquests/extensions/_async_ocsp.py` & `niquests-3.6.5/src/niquests/extensions/_async_ocsp.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/extensions/_ocsp.py` & `niquests-3.6.5/src/niquests/extensions/_ocsp.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/src/niquests/extensions/_picotls.py` & `niquests-3.6.5/src/niquests/extensions/_picotls.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/conftest.py` & `niquests-3.6.5/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,30 +30,45 @@
 
 
 @pytest.fixture
 def httpbin_secure(httpbin_secure):
     return prepare_url(httpbin_secure)
 
 
+class LocalhostCookieTestServer(SimpleHTTPRequestHandler):
+    def do_GET(self):
+        spot = self.headers.get("Cookie", None)
+
+        self.send_response(204)
+        self.send_header("Content-Length", "0")
+
+        if spot is None:
+            self.send_header("Set-Cookie", "hello=world; Domain=localhost; Max-Age=120")
+        else:
+            self.send_header("X-Cookie-Pass", "1" if "hello=world" in spot else "0")
+
+        self.end_headers()
+
+
 @pytest.fixture
-def nosan_server(tmp_path_factory):
+def san_server(tmp_path_factory):
     # delay importing until the fixture in order to make it possible
     # to deselect the test via command-line when trustme is not available
     import trustme
 
     tmpdir = tmp_path_factory.mktemp("certs")
     ca = trustme.CA()
-    # only commonName, no subjectAltName
-    server_cert = ca.issue_cert(common_name="localhost")
+
+    server_cert = ca.issue_cert("localhost", common_name="localhost")
     ca_bundle = str(tmpdir / "ca.pem")
     ca.cert_pem.write_to_path(ca_bundle)
 
     context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
     server_cert.configure_cert(context)
-    server = HTTPServer(("localhost", 0), SimpleHTTPRequestHandler)
+    server = HTTPServer(("localhost", 0), LocalhostCookieTestServer)
     server.socket = context.wrap_socket(server.socket, server_side=True)
     server_thread = threading.Thread(target=server.serve_forever)
     server_thread.start()
 
     yield "localhost", server.server_address[1], ca_bundle
 
     server.shutdown()
```

### Comparing `niquests-3.6.4/tests/test_async.py` & `niquests-3.6.5/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/test_help.py` & `niquests-3.6.5/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/test_hooks.py` & `niquests-3.6.5/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/test_live.py` & `niquests-3.6.5/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/test_lowlevel.py` & `niquests-3.6.5/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/test_multiplexed.py` & `niquests-3.6.5/tests/test_multiplexed.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/test_requests.py` & `niquests-3.6.5/tests/test_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1351,14 +1351,29 @@
         class MyCookiePolicy(cookielib.DefaultCookiePolicy):
             pass
 
         jar = niquests.cookies.RequestsCookieJar()
         jar.set_policy(MyCookiePolicy())
         assert isinstance(jar.copy().get_policy(), MyCookiePolicy)
 
+    def test_cookie_allow_localhost_default(self, san_server):
+        server, port, ca_bundle = san_server
+
+        s = niquests.Session()
+
+        r = s.get(f"https://localhost:{port}/", verify=ca_bundle)
+
+        assert r.cookies
+        assert r.cookies["hello"] == "world"
+
+        r = s.get(f"https://localhost:{port}/", verify=ca_bundle)
+
+        assert "x-cookie-pass" in r.headers
+        assert r.headers["x-cookie-pass"] == "1"
+
     def test_time_elapsed_blank(self, httpbin):
         r = niquests.get(httpbin("get"))
         td = r.elapsed
         total_seconds = (
             td.microseconds + (td.seconds + td.days * 24 * 3600) * 10**6
         ) / 10**6
         assert total_seconds > 0.0
```

### Comparing `niquests-3.6.4/tests/test_structures.py` & `niquests-3.6.5/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/test_testserver.py` & `niquests-3.6.5/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/test_utils.py` & `niquests-3.6.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/utils.py` & `niquests-3.6.5/tests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/tests/testserver/server.py` & `niquests-3.6.5/tests/testserver/server.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/LICENSE` & `niquests-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/README.md` & `niquests-3.6.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,24 +48,24 @@
 
 **High-Level APIs**
 
 | Client   | Average Delay to Complete | Notes                        |
 |----------|---------------------------|------------------------------|
 | requests | 987 ms                    | ThreadPoolExecutor. HTTP/1.1 |
 | httpx    | 720 ms                    | Asyncio. HTTP/2              |
-| niquests | 390 ms                    | Asyncio. HTTP/2              |
+| niquests | 370 ms                    | Asyncio. HTTP/2              |
 
 **Simplified APIs**
 
 | Client        | Average Delay to Complete | Notes                        |
 |---------------|---------------------------|------------------------------|
 | requests core | 643 ms                    | ThreadPoolExecutor. HTTP/1.1 |
 | httpx core    | 530 ms                    | Asyncio. HTTP/2              |
 | aiohttp       | 210 ms                    | Asyncio. HTTP/1.1            |
-| niquests core | 190 ms                    | Asyncio. HTTP/2              |
+| niquests core | 170 ms                    | Asyncio. HTTP/2              |
 
 Did you give up on HTTP/2 due to performance concerns? Think again! Do you realize that you can get 2.53 times faster with the same CPU if you ever switched to Niquests from Requests?
 Multiplexing and response lazyness open up a wide range of possibilities! Want to learn more about the tests? scripts? reasoning?
 
 Take a deeper look at https://github.com/Ousret/niquests-stats
 
 ⚠️ Do the responsible thing with this library and do not attempt DoS remote servers using its abilities.
@@ -190,9 +190,9 @@
 [^3]: while the HTTP/2 connection object can handle concurrent requests, you cannot leverage its true potential.
 [^4]: loading client certificate without file can't be done.
 [^5]: httpx officially claim to be thread safe but recent tests demonstrate otherwise as of february 2024. https://github.com/jawah/niquests/issues/83#issuecomment-1956065258 https://github.com/encode/httpx/issues/3072 https://github.com/encode/httpx/issues/3002
 [^6]: they do not expose anything to control network aspects such as IPv4/IPv6 toggles, and timings (e.g. DNS response time, established delay, TLS handshake delay, etc...) and such.
 [^7]: while advertised as possible, they refuse to make it the default due to performance issues. as of february 2024 an extra is required to enable it manually.
 [^8]: they don't support HTTP/3 at all.
 [^9]: you must use a custom DNS resolver so that it can preemptively connect using HTTP/3 over QUIC when remote is compatible.
-[^10]: performance measured when leveraging a multiplexed connection with or without uses of any form of concurrency as of March 2024. The research compared `httpx`, `requests`, `aiohttp` against `niquests`. See https://github.com/Ousret/niquests-stats
+[^10]: performance measured when leveraging a multiplexed connection with or without uses of any form of concurrency as of May 2024. The research compared `httpx`, `requests`, `aiohttp` against `niquests`. See https://github.com/Ousret/niquests-stats
 [^11]: enabled when using a custom DNS resolver.
```

### Comparing `niquests-3.6.4/pyproject.toml` & `niquests-3.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `niquests-3.6.4/PKG-INFO` & `niquests-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: niquests
-Version: 3.6.4
+Version: 3.6.5
 Summary: Niquests is a simple, yet elegant, HTTP library. It is a drop-in replacement for Requests, which is under feature freeze.
 Project-URL: Changelog, https://github.com/jawah/niquests/blob/main/HISTORY.md
 Project-URL: Documentation, https://niquests.readthedocs.io
 Project-URL: Code, https://github.com/jawah/niquests
 Project-URL: Issue tracker, https://github.com/jawah/niquests/issues
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -97,24 +97,24 @@
 
 **High-Level APIs**
 
 | Client   | Average Delay to Complete | Notes                        |
 |----------|---------------------------|------------------------------|
 | requests | 987 ms                    | ThreadPoolExecutor. HTTP/1.1 |
 | httpx    | 720 ms                    | Asyncio. HTTP/2              |
-| niquests | 390 ms                    | Asyncio. HTTP/2              |
+| niquests | 370 ms                    | Asyncio. HTTP/2              |
 
 **Simplified APIs**
 
 | Client        | Average Delay to Complete | Notes                        |
 |---------------|---------------------------|------------------------------|
 | requests core | 643 ms                    | ThreadPoolExecutor. HTTP/1.1 |
 | httpx core    | 530 ms                    | Asyncio. HTTP/2              |
 | aiohttp       | 210 ms                    | Asyncio. HTTP/1.1            |
-| niquests core | 190 ms                    | Asyncio. HTTP/2              |
+| niquests core | 170 ms                    | Asyncio. HTTP/2              |
 
 Did you give up on HTTP/2 due to performance concerns? Think again! Do you realize that you can get 2.53 times faster with the same CPU if you ever switched to Niquests from Requests?
 Multiplexing and response lazyness open up a wide range of possibilities! Want to learn more about the tests? scripts? reasoning?
 
 Take a deeper look at https://github.com/Ousret/niquests-stats
 
 ⚠️ Do the responsible thing with this library and do not attempt DoS remote servers using its abilities.
@@ -239,9 +239,9 @@
 [^3]: while the HTTP/2 connection object can handle concurrent requests, you cannot leverage its true potential.
 [^4]: loading client certificate without file can't be done.
 [^5]: httpx officially claim to be thread safe but recent tests demonstrate otherwise as of february 2024. https://github.com/jawah/niquests/issues/83#issuecomment-1956065258 https://github.com/encode/httpx/issues/3072 https://github.com/encode/httpx/issues/3002
 [^6]: they do not expose anything to control network aspects such as IPv4/IPv6 toggles, and timings (e.g. DNS response time, established delay, TLS handshake delay, etc...) and such.
 [^7]: while advertised as possible, they refuse to make it the default due to performance issues. as of february 2024 an extra is required to enable it manually.
 [^8]: they don't support HTTP/3 at all.
 [^9]: you must use a custom DNS resolver so that it can preemptively connect using HTTP/3 over QUIC when remote is compatible.
-[^10]: performance measured when leveraging a multiplexed connection with or without uses of any form of concurrency as of March 2024. The research compared `httpx`, `requests`, `aiohttp` against `niquests`. See https://github.com/Ousret/niquests-stats
+[^10]: performance measured when leveraging a multiplexed connection with or without uses of any form of concurrency as of May 2024. The research compared `httpx`, `requests`, `aiohttp` against `niquests`. See https://github.com/Ousret/niquests-stats
 [^11]: enabled when using a custom DNS resolver.
```

