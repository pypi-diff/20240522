# Comparing `tmp/ipywebview-5.2.tar.gz` & `tmp/ipywebview-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PycharmProjects\ipywebview\dist\.tmp-fvcyljeh\ipywebview-5.2.tar", last modified: Thu May 16 18:48:06 2024, max compression
+gzip compressed data, was "D:\PycharmProjects\ipywebview\dist\.tmp-cblqokrl\ipywebview-5.2.1.tar", last modified: Wed May 22 10:51:30 2024, max compression
```

## Comparing `ipywebview-5.2.tar` & `ipywebview-5.2.1.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/
--rw-rw-rw-   0        0        0      148 2024-05-16 17:34:29.000000 ipywebview-5.2/.editorconfig
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/.github/
--rw-rw-rw-   0        0        0      556 2024-05-16 17:34:29.000000 ipywebview-5.2/.github/funding.yml
--rw-rw-rw-   0        0        0      344 2024-05-16 17:34:29.000000 ipywebview-5.2/.github/issue_template.md
--rw-rw-rw-   0        0        0      695 2024-05-16 17:34:29.000000 ipywebview-5.2/.github/stale.yml
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/.github/workflows/
--rw-rw-rw-   0        0        0      560 2024-05-16 17:34:29.000000 ipywebview-5.2/.github/workflows/docs.yaml
--rw-rw-rw-   0        0        0     1233 2024-05-16 17:34:29.000000 ipywebview-5.2/.github/workflows/stale.yml
--rw-rw-rw-   0        0        0      293 2024-05-16 17:34:29.000000 ipywebview-5.2/.gitignore
--rw-rw-rw-   0        0        0      401 2024-05-16 17:34:29.000000 ipywebview-5.2/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1547 2024-05-16 17:34:29.000000 ipywebview-5.2/LICENSE
--rw-rw-rw-   0        0        0      201 2024-05-16 17:34:29.000000 ipywebview-5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3193 2024-05-16 18:48:06.000000 ipywebview-5.2/PKG-INFO
--rw-rw-rw-   0        0        0     5276 2024-05-16 17:34:29.000000 ipywebview-5.2/README.md
--rw-rw-rw-   0        0        0      483 2024-05-16 17:34:29.000000 ipywebview-5.2/SECURITY.md
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/ipywebview.egg-info/
--rw-rw-rw-   0        0        0     3193 2024-05-16 18:48:05.000000 ipywebview-5.2/ipywebview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2024-05-16 18:48:06.000000 ipywebview-5.2/ipywebview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:48:05.000000 ipywebview-5.2/ipywebview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      424 2024-05-16 18:48:05.000000 ipywebview-5.2/ipywebview.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 18:48:05.000000 ipywebview-5.2/ipywebview.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2536 2024-05-16 18:41:31.000000 ipywebview-5.2/pyproject.toml
--rw-rw-rw-   0        0        0      502 2024-05-16 17:34:30.000000 ipywebview-5.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 18:48:06.000000 ipywebview-5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/
--rw-rw-rw-   0        0        0    13975 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/__init__.py
--rw-rw-rw-   0        0        0      159 2024-05-16 18:48:05.000000 ipywebview-5.2/webview/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/dom/
--rw-rw-rw-   0        0        0     1027 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/dom/__init__.py
--rw-rw-rw-   0        0        0     1436 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/dom/classlist.py
--rw-rw-rw-   0        0        0     2609 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/dom/dom.py
--rw-rw-rw-   0        0        0    15098 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/dom/element.py
--rw-rw-rw-   0        0        0     1163 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/dom/event.py
--rw-rw-rw-   0        0        0     6168 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/dom/propsdict.py
--rw-rw-rw-   0        0        0       99 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/errors.py
--rw-rw-rw-   0        0        0     2583 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/event.py
--rw-rw-rw-   0        0        0     3953 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/guilib.py
--rw-rw-rw-   0        0        0     8290 2024-05-16 18:40:36.000000 ipywebview-5.2/webview/http.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/js/
--rw-rw-rw-   0        0        0      118 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/js/__init__.py
--rw-rw-rw-   0        0        0      385 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/js/alert.py
--rw-rw-rw-   0        0        0     8328 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/js/api.py
--rw-rw-rw-   0        0        0      534 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/js/css.py
--rw-rw-rw-   0        0        0    26937 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/js/dom_json.py
--rw-rw-rw-   0        0        0     1745 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/js/events.py
--rw-rw-rw-   0        0        0     1741 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/js/mouse.py
--rw-rw-rw-   0        0        0     8503 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/js/npo.py
--rw-rw-rw-   0        0        0      533 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/js/polyfill.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/lib/
--rw-rw-rw-   0        0        0   500712 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/lib/Microsoft.Web.WebView2.Core.dll
--rw-rw-rw-   0        0        0     1641 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/lib/Microsoft.Web.WebView2.LICENSE.md
--rw-rw-rw-   0        0        0    38376 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/lib/Microsoft.Web.WebView2.WinForms.dll
--rw-rw-rw-   0        0        0     7168 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/lib/WebBrowserInterop.x64.dll
--rw-rw-rw-   0        0        0     7168 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/lib/WebBrowserInterop.x86.dll
--rw-rw-rw-   0        0        0     9071 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/lib/pywebview-android.jar
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/lib/runtimes/
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/lib/runtimes/win-arm64/
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/lib/runtimes/win-arm64/native/
--rw-rw-rw-   0        0        0   137176 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/lib/runtimes/win-arm64/native/WebView2Loader.dll
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/lib/runtimes/win-x64/
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/lib/runtimes/win-x64/native/
--rw-rw-rw-   0        0        0   161240 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/lib/runtimes/win-x64/native/WebView2Loader.dll
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/lib/runtimes/win-x86/
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/lib/runtimes/win-x86/native/
--rw-rw-rw-   0        0        0   116184 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/lib/runtimes/win-x86/native/WebView2Loader.dll
--rw-rw-rw-   0        0        0      782 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/localization.py
--rw-rw-rw-   0        0        0      695 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/menu.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:48:06.000000 ipywebview-5.2/webview/platforms/
--rw-rw-rw-   0        0        0        0 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/platforms/__init__.py
--rw-rw-rw-   0        0        0    13423 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/platforms/android.py
--rw-rw-rw-   0        0        0    11508 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/platforms/cef.py
--rw-rw-rw-   0        0        0    52467 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/platforms/cocoa.py
--rw-rw-rw-   0        0        0    10829 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/platforms/edgechromium.py
--rw-rw-rw-   0        0        0    30887 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/platforms/gtk.py
--rw-rw-rw-   0        0        0     8996 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/platforms/mshtml.py
--rw-rw-rw-   0        0        0    37748 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/platforms/qt.py
--rw-rw-rw-   0        0        0    29118 2024-05-16 18:41:04.000000 ipywebview-5.2/webview/platforms/winforms.py
--rw-rw-rw-   0        0        0        0 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/py.typed
--rw-rw-rw-   0        0        0      340 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/screen.py
--rw-rw-rw-   0        0        0    12429 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/util.py
--rw-rw-rw-   0        0        0    17569 2024-05-16 17:34:30.000000 ipywebview-5.2/webview/window.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/
+-rw-rw-rw-   0        0        0      148 2024-05-16 17:34:29.000000 ipywebview-5.2.1/.editorconfig
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/.github/
+-rw-rw-rw-   0        0        0      556 2024-05-16 17:34:29.000000 ipywebview-5.2.1/.github/funding.yml
+-rw-rw-rw-   0        0        0      344 2024-05-16 17:34:29.000000 ipywebview-5.2.1/.github/issue_template.md
+-rw-rw-rw-   0        0        0      695 2024-05-16 17:34:29.000000 ipywebview-5.2.1/.github/stale.yml
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/.github/workflows/
+-rw-rw-rw-   0        0        0      560 2024-05-16 17:34:29.000000 ipywebview-5.2.1/.github/workflows/docs.yaml
+-rw-rw-rw-   0        0        0     1233 2024-05-16 17:34:29.000000 ipywebview-5.2.1/.github/workflows/stale.yml
+-rw-rw-rw-   0        0        0      324 2024-05-22 10:48:17.000000 ipywebview-5.2.1/.gitignore
+-rw-rw-rw-   0        0        0      401 2024-05-16 17:34:29.000000 ipywebview-5.2.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1547 2024-05-16 17:34:29.000000 ipywebview-5.2.1/LICENSE
+-rw-rw-rw-   0        0        0      201 2024-05-16 17:34:29.000000 ipywebview-5.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3195 2024-05-22 10:51:30.000000 ipywebview-5.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5276 2024-05-16 17:34:29.000000 ipywebview-5.2.1/README.md
+-rw-rw-rw-   0        0        0      483 2024-05-16 17:34:29.000000 ipywebview-5.2.1/SECURITY.md
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/ipywebview.egg-info/
+-rw-rw-rw-   0        0        0     3195 2024-05-22 10:51:29.000000 ipywebview-5.2.1/ipywebview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1635 2024-05-22 10:51:30.000000 ipywebview-5.2.1/ipywebview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 10:51:29.000000 ipywebview-5.2.1/ipywebview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      424 2024-05-22 10:51:29.000000 ipywebview-5.2.1/ipywebview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 10:51:29.000000 ipywebview-5.2.1/ipywebview.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      904 2024-05-22 10:48:17.000000 ipywebview-5.2.1/package-lock.json
+-rw-rw-rw-   0        0        0     2536 2024-05-16 18:41:31.000000 ipywebview-5.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      502 2024-05-16 17:34:30.000000 ipywebview-5.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 10:51:30.000000 ipywebview-5.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/
+-rw-rw-rw-   0        0        0    13975 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/__init__.py
+-rw-rw-rw-   0        0        0      164 2024-05-22 10:51:29.000000 ipywebview-5.2.1/webview/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/dom/
+-rw-rw-rw-   0        0        0     1027 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/dom/__init__.py
+-rw-rw-rw-   0        0        0     1436 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/dom/classlist.py
+-rw-rw-rw-   0        0        0     2609 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/dom/dom.py
+-rw-rw-rw-   0        0        0    15098 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/dom/element.py
+-rw-rw-rw-   0        0        0     1163 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/dom/event.py
+-rw-rw-rw-   0        0        0     6168 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/dom/propsdict.py
+-rw-rw-rw-   0        0        0       99 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/errors.py
+-rw-rw-rw-   0        0        0     2583 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/event.py
+-rw-rw-rw-   0        0        0     3953 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/guilib.py
+-rw-rw-rw-   0        0        0     8311 2024-05-22 10:02:32.000000 ipywebview-5.2.1/webview/http.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/js/
+-rw-rw-rw-   0        0        0      118 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/js/__init__.py
+-rw-rw-rw-   0        0        0      385 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/js/alert.py
+-rw-rw-rw-   0        0        0     8328 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/js/api.py
+-rw-rw-rw-   0        0        0      534 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/js/css.py
+-rw-rw-rw-   0        0        0    26937 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/js/dom_json.py
+-rw-rw-rw-   0        0        0     1745 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/js/events.py
+-rw-rw-rw-   0        0        0     1741 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/js/mouse.py
+-rw-rw-rw-   0        0        0     8503 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/js/npo.py
+-rw-rw-rw-   0        0        0      533 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/js/polyfill.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/lib/
+-rw-rw-rw-   0        0        0   500712 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/lib/Microsoft.Web.WebView2.Core.dll
+-rw-rw-rw-   0        0        0     1641 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md
+-rw-rw-rw-   0        0        0    38376 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll
+-rw-rw-rw-   0        0        0     7168 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/lib/WebBrowserInterop.x64.dll
+-rw-rw-rw-   0        0        0     7168 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/lib/WebBrowserInterop.x86.dll
+-rw-rw-rw-   0        0        0     9071 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/lib/pywebview-android.jar
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/lib/runtimes/
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/lib/runtimes/win-arm64/
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/lib/runtimes/win-arm64/native/
+-rw-rw-rw-   0        0        0   137176 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/lib/runtimes/win-arm64/native/WebView2Loader.dll
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/lib/runtimes/win-x64/
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/lib/runtimes/win-x64/native/
+-rw-rw-rw-   0        0        0   161240 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/lib/runtimes/win-x64/native/WebView2Loader.dll
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/lib/runtimes/win-x86/
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/lib/runtimes/win-x86/native/
+-rw-rw-rw-   0        0        0   116184 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/lib/runtimes/win-x86/native/WebView2Loader.dll
+-rw-rw-rw-   0        0        0      782 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/localization.py
+-rw-rw-rw-   0        0        0      695 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/menu.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:51:30.000000 ipywebview-5.2.1/webview/platforms/
+-rw-rw-rw-   0        0        0        0 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/platforms/__init__.py
+-rw-rw-rw-   0        0        0    13423 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/platforms/android.py
+-rw-rw-rw-   0        0        0    11638 2024-05-22 09:45:07.000000 ipywebview-5.2.1/webview/platforms/cef.py
+-rw-rw-rw-   0        0        0    52467 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/platforms/cocoa.py
+-rw-rw-rw-   0        0        0    10829 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/platforms/edgechromium.py
+-rw-rw-rw-   0        0        0    30887 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/platforms/gtk.py
+-rw-rw-rw-   0        0        0     8996 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/platforms/mshtml.py
+-rw-rw-rw-   0        0        0    37748 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/platforms/qt.py
+-rw-rw-rw-   0        0        0    29118 2024-05-16 18:41:04.000000 ipywebview-5.2.1/webview/platforms/winforms.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/py.typed
+-rw-rw-rw-   0        0        0      340 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/screen.py
+-rw-rw-rw-   0        0        0    12429 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/util.py
+-rw-rw-rw-   0        0        0    17569 2024-05-16 17:34:30.000000 ipywebview-5.2.1/webview/window.py
```

### Comparing `ipywebview-5.2/.github/funding.yml` & `ipywebview-5.2.1/.github/funding.yml`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/.github/stale.yml` & `ipywebview-5.2.1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/.github/workflows/docs.yaml` & `ipywebview-5.2.1/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/.github/workflows/stale.yml` & `ipywebview-5.2.1/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/LICENSE` & `ipywebview-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/PKG-INFO` & `ipywebview-5.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywebview
-Version: 5.2
+Version: 5.2.1
 Summary: Build GUI for your Python program with JavaScript, HTML, and CSS
 Author-email: sqwindows <sqwindows@qq.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `ipywebview-5.2/README.md` & `ipywebview-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/ipywebview.egg-info/PKG-INFO` & `ipywebview-5.2.1/ipywebview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywebview
