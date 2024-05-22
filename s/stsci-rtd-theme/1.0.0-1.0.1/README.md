# Comparing `tmp/stsci_rtd_theme-1.0.0.tar.gz` & `tmp/stsci_rtd_theme-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stsci_rtd_theme-1.0.0.tar", last modified: Thu Jun 30 21:14:41 2022, max compression
+gzip compressed data, was "stsci_rtd_theme-1.0.1.tar", last modified: Wed May 22 14:31:58 2024, max compression
```

## Comparing `stsci_rtd_theme-1.0.0.tar` & `stsci_rtd_theme-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1028 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      635 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme.egg-info/
--rw-r--r--   0 root         (0) root         (0)       16 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      635 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      494 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-30 21:14:35.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1504 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme/
--rw-r--r--   0 root         (0) root         (0)     1372 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme/layout.html
--rw-r--r--   0 root         (0) root         (0)      213 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme/theme.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme/static/
--rw-r--r--   0 root         (0) root         (0)    65413 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme/static/stsci_pri_combo_mark_white.png
--rw-r--r--   0 root         (0) root         (0)   122448 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme/static/stsci.css
--rw-r--r--   0 root         (0) root         (0)      259 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/stsci_rtd_theme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1430 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/LICENSE.rst
--rw-r--r--   0 root         (0) root         (0)     1873 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-30 21:14:41.000000 stsci_rtd_theme-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      178 2022-06-30 21:14:32.000000 stsci_rtd_theme-1.0.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:31:58.686464 stsci_rtd_theme-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:31:58.678464 stsci_rtd_theme-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:31:58.682464 stsci_rtd_theme-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-22 14:31:58.686464 stsci_rtd_theme-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:31:58.686464 stsci_rtd_theme-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:31:58.682464 stsci_rtd_theme-1.0.1/stsci_rtd_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:31:58.682464 stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:31:58.686464 stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    73332 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    75152 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/fonts/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   126676 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/fonts/RobotoSlab-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   125936 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/fonts/RobotoSlab-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   123323 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/stsci.css
+-rw-r--r--   0 runner    (1001) docker     (127)    65413 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/stsci_pri_combo_mark_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:31:58.686464 stsci_rtd_theme-1.0.1/stsci_rtd_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-22 14:31:58.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 14:31:58.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:31:58.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 14:31:58.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 14:31:58.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 14:31:58.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   209030 2024-05-22 14:31:48.000000 stsci_rtd_theme-1.0.1/stsci_rtd_theme_example.png
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stsci_rtd_theme-1.0.0/LICENSE` & `stsci_rtd_theme-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stsci_rtd_theme-1.0.0/stsci_rtd_theme/layout.html` & `stsci_rtd_theme-1.0.1/stsci_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `stsci_rtd_theme-1.0.0/stsci_rtd_theme/static/stsci_pri_combo_mark_white.png` & `stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/stsci_pri_combo_mark_white.png`

 * *Files identical despite different names*

### Comparing `stsci_rtd_theme-1.0.0/stsci_rtd_theme/static/stsci.css` & `stsci_rtd_theme-1.0.1/stsci_rtd_theme/static/stsci.css`

 * *Files 3% similar despite different names*

