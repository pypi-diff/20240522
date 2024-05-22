# Comparing `tmp/djangocms_blog_agenda-0.5.6.tar.gz` & `tmp/djangocms_blog_agenda-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_blog_agenda-0.5.6.tar", last modified: Thu Apr 18 15:59:53 2024, max compression
+gzip compressed data, was "djangocms_blog_agenda-0.6.0.tar", last modified: Wed May 22 08:05:19 2024, max compression
```

## Comparing `djangocms_blog_agenda-0.5.6.tar` & `djangocms_blog_agenda-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.641004 djangocms_blog_agenda-0.5.6/
--rw-r--r--   0 kapt       (501) kapt        (20)       45 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/AUTHORS.md
--rw-r--r--   0 kapt       (501) kapt        (20)     1318 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/CONTRIBUTING.md
--rw-r--r--   0 kapt       (501) kapt        (20)    35149 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/LICENSE
--rw-r--r--   0 kapt       (501) kapt        (20)      159 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/MANIFEST.in
--rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-04-18 15:59:53.641004 djangocms_blog_agenda-0.5.6/PKG-INFO
--rw-r--r--   0 kapt       (501) kapt        (20)     2682 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/README.md
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.630004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/__init__.py
--rw-r--r--   0 kapt       (501) kapt        (20)     4389 2023-05-25 06:47:09.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/admin.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1746 2023-03-31 09:10:44.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/apps.py
--rw-r--r--   0 kapt       (501) kapt        (20)     3921 2023-12-12 08:25:46.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/cms_plugins.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.622004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.622004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.633004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt       (501) kapt        (20)     2095 2023-11-27 13:10:23.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt       (501) kapt        (20)     4357 2023-11-27 13:10:10.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.638004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/
--rw-r--r--   0 kapt       (501) kapt        (20)     1076 2023-03-30 10:38:48.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0001_initial.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1139 2023-03-30 14:50:16.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
--rw-r--r--   0 kapt       (501) kapt        (20)      746 2023-11-13 16:05:40.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py
--rw-r--r--   0 kapt       (501) kapt        (20)      651 2023-12-12 08:49:47.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py
--rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/__init__.py
--rw-r--r--   0 kapt       (501) kapt        (20)      951 2024-04-18 15:57:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/misc.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1273 2023-11-27 13:02:24.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/models.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1117 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/patched_urls.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.623004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.640004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501) kapt        (20)     1341 2023-03-30 10:37:22.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
--rw-r--r--   0 kapt       (501) kapt        (20)     1742 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
--rw-r--r--   0 kapt       (501) kapt        (20)     1361 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
--rw-r--r--   0 kapt       (501) kapt        (20)     1889 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
--rw-r--r--   0 kapt       (501) kapt        (20)     2549 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/views.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.641004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/
--rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/PKG-INFO
--rw-r--r--   0 kapt       (501) kapt        (20)     1222 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/SOURCES.txt
--rw-r--r--   0 kapt       (501) kapt        (20)        1 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/dependency_links.txt
--rw-r--r--   0 kapt       (501) kapt        (20)       15 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/requires.txt
--rw-r--r--   0 kapt       (501) kapt        (20)       22 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/top_level.txt
--rw-r--r--   0 kapt       (501) kapt        (20)      786 2024-04-18 15:59:53.642004 djangocms_blog_agenda-0.5.6/setup.cfg
--rw-r--r--   0 kapt       (501) kapt        (20)       53 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/setup.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:05:19.173882 djangocms_blog_agenda-0.6.0/
+-rw-r--r--   0 kapt       (501) kapt        (20)       45 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/AUTHORS.md
+-rw-r--r--   0 kapt       (501) kapt        (20)     1318 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 kapt       (501) kapt        (20)    35149 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/LICENSE
+-rw-r--r--   0 kapt       (501) kapt        (20)      159 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/MANIFEST.in
+-rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-05-22 08:05:19.173882 djangocms_blog_agenda-0.6.0/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)     2682 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/README.md
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:05:19.160882 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     4389 2023-05-25 06:47:09.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/admin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1746 2023-03-31 09:10:44.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/apps.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     4101 2024-05-22 08:04:25.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/cms_plugins.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:05:19.142882 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/locale/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:05:19.142882 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/locale/fr/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:05:19.167882 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt       (501) kapt        (20)     2229 2024-05-22 08:01:11.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt       (501) kapt        (20)     3599 2024-05-22 08:01:04.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:05:19.170882 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/
+-rw-r--r--   0 kapt       (501) kapt        (20)     1076 2023-03-30 10:38:48.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/0001_initial.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1139 2023-03-30 14:50:16.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      746 2023-11-13 16:05:40.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      651 2023-12-12 08:49:47.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     3242 2024-05-22 08:04:25.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/0005_auto_20240521_1359.py
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      951 2024-04-18 15:57:53.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/misc.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1380 2024-05-22 08:04:25.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/models.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1117 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/patched_urls.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:05:19.144882 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:05:19.172882 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501) kapt        (20)     1341 2023-03-30 10:37:22.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     1742 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     1361 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     1889 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     2549 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/views.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:05:19.172882 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda.egg-info/
+-rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-05-22 08:05:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda.egg-info/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)     1282 2024-05-22 08:05:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)        1 2024-05-22 08:05:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       15 2024-05-22 08:05:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda.egg-info/requires.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       22 2024-05-22 08:05:19.000000 djangocms_blog_agenda-0.6.0/djangocms_blog_agenda.egg-info/top_level.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)      786 2024-05-22 08:05:19.174882 djangocms_blog_agenda-0.6.0/setup.cfg
+-rw-r--r--   0 kapt       (501) kapt        (20)       53 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.0/setup.py
```

### Comparing `djangocms_blog_agenda-0.5.6/CONTRIBUTING.md` & `djangocms_blog_agenda-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/LICENSE` & `djangocms_blog_agenda-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/PKG-INFO` & `djangocms_blog_agenda-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.5.6
+Version: 0.6.0
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms_blog_agenda-0.5.6/README.md` & `djangocms_blog_agenda-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/admin.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/apps.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/cms_plugins.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/cms_plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,29 +42,34 @@
     """
     Return upcoming events
     """
 
     name = _("Upcoming events")
     model = UpcomingEventsPlugin
 