-Version: 5.2
+Version: 5.2.1
 Summary: Build GUI for your Python program with JavaScript, HTML, and CSS
 Author-email: sqwindows <sqwindows@qq.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `ipywebview-5.2/ipywebview.egg-info/SOURCES.txt` & `ipywebview-5.2.1/ipywebview.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
 SECURITY.md
+package-lock.json
 pyproject.toml
 requirements.txt
 .github/funding.yml
 .github/issue_template.md
 .github/stale.yml
 .github/workflows/docs.yaml
 .github/workflows/stale.yml
```

### Comparing `ipywebview-5.2/pyproject.toml` & `ipywebview-5.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/__init__.py` & `ipywebview-5.2.1/webview/__init__.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/dom/__init__.py` & `ipywebview-5.2.1/webview/dom/__init__.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/dom/classlist.py` & `ipywebview-5.2.1/webview/dom/classlist.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/dom/dom.py` & `ipywebview-5.2.1/webview/dom/dom.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/dom/element.py` & `ipywebview-5.2.1/webview/dom/element.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/dom/event.py` & `ipywebview-5.2.1/webview/dom/event.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/dom/propsdict.py` & `ipywebview-5.2.1/webview/dom/propsdict.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/event.py` & `ipywebview-5.2.1/webview/event.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/guilib.py` & `ipywebview-5.2.1/webview/guilib.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/http.py` & `ipywebview-5.2.1/webview/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-
+import encodings.idna
 import os
 import sys
 from typing import TypeVar, cast
 
 if sys.platform == 'win32' and ('pythonw.exe' in sys.executable or getattr(sys, 'frozen', False)):
     # bottle.py versions prior to 0.12.23 (the latest on PyPi as of Feb 2023) require stdout and
     # stderr to exist, which is not the case on Windows with pythonw.exe or PyInstaller >= 5.8.0