```diff
@@ -374,14 +374,15 @@
 .rst-content .admonition-title:before,
 .rst-content h1 .headerlink:before,
 .rst-content h2 .headerlink:before,
 .rst-content h3 .headerlink:before,
 .rst-content h4 .headerlink:before,
 .rst-content h5 .headerlink:before,
 .rst-content h6 .headerlink:before,
+.rst-content p .headerlink:before,
 .rst-content dl dt .headerlink:before,
 .rst-content p.caption .headerlink:before,
 .rst-content tt.download span:first-child:before,
 .rst-content code.download span:first-child:before,
 .icon:before,
 .wy-dropdown .caret:before,
 .wy-inline-validate.wy-inline-validate-success .wy-input-context:before,
@@ -461,15 +462,15 @@
 .rst-content h1 .headerlink,
 .rst-content h2 .headerlink,
 .rst-content h3 .headerlink,
 .rst-content h4 .headerlink,
 .rst-content h5 .headerlink,
 .rst-content h6 .headerlink,
 .rst-content dl dt .headerlink,
-.rst-content p.caption .headerlink,
+.rst-content p .headerlink,
 .rst-content tt.download span:first-child,
 .rst-content code.download span:first-child,
 .icon {
     display: inline-block;
     font: normal normal normal 14px/1 FontAwesome;
     font-size: inherit;
     text-rendering: auto;
@@ -548,15 +549,15 @@
 .rst-content h1 .pull-left.headerlink,
 .rst-content h2 .pull-left.headerlink,
 .rst-content h3 .pull-left.headerlink,
 .rst-content h4 .pull-left.headerlink,
 .rst-content h5 .pull-left.headerlink,
 .rst-content h6 .pull-left.headerlink,
 .rst-content dl dt .pull-left.headerlink,
-.rst-content p.caption .pull-left.headerlink,
+.rst-content p .pull-left.headerlink,
 .rst-content tt.download span.pull-left:first-child,
 .rst-content code.download span.pull-left:first-child,
 .pull-left.icon {
     margin-right: .3em
 }
 
 .fa.pull-right,
@@ -567,15 +568,15 @@
 .rst-content h1 .pull-right.headerlink,
 .rst-content h2 .pull-right.headerlink,
 .rst-content h3 .pull-right.headerlink,
 .rst-content h4 .pull-right.headerlink,
 .rst-content h5 .pull-right.headerlink,
 .rst-content h6 .pull-right.headerlink,
 .rst-content dl dt .pull-right.headerlink,
-.rst-content p.caption .pull-right.headerlink,
+.rst-content p .pull-right.headerlink,
 .rst-content tt.download span.pull-right:first-child,
 .rst-content code.download span.pull-right:first-child,
 .pull-right.icon {
     margin-left: .3em
 }
 
 .fa-spin {
@@ -2693,15 +2694,15 @@
 .rst-content h1 .headerlink,
 .rst-content h2 .headerlink,
 .rst-content h3 .headerlink,
 .rst-content h4 .headerlink,
 .rst-content h5 .headerlink,
 .rst-content h6 .headerlink,
 .rst-content dl dt .headerlink,
-.rst-content p.caption .headerlink,
+.rst-content p .headerlink,
 .rst-content tt.download span:first-child,
 .rst-content code.download span:first-child,
 .icon,
 .wy-dropdown .caret,
 .wy-inline-validate.wy-inline-validate-success .wy-input-context,
 .wy-inline-validate.wy-inline-validate-danger .wy-input-context,
 .wy-inline-validate.wy-inline-validate-warning .wy-input-context,
@@ -2717,15 +2718,15 @@
 .rst-content h1 .headerlink:before,
 .rst-content h2 .headerlink:before,
 .rst-content h3 .headerlink:before,
 .rst-content h4 .headerlink:before,
 .rst-content h5 .headerlink:before,
 .rst-content h6 .headerlink:before,
 .rst-content dl dt .headerlink:before,
-.rst-content p.caption .headerlink:before,
+.rst-content p .headerlink:before,
 .rst-content tt.download span:first-child:before,
 .rst-content code.download span:first-child:before,
 .icon:before,
 .wy-dropdown .caret:before,
 .wy-inline-validate.wy-inline-validate-success .wy-input-context:before,
 .wy-inline-validate.wy-inline-validate-danger .wy-input-context:before,
 .wy-inline-validate.wy-inline-validate-warning .wy-input-context:before,
@@ -2755,16 +2756,16 @@
 .rst-content h4 a .headerlink,
 a .rst-content h5 .headerlink,
 .rst-content h5 a .headerlink,
 a .rst-content h6 .headerlink,
 .rst-content h6 a .headerlink,
 a .rst-content dl dt .headerlink,
 .rst-content dl dt a .headerlink,
-a .rst-content p.caption .headerlink,
-.rst-content p.caption a .headerlink,
+a .rst-content p .headerlink,
+.rst-content p a .headerlink,
 a .rst-content tt.download span:first-child,
 .rst-content tt.download a span:first-child,
 a .rst-content code.download span:first-child,
 .rst-content code.download a span:first-child,
 a .icon {
     display: inline-block;
     text-decoration: inherit
@@ -2789,16 +2790,16 @@
 .rst-content h4 .btn .headerlink,
 .btn .rst-content h5 .headerlink,
 .rst-content h5 .btn .headerlink,
 .btn .rst-content h6 .headerlink,
 .rst-content h6 .btn .headerlink,
 .btn .rst-content dl dt .headerlink,
 .rst-content dl dt .btn .headerlink,
-.btn .rst-content p.caption .headerlink,
-.rst-content p.caption .btn .headerlink,
+.btn .rst-content p .headerlink,
+.rst-content p .btn .headerlink,
 .btn .rst-content tt.download span:first-child,
 .rst-content tt.download .btn span:first-child,
 .btn .rst-content code.download span:first-child,
 .rst-content code.download .btn span:first-child,
 .btn .icon,
 .nav .fa,
 .nav .wy-menu-vertical li span.toctree-expand,
@@ -2819,16 +2820,16 @@
 .rst-content h4 .nav .headerlink,
 .nav .rst-content h5 .headerlink,
 .rst-content h5 .nav .headerlink,
 .nav .rst-content h6 .headerlink,
 .rst-content h6 .nav .headerlink,
 .nav .rst-content dl dt .headerlink,
 .rst-content dl dt .nav .headerlink,
-.nav .rst-content p.caption .headerlink,
-.rst-content p.caption .nav .headerlink,
+.nav .rst-content p .headerlink,
+.rst-content p .nav .headerlink,
 .nav .rst-content tt.download span:first-child,
 .rst-content tt.download .nav span:first-child,
 .nav .rst-content code.download span:first-child,
 .rst-content code.download .nav span:first-child,
 .nav .icon {
     display: inline
 }
@@ -2848,16 +2849,16 @@
 .rst-content h4 .btn .fa-large.headerlink,
 .btn .rst-content h5 .fa-large.headerlink,
 .rst-content h5 .btn .fa-large.headerlink,
 .btn .rst-content h6 .fa-large.headerlink,
 .rst-content h6 .btn .fa-large.headerlink,
 .btn .rst-content dl dt .fa-large.headerlink,
 .rst-content dl dt .btn .fa-large.headerlink,
-.btn .rst-content p.caption .fa-large.headerlink,
-.rst-content p.caption .btn .fa-large.headerlink,
+.btn .rst-content p .fa-large.headerlink,
+.rst-content p .btn .fa-large.headerlink,
 .btn .rst-content tt.download span.fa-large:first-child,
 .rst-content tt.download .btn span.fa-large:first-child,
 .btn .rst-content code.download span.fa-large:first-child,
 .rst-content code.download .btn span.fa-large:first-child,
 .btn .fa-large.icon,
 .nav .fa.fa-large,
 .nav .wy-menu-vertical li span.fa-large.toctree-expand,
@@ -2874,16 +2875,16 @@
 .rst-content h4 .nav .fa-large.headerlink,
 .nav .rst-content h5 .fa-large.headerlink,
 .rst-content h5 .nav .fa-large.headerlink,
 .nav .rst-content h6 .fa-large.headerlink,
 .rst-content h6 .nav .fa-large.headerlink,
 .nav .rst-content dl dt .fa-large.headerlink,
 .rst-content dl dt .nav .fa-large.headerlink,
-.nav .rst-content p.caption .fa-large.headerlink,
-.rst-content p.caption .nav .fa-large.headerlink,
+.nav .rst-content p .fa-large.headerlink,
+.rst-content p .nav .fa-large.headerlink,
 .nav .rst-content tt.download span.fa-large:first-child,
 .rst-content tt.download .nav span.fa-large:first-child,
 .nav .rst-content code.download span.fa-large:first-child,
 .rst-content code.download .nav span.fa-large:first-child,
 .nav .fa-large.icon {
     line-height: 0.9em
 }
@@ -2903,16 +2904,16 @@
 .rst-content h4 .btn .fa-spin.headerlink,
 .btn .rst-content h5 .fa-spin.headerlink,
 .rst-content h5 .btn .fa-spin.headerlink,
 .btn .rst-content h6 .fa-spin.headerlink,
 .rst-content h6 .btn .fa-spin.headerlink,
 .btn .rst-content dl dt .fa-spin.headerlink,
 .rst-content dl dt .btn .fa-spin.headerlink,
-.btn .rst-content p.caption .fa-spin.headerlink,
-.rst-content p.caption .btn .fa-spin.headerlink,
+.btn .rst-content p .fa-spin.headerlink,
+.rst-content p .btn .fa-spin.headerlink,
 .btn .rst-content tt.download span.fa-spin:first-child,
 .rst-content tt.download .btn span.fa-spin:first-child,
 .btn .rst-content code.download span.fa-spin:first-child,
 .rst-content code.download .btn span.fa-spin:first-child,
 .btn .fa-spin.icon,
 .nav .fa.fa-spin,
 .nav .wy-menu-vertical li span.fa-spin.toctree-expand,
@@ -2929,16 +2930,16 @@
 .rst-content h4 .nav .fa-spin.headerlink,
 .nav .rst-content h5 .fa-spin.headerlink,
 .rst-content h5 .nav .fa-spin.headerlink,
 .nav .rst-content h6 .fa-spin.headerlink,
 .rst-content h6 .nav .fa-spin.headerlink,
 .nav .rst-content dl dt .fa-spin.headerlink,
 .rst-content dl dt .nav .fa-spin.headerlink,
-.nav .rst-content p.caption .fa-spin.headerlink,
-.rst-content p.caption .nav .fa-spin.headerlink,
+.nav .rst-content p .fa-spin.headerlink,
+.rst-content p .nav .fa-spin.headerlink,
 .nav .rst-content tt.download span.fa-spin:first-child,
 .rst-content tt.download .nav span.fa-spin:first-child,
 .nav .rst-content code.download span.fa-spin:first-child,
 .rst-content code.download .nav span.fa-spin:first-child,
 .nav .fa-spin.icon {
     display: inline-block
 }
@@ -2949,15 +2950,15 @@
 .rst-content h1 .btn.headerlink:before,
 .rst-content h2 .btn.headerlink:before,
 .rst-content h3 .btn.headerlink:before,
 .rst-content h4 .btn.headerlink:before,
 .rst-content h5 .btn.headerlink:before,
 .rst-content h6 .btn.headerlink:before,
 .rst-content dl dt .btn.headerlink:before,
-.rst-content p.caption .btn.headerlink:before,
+.rst-content p .btn.headerlink:before,
 .rst-content tt.download span.btn:first-child:before,
 .rst-content code.download span.btn:first-child:before,
 .btn.icon:before {
     opacity: 0.5;
     -webkit-transition: opacity 0.05s ease-in;
     -moz-transition: opacity 0.05s ease-in;
     transition: opacity 0.05s ease-in
@@ -2969,15 +2970,15 @@
 .rst-content h1 .btn.headerlink:hover:before,
 .rst-content h2 .btn.headerlink:hover:before,
 .rst-content h3 .btn.headerlink:hover:before,
 .rst-content h4 .btn.headerlink:hover:before,
 .rst-content h5 .btn.headerlink:hover:before,
 .rst-content h6 .btn.headerlink:hover:before,
 .rst-content dl dt .btn.headerlink:hover:before,
-.rst-content p.caption .btn.headerlink:hover:before,
+.rst-content p .btn.headerlink:hover:before,
 .rst-content tt.download span.btn:first-child:hover:before,
 .rst-content code.download span.btn:first-child:hover:before,
 .btn.icon:hover:before {
     opacity: 1
 }
 
 .btn-mini .fa:before,
@@ -2995,16 +2996,16 @@
 .rst-content h4 .btn-mini .headerlink:before,
 .btn-mini .rst-content h5 .headerlink:before,
 .rst-content h5 .btn-mini .headerlink:before,
 .btn-mini .rst-content h6 .headerlink:before,
 .rst-content h6 .btn-mini .headerlink:before,
 .btn-mini .rst-content dl dt .headerlink:before,
 .rst-content dl dt .btn-mini .headerlink:before,
-.btn-mini .rst-content p.caption .headerlink:before,
-.rst-content p.caption .btn-mini .headerlink:before,
+.btn-mini .rst-content p .headerlink:before,
+.rst-content p .btn-mini .headerlink:before,
 .btn-mini .rst-content tt.download span:first-child:before,
 .rst-content tt.download .btn-mini span:first-child:before,
 .btn-mini .rst-content code.download span:first-child:before,
 .rst-content code.download .btn-mini span:first-child:before,
 .btn-mini .icon:before {
     font-size: 14px;
     vertical-align: -15%
@@ -4743,101 +4744,129 @@
 
 code.code-large,
 .rst-content tt.code-large {
     font-size: 90%
 }
 
 .wy-plain-list-disc,
+/* L6-7 in og sphinx */
+.rst-content .section .toctree-wrapper ul,
 .rst-content .section ul,
-.rst-content .toctree-wrapper ul,
+.rst-content section .toctree-wrapper ul,
+.rst-content section ul,
 article ul {
     list-style: disc;
     line-height: 24px;
     margin-bottom: 24px;
     font-size: 16px
 }
 
 .wy-plain-list-disc li,
+/* L15 in og sphinx */
+.rst-content .section .toctree-wrapper ul li,
 .rst-content .section ul li,
-.rst-content .toctree-wrapper ul li,
+.rst-content section .toctree-wrapper ul li,
+.rst-content section ul li,
 article ul li {
     list-style: disc;
     margin-left: 24px
 }
 
 .wy-plain-list-disc li p:last-child,
+/* L23-24 in og sphinx; didn't add every change */
+.rst-content .section .toctree-wrapper ul li ul,
 .rst-content .section ul li p:last-child,
-.rst-content .toctree-wrapper ul li p:last-child,
+.rst-content section .toctree-wrapper ul li p:last-child,
 article ul li p:last-child {
     margin-bottom: 0
 }
 
 .wy-plain-list-disc li ul,
 .rst-content .section ul li ul,
 .rst-content .toctree-wrapper ul li ul,
 article ul li ul {
     margin-bottom: 0
 }
 
 .wy-plain-list-disc li li,
+/* L32 in og sphinx */
+.rst-content .section .toctree-wrapper ul li li,
 .rst-content .section ul li li,
-.rst-content .toctree-wrapper ul li li,
+.rst-content section .toctree-wrapper ul li li,
+.rst-content section ul li li,
 article ul li li {
     list-style: circle
 }
 
 .wy-plain-list-disc li li li,
+/* L38 in og sphinx */
+.rst-content .section .toctree-wrapper ul li li li,
 .rst-content .section ul li li li,
-.rst-content .toctree-wrapper ul li li li,
+.rst-content section .toctree-wrapper ul li li li,
+.rst-content section ul li li li,
 article ul li li li {
     list-style: square
 }
 
 .wy-plain-list-disc li ol li,
+/* L44 in og sphinx */
+.rst-content .section .toctree-wrapper ul li ol li,
 .rst-content .section ul li ol li,
-.rst-content .toctree-wrapper ul li ol li,
+.rst-content section .toctree-wrapper ul li ol li,
+.rst-content section ul li ol li,
 article ul li ol li {
     list-style: decimal
 }
 
 .wy-plain-list-decimal,
+/* L50 in og sphinx */
 .rst-content .section ol,
-.rst-content ol.arabic,
+.rst-content .section ol.arabic,
+.rst-content section ol,
+.rst-content section ol.arabic,
 article ol {
     list-style: decimal;
     line-height: 24px;
     margin-bottom: 24px;
     font-size: 16px
 }
 
 .wy-plain-list-decimal li,
+/* L58 in og sphinx */
+.rst-content .section ol.arabic li,
 .rst-content .section ol li,
-.rst-content ol.arabic li,
+.rst-content section ol.arabic li,
+.rst-content section ol li,
 article ol li {
     list-style: decimal;
     margin-left: 24px
 }
 
 .wy-plain-list-decimal li p:last-child,
+/* L66-67 in og sphinx; didn't add every change */
+.rst-content .section ol.arabic li ul,
 .rst-content .section ol li p:last-child,
-.rst-content ol.arabic li p:last-child,
+.rst-content section ol li p:last-child,
 article ol li p:last-child {
     margin-bottom: 0
 }
 
 .wy-plain-list-decimal li ul,
 .rst-content .section ol li ul,
 .rst-content ol.arabic li ul,
 article ol li ul {
     margin-bottom: 0
 }
 
 .wy-plain-list-decimal li ul li,
+/* L75 in og sphinx */
+.rst-content .section ol.arabic li ul li,
 .rst-content .section ol li ul li,
-.rst-content ol.arabic li ul li,
+.rst-content section ol.arabic li ul li,
+.rst-content section ol li ul li,
 article ol li ul li {
     list-style: disc
 }
 
 .codeblock-example {
     border: 1px solid #e1e4e5;
     border-bottom: none;
@@ -5883,16 +5912,16 @@
 .rst-content h4 .rst-versions .rst-current-version .headerlink,
 .rst-versions .rst-current-version .rst-content h5 .headerlink,
 .rst-content h5 .rst-versions .rst-current-version .headerlink,
 .rst-versions .rst-current-version .rst-content h6 .headerlink,
 .rst-content h6 .rst-versions .rst-current-version .headerlink,
 .rst-versions .rst-current-version .rst-content dl dt .headerlink,
 .rst-content dl dt .rst-versions .rst-current-version .headerlink,
-.rst-versions .rst-current-version .rst-content p.caption .headerlink,
-.rst-content p.caption .rst-versions .rst-current-version .headerlink,
+.rst-versions .rst-current-version .rst-content p .headerlink,
+.rst-content p .rst-versions .rst-current-version .headerlink,
 .rst-versions .rst-current-version .rst-content tt.download span:first-child,
 .rst-content tt.download .rst-versions .rst-current-version span:first-child,
 .rst-versions .rst-current-version .rst-content code.download span:first-child,
 .rst-content code.download .rst-versions .rst-current-version span:first-child,
 .rst-versions .rst-current-version .icon {
     color: #fcfcfc
 }
```

