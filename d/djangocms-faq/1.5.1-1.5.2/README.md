# Comparing `tmp/djangocms-faq-1.5.1.tar.gz` & `tmp/djangocms_faq-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-faq-1.5.1.tar", last modified: Mon Sep 26 15:59:55 2022, max compression
+gzip compressed data, was "djangocms_faq-1.5.2.tar", last modified: Wed May 22 15:47:34 2024, max compression
```

## Comparing `djangocms-faq-1.5.1.tar` & `djangocms_faq-1.5.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/
--rw-r--r--   0 kapt      (1000) kapt      (1000)       45 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/AUTHORS.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1302 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/CONTRIBUTING.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)    35148 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/LICENSE
--rw-r--r--   0 kapt      (1000) kapt      (1000)      143 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/MANIFEST.in
--rw-r--r--   0 kapt      (1000) kapt      (1000)     9505 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     8583 2022-09-26 15:58:18.000000 djangocms-faq-1.5.1/README.md
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/djangocms_faq/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2782 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/admin.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      100 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/apps.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2544 2022-09-26 15:36:26.000000 djangocms-faq-1.5.1/djangocms_faq/cms_plugins.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/djangocms_faq/locale/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/djangocms_faq/locale/fr/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/djangocms_faq/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3139 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4556 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/djangocms_faq/migrations/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4180 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/migrations/0001_initial.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3310 2022-07-28 08:21:04.000000 djangocms-faq-1.5.1/djangocms_faq/migrations/0002_auto_20210531_1650.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4402 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/migrations/0003_auto_20210825_1012.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/migrations/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5416 2022-09-26 15:58:01.000000 djangocms-faq-1.5.1/djangocms_faq/models.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      768 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/settings.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/djangocms_faq/templates/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/djangocms_faq/templates/admin/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      127 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/templates/admin/change_form_help_text.html
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/djangocms_faq/templates/faq/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      241 2022-09-26 15:58:02.000000 djangocms-faq-1.5.1/djangocms_faq/templates/faq/faq_plugin.html
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1642 2022-09-26 15:40:46.000000 djangocms-faq-1.5.1/djangocms_faq/templates/faq/faq_question.html
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4653 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/templates/faq/faq_search.html
--rw-r--r--   0 kapt      (1000) kapt      (1000)      121 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/urls.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4467 2022-09-26 15:58:02.000000 djangocms-faq-1.5.1/djangocms_faq/utils.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1208 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/djangocms_faq/views.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2022-09-26 15:59:55.629532 djangocms-faq-1.5.1/djangocms_faq.egg-info/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     9505 2022-09-26 15:59:55.000000 djangocms-faq-1.5.1/djangocms_faq.egg-info/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)      942 2022-09-26 15:59:55.000000 djangocms-faq-1.5.1/djangocms_faq.egg-info/SOURCES.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2022-09-26 15:59:55.000000 djangocms-faq-1.5.1/djangocms_faq.egg-info/dependency_links.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       35 2022-09-26 15:59:55.000000 djangocms-faq-1.5.1/djangocms_faq.egg-info/requires.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       14 2022-09-26 15:59:55.000000 djangocms-faq-1.5.1/djangocms_faq.egg-info/top_level.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)      923 2022-09-26 15:59:55.633532 djangocms-faq-1.5.1/setup.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)       53 2022-07-28 07:50:49.000000 djangocms-faq-1.5.1/setup.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.131332 djangocms_faq-1.5.2/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       45 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/AUTHORS.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1302 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/CONTRIBUTING.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    35148 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/LICENSE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      143 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/MANIFEST.in
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     9542 2024-05-22 15:47:34.131332 djangocms_faq-1.5.2/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     8583 2022-09-26 15:58:18.000000 djangocms_faq-1.5.2/README.md
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.127332 djangocms_faq-1.5.2/djangocms_faq/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2782 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/admin.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      100 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/apps.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2544 2022-09-26 15:36:26.000000 djangocms_faq-1.5.2/djangocms_faq/cms_plugins.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.127332 djangocms_faq-1.5.2/djangocms_faq/locale/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.127332 djangocms_faq-1.5.2/djangocms_faq/locale/fr/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.131332 djangocms_faq-1.5.2/djangocms_faq/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3609 2024-05-22 15:41:44.000000 djangocms_faq-1.5.2/djangocms_faq/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3796 2024-05-22 15:41:44.000000 djangocms_faq-1.5.2/djangocms_faq/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.131332 djangocms_faq-1.5.2/djangocms_faq/migrations/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4180 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/migrations/0001_initial.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3310 2022-07-28 08:21:04.000000 djangocms_faq-1.5.2/djangocms_faq/migrations/0002_auto_20210531_1650.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4402 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/migrations/0003_auto_20210825_1012.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/migrations/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5679 2024-05-22 15:45:39.000000 djangocms_faq-1.5.2/djangocms_faq/models.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      768 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/settings.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.127332 djangocms_faq-1.5.2/djangocms_faq/templates/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.131332 djangocms_faq-1.5.2/djangocms_faq/templates/admin/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      127 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/templates/admin/change_form_help_text.html
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.131332 djangocms_faq-1.5.2/djangocms_faq/templates/faq/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      241 2022-09-26 15:58:02.000000 djangocms_faq-1.5.2/djangocms_faq/templates/faq/faq_plugin.html
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1642 2022-09-26 15:40:46.000000 djangocms_faq-1.5.2/djangocms_faq/templates/faq/faq_question.html
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4653 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/templates/faq/faq_search.html
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      121 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/urls.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4475 2024-05-22 15:35:40.000000 djangocms_faq-1.5.2/djangocms_faq/utils.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1208 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/djangocms_faq/views.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-22 15:47:34.131332 djangocms_faq-1.5.2/djangocms_faq.egg-info/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     9542 2024-05-22 15:47:34.000000 djangocms_faq-1.5.2/djangocms_faq.egg-info/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      942 2024-05-22 15:47:34.000000 djangocms_faq-1.5.2/djangocms_faq.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2024-05-22 15:47:34.000000 djangocms_faq-1.5.2/djangocms_faq.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       35 2024-05-22 15:47:34.000000 djangocms_faq-1.5.2/djangocms_faq.egg-info/requires.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       14 2024-05-22 15:47:34.000000 djangocms_faq-1.5.2/djangocms_faq.egg-info/top_level.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      923 2024-05-22 15:47:34.131332 djangocms_faq-1.5.2/setup.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       53 2022-07-28 07:50:49.000000 djangocms_faq-1.5.2/setup.py
```

### Comparing `djangocms-faq-1.5.1/CONTRIBUTING.md` & `djangocms_faq-1.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/LICENSE` & `djangocms_faq-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/PKG-INFO` & `djangocms_faq-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: djangocms-faq
-Version: 1.5.1
+Version: 1.5.2
 Summary: DjangoCMS FAQ let you create FAQ plugins that contains other plugins and provide an API to get questions/answers from keywords!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-faq
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
-Provides-Extra: fuzzy_search
 License-File: LICENSE
 License-File: AUTHORS.md