```

### Comparing `ipywebview-5.2/webview/js/api.py` & `ipywebview-5.2.1/webview/js/api.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/js/css.py` & `ipywebview-5.2.1/webview/js/css.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/js/dom_json.py` & `ipywebview-5.2.1/webview/js/dom_json.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/js/events.py` & `ipywebview-5.2.1/webview/js/events.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/js/mouse.py` & `ipywebview-5.2.1/webview/js/mouse.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/js/npo.py` & `ipywebview-5.2.1/webview/js/npo.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/js/polyfill.py` & `ipywebview-5.2.1/webview/js/polyfill.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/lib/Microsoft.Web.WebView2.Core.dll` & `ipywebview-5.2.1/webview/lib/Microsoft.Web.WebView2.Core.dll`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/lib/Microsoft.Web.WebView2.LICENSE.md` & `ipywebview-5.2.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/lib/Microsoft.Web.WebView2.WinForms.dll` & `ipywebview-5.2.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/lib/WebBrowserInterop.x64.dll` & `ipywebview-5.2.1/webview/lib/WebBrowserInterop.x64.dll`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/lib/WebBrowserInterop.x86.dll` & `ipywebview-5.2.1/webview/lib/WebBrowserInterop.x86.dll`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/lib/pywebview-android.jar` & `ipywebview-5.2.1/webview/lib/pywebview-android.jar`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/lib/runtimes/win-arm64/native/WebView2Loader.dll` & `ipywebview-5.2.1/webview/lib/runtimes/win-arm64/native/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/lib/runtimes/win-x64/native/WebView2Loader.dll` & `ipywebview-5.2.1/webview/lib/runtimes/win-x64/native/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/lib/runtimes/win-x86/native/WebView2Loader.dll` & `ipywebview-5.2.1/webview/lib/runtimes/win-x86/native/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/localization.py` & `ipywebview-5.2.1/webview/localization.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/menu.py` & `ipywebview-5.2.1/webview/menu.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/platforms/android.py` & `ipywebview-5.2.1/webview/platforms/android.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/platforms/cef.py` & `ipywebview-5.2.1/webview/platforms/cef.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,16 @@
             'data:text/html,{0}'.format(window.html)
             if window.html
             else window.real_url or 'data:text/html,{0}'.format(DEFAULT_HTML)
         )
 
         default_browser_settings = {}
         all_browser_settings = dict(default_browser_settings, **browser_settings)
