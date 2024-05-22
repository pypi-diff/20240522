# Comparing `tmp/ansys-sphinx-theme-0.9.8.tar.gz` & `tmp/ansys-sphinx-theme-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-sphinx-theme-0.9.8.tar", last modified: Thu Apr 20 13:32:49 2023, max compression
+gzip compressed data, was "ansys-sphinx-theme-0.9.9.tar", last modified: Tue May  9 13:36:10 2023, max compression
```

## Comparing `ansys-sphinx-theme-0.9.8.tar` & `ansys-sphinx-theme-0.9.9.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0     1089 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/LICENSE
--rw-r--r--   0        0        0     4224 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/README.rst
--rw-r--r--   0        0        0     2172 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     4933 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/__init__.py
--rw-r--r--   0        0        0       78 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/__init__.py
--rw-r--r--   0        0        0      726 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/sample_func.py
--rw-r--r--   0        0        0     6335 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/samples.py
--rw-r--r--   0        0        0      755 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/type_hint_example.py
--rw-r--r--   0        0        0      423 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/404.html
--rw-r--r--   0        0        0     2432 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/__init__.py
--rw-r--r--   0        0        0     4523 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/cover.tex
--rw-r--r--   0        0        0      102 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      606 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      391 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/announcement_version.html
--rw-r--r--   0        0        0      237 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0        0        0     2560 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html
--rw-r--r--   0        0        0      557 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/theme-version.html
--rw-r--r--   0        0        0     1183 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html
--rw-r--r--   0        0        0      175 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/404.rst
--rw-r--r--   0        0        0      327 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys-favicon.png
--rw-r--r--   0        0        0    45165 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg
--rw-r--r--   0        0        0    50754 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg
--rw-r--r--   0        0        0     4788 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf
--rw-r--r--   0        0        0     4503 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf
--rw-r--r--   0        0        0    19674 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css
--rw-r--r--   0        0        0     1133 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css
--rw-r--r--   0        0        0     2626 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css
--rw-r--r--   0        0        0   268588 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf
--rw-r--r--   0        0        0   269108 2023-04-20 13:32:34.992655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf
--rw-r--r--   0        0        0   268280 2023-04-20 13:32:34.992655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf
--rw-r--r--   0        0        0      227 2023-04-20 13:32:34.992655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/download_target_blank.js
--rw-r--r--   0        0        0       76 2023-04-20 13:32:34.992655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/table.js
--rw-r--r--   0        0        0    54761 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0    54600 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png
--rw-r--r--   0        0        0    54836 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png
--rw-r--r--   0        0        0    32456 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png
--rw-r--r--   0        0        0    54325 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png
--rw-r--r--   0        0        0    31713 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png
--rw-r--r--   0        0        0     1729 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf
--rw-r--r--   0        0        0      358 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/theme.conf
--rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 ansys-sphinx-theme-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-09 13:35:57.239913 ansys-sphinx-theme-0.9.9/LICENSE
+-rw-r--r--   0        0        0     4224 2023-05-09 13:35:57.239913 ansys-sphinx-theme-0.9.9/README.rst
+-rw-r--r--   0        0        0     2172 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     4933 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/examples/__init__.py
+-rw-r--r--   0        0        0      726 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/examples/sample_func.py
+-rw-r--r--   0        0        0     6335 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/examples/samples.py
+-rw-r--r--   0        0        0      755 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/examples/type_hint_example.py
+-rw-r--r--   0        0        0      423 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/latex/404.html
+-rw-r--r--   0        0        0     2432 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/latex/__init__.py
+-rw-r--r--   0        0        0     4523 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/latex/cover.tex
+-rw-r--r--   0        0        0      102 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      606 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      391 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/announcement_version.html
+-rw-r--r--   0        0        0      237 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0        0        0     2363 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html
+-rw-r--r--   0        0        0      557 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/theme-version.html
+-rw-r--r--   0        0        0     1183 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html
+-rw-r--r--   0        0        0     2835 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/search.html
+-rw-r--r--   0        0        0      175 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/404.rst
+-rw-r--r--   0        0        0      327 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys-favicon.png
+-rw-r--r--   0        0        0    45165 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg
+-rw-r--r--   0        0        0    50754 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg
+-rw-r--r--   0        0        0     4788 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf
+-rw-r--r--   0        0        0     4503 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf
+-rw-r--r--   0        0        0    19674 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css
+-rw-r--r--   0        0        0     1133 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css
+-rw-r--r--   0        0        0     2626 2023-05-09 13:35:57.243913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css
+-rw-r--r--   0        0        0   268588 2023-05-09 13:35:57.247913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf
+-rw-r--r--   0        0        0   269108 2023-05-09 13:35:57.247913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf
+-rw-r--r--   0        0        0   268280 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf
+-rw-r--r--   0        0        0      227 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/download_target_blank.js
+-rw-r--r--   0        0        0       76 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/table.js
+-rw-r--r--   0        0        0    54761 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0    54600 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png
+-rw-r--r--   0        0        0    54836 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png
+-rw-r--r--   0        0        0    32456 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png
+-rw-r--r--   0        0        0    54325 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png
+-rw-r--r--   0        0        0    31713 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png
+-rw-r--r--   0        0        0     1729 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf
+-rw-r--r--   0        0        0      358 2023-05-09 13:35:57.251913 ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/theme.conf
+-rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 ansys-sphinx-theme-0.9.9/PKG-INFO
```

### Comparing `ansys-sphinx-theme-0.9.8/LICENSE` & `ansys-sphinx-theme-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/README.rst` & `ansys-sphinx-theme-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/pyproject.toml` & `ansys-sphinx-theme-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/__init__.py` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Dict
 
 from docutils.nodes import document
 from sphinx.application import Sphinx
 
 from ansys_sphinx_theme.latex import generate_404  # noqa: F401
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 # Declare the fundamental paths of the theme
 THIS_PATH = pathlib.Path(__file__).parent.resolve()
 THEME_PATH = THIS_PATH / "theme" / "ansys_sphinx_theme"
 STATIC_PATH = THEME_PATH / "static"
 STYLE_PATH = STATIC_PATH / "css"
 JS_PATH = STATIC_PATH / "js"
```

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/sample_func.py` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/examples/sample_func.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/samples.py` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/examples/samples.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/type_hint_example.py` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/examples/type_hint_example.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/__init__.py` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/cover.tex` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/latex/cover.tex`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 <!-- Debugging: html_theme_options = {{ html_theme_options }} -->
 {% if theme_use_meilisearch %}
