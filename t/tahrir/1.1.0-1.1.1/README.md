# Comparing `tmp/tahrir-1.1.0.tar.gz` & `tmp/tahrir-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahrir-1.1.0.tar", max compression
+gzip compressed data, was "tahrir-1.1.1.tar", max compression
```

## Comparing `tahrir-1.1.0.tar` & `tahrir-1.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    34917 2024-05-19 07:32:48.736635 tahrir-1.1.0/LICENSE
--rw-r--r--   0        0        0     2699 2024-05-19 07:32:48.736635 tahrir-1.1.0/README.md
--rw-r--r--   0        0        0     2067 2024-05-19 07:32:48.740635 tahrir-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6089 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/__init__.py
--rw-r--r--   0        0        0     1522 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/app.py
--rw-r--r--   0        0        0      828 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/__init__.py
--rw-r--r--   0        0        0      251 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/constants.py
--rw-r--r--   0        0        0     5775 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/fedora.py
--rw-r--r--   0        0        0     2652 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/oauth.py
--rw-r--r--   0        0        0     3598 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/oauth_1.py
--rw-r--r--   0        0        0     2497 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/utils.py
--rw-r--r--   0        0        0     1906 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/views.py
--rw-r--r--   0        0        0     1506 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/events.py
--rw-r--r--   0        0        0     1061 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/notifications.py
--rw-r--r--   0        0        0      152 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/sitedocs/about.rst
--rw-r--r--   0        0        0      348 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/sitedocs/footer.rst
--rw-r--r--   0        0        0     2682 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/monokai.css
--rw-r--r--   0        0        0     6692 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/tahrir.css
--rw-r--r--   0        0        0    19275 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/unsemantic-grid-mobile.css
--rw-r--r--   0        0        0    64230 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/unsemantic-grid-responsive-tablet.css
--rw-r--r--   0        0        0    42765 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/unsemantic-grid-responsive.css
--rw-r--r--   0        0        0   337688 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/img/404.png
--rw-r--r--   0        0        0   353383 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/404.svg
--rw-r--r--   0        0        0   411482 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/500.png
--rw-r--r--   0        0        0   374146 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/500.svg
--rw-r--r--   0        0        0     9455 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badge.png
--rw-r--r--   0        0        0     1695 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badge_bullet.png
--rw-r--r--   0        0        0     3124 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badge_bullet_fedora.png
--rw-r--r--   0        0        0    10473 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badger_avatar.png
--rw-r--r--   0        0        0    21187 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badger_avatar.svg
--rw-r--r--   0        0        0      645 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/favicon.ico
--rw-r--r--   0        0        0    71006 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/fedora_badges.png
--rw-r--r--   0        0        0    13083 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/fedora_badges_small.png
--rw-r--r--   0        0        0     9380 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/fedora_logo.png
--rw-r--r--   0        0        0     3534 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/builder.js
--rw-r--r--   0        0        0     8380 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/favico-0.3.4.min.js
--rw-r--r--   0        0        0    86927 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/jquery-3.3.1.min.js
--rw-r--r--   0        0        0      619 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/social.js
--rw-r--r--   0        0        0    95029 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/Three.js
--rw-r--r--   0        0        0     3601 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/binaryReader.js
--rw-r--r--   0        0        0     1457 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/plane.js
--rw-r--r--   0        0        0     3801 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/stats.js
--rw-r--r--   0        0        0    10202 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/thingiloader.js
--rw-r--r--   0        0        0    26581 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/thingiview.js
--rw-r--r--   0        0        0      610 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/404.mak
--rw-r--r--   0        0        0      616 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/500.mak
--rw-r--r--   0        0        0        0 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/__init__.py
--rw-r--r--   0        0        0      154 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/about.mak
--rw-r--r--   0        0        0    12097 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/admin.mak
--rw-r--r--   0        0        0      525 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/assertion_widget.mak
--rw-r--r--   0        0        0     7160 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/badge-base.mak
--rw-r--r--   0        0        0       96 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/badge.mak
--rw-r--r--   0        0        0      156 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/badge_full.mak
--rw-r--r--   0        0        0     3938 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/builder.mak
--rw-r--r--   0        0        0     3083 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/diff.mak
--rw-r--r--   0        0        0     5527 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/explore.mak
--rw-r--r--   0        0        0     2781 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/explore_badges.mak
--rw-r--r--   0        0        0     2597 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/functions.mak
--rw-r--r--   0        0        0     2680 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/index.mak
--rw-r--r--   0        0        0     3064 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/leaderboard.mak
--rw-r--r--   0        0        0      402 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/login.mak
--rw-r--r--   0        0        0     6654 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/master.mak
--rw-r--r--   0        0        0     1291 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/report.mak
--rw-r--r--   0        0        0      764 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/tags.mak
--rw-r--r--   0        0        0     1210 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/thingiview.mak
--rw-r--r--   0        0        0     8867 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/user.mak
--rw-r--r--   0        0        0     4199 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/utils.py
--rw-r--r--   0        0        0    53811 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/views.py
--rw-r--r--   0        0        0      652 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/widgets.py
--rw-r--r--   0        0        0        0 2024-05-19 07:32:48.752635 tahrir-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0      758 2024-05-19 07:32:48.752635 tahrir-1.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 tahrir-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34917 2024-05-22 20:38:50.151341 tahrir-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2699 2024-05-22 20:38:50.151341 tahrir-1.1.1/README.md
+-rw-r--r--   0        0        0     2067 2024-05-22 20:38:50.155341 tahrir-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6089 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/__init__.py
+-rw-r--r--   0        0        0     1522 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/app.py
+-rw-r--r--   0        0        0      828 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/auth/__init__.py
+-rw-r--r--   0        0        0      251 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/auth/constants.py
+-rw-r--r--   0        0        0     5775 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/auth/fedora.py
+-rw-r--r--   0        0        0     2652 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/auth/oauth.py
+-rw-r--r--   0        0        0     3598 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/auth/oauth_1.py
+-rw-r--r--   0        0        0     2497 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/auth/utils.py
+-rw-r--r--   0        0        0     1906 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/auth/views.py
+-rw-r--r--   0        0        0     1506 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/events.py
+-rw-r--r--   0        0        0     1061 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/notifications.py
+-rw-r--r--   0        0        0      152 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/sitedocs/about.rst
+-rw-r--r--   0        0        0      348 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/sitedocs/footer.rst
+-rw-r--r--   0        0        0     2682 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/static/css/monokai.css
+-rw-r--r--   0        0        0     6692 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/static/css/tahrir.css
+-rw-r--r--   0        0        0    19275 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/static/css/unsemantic-grid-mobile.css
+-rw-r--r--   0        0        0    64230 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/static/css/unsemantic-grid-responsive-tablet.css
+-rw-r--r--   0        0        0    42765 2024-05-22 20:38:50.155341 tahrir-1.1.1/tahrir/static/css/unsemantic-grid-responsive.css
+-rw-r--r--   0        0        0   337688 2024-05-22 20:38:50.159341 tahrir-1.1.1/tahrir/static/img/404.png
+-rw-r--r--   0        0        0   353383 2024-05-22 20:38:50.159341 tahrir-1.1.1/tahrir/static/img/404.svg
+-rw-r--r--   0        0        0   411482 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/500.png
+-rw-r--r--   0        0        0   374146 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/500.svg
+-rw-r--r--   0        0        0     9455 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/badge.png
+-rw-r--r--   0        0        0     1695 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/badge_bullet.png
+-rw-r--r--   0        0        0     3124 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/badge_bullet_fedora.png
+-rw-r--r--   0        0        0    10473 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/badger_avatar.png
+-rw-r--r--   0        0        0    21187 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/badger_avatar.svg
+-rw-r--r--   0        0        0      645 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/favicon.ico
+-rw-r--r--   0        0        0    71006 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/fedora_badges.png
+-rw-r--r--   0        0        0    13083 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/fedora_badges_small.png
+-rw-r--r--   0        0        0     9380 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/img/fedora_logo.png
+-rw-r--r--   0        0        0     3534 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/builder.js
+-rw-r--r--   0        0        0     8380 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/favico-0.3.4.min.js
+-rw-r--r--   0        0        0    86927 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/jquery-3.3.1.min.js
+-rw-r--r--   0        0        0      619 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/social.js
+-rw-r--r--   0        0        0    95029 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/thingiview/Three.js
+-rw-r--r--   0        0        0     3601 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/thingiview/binaryReader.js
+-rw-r--r--   0        0        0     1457 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/thingiview/plane.js
+-rw-r--r--   0        0        0     3801 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/thingiview/stats.js
+-rw-r--r--   0        0        0    10202 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/thingiview/thingiloader.js
+-rw-r--r--   0        0        0    26581 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/static/js/thingiview/thingiview.js
+-rw-r--r--   0        0        0      610 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/404.mak
+-rw-r--r--   0        0        0      616 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/500.mak
+-rw-r--r--   0        0        0        0 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/__init__.py
+-rw-r--r--   0        0        0      154 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/about.mak
+-rw-r--r--   0        0        0    12097 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/admin.mak
+-rw-r--r--   0        0        0      525 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/assertion_widget.mak
+-rw-r--r--   0        0        0     7160 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/badge-base.mak
+-rw-r--r--   0        0        0       96 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/badge.mak
+-rw-r--r--   0        0        0      156 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/badge_full.mak
+-rw-r--r--   0        0        0     3938 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/builder.mak
+-rw-r--r--   0        0        0     3083 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/diff.mak
+-rw-r--r--   0        0        0     5527 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/explore.mak
+-rw-r--r--   0        0        0     2781 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/explore_badges.mak
+-rw-r--r--   0        0        0     2597 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/functions.mak
+-rw-r--r--   0        0        0     2680 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/index.mak
+-rw-r--r--   0        0        0     3064 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/leaderboard.mak
+-rw-r--r--   0        0        0      402 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/login.mak
+-rw-r--r--   0        0        0     6654 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/master.mak
+-rw-r--r--   0        0        0     1291 2024-05-22 20:38:50.163341 tahrir-1.1.1/tahrir/templates/report.mak
+-rw-r--r--   0        0        0      764 2024-05-22 20:38:50.167341 tahrir-1.1.1/tahrir/templates/tags.mak
+-rw-r--r--   0        0        0     1210 2024-05-22 20:38:50.167341 tahrir-1.1.1/tahrir/templates/thingiview.mak
+-rw-r--r--   0        0        0     8867 2024-05-22 20:38:50.167341 tahrir-1.1.1/tahrir/templates/user.mak
+-rw-r--r--   0        0        0     4199 2024-05-22 20:38:50.167341 tahrir-1.1.1/tahrir/utils.py
+-rw-r--r--   0        0        0    53943 2024-05-22 20:38:50.167341 tahrir-1.1.1/tahrir/views.py
+-rw-r--r--   0        0        0      652 2024-05-22 20:38:50.167341 tahrir-1.1.1/tahrir/widgets.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:38:50.167341 tahrir-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-22 20:38:50.167341 tahrir-1.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 tahrir-1.1.1/PKG-INFO
```

### Comparing `tahrir-1.1.0/LICENSE` & `tahrir-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/README.md` & `tahrir-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/pyproject.toml` & `tahrir-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tahrir"
-version = "1.1.0"
+version = "1.1.1"
 description = "A pyramid app for issuing your own Open Badges"
 
 license = "AGPLv3+ with additional permission"
 
 authors = [
   "Ralph Bean <rbean@redhat.com>",
   "Fedora Infrastructure <admin@fedoraproject.org>",
```

### Comparing `tahrir-1.1.0/tahrir/__init__.py` & `tahrir-1.1.1/tahrir/__init__.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/app.py` & `tahrir-1.1.1/tahrir/app.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/auth/__init__.py` & `tahrir-1.1.1/tahrir/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/auth/fedora.py` & `tahrir-1.1.1/tahrir/auth/fedora.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/auth/oauth.py` & `tahrir-1.1.1/tahrir/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/auth/oauth_1.py` & `tahrir-1.1.1/tahrir/auth/oauth_1.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/auth/utils.py` & `tahrir-1.1.1/tahrir/auth/utils.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/auth/views.py` & `tahrir-1.1.1/tahrir/auth/views.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/events.py` & `tahrir-1.1.1/tahrir/events.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/notifications.py` & `tahrir-1.1.1/tahrir/notifications.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/css/monokai.css` & `tahrir-1.1.1/tahrir/static/css/monokai.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/css/tahrir.css` & `tahrir-1.1.1/tahrir/static/css/tahrir.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/css/unsemantic-grid-mobile.css` & `tahrir-1.1.1/tahrir/static/css/unsemantic-grid-mobile.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/css/unsemantic-grid-responsive-tablet.css` & `tahrir-1.1.1/tahrir/static/css/unsemantic-grid-responsive-tablet.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/css/unsemantic-grid-responsive.css` & `tahrir-1.1.1/tahrir/static/css/unsemantic-grid-responsive.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/404.png` & `tahrir-1.1.1/tahrir/static/img/404.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/404.svg` & `tahrir-1.1.1/tahrir/static/img/404.svg`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/500.png` & `tahrir-1.1.1/tahrir/static/img/500.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/500.svg` & `tahrir-1.1.1/tahrir/static/img/500.svg`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/badge.png` & `tahrir-1.1.1/tahrir/static/img/badge.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/badge_bullet.png` & `tahrir-1.1.1/tahrir/static/img/badge_bullet.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/badge_bullet_fedora.png` & `tahrir-1.1.1/tahrir/static/img/badge_bullet_fedora.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/badger_avatar.png` & `tahrir-1.1.1/tahrir/static/img/badger_avatar.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/badger_avatar.svg` & `tahrir-1.1.1/tahrir/static/img/badger_avatar.svg`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/favicon.ico` & `tahrir-1.1.1/tahrir/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/fedora_badges.png` & `tahrir-1.1.1/tahrir/static/img/fedora_badges.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/fedora_badges_small.png` & `tahrir-1.1.1/tahrir/static/img/fedora_badges_small.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/img/fedora_logo.png` & `tahrir-1.1.1/tahrir/static/img/fedora_logo.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/builder.js` & `tahrir-1.1.1/tahrir/static/js/builder.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/favico-0.3.4.min.js` & `tahrir-1.1.1/tahrir/static/js/favico-0.3.4.min.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/jquery-3.3.1.min.js` & `tahrir-1.1.1/tahrir/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/social.js` & `tahrir-1.1.1/tahrir/static/js/social.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/thingiview/Three.js` & `tahrir-1.1.1/tahrir/static/js/thingiview/Three.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/thingiview/binaryReader.js` & `tahrir-1.1.1/tahrir/static/js/thingiview/binaryReader.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/thingiview/plane.js` & `tahrir-1.1.1/tahrir/static/js/thingiview/plane.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/thingiview/stats.js` & `tahrir-1.1.1/tahrir/static/js/thingiview/stats.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/thingiview/thingiloader.js` & `tahrir-1.1.1/tahrir/static/js/thingiview/thingiloader.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/static/js/thingiview/thingiview.js` & `tahrir-1.1.1/tahrir/static/js/thingiview/thingiview.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/404.mak` & `tahrir-1.1.1/tahrir/templates/404.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/500.mak` & `tahrir-1.1.1/tahrir/templates/500.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/admin.mak` & `tahrir-1.1.1/tahrir/templates/admin.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/assertion_widget.mak` & `tahrir-1.1.1/tahrir/templates/assertion_widget.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/badge-base.mak` & `tahrir-1.1.1/tahrir/templates/badge-base.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/builder.mak` & `tahrir-1.1.1/tahrir/templates/builder.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/diff.mak` & `tahrir-1.1.1/tahrir/templates/diff.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/explore.mak` & `tahrir-1.1.1/tahrir/templates/explore.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/explore_badges.mak` & `tahrir-1.1.1/tahrir/templates/explore_badges.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/functions.mak` & `tahrir-1.1.1/tahrir/templates/functions.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/index.mak` & `tahrir-1.1.1/tahrir/templates/index.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/leaderboard.mak` & `tahrir-1.1.1/tahrir/templates/leaderboard.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/master.mak` & `tahrir-1.1.1/tahrir/templates/master.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/report.mak` & `tahrir-1.1.1/tahrir/templates/report.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/tags.mak` & `tahrir-1.1.1/tahrir/templates/tags.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/thingiview.mak` & `tahrir-1.1.1/tahrir/templates/thingiview.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/templates/user.mak` & `tahrir-1.1.1/tahrir/templates/user.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/utils.py` & `tahrir-1.1.1/tahrir/utils.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tahrir/views.py` & `tahrir-1.1.1/tahrir/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,25 +293,29 @@
             try:
                 expires_on = datetime.strptime(
                     request.POST.get("invitation-expires"), "%Y-%m-%d %H:%M"
                 )
             except ValueError:
                 expires_on = None  # Will default to datettime.now(timezone.utc)
 
-            request.db.add_invitation(
-                request.POST.get("invitation-badge-id"),
-                created_on=created_on,
-                expires_on=expires_on,
-                created_by_email=request.POST.get("invitation-issuer-email"),
-            )
-            request.session.flash(
-                "You added an invitation for badge {}".format(
-                    request.POST.get("invitation-badge-id")
+            try:
+                request.db.add_invitation(
+                    request.POST.get("invitation-badge-id"),
+                    created_on=created_on,
+                    expires_on=expires_on,
+                    created_by_email=request.POST.get("invitation-issuer-email"),
+                )
+            except ValueError as e:
+                request.session.flash(str(e))
+            else:
+                request.session.flash(
+                    "You added an invitation for badge {}".format(
+                        request.POST.get("invitation-badge-id")
+                    )
                 )
-            )
         elif request.POST.get("add-issuer"):
             origin = request.POST.get("issuer-origin")
             name = request.POST.get("issuer-name")
             if not request.db.issuer_exists(origin, name):
                 # Add an Issuer to the DB.
                 request.db.add_issuer(
                     origin, name, request.POST.get("issuer-org"), request.POST.get("issuer-contact")
@@ -441,17 +445,15 @@
     person = request.db.get_person(person_email=request.authenticated_userid)
 
     # Check to see if the user already has the badge.
     if request.context.badge in [a.badge for a in person.assertions]:
         request.session.flash("You already have " + request.context.badge_id + " badge")
         return HTTPFound(location=request.route_url("home"))
 
-    # result = request.db.add_assertion(
-    #     request.context.badge_id, person.email, datetime.now(timezone.utc)
-    # )
+    request.db.add_assertion(request.context.badge_id, person.email, datetime.now(timezone.utc))
 
     # TODO -- return them to a page that auto-exports their badges.
     request.session.flash("You have earned " + request.context.badge_id + " badge")
     return HTTPFound(location=request.route_url("home"))
 
 
 @view_config(context=m.Invitation, name="qrcode")
```

### Comparing `tahrir-1.1.0/tahrir/widgets.py` & `tahrir-1.1.1/tahrir/widgets.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/tests/test_utils.py` & `tahrir-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.1.0/PKG-INFO` & `tahrir-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahrir
-Version: 1.1.0
+Version: 1.1.1
 Summary: A pyramid app for issuing your own Open Badges
 Home-page: https://github.com/fedora-infra/tahrir
 License: AGPLv3+ with additional permission
 Author: Ralph Bean
 Author-email: rbean@redhat.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Environment :: Web Environment
```