-
+        if 'ignore_certificate_errors' in all_browser_settings:
+            del all_browser_settings['ignore_certificate_errors']
         cef_browser = cef.CreateBrowserSync(
             window_info=window_info, settings=all_browser_settings, url=real_url
         )
         browser = Browser(window, handle, cef_browser, parent)
 
         bindings = cef.JavascriptBindings()
         bindings.SetObject('external', browser.js_bridge)
```

### Comparing `ipywebview-5.2/webview/platforms/cocoa.py` & `ipywebview-5.2.1/webview/platforms/cocoa.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/platforms/edgechromium.py` & `ipywebview-5.2.1/webview/platforms/edgechromium.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/platforms/gtk.py` & `ipywebview-5.2.1/webview/platforms/gtk.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/platforms/mshtml.py` & `ipywebview-5.2.1/webview/platforms/mshtml.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/platforms/qt.py` & `ipywebview-5.2.1/webview/platforms/qt.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/platforms/winforms.py` & `ipywebview-5.2.1/webview/platforms/winforms.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/util.py` & `ipywebview-5.2.1/webview/util.py`

 * *Files identical despite different names*

### Comparing `ipywebview-5.2/webview/window.py` & `ipywebview-5.2.1/webview/window.py`

 * *Files identical despite different names*