+  {% set API_KEY = theme_use_meilisearch.api_key %}
   <!-- Include the MeiliSearch CSS stylesheet only if theme present -->
   <link href="{{ pathto('_static/css/meilisearch.css', 1) }}" rel="stylesheet">
 
   <!-- Create a search bar form with a text input and a dropdown selector for the search index -->
   <form class="bd-search d-flex align-items-center" action="{{ pathto('search') }}" method="get">
     <input type="search" placeholder="Search" class="form-control" id="search-bar-input" autofocus />
 
     {% if theme_use_meilisearch.index_uids %}
-      <select id="indexUidSelector" class="index-select">
-      {% for index_uid, index_name in theme_use_meilisearch.index_uids.items() %}
-        <option value="{{ index_uid }}">{{ index_name }}</option>
-      {% endfor %}
-      </select>
-    {% endif %}
+        <select id="indexUidSelector" class="index-select">
+          {% for index_uid, index_name in theme_use_meilisearch.index_uids.items() %}
+            <option value="{{ index_uid }}">{{ index_name }}</option>
+          {% endfor %}
+        </select>
+      {% endif %}
     <i class="fa-solid fa-magnifying-glass"></i>
     <!-- Include the MeiliSearch JavaScript library for the search bar -->
     <script src="https://cdn.jsdelivr.net/npm/docs-searchbar.js@latest/dist/cdn/docs-searchbar.min.js"></script>