+Requires-Dist: django-cms
+Provides-Extra: fuzzy-search
+Requires-Dist: thefuzz; extra == "fuzzy-search"
 
 # DjangoCMS FAQ
 
 Frequently asked questions plugin for Django CMS, with an API to load questions from another page!
 
 ## Install
 
@@ -199,9 +199,7 @@
 
 It's a custom and *dirty* solution to the problem of handling relations *between* CMSPlugins.
 
 > It is much harder to manage the copying of relations when they are from one plugin to another.
 >
 > *source: Django-cms doc, [
 Handling Relations > Relations between plugins](https://docs.django-cms.org/en/latest/how_to/custom_plugins.html#relations-between-plugins)*.
-
-
```

### Comparing `djangocms-faq-1.5.1/README.md` & `djangocms_faq-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq/admin.py` & `djangocms_faq-1.5.2/djangocms_faq/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq/cms_plugins.py` & `djangocms_faq-1.5.2/djangocms_faq/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq/locale/fr/LC_MESSAGES/django.mo` & `djangocms_faq-1.5.2/djangocms_faq/locale/fr/LC_MESSAGES/django.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -51,14 +51,24 @@
 
 msgid "Keyword"
 msgstr "Mot-clef"
 
 msgid "Keywords"
 msgstr "Mot-clefs"
 
+msgid ""
+"Keywords are not used for SEO purposes, but to allow visitors to find FAQ "
+"questions via synonyms. For example, for a question such as \"Are pets "
+"allowed?\", you could add the keyword \"dog\"."
+msgstr ""
+"Les mot-clef ne sont pas utilisés à des fins de référencement, mais pour "
+"permettre aux visiteurs de trouver des questions de FAQ via des synonymes. "
+"Par exemple, pour une question \"les animaux sont-ils acceptés\", vous "
+"pouvez ajouter le mot-clef \"chien\"."
+
 msgid "Name"
 msgstr "Nom"
 
 msgid "No result found."
 msgstr "Aucun résultat n'a été trouvé."
 
 msgid "Not on a page (maybe an apphook, like the blog)"
```

### Comparing `djangocms-faq-1.5.1/djangocms_faq/migrations/0001_initial.py` & `djangocms_faq-1.5.2/djangocms_faq/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq/migrations/0002_auto_20210531_1650.py` & `djangocms_faq-1.5.2/djangocms_faq/migrations/0002_auto_20210531_1650.py`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq/migrations/0003_auto_20210825_1012.py` & `djangocms_faq-1.5.2/djangocms_faq/migrations/0003_auto_20210825_1012.py`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq/models.py` & `djangocms_faq-1.5.2/djangocms_faq/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,20 @@
             faq = SearchFaqPluginModel.objects.filter(uuid=relation.faq)
             faq.search_in.add(self)
 
 
 class QuestionFaqPluginModel(CMSPlugin):
     question = models.CharField(_("Question"), max_length=300)
     keywords = models.ManyToManyField(
-        "djangocms_faq.Keyword", verbose_name=_("Keywords")
+        "djangocms_faq.Keyword",
+        verbose_name=_("Keywords"),
+        help_text=_(
+            'Keywords are not used for SEO purposes, but to allow visitors to find FAQ questions via synonyms. For example, for a question such as "Are pets allowed?", you could add the keyword "dog".'
+        ),
+        blank=True,
     )
     slug = models.SlugField(
         blank=True,
         default="",
         help_text=_(
             "Unique slug for this question. Keep empty to let it be auto-generated. <br /><i>Warning: There is no control that the slug is unique, so you have to update it yourself if there is another question on the same page with the same slug.</i>"
         ),
```

### Comparing `djangocms-faq-1.5.1/djangocms_faq/settings.py` & `djangocms_faq-1.5.2/djangocms_faq/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq/templates/faq/faq_question.html` & `djangocms_faq-1.5.2/djangocms_faq/templates/faq/faq_question.html`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq/templates/faq/faq_search.html` & `djangocms_faq-1.5.2/djangocms_faq/templates/faq/faq_search.html`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq/utils.py` & `djangocms_faq-1.5.2/djangocms_faq/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 if query in slugify(keyword):
                     answers_keywords.append(question)
 
             # search correspondance word by word for each word in query and slugs
             if SEARCH_WORD_BY_WORD_KEYWORDS:
                 query_list = query.split(" ")
                 for query_word in query_list:
-                    for keyword_word in keyword.split(" "):
+                    for keyword_word in keyword.keyword.split(" "):
                         if ENABLE_FUZZY_SEARCH:
                             if (
                                 fuzz.token_sort_ratio(query_word, keyword_word)
                                 >= FUZZY_SEARCH_PERCENTAGE
                             ):
                                 answers_keywords.append(question)
                         else:
```

### Comparing `djangocms-faq-1.5.1/djangocms_faq/views.py` & `djangocms_faq-1.5.2/djangocms_faq/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/djangocms_faq.egg-info/PKG-INFO` & `djangocms_faq-1.5.2/djangocms_faq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: djangocms-faq
-Version: 1.5.1
+Version: 1.5.2
 Summary: DjangoCMS FAQ let you create FAQ plugins that contains other plugins and provide an API to get questions/answers from keywords!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-faq
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
-Provides-Extra: fuzzy_search
 License-File: LICENSE
 License-File: AUTHORS.md
+Requires-Dist: django-cms
+Provides-Extra: fuzzy-search
+Requires-Dist: thefuzz; extra == "fuzzy-search"
 
 # DjangoCMS FAQ
 
 Frequently asked questions plugin for Django CMS, with an API to load questions from another page!
 
 ## Install
 
@@ -199,9 +199,7 @@
 
 It's a custom and *dirty* solution to the problem of handling relations *between* CMSPlugins.
 
 > It is much harder to manage the copying of relations when they are from one plugin to another.
 >
 > *source: Django-cms doc, [
 Handling Relations > Relations between plugins](https://docs.django-cms.org/en/latest/how_to/custom_plugins.html#relations-between-plugins)*.
-
-
```

### Comparing `djangocms-faq-1.5.1/djangocms_faq.egg-info/SOURCES.txt` & `djangocms_faq-1.5.2/djangocms_faq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-faq-1.5.1/setup.cfg` & `djangocms_faq-1.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangocms-faq
-version = 1.5.1
+version = 1.5.2
 description = DjangoCMS FAQ let you create FAQ plugins that contains other plugins and provide an API to get questions/answers from keywords!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kapt/open-source/djangocms-faq
 author = Dev Kapt
 author_email = dev@kapt.mobi
 classifiers =
```

