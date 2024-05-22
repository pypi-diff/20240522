# Comparing `tmp/qtile-extras-0.25.0.tar.gz` & `tmp/qtile_extras-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtile-extras-0.25.0.tar", last modified: Sat Apr  6 16:50:59 2024, max compression
+gzip compressed data, was "qtile_extras-0.26.0.tar", last modified: Wed May 22 04:37:47 2024, max compression
```

## Comparing `qtile-extras-0.25.0.tar` & `qtile_extras-0.26.0.tar`

### file list

```diff
@@ -1,244 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.382254 qtile-extras-0.25.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/.github/
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/check_for_changes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-06 16:50:59.382254 qtile-extras-0.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/popup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/popup/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/templates/mpris2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/templates/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    51899 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/dbusmenu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/footballscores/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/fixtures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24538 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/footballmatch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5213 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/league.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3551 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/matchdict.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2382 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/matchevent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/morphlinks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/playeraction.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1317 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/github-icons/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/github-icons/github.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/global_menu/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/global_menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/global_menu/registrar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/media-icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/default.png
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/default.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/next.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/play_pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/previous.svg
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/stop.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/snapcast-icons/
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/snapcast-icons/snapcast.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/stravadata/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/stravadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/stravadata/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/stravadata/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/syncthing/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/syncthing/syncthing.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/tvheadend-icons/
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/tvheadend-icons/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.354254 qtile-extras-0.25.0/qtile_extras/resources/visualiser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/visualiser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5038 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/visualiser/cava_draw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.354254 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27699 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)   326251 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_triangles.png
--rw-r--r--   0 runner    (1001) docker     (127)   330247 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_triangles_rounded.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.354254 qtile-extras-0.25.0/qtile_extras/resources/wordclock/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/dutch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/english.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/finnish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/french.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/portuguese.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/spanish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/swedish.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/qtile_extras/widget/
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/alsavolumecontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/analogueclock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/animatedimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/brightnesscontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/continuous_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/currentlayout.py
--rw-r--r--   0 runner    (1001) docker     (127)    33001 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/decorations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/githubnotifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/globalmenu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    33152 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/groupbox2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    23460 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/iwd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23089 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/livefootballscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/qtile_extras/widget/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)    25797 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/mpris2widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/pulse_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/pulse_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/scriptexit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/snapcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/statusnotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/strava.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/syncthing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/systray.py
--rw-r--r--   0 runner    (1001) docker     (127)    10887 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/tvheadend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/unitstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/upower.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/visualiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/wordclock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/qtile_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-06 16:50:59.000000 qtile-extras-0.25.0/qtile_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-06 16:50:59.000000 qtile-extras-0.25.0/qtile_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:50:59.000000 qtile-extras-0.25.0/qtile_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 16:50:59.000000 qtile-extras-0.25.0/qtile_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-06 16:50:59.382254 qtile-extras-0.25.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/backend/wayland/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/wayland/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/wayland/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/backend/x11/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/x11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/x11/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/popup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/popup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/popup/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/popup/test_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.342254 qtile-extras-0.25.0/test/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.366254 qtile-extras-0.25.0/test/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/audio-volume-high.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/audio-volume-low.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/audio-volume-medium.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/audio-volume-muted.svg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/menuitem.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.370254 qtile-extras-0.25.0/test/resources/test_images/
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding_x.png
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding_y.png
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default.png
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-E-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-E.png
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-N-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-N.png
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-S-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-S.png
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-W-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-W.png
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-stacked-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-stacked-same-position.png
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-stacked.png
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/combo-rect-plus-powerline.png
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_left-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_left.png
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_right-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_right.png
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-back_slash-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-back_slash.png
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-custom-path.png
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-forward_slash-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-forward_slash.png
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_left-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_left.png
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_right-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_right.png
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-zig_zag-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-zig_zag.png
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-filled.png
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled-no-radius.png
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled-widget-background.png
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled.png
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-line.png
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default.png
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-stacked.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.370254 qtile-extras-0.25.0/test/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/scripts/cpoll.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/scripts/exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/scripts/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/test_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/test_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/test/widget/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/test/widget/decorations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/decorations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/decorations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/decorations/test_decoration_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/decorations/test_widget_decorations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/test/widget/docs_screenshots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/docs_screenshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/docs_screenshots/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/docs_screenshots/ss_groupbox2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/docs_screenshots/ss_iwd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/test/widget/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47648 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/resources/lfs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_alsawidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_analogueclock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_animated_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_brightness_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_continuous_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_currentlayouticon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_githubnotifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_global_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_groupbox2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_init_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_injection_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_iwd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_livefootballscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_mpris2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_popup_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_scriptexit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_snapcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_statusnotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_strava.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_syncthing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_tvhwidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_unitstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_upower.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_visualiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_widget_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_wordclock.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/whitelist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.969831 qtile_extras-0.26.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.929830 qtile_extras-0.26.0/.github/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/.github/check_for_changes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.929830 qtile_extras-0.26.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-22 04:37:47.969831 qtile_extras-0.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.929830 qtile_extras-0.26.0/qtile_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.933830 qtile_extras-0.26.0/qtile_extras/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/layout/_mods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.933830 qtile_extras-0.26.0/qtile_extras/layout/decorations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/layout/decorations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/layout/decorations/borders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/layout/decorations/injections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/layout/plasma.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.933830 qtile_extras-0.26.0/qtile_extras/popup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/popup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/popup/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.933830 qtile_extras-0.26.0/qtile_extras/popup/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/popup/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/popup/templates/mpris2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/popup/templates/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53867 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/popup/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.933830 qtile_extras-0.26.0/qtile_extras/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.933830 qtile_extras-0.26.0/qtile_extras/resources/dbusmenu/
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/dbusmenu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/dbusmenu/dbusmenu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.937830 qtile_extras-0.26.0/qtile_extras/resources/footballscores/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/fixtures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24538 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/footballmatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5213 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/league.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3551 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/matchdict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2382 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/matchevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/morphlinks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/playeraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1317 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/footballscores/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.937830 qtile_extras-0.26.0/qtile_extras/resources/github-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/github-icons/github.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.937830 qtile_extras-0.26.0/qtile_extras/resources/global_menu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/global_menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/global_menu/registrar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.937830 qtile_extras-0.26.0/qtile_extras/resources/media-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/media-icons/default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/media-icons/default.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/media-icons/next.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/media-icons/play_pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/media-icons/previous.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/media-icons/stop.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.937830 qtile_extras-0.26.0/qtile_extras/resources/snapcast-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/snapcast-icons/snapcast.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.937830 qtile_extras-0.26.0/qtile_extras/resources/stravadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/stravadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/stravadata/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/stravadata/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.937830 qtile_extras-0.26.0/qtile_extras/resources/syncthing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/syncthing/syncthing.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.937830 qtile_extras-0.26.0/qtile_extras/resources/tvheadend-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/tvheadend-icons/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.937830 qtile_extras-0.26.0/qtile_extras/resources/visualiser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/visualiser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5038 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/visualiser/cava_draw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.941830 qtile_extras-0.26.0/qtile_extras/resources/wallpapers/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wallpapers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27699 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wallpapers/qte_tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)   326251 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wallpapers/qte_triangles.png
+-rw-r--r--   0 runner    (1001) docker     (127)   330247 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wallpapers/qte_triangles_rounded.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.941830 qtile_extras-0.26.0/qtile_extras/resources/wordclock/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wordclock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wordclock/dutch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wordclock/english.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wordclock/finnish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wordclock/french.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wordclock/portuguese.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wordclock/spanish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/resources/wordclock/swedish.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.949830 qtile_extras-0.26.0/qtile_extras/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/alsavolumecontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/analogueclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/animatedimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/brightnesscontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/continuous_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/currentlayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33001 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/decorations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/githubnotifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/globalmenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33152 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/groupbox2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23460 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/iwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23089 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/livefootballscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.949830 qtile_extras-0.26.0/qtile_extras/widget/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)    25797 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/mpris2widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/pulse_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/pulse_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/scriptexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/snapcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/statusnotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/strava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/syncthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/systray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10887 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/tvheadend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/unitstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/upower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/visualiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/qtile_extras/widget/wordclock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.969831 qtile_extras-0.26.0/qtile_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-22 04:37:47.000000 qtile_extras-0.26.0/qtile_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-22 04:37:47.000000 qtile_extras-0.26.0/qtile_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:37:47.000000 qtile_extras-0.26.0/qtile_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 04:37:47.000000 qtile_extras-0.26.0/qtile_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-22 04:37:47.969831 qtile_extras-0.26.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.949830 qtile_extras-0.26.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.949830 qtile_extras-0.26.0/test/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.949830 qtile_extras-0.26.0/test/backend/wayland/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/backend/wayland/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/backend/wayland/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.949830 qtile_extras-0.26.0/test/backend/x11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/backend/x11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/backend/x11/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.949830 qtile_extras-0.26.0/test/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.949830 qtile_extras-0.26.0/test/layout/decorations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/layout/decorations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/layout/decorations/test_border_decorations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.953831 qtile_extras-0.26.0/test/popup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/popup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/popup/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/popup/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.925830 qtile_extras-0.26.0/test/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.953831 qtile_extras-0.26.0/test/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/icons/audio-volume-high.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/icons/audio-volume-low.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/icons/audio-volume-medium.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/icons/audio-volume-muted.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/icons/menuitem.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.961830 qtile_extras-0.26.0/test/resources/test_images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-default-grouped-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-default-grouped-padding_x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-default-grouped-padding_y.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-default-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-default-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-single-E-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-single-E.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-single-N-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-single-N.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-single-S-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-single-S.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-single-W-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-single-W.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-stacked-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-stacked-same-position.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/border-stacked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/combo-rect-plus-powerline.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-arrow_left-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-arrow_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-arrow_right-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-arrow_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-back_slash-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-back_slash.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-custom-path.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-forward_slash-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-forward_slash.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-rounded_left-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-rounded_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-rounded_right-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-rounded_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-zig_zag-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/powerline-zig_zag.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/rect-default-filled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/rect-default-group-filled-no-radius.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/rect-default-group-filled-widget-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/rect-default-group-filled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/rect-default-line.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/rect-default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/resources/test_images/rect-stacked.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.961830 qtile_extras-0.26.0/test/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/scripts/cpoll.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/scripts/exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/scripts/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/test_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/test_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.965830 qtile_extras-0.26.0/test/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.965830 qtile_extras-0.26.0/test/widget/decorations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/decorations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/decorations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/decorations/test_decoration_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/decorations/test_widget_decorations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.969831 qtile_extras-0.26.0/test/widget/docs_screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/docs_screenshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/docs_screenshots/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/docs_screenshots/ss_groupbox2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/docs_screenshots/ss_iwd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:47.969831 qtile_extras-0.26.0/test/widget/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47648 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/resources/lfs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_alsawidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_analogueclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_animated_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_brightness_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_continuous_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_currentlayouticon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_githubnotifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_global_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_groupbox2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_init_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_injection_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_iwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_livefootballscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_mpris2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_popup_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_scriptexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_snapcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_statusnotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_strava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_syncthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_tvhwidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_unitstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_upower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_visualiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_widget_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/test/widget/test_wordclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 04:37:43.000000 qtile_extras-0.26.0/whitelist.py
```

### Comparing `qtile-extras-0.25.0/.github/workflows/changelog.yml` & `qtile_extras-0.26.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/.github/workflows/ci.yml` & `qtile_extras-0.26.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/.github/workflows/release.yml` & `qtile_extras-0.26.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/.gitignore` & `qtile_extras-0.26.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/.pre-commit-config.yaml` & `qtile_extras-0.26.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/CHANGELOG` & `qtile_extras-0.26.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2024-05-22: [RELEASE] v0.26.0 release - compatible with qtile 0.26.0
+2024-05-19: [FEATURE] Add modified `Plasma` layout to include border highlighting
+2024-05-10: [FEATURE] Add window border decorations (NB experimental)
+2024-04-26: [FEATURE] Add hooks to `ALSAWidget` and `PulseVolumeExtra`
+2024-04-25: [FEATURE] Add ability to drag `PopupSlider` and `PopupCircularProgress` controls (NB experimental)
+2024-04-25: [BREAKING CHANGE] Update to using lazy calls in popups. Needs latest qtile.
 2024-04-08: [RELEASE] v0.25.0 release - compatible with qtile 0.25.0
 2024-03-10: [FEATURE] Expose widget popup menu commands and allow custom positioning
 2024-03-02: [BUGFIX] Fix bug for volume widgets where bar crashes if volume is greater than 100%
 2024-03-02: [BUGFIX] Fix popup menus ignoring config
 2024-02-17: [FEATURE] Add `AnimatedImage` widget
 2024-02-16: [FEATURE] Allow pango markup in `PopupText` controls
 2024-02-09: [BUGFIX] Handle connection errors in `GithubNotifications` widget