### Comparing `stsci_rtd_theme-1.0.0/LICENSE.rst` & `stsci_rtd_theme-1.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `stsci_rtd_theme-1.0.0/README.md` & `stsci_rtd_theme-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,94 @@
-# stsci_rtd_theme
-STScI branded sphinx theme that inherits from sphinx_rtd_theme
+# `stsci-rtd-theme`
 
-This theme is based off of the sphinx_rtd_theme, from which it inherits, but the CSS styling
-has been altered for easier reading on a variety of platforms and browsers.
+This is a Sphinx theme for packages maintained by the Space Telescope Sciences Institute (STScI).
+
+![Example](stsci_rtd_theme_example.png)
+
+This theme inherits from `sphinx-rtd-theme`; however, the CSS styling has been altered for easier reading on a variety
+of platforms and browsers.
 
 ## Installation
-You can apply this theme to your current documents by installing this repository like any other python package:
 
-Either from GIT:
-```
-git clone https://github.com/spacetelescope/stsci_rtd_theme.git
-python setup.py install
+You can apply this theme to your current documents by installing the latest release from PyPI:
+
+```shell
+pip install stsci-rtd-theme
 ```
-Or with PIP:
+
+If you need the most up-to-date version of the `master` branch, you can install directly from GitHub:
+
+```shell
+pip install https://github.com/spacetelescope/stsci_rtd_theme.git
 ```
-# install directly from the git repository
-pip install -e https://github.com/spacetelescope/stsci_rtd_theme.git
 
-# install from pypi release
-pip install stsci_rtd_theme
+If you wish to modify the source code, you should clone the repository locally and install editable (`-e`):
+
+```shell
+git clone https://github.com/spacetelescope/stsci_rtd_theme.git
+cd stsci_rtd_theme
+pip install -e .
 ```
-## Adding to your Sphinx docs
+
+### Sphinx configuration
+
 If you haven't already created your Sphinx documentation, you can start sphinx with
-`sphinx-quickstart` and follow the guided steps. When you are finished,
-add these lines to your `conf.py` file:
-```
+`sphinx-quickstart` and follow the guided steps. When you are finished, add these lines to your `docs/conf.py` file:
+
+```python
+# docs/conf.py
+
 import stsci_rtd_theme
+
 html_theme = 'stsci_rtd_theme'
 html_theme_path = [stsci_rtd_theme.get_html_theme_path()]
 ```