+
+    {% if not theme_use_meilisearch.host %}
+      {% set HOST_URL = "https://backend.search.pyansys.com/" %}
+    {% else %}
+      {% set HOST_URL = theme_use_meilisearch.host %}
+    {% endif %}
     
-      <!-- If no credentials provided, use the default ones  -->
-      {% if not theme_use_meilisearch.host and not theme_use_meilisearch.api_key %}
-        {% set HOST_URL = "https://search.pyansys.com" %}
-        {% set API_KEY = "A1Qxly2sls6g1rb1sIKEVEtE7R1UsHad0VgqnvKhD5nhBNf5de" %}
-      {% else %}
-        {% set HOST_URL = theme_use_meilisearch.host %}
-        {% set API_KEY = theme_use_meilisearch.api_key %}
-      {% endif %}
       <script>
       // Initialize the MeiliSearch bar with the given API key and host
       // inspect the first value of index UID as default
-      let theSearchBar = docsSearchBar({
-        hostUrl: "{{ HOST_URL }}",
-        apiKey: "{{ API_KEY }}",
-        indexUid: "{{ theme_use_meilisearch.index_uids.items()|first|first }}",
-        inputSelector: '#search-bar-input, #indexUidSelector',
-        enableDarkMode: 'auto',
-        debug: true // Set debug to true if you want to inspect the dropdown
+      var theSearchBar = docsSearchBar({
+          hostUrl: "{{ HOST_URL }}",
+          apiKey: "{{ API_KEY }}",
+          indexUid: "{{ theme_use_meilisearch.index_uids.items()|first|first }}",
+          inputSelector: '#search-bar-input',
+          enableDarkMode: 'auto',
+          debug: true // Set debug to true if you want to inspect the dropdown
       });
 
       document.getElementById('indexUidSelector').addEventListener('change', function() {
         theSearchBar.indexUid = this.value;
-        theSearchBar.inputSelector = '#docs-searchbar-suggestion';
+        theSearchBar.inputSelector = '#search-bar-input';
       });
 
       // Set the focus on the search bar input
-      document.getElementById('docs-searchbar-suggestion').focus();
+      document.getElementById('search-bar-input').focus();
     </script>
   </form>
 {% else %}
   <!-- If there is no MiliSearch enabled, use the PyData search -->
-  {%- extends "pydata_sphinx_theme/components/search-field.html" -%}
+  {%- include "pydata_sphinx_theme/components/search-field.html" -%}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
-{% if theme_use_meilisearch %}
+{% if theme_use_meilisearch %} {% set API_KEY = theme_use_meilisearch.api_key
+%}
 {% for index_uid, index_name in theme_use_meilisearch.index_uids.items() %}
 {{ index_name }}
 {% endfor %}
 {% endif %}
-{% if not theme_use_meilisearch.host and not theme_use_meilisearch.api_key %}
-{% set HOST_URL = "https://search.pyansys.com" %} {% set API_KEY =
-"A1Qxly2sls6g1rb1sIKEVEtE7R1UsHad0VgqnvKhD5nhBNf5de" %} {% else %} {% set
-HOST_URL = theme_use_meilisearch.host %} {% set API_KEY =
-theme_use_meilisearch.api_key %} {% endif %}
-{% else %} {%- extends "pydata_sphinx_theme/components/search-field.html" -%}
+{% if not theme_use_meilisearch.host %} {% set HOST_URL = "https://
+backend.search.pyansys.com/" %} {% else %} {% set HOST_URL =
+theme_use_meilisearch.host %} {% endif %}
+{% else %} {%- include "pydata_sphinx_theme/components/search-field.html" -%}
 {% endif %}
```

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/theme-version.html` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/theme-version.html`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf` & `ansys-sphinx-theme-0.9.9/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.8/PKG-INFO` & `ansys-sphinx-theme-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-sphinx-theme
-Version: 0.9.8
+Version: 0.9.9
 Summary: A theme devised by ANSYS, Inc. for Sphinx documentation.
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx
```