```

### Comparing `qtile-extras-0.25.0/LICENSE` & `qtile_extras-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/PKG-INFO` & `qtile_extras-0.26.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtile-extras
-Version: 0.25.0
+Version: 0.26.0
 Summary: Extra items for qtile that are unlikely to be maintained in the main repo.
 Author: elParaguayo
 License: MIT
 Project-URL: homepage, https://github.com/elParaguayo/qtile-extras
 Project-URL: documentation, https://qtile-extras.readthedocs.io/en/stable/
 Project-URL: changelog, https://qtile-extras.readthedocs.io/en/stable/changelog.html
 Project-URL: issues, https://github.com/elParaguayo/qtile-extras/issues
```

### Comparing `qtile-extras-0.25.0/README.md` & `qtile_extras-0.26.0/README.md`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/pyproject.toml` & `qtile_extras-0.26.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/bar.py` & `qtile_extras-0.26.0/qtile_extras/bar.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/hook.py` & `qtile_extras-0.26.0/qtile_extras/hook.py`

 * *Files 22% similar despite different names*

```diff
@@ -372,13 +372,63 @@
 
         """,
     ),
 ]
 
 hooks.extend(mpris_hooks)
 
+# Volume hooks
+volume_hooks = [
+    Hook(
+        "volume_change",
+        """
+        Fired when the volume value changes.
+
+        Receives an integer volume percentage (0-100) and boolean muted status.
+
+        .. code:: python
+
+          from libqtile import qtile
+          from libqtile.utils import send_notification
+
+          import qtile_extras.hook
+
+          @qtile_extras.hook.subscribe.volume_change
+          def vol_change(volume, muted):
+              send_notification("Volume change", f"Volume is now {volume}%")
+
+        """,
+    ),
+    Hook(
+        "volume_mute_change",
+        """
+        Fired when the volume mute status changes.
+
+        Receives an integer volume percentage (0-100) and boolean muted status.
+
+        The signature is the same as ``volume_change`` to allow the same function to be
+        used for both hooks.
+
+        .. code:: python
+
+          from libqtile import qtile
+          from libqtile.utils import send_notification
+
+          import qtile_extras.hook
+
+          @qtile_extras.hook.subscribe.volume_mute_change
+          def mute_change(volume, muted):
+              if muted:
+                send_notification("Volume change", "Volume is now muted.")
+
+        """,
+    ),
+]
+
+hooks.extend(volume_hooks)
+
 # Build the registry and expose helpful entrypoints
 qte = Registry("qtile-extras", hooks)
 
 subscribe = qte.subscribe
 unsubscribe = qte.unsubscribe
 fire = qte.fire
```