-![Example theme render](stsci_rtd_theme_example.png)
 
-## Making this theme work on Readthedocs
-Add the following lines to your documentations conf.py file:
-```
+### ReadTheDocs configuration
+
+Add the following lines to your `docs/conf.py` file:
+
+```python
+# docs/conf.py
+
 import sphinx
-import stsci_rtd_theme
+import os
+from packaging.version import Version
+
 
 def setup(app):
     app.add_css_file("stsci.css")
 
-# the below is not strictly necessary but helps with extensions you may use across versions
-from packaging.version import Version
+
+extensions = [
+    ...
+]
 
 on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
 if on_rtd:
     extensions.append('sphinx.ext.mathjax')
 elif Version(sphinx.__version__) < Version('1.4'):
     extensions.append('sphinx.ext.pngmath')
 else:
     extensions.append('sphinx.ext.imgmath')
 ```
-Finally, when setting up your documentation build on readthedocs, make sure to include a requirements file which installs this theme. The `sphinx_rtd_theme` that it inherits from should already be there.
+
+Finally, make sure to include `stsci-rtd-theme` to the `docs` extra, or alternatively add `stsci-rtd-theme` to
+a `rtd-requirements.txt` file. Then, in `.readthedocs.yaml`, include the following (depending on which of the two methods
+are used to define the `stsci-rtd-theme` dependency):
+
+```yaml
+# .readthedocs.yaml
+install:
+  - method: pip
+    path: .
+    extra_requirements:
+      - docs
+```
+
+```yaml
+# .readthedocs.yaml
+install:
+  - requirements: .rtd-requirements.txt
+  - method: pip
+    path: .
+```
```