+    def get_fields(self, request, obj=None):
+        fields = super().get_fields(request, obj)
+        fields.insert(2, "show_until_event_end")
+        return fields
+
     def get_posts(self, instance, request, published_only=True):
         posts = instance.post_queryset(request, published_only)
 
         # Keep only posts with an event date in the futur
-        posts = posts.order_by("extension__event_start_date").filter(
-            (
-                Q(extension__event_end_date__isnull=True)
-                & Q(extension__event_start_date__gte=timezone.now())
-            )
-            | (
-                Q(extension__event_end_date__isnull=False)
-                & Q(extension__event_end_date__gte=timezone.now())
-            )
+        filters = Q(extension__event_end_date__isnull=True) & Q(
+            extension__event_start_date__gte=timezone.now()
         )
 
+        if instance.show_until_event_end:
+            filters |= Q(extension__event_end_date__isnull=False) & Q(
+                extension__event_end_date__gte=timezone.now()
+            )
+
+        posts = posts.order_by("extension__event_start_date").filter(filters)
+
         if instance.tags.exists():
             posts = posts.filter(tags__in=list(instance.tags.all()))
         if instance.categories.exists():
             posts = posts.filter(categories__in=list(instance.categories.all()))
         return instance.optimize(posts.distinct())[: instance.latest_posts]
```

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po`

 * *Files 23% similar despite different names*

```diff
@@ -4,161 +4,163 @@
 # DEV KAPT <dev@kapt.mobi>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-27 14:09+0100\n"
+"POT-Creation-Date: 2024-05-22 10:00+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: djangocms_blog_agenda/admin.py:23 djangocms_blog_agenda/admin.py:24
-#: djangocms_blog_agenda/models.py:17 djangocms_blog_agenda/models.py:21
+#: admin.py:23 admin.py:24 models.py:17 models.py:21
 msgid "Event infos"
 msgstr "Informations sur l'événement"
 
-#: djangocms_blog_agenda/admin.py:55
+#: admin.py:55
 msgid "Info"
 msgstr "Information"
 
-#: djangocms_blog_agenda/admin.py:66
+#: admin.py:66
 msgid "Images"
 msgstr "Images"
 
-#: djangocms_blog_agenda/admin.py:73
+#: admin.py:73
 msgid "SEO"
 msgstr "SEO"
 
-#: djangocms_blog_agenda/admin.py:90
+#: admin.py:90
 msgid "Event dates"
 msgstr "Dates de l’événement"
 
-#: djangocms_blog_agenda/admin.py:99
+#: admin.py:99
 msgid "jS"
 msgstr "j"
 
-#: djangocms_blog_agenda/admin.py:100
+#: admin.py:100
 msgid "jS F"
 msgstr "j F"
 
-#: djangocms_blog_agenda/admin.py:101
+#: admin.py:101
 msgid "jS F Y"
 msgstr "j F Y"
 
-#: djangocms_blog_agenda/admin.py:104 djangocms_blog_agenda/admin.py:111
+#: admin.py:104 admin.py:111
 #, python-brace-format
 msgid "on {date}"
 msgstr "le {date}"
 
-#: djangocms_blog_agenda/admin.py:117 djangocms_blog_agenda/admin.py:123
-#: djangocms_blog_agenda/admin.py:129
+#: admin.py:117 admin.py:123 admin.py:129
 #, python-brace-format
 msgid "from {start_part} to {end_part}"
 msgstr "du {start_part} au {end_part}"
 
-#: djangocms_blog_agenda/cms_plugins.py:45
+#: cms_plugins.py:46
 msgid "Upcoming events"
 msgstr "Prochains événements"
 
-#: djangocms_blog_agenda/cms_plugins.py:75
+#: cms_plugins.py:84
 msgid "Past events"
 msgstr "Événements passés"
 
-#: djangocms_blog_agenda/models.py:8
+#: models.py:8
 msgid "Event start"
 msgstr "Début de l’événement"
 
-#: djangocms_blog_agenda/models.py:10
+#: models.py:10
 msgid "Event end"
 msgstr "Fin de l’événement"
 
-#: djangocms_blog_agenda/models.py:13
+#: models.py:13
 msgid "If the event is held over several days"
 msgstr "Si l’événement se tient sur plusieurs jours"
 
-#: djangocms_blog_agenda/models.py:18
+#: models.py:18
 msgid "Events infos"
 msgstr "Informations sur les événements"
 
-#: djangocms_blog_agenda/models.py:26
+#: models.py:25
+msgid "Show events until their end date"
+msgstr "Garder affiché les événements jusqu’à leur date de fin"
+
+#: models.py:28
 msgid "{} upcoming events"
 msgstr "{} prochains événements"
 
-#: djangocms_blog_agenda/models.py:30
+#: models.py:31
 msgid "Upcoming events plugin"
 msgstr "Plugin Prochains événements"
 
-#: djangocms_blog_agenda/models.py:31
+#: models.py:32
 msgid "Upcoming events plugins"
 msgstr "Plugins Prochains événements"
 
-#: djangocms_blog_agenda/models.py:36
+#: models.py:37
 msgid "{} past events"
 msgstr "{} événements passés"
 
-#: djangocms_blog_agenda/models.py:40
+#: models.py:41
 msgid "Past events plugin"
 msgstr "Plugin Événements passés"
 
-#: djangocms_blog_agenda/models.py:41
+#: models.py:42
 msgid "Past events plugins"
 msgstr "Plugins Événements passés"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html:6
+#: templates/djangocms_blog_agenda/blog_meta.html:6
 msgid "by"
 msgstr "par"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html:32
+#: templates/djangocms_blog_agenda/post_item.html:32
 msgid "read more"
 msgstr "lire la suite"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:11
+#: templates/djangocms_blog_agenda/post_list.html:11
 msgid "Articles by"
 msgstr "Article par"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:12
+#: templates/djangocms_blog_agenda/post_list.html:12
 msgid "Archive"
 msgstr "Archive"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:13
+#: templates/djangocms_blog_agenda/post_list.html:13
 msgid "Tag"
 msgstr "Tag"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:14
+#: templates/djangocms_blog_agenda/post_list.html:14
 msgid "Category"
 msgstr "Catégorie"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:21
+#: templates/djangocms_blog_agenda/post_list.html:21
 msgid "No article found."
 msgstr "Aucun article trouvé."
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:24
+#: templates/djangocms_blog_agenda/post_list.html:24
 msgid "Back"
 msgstr "Retour"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:29
+#: templates/djangocms_blog_agenda/post_list.html:29
 msgid "previous"
 msgstr "précédent"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:32
+#: templates/djangocms_blog_agenda/post_list.html:32
 msgid "Page"
 msgstr "Page"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:32
+#: templates/djangocms_blog_agenda/post_list.html:32
 msgid "of"
 msgstr "sur"
 
-#: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:35
+#: templates/djangocms_blog_agenda/post_list.html:35
 msgid "next"
 msgstr "suivant"
 
 #~ msgctxt "agenda_view_url"
 #~ msgid "archives/"
 #~ msgstr "archives/"
```

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0001_initial.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/misc.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/misc.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/models.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,19 +18,22 @@
         verbose_name_plural = _("Events infos")
 
     def __str__(self):
         return _("Event infos") + " (#" + str(self.id) + ")"
 
 
 class UpcomingEventsPlugin(LatestPostsPlugin):
+    show_until_event_end = models.BooleanField(
+        verbose_name=_("Show events until their end date"), default=True
+    )
+
     def __str__(self):
         return _("{} upcoming events").format(self.latest_posts)
 
     class Meta:
-        proxy = True
         verbose_name = _("Upcoming events plugin")
         verbose_name_plural = _("Upcoming events plugins")
 
 
 class PastEventsPlugin(LatestPostsPlugin):
     def __str__(self):
         return _("{} past events").format(self.latest_posts)
```

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/patched_urls.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/patched_urls.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/views.py` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda/views.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/PKG-INFO` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.5.6
+Version: 0.6.0
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/SOURCES.txt` & `djangocms_blog_agenda-0.6.0/djangocms_blog_agenda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,12 +20,13 @@
 djangocms_blog_agenda.egg-info/top_level.txt
 djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
 djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
 djangocms_blog_agenda/migrations/0001_initial.py
 djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
 djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py
 djangocms_blog_agenda/migrations/0004_pasteventsplugin.py
+djangocms_blog_agenda/migrations/0005_auto_20240521_1359.py
 djangocms_blog_agenda/migrations/__init__.py
 djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
 djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
 djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
 djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
```

### Comparing `djangocms_blog_agenda-0.5.6/setup.cfg` & `djangocms_blog_agenda-0.6.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangocms-blog-agenda
-version = 0.5.6
+version = 0.6.0
 description = Create an agenda on top of djangocms-blog!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 author = Corentin Bettiol
 author_email = dev@kapt.mobi
 classifiers =
```