### Comparing `qtile-extras-0.25.0/qtile_extras/images.py` & `qtile_extras-0.26.0/qtile_extras/images.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/popup/menu.py` & `qtile_extras-0.26.0/qtile_extras/popup/menu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/popup/templates/__init__.py` & `qtile_extras-0.26.0/qtile_extras/popup/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/popup/templates/mpris2.py` & `qtile_extras-0.26.0/qtile_extras/popup/templates/mpris2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/popup/templates/volume.py` & `qtile_extras-0.26.0/qtile_extras/popup/templates/volume.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/popup/toolkit.py` & `qtile_extras-0.26.0/qtile_extras/popup/toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,16 @@
         # Build dict of updateable controls
         self._set_updateable_controls()
 
         self._autohide_timer = None
         self._hide_timer = None
         self._killed = False
 
+        self._clicked = None
+
     def _configure(self, qtile: Qtile | None = None):
         """
         This method creates an instances of a Popup window which serves as the
         base for the tooltip.
 
         We also attach handlers for mouse events so that these can be passed to
         the relevant controls.
@@ -245,14 +247,17 @@
         coordinates i.e. for ``relative_to=7`` an x, y value of 0, 0 would place the
         bottom left corner of the popup in the bottom left corner of the screen. The
         x, y values can be integers representing the number of pixels to move, or a float
         representing the percentage of the screen's dimensions to move. In all cases, a
         positive x value will shift the popup to the right and a positive y value will shift
         the popup down.
 
+        Setting ``relative_to=0`` is a special case which positions the top left corner of the
+        popup at the mouse's current location.
+
         Setting ``relative_to_bar=True`` will automatically adjust the offset by the width of
         the bar or gap (including any margin) nearest the point on the above grid
         i.e. if ``relative_to=1`` then the y coordinate would be adjusted for any bar on the
         top of the screen and the x would be adjusted for any bar on the left. NB If you set
         ``relative_to-bar=True`` and you use a float value for x and/or y, the float value is
         still calculated by reference to the whole screen's dimensions (i.e. including the space
         occupied by the bar).
@@ -276,15 +281,18 @@
             # If x and y are floats then we calculate the percentage of screen dimensions
             if isinstance(x, float):
                 x = int(scr.width * x)
 
             if isinstance(y, float):
                 y = int(scr.height * y)
 
-            if relative_to == 1:
+            if relative_to == 0:
+                x, y = self.qtile.core.get_mouse_position()
+
+            elif relative_to == 1:
                 x += scr.x
                 y += scr.y
 
             elif relative_to == 2:
                 x += scr.x + (scr.width - self.popup.width) // 2
                 y += scr.y
 
@@ -399,21 +407,28 @@
         for c in self.controls:
             if c.mouse_in_control(x, y):
                 controls.insert(0, c)
         return controls
 
     def process_button_click(self, x, y, button):  # noqa: N802
         controls = self.get_control_in_position(x, y)
+        if self._clicked is None:
+            self._clicked = next(iter(controls), None)
         for control in controls:
             control.button_press(x - control.offsetx, y - control.offsety, button)
         if self.close_on_click:
             self.kill()
 
     def process_button_release(self, x, y, button):  # noqa: N802
         controls = self.get_control_in_position(x, y)
+        if self._clicked is not None:
+            self._clicked.button_release(
+                x - self._clicked.offsetx, y - self._clicked.offsety, button
+            )
+            self._clicked = None
         for control in controls:
             control.button_release(x - control.offsetx, y - control.offsety, button)
 
     def process_pointer_enter(self, x, y):  # noqa: N802
         controls = self.get_control_in_position(x, y)
         for control in controls:
             control.mouse_enter(
@@ -433,14 +448,19 @@
             )
             self.cursor_in = None
         if self.hide_on_mouse_leave:
             self._hide_timer = self.qtile.call_later(self.hide_interval, self.kill)
 
     def process_pointer_motion(self, x, y):  # noqa: N802
         controls = self.get_control_in_position(x, y)
+        if self._clicked:
+            self._clicked.pointer_motion(
+                x - self._clicked.offsetx,
+                y - self._clicked.offsety,
+            )
         if self.cursor_in and self.cursor_in not in controls:
             self.cursor_in.mouse_leave(
                 x - self.cursor_in.offsetx,
                 y - self.cursor_in.offsety,
             )
         for control in controls:
             control.mouse_enter(
@@ -933,15 +953,15 @@
 
     def button_press(self, x, y, button):
         name = "Button{0}".format(button)
         if name in self.mouse_callbacks:
             cmd = self.mouse_callbacks[name]
             if isinstance(cmd, LazyCall):
                 status, val = self.qtile.server.call(
-                    (cmd.selectors, cmd.name, cmd.args, cmd.kwargs)
+                    (cmd.selectors, cmd.name, cmd.args, cmd.kwargs, False)
                 )
                 if status in (interface.ERROR, interface.EXCEPTION):
                     logger.error("KB command error %s: %s", cmd.name, val)
             else:
                 cmd()
 
     def button_release(self, x, y, button):
@@ -955,14 +975,17 @@
 
     def mouse_leave(self, x, y):
         if self.can_focus and self._highlight:
             self.unfocus()
             self.draw()
             self.container.draw()
 
+    def pointer_motion(self, x, y):
+        pass
+
     def info(self):
         return {
             "name": self.name or self.__class__.__name__.lower(),
             "x": self.offsetx,
             "y": self.offsety,
             "width": self.width,
             "height": self.height,
@@ -1117,20 +1140,26 @@
         ("bar_size", 2, "Thickness of bar"),
         ("marker_size", 10, "Size of marker"),
         ("marker_colour", "#bbbbbb", "Colour of marker"),
         ("end_margin", 5, "Gap between edge of control and ends of the bar/border"),
         ("bar_border_colour", "ffffff", "Colour of border drawn around bar"),
         ("bar_border_size", 0, "Thickness of border around bar"),
         ("bar_border_margin", 0, "Size of gap between border and bar"),
+        (
+            "drag_callback",
+            None,
+            "Callback to run after dragging slider. Callback should take a single argument ``new_value``.",
+        ),
     ]  # type: list[tuple[str, Any, str]]
 
     def __init__(self, value=None, **config):
         _PopupWidget.__init__(self, **config)
         self.add_defaults(PopupSlider.defaults)
         self._value = self._check_value(value)
+        self._drag = False
 
     def _check_value(self, val):
         if val is None or type(val) not in (int, float):
             return self.min_value
         return min(max(val, self.min_value), self.max_value)
 
     def _configure(self, qtile, container):
@@ -1182,22 +1211,50 @@
         if self.marker_size:
             self.drawer.set_source_rgb(self.marker_colour)
             ctx.arc(self.bar_length * self.percentage, 0, self.marker_size / 2, 0, math.pi * 2)
             ctx.fill()
 
         ctx.restore()
 
+    def button_press(self, x, y, button):
+        if not self._drag:
+            self._drag = True
+            self._old_value = self.value
+            _PopupWidget.button_press(self, x, y, button)
+
+    def button_release(self, x, y, button):
+        if self._drag:
+            if self.drag_callback:
+                try:
+                    self.drag_callback(self.value)
+                except Exception:
+                    logger.exception("Error calling drag_callback.")
+
+            self._drag = False
+        _PopupWidget.button_release(self, x, y, button)
+
+    def pointer_motion(self, x, y):
+        if self._drag:
+            if self.horizontal:
+                percent = (x - self.end_margin) / self.bar_length
+            else:
+                percent = (y - self.end_margin) / self.bar_length
+            percent = max(min(percent, 1), 0)
+
+            self.value = ((self.max_value - self.min_value) * percent) + self.min_value
+
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, val):
         self._value = self._check_value(val)
         self.draw()
+        self.container.popup.draw()
 
     @property
     def percentage(self):
         return (self.value - self.min_value) / (self.max_value - self.min_value)
 
     @property
     def length(self):
```

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/__init__.py` & `qtile_extras-0.26.0/qtile_extras/resources/dbusmenu/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/dbusmenu.py` & `qtile_extras-0.26.0/qtile_extras/resources/dbusmenu/dbusmenu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/footballscores/__init__.py` & `qtile_extras-0.26.0/qtile_extras/resources/footballscores/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/footballscores/exceptions.py` & `qtile_extras-0.26.0/qtile_extras/resources/footballscores/exceptions.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/footballscores/footballmatch.py` & `qtile_extras-0.26.0/qtile_extras/resources/footballscores/footballmatch.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/footballscores/league.py` & `qtile_extras-0.26.0/qtile_extras/resources/footballscores/league.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/footballscores/matchdict.py` & `qtile_extras-0.26.0/qtile_extras/resources/footballscores/matchdict.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/footballscores/matchevent.py` & `qtile_extras-0.26.0/qtile_extras/resources/footballscores/matchevent.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/footballscores/morphlinks.py` & `qtile_extras-0.26.0/qtile_extras/resources/footballscores/morphlinks.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/footballscores/playeraction.py` & `qtile_extras-0.26.0/qtile_extras/resources/footballscores/playeraction.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/footballscores/utils.py` & `qtile_extras-0.26.0/qtile_extras/resources/footballscores/utils.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/github-icons/github.svg` & `qtile_extras-0.26.0/qtile_extras/resources/github-icons/github.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/global_menu/__init__.py` & `qtile_extras-0.26.0/qtile_extras/resources/global_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/global_menu/registrar.py` & `qtile_extras-0.26.0/qtile_extras/resources/global_menu/registrar.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/media-icons/default.png` & `qtile_extras-0.26.0/qtile_extras/resources/media-icons/default.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/media-icons/default.svg` & `qtile_extras-0.26.0/qtile_extras/resources/media-icons/default.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/media-icons/next.svg` & `qtile_extras-0.26.0/qtile_extras/resources/media-icons/next.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/media-icons/play_pause.svg` & `qtile_extras-0.26.0/qtile_extras/resources/media-icons/play_pause.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/media-icons/previous.svg` & `qtile_extras-0.26.0/qtile_extras/resources/media-icons/previous.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/media-icons/stop.svg` & `qtile_extras-0.26.0/qtile_extras/resources/media-icons/stop.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/snapcast-icons/snapcast.svg` & `qtile_extras-0.26.0/qtile_extras/resources/snapcast-icons/snapcast.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/stravadata/locations.py` & `qtile_extras-0.26.0/qtile_extras/resources/stravadata/locations.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/stravadata/sync.py` & `qtile_extras-0.26.0/qtile_extras/resources/stravadata/sync.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/syncthing/syncthing.svg` & `qtile_extras-0.26.0/qtile_extras/resources/syncthing/syncthing.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/tvheadend-icons/icon.svg` & `qtile_extras-0.26.0/qtile_extras/resources/tvheadend-icons/icon.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/visualiser/cava_draw.py` & `qtile_extras-0.26.0/qtile_extras/resources/visualiser/cava_draw.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_tiles.png` & `qtile_extras-0.26.0/qtile_extras/resources/wallpapers/qte_tiles.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_triangles.png` & `qtile_extras-0.26.0/qtile_extras/resources/wallpapers/qte_triangles.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_triangles_rounded.png` & `qtile_extras-0.26.0/qtile_extras/resources/wallpapers/qte_triangles_rounded.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wordclock/dutch.py` & `qtile_extras-0.26.0/qtile_extras/resources/wordclock/dutch.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wordclock/english.py` & `qtile_extras-0.26.0/qtile_extras/resources/wordclock/english.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wordclock/finnish.py` & `qtile_extras-0.26.0/qtile_extras/resources/wordclock/finnish.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wordclock/french.py` & `qtile_extras-0.26.0/qtile_extras/resources/wordclock/french.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wordclock/portuguese.py` & `qtile_extras-0.26.0/qtile_extras/resources/wordclock/portuguese.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wordclock/spanish.py` & `qtile_extras-0.26.0/qtile_extras/resources/wordclock/spanish.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/resources/wordclock/swedish.py` & `qtile_extras-0.26.0/qtile_extras/resources/wordclock/swedish.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/__init__.py` & `qtile_extras-0.26.0/qtile_extras/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/alsavolumecontrol.py` & `qtile_extras-0.26.0/qtile_extras/widget/alsavolumecontrol.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/analogueclock.py` & `qtile_extras-0.26.0/qtile_extras/widget/analogueclock.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/animatedimage.py` & `qtile_extras-0.26.0/qtile_extras/widget/animatedimage.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/base.py` & `qtile_extras-0.26.0/qtile_extras/widget/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from typing import TYPE_CHECKING
 
 from libqtile import bar, confreader, images
 from libqtile.command.base import expose_command
 from libqtile.log_utils import logger
 from libqtile.widget import base
 
+from qtile_extras import hook
 from qtile_extras.popup.templates.volume import VOLUME_NOTIFICATION
 from qtile_extras.widget.mixins import ExtendedPopupMixin, ProgressBarMixin
 
 if TYPE_CHECKING:
     from typing import Any
 
 
@@ -81,14 +82,16 @@
         (
             "popup_show_args",
             {"relative_to": 2, "relative_to_bar": True, "y": 50},
             "Control position of popup",
         ),
     ]
 
+    _hooks = [h.name for h in hook.volume_hooks]
+
     def __init__(self, **config):
         base._Widget.__init__(self, bar.CALCULATED, **config)
         ExtendedPopupMixin.__init__(self, **config)
         ProgressBarMixin.__init__(self, **config)
         self.add_defaults(ExtendedPopupMixin.defaults)
         self.add_defaults(ProgressBarMixin.defaults)
         self.add_defaults(_Volume.defaults)
@@ -183,14 +186,20 @@
         return width
 
     def status_change(self, vol, muted):
         # Something's changed so let's update display
         # Unhide bar
         self.hidden = False
 
+        # Fire any hooks
+        if muted != self.muted:
+            hook.fire("volume_mute_change", int(vol), bool(muted))
+        elif vol != self.volume:
+            hook.fire("volume_change", int(vol), bool(muted))
+
         # Get new values
         self.volume = vol
         self.muted = muted
 
         # Restart timer
         self.set_refresh_timer()
```

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/bluetooth.py` & `qtile_extras-0.26.0/qtile_extras/widget/bluetooth.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/brightnesscontrol.py` & `qtile_extras-0.26.0/qtile_extras/widget/brightnesscontrol.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/continuous_poll.py` & `qtile_extras-0.26.0/qtile_extras/widget/continuous_poll.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/currentlayout.py` & `qtile_extras-0.26.0/qtile_extras/widget/currentlayout.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/decorations.py` & `qtile_extras-0.26.0/qtile_extras/widget/decorations.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/githubnotifications.py` & `qtile_extras-0.26.0/qtile_extras/widget/githubnotifications.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/globalmenu.py` & `qtile_extras-0.26.0/qtile_extras/widget/globalmenu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/graph.py` & `qtile_extras-0.26.0/qtile_extras/widget/graph.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/groupbox2.py` & `qtile_extras-0.26.0/qtile_extras/widget/groupbox2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/image.py` & `qtile_extras-0.26.0/qtile_extras/widget/image.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/iwd.py` & `qtile_extras-0.26.0/qtile_extras/widget/iwd.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/livefootballscores.py` & `qtile_extras-0.26.0/qtile_extras/widget/livefootballscores.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/mirror.py` & `qtile_extras-0.26.0/qtile_extras/widget/mirror.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/mixins/__init__.py` & `qtile_extras-0.26.0/qtile_extras/widget/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/mpris2widget.py` & `qtile_extras-0.26.0/qtile_extras/widget/mpris2widget.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/network.py` & `qtile_extras-0.26.0/qtile_extras/widget/network.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/pulse_extra.py` & `qtile_extras-0.26.0/qtile_extras/widget/pulse_extra.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/pulse_volume.py` & `qtile_extras-0.26.0/qtile_extras/widget/pulse_volume.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/scriptexit.py` & `qtile_extras-0.26.0/qtile_extras/widget/scriptexit.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/snapcast.py` & `qtile_extras-0.26.0/qtile_extras/widget/snapcast.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/statusnotifier.py` & `qtile_extras-0.26.0/qtile_extras/widget/statusnotifier.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/strava.py` & `qtile_extras-0.26.0/qtile_extras/widget/strava.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/syncthing.py` & `qtile_extras-0.26.0/qtile_extras/widget/syncthing.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/systray.py` & `qtile_extras-0.26.0/qtile_extras/widget/systray.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/tvheadend.py` & `qtile_extras-0.26.0/qtile_extras/widget/tvheadend.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/unitstatus.py` & `qtile_extras-0.26.0/qtile_extras/widget/unitstatus.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/upower.py` & `qtile_extras-0.26.0/qtile_extras/widget/upower.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/visualiser.py` & `qtile_extras-0.26.0/qtile_extras/widget/visualiser.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras/widget/wordclock.py` & `qtile_extras-0.26.0/qtile_extras/widget/wordclock.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/qtile_extras.egg-info/PKG-INFO` & `qtile_extras-0.26.0/qtile_extras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtile-extras
-Version: 0.25.0
+Version: 0.26.0
 Summary: Extra items for qtile that are unlikely to be maintained in the main repo.
 Author: elParaguayo
 License: MIT
 Project-URL: homepage, https://github.com/elParaguayo/qtile-extras
 Project-URL: documentation, https://qtile-extras.readthedocs.io/en/stable/
 Project-URL: changelog, https://qtile-extras.readthedocs.io/en/stable/changelog.html
 Project-URL: issues, https://github.com/elParaguayo/qtile-extras/issues
```

### Comparing `qtile-extras-0.25.0/qtile_extras.egg-info/SOURCES.txt` & `qtile_extras-0.26.0/qtile_extras.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 qtile_extras/hook.py
 qtile_extras/images.py
 qtile_extras/py.typed
 qtile_extras.egg-info/PKG-INFO
 qtile_extras.egg-info/SOURCES.txt
 qtile_extras.egg-info/dependency_links.txt
 qtile_extras.egg-info/top_level.txt
+qtile_extras/layout/__init__.py
+qtile_extras/layout/_mods.py
+qtile_extras/layout/plasma.py
+qtile_extras/layout/decorations/__init__.py
+qtile_extras/layout/decorations/borders.py
+qtile_extras/layout/decorations/injections.py
 qtile_extras/popup/__init__.py
 qtile_extras/popup/menu.py
 qtile_extras/popup/toolkit.py
 qtile_extras/popup/templates/__init__.py
 qtile_extras/popup/templates/mpris2.py
 qtile_extras/popup/templates/volume.py
 qtile_extras/resources/__init__.py
@@ -109,14 +115,17 @@
 test/test_bar.py
 test/test_images.py
 test/backend/__init__.py
 test/backend/wayland/__init__.py
 test/backend/wayland/conftest.py
 test/backend/x11/__init__.py
 test/backend/x11/conftest.py
+test/layout/__init__.py
+test/layout/decorations/__init__.py
+test/layout/decorations/test_border_decorations.py
 test/popup/__init__.py
 test/popup/test_menu.py
 test/popup/test_toolkit.py
 test/resources/icons/audio-volume-high.svg
 test/resources/icons/audio-volume-low.svg
 test/resources/icons/audio-volume-medium.svg
 test/resources/icons/audio-volume-muted.svg
```

### Comparing `qtile-extras-0.25.0/setup.cfg` & `qtile_extras-0.26.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/backend/wayland/conftest.py` & `qtile_extras-0.26.0/test/backend/wayland/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/backend/x11/conftest.py` & `qtile_extras-0.26.0/test/backend/x11/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/conftest.py` & `qtile_extras-0.26.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/helpers.py` & `qtile_extras-0.26.0/test/helpers.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/popup/test_menu.py` & `qtile_extras-0.26.0/test/popup/test_menu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/popup/test_toolkit.py` & `qtile_extras-0.26.0/test/popup/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding.png` & `qtile_extras-0.26.0/test/resources/test_images/border-default-grouped-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding_x.png` & `qtile_extras-0.26.0/test/resources/test_images/border-default-grouped-padding_x.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding_y.png` & `qtile_extras-0.26.0/test/resources/test_images/border-default-grouped-padding_y.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-default-grouped.png` & `qtile_extras-0.26.0/test/resources/test_images/border-default-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-default-padding.png` & `qtile_extras-0.26.0/test/resources/test_images/border-default-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-default.png` & `qtile_extras-0.26.0/test/resources/test_images/border-default.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-single-E-grouped.png` & `qtile_extras-0.26.0/test/resources/test_images/border-single-E-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-single-E.png` & `qtile_extras-0.26.0/test/resources/test_images/border-single-E.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-single-N-grouped.png` & `qtile_extras-0.26.0/test/resources/test_images/border-single-N-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-single-N.png` & `qtile_extras-0.26.0/test/resources/test_images/border-single-N.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-single-S-grouped.png` & `qtile_extras-0.26.0/test/resources/test_images/border-single-S-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-single-S.png` & `qtile_extras-0.26.0/test/resources/test_images/border-single-S.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-single-W-grouped.png` & `qtile_extras-0.26.0/test/resources/test_images/border-single-W-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-single-W.png` & `qtile_extras-0.26.0/test/resources/test_images/border-single-W.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-stacked-grouped.png` & `qtile_extras-0.26.0/test/resources/test_images/border-stacked-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-stacked-same-position.png` & `qtile_extras-0.26.0/test/resources/test_images/border-stacked-same-position.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/border-stacked.png` & `qtile_extras-0.26.0/test/resources/test_images/border-stacked.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/combo-rect-plus-powerline.png` & `qtile_extras-0.26.0/test/resources/test_images/combo-rect-plus-powerline.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_left-padding.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-arrow_left-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_left.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-arrow_left.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_right-padding.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-arrow_right-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_right.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-arrow_right.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-back_slash-padding.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-back_slash-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-back_slash.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-back_slash.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-custom-path.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-custom-path.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-forward_slash-padding.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-forward_slash-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-forward_slash.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-forward_slash.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_left-padding.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-rounded_left-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_left.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-rounded_left.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_right-padding.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-rounded_right-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_right.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-rounded_right.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-zig_zag-padding.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-zig_zag-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/powerline-zig_zag.png` & `qtile_extras-0.26.0/test/resources/test_images/powerline-zig_zag.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/rect-default-filled.png` & `qtile_extras-0.26.0/test/resources/test_images/rect-default-filled.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled-no-radius.png` & `qtile_extras-0.26.0/test/resources/test_images/rect-default-group-filled-no-radius.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled-widget-background.png` & `qtile_extras-0.26.0/test/resources/test_images/rect-default-group-filled-widget-background.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled.png` & `qtile_extras-0.26.0/test/resources/test_images/rect-default-group-filled.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/rect-default-line.png` & `qtile_extras-0.26.0/test/resources/test_images/rect-default-line.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/rect-default.png` & `qtile_extras-0.26.0/test/resources/test_images/rect-default.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/resources/test_images/rect-stacked.png` & `qtile_extras-0.26.0/test/resources/test_images/rect-stacked.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/scripts/window.py` & `qtile_extras-0.26.0/test/scripts/window.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/test_bar.py` & `qtile_extras-0.26.0/test/test_bar.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/test_images.py` & `qtile_extras-0.26.0/test/test_images.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/conftest.py` & `qtile_extras-0.26.0/test/widget/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/decorations/conftest.py` & `qtile_extras-0.26.0/test/widget/decorations/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/decorations/test_decoration_output.py` & `qtile_extras-0.26.0/test/widget/decorations/test_decoration_output.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/decorations/test_widget_decorations.py` & `qtile_extras-0.26.0/test/widget/decorations/test_widget_decorations.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/docs_screenshots/conftest.py` & `qtile_extras-0.26.0/test/widget/docs_screenshots/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/docs_screenshots/ss_groupbox2.py` & `qtile_extras-0.26.0/test/widget/docs_screenshots/ss_groupbox2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/docs_screenshots/ss_iwd.py` & `qtile_extras-0.26.0/test/widget/docs_screenshots/ss_iwd.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/resources/lfs_data.py` & `qtile_extras-0.26.0/test/widget/resources/lfs_data.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_alsawidget.py` & `qtile_extras-0.26.0/test/widget/test_alsawidget.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_analogueclock.py` & `qtile_extras-0.26.0/test/widget/test_analogueclock.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_animated_image.py` & `qtile_extras-0.26.0/test/widget/test_animated_image.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_brightness_control.py` & `qtile_extras-0.26.0/test/widget/test_brightness_control.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_continuous_poll.py` & `qtile_extras-0.26.0/test/widget/test_continuous_poll.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_currentlayouticon.py` & `qtile_extras-0.26.0/test/widget/test_currentlayouticon.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_githubnotifications.py` & `qtile_extras-0.26.0/test/widget/test_githubnotifications.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_global_menu.py` & `qtile_extras-0.26.0/test/widget/test_global_menu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_groupbox2.py` & `qtile_extras-0.26.0/test/widget/test_groupbox2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_image.py` & `qtile_extras-0.26.0/test/widget/test_image.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_init_configure.py` & `qtile_extras-0.26.0/test/widget/test_init_configure.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_injection_wrapper.py` & `qtile_extras-0.26.0/test/widget/test_injection_wrapper.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_iwd.py` & `qtile_extras-0.26.0/test/widget/test_iwd.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,44 +287,48 @@
 @config(interface="wlan0")
 def test_named_interface(iwd_manager):
     widget = iwd_manager.c.widget["iwd"]
     wait_for_text(widget, "qtile_extras (50%)")
 
 
 @config(interface="wlan1")
-@pytest.mark.flaky(reruns=5)
+# @pytest.mark.flaky(reruns=5)
+@pytest.mark.xfail
 def test_invalid_interface(iwd_manager, logger):
     widget = iwd_manager.c.widget["iwd"]
     wait_for_text(widget, "Error")
     assert "The interface 'wlan1' was not found." in logger.text
 
 
 @config(format="{ssid} {rssi} {quality}")
 def test_string_format(iwd_manager):
     widget = iwd_manager.c.widget["iwd"]
     wait_for_text(widget, "qtile_extras -75 50")
 
 
 @config(password_entry_app=None)
-@pytest.mark.flaky(reruns=5)
+# @pytest.mark.flaky(reruns=5)
+@pytest.mark.xfail
 def test_no_password_entry_app(iwd_manager, logger):
     widget = iwd_manager.c.widget["iwd"]
     wait_for_text(widget, "qtile_extras (50%)")
     assert "No password entry app provided. Agent will not be started." in logger.text
 
 
 @config(password_entry_app="qtileextraapp")
-@pytest.mark.flaky(reruns=5)
+# @pytest.mark.flaky(reruns=5)
+@pytest.mark.xfail
 def test_invalid_password_entry_app(iwd_manager, logger):
     widget = iwd_manager.c.widget["iwd"]
     wait_for_text(widget, "qtile_extras (50%)")
     assert "Cannot find password entry app. Agent will not be started." in logger.text
 
 
 @config(password_entry_args="This should be a list")
+@pytest.mark.xfail
 def test_bad_password_entry_args(iwd_manager, logger):
     widget = iwd_manager.c.widget["iwd"]
     wait_for_text(widget, "qtile_extras (50%)")
     assert "password_entry_args must be a list. Agent will not be started." in logger.text
 
 
 def test_menu(iwd_manager):
```

### Comparing `qtile-extras-0.25.0/test/widget/test_livefootballscores.py` & `qtile_extras-0.26.0/test/widget/test_livefootballscores.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_mpris2.py` & `qtile_extras-0.26.0/test/widget/test_mpris2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_network.py` & `qtile_extras-0.26.0/test/widget/test_network.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_popup_mixin.py` & `qtile_extras-0.26.0/test/widget/test_popup_mixin.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_scriptexit.py` & `qtile_extras-0.26.0/test/widget/test_scriptexit.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_snapcast.py` & `qtile_extras-0.26.0/test/widget/test_snapcast.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_statusnotifier.py` & `qtile_extras-0.26.0/test/widget/test_statusnotifier.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_strava.py` & `qtile_extras-0.26.0/test/widget/test_strava.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_syncthing.py` & `qtile_extras-0.26.0/test/widget/test_syncthing.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_tooltip.py` & `qtile_extras-0.26.0/test/widget/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_tvhwidget.py` & `qtile_extras-0.26.0/test/widget/test_tvhwidget.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_unitstatus.py` & `qtile_extras-0.26.0/test/widget/test_unitstatus.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_upower.py` & `qtile_extras-0.26.0/test/widget/test_upower.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_visualiser.py` & `qtile_extras-0.26.0/test/widget/test_visualiser.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_widget_init.py` & `qtile_extras-0.26.0/test/widget/test_widget_init.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.25.0/test/widget/test_wordclock.py` & `qtile_extras-0.26.0/test/widget/test_wordclock.py`

 * *Files identical despite different names*

