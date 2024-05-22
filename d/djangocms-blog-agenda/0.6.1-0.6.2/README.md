# Comparing `tmp/djangocms_blog_agenda-0.6.1.tar.gz` & `tmp/djangocms_blog_agenda-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_blog_agenda-0.6.1.tar", last modified: Wed May 22 08:14:36 2024, max compression
+gzip compressed data, was "djangocms_blog_agenda-0.6.2.tar", last modified: Wed May 22 14:12:16 2024, max compression
```

## Comparing `djangocms_blog_agenda-0.6.1.tar` & `djangocms_blog_agenda-0.6.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:14:36.604651 djangocms_blog_agenda-0.6.1/
--rw-r--r--   0 kapt       (501) kapt        (20)       45 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/AUTHORS.md
--rw-r--r--   0 kapt       (501) kapt        (20)     1318 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 kapt       (501) kapt        (20)    35149 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/LICENSE
--rw-r--r--   0 kapt       (501) kapt        (20)      159 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/MANIFEST.in
--rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-05-22 08:14:36.604651 djangocms_blog_agenda-0.6.1/PKG-INFO
--rw-r--r--   0 kapt       (501) kapt        (20)     2682 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/README.md
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:14:36.598651 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/__init__.py
--rw-r--r--   0 kapt       (501) kapt        (20)     4389 2023-05-25 06:47:09.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/admin.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1746 2023-03-31 09:10:44.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/apps.py
--rw-r--r--   0 kapt       (501) kapt        (20)     4101 2024-05-22 08:04:25.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/cms_plugins.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:14:36.593651 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/locale/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:14:36.593651 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/locale/fr/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:14:36.601651 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt       (501) kapt        (20)     2229 2024-05-22 08:01:11.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt       (501) kapt        (20)     3599 2024-05-22 08:01:04.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:14:36.602651 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/
--rw-r--r--   0 kapt       (501) kapt        (20)     1076 2023-03-30 10:38:48.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/0001_initial.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1139 2023-03-30 14:50:16.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
--rw-r--r--   0 kapt       (501) kapt        (20)      746 2023-11-13 16:05:40.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py
--rw-r--r--   0 kapt       (501) kapt        (20)      651 2023-12-12 08:49:47.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py
--rw-r--r--   0 kapt       (501) kapt        (20)     3272 2024-05-22 08:13:48.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/0005_auto_20240521_1359.py
--rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/__init__.py
--rw-r--r--   0 kapt       (501) kapt        (20)      951 2024-04-18 15:57:53.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/misc.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1380 2024-05-22 08:04:25.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/models.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1117 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/patched_urls.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:14:36.593651 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:14:36.603651 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501) kapt        (20)     1341 2023-03-30 10:37:22.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
--rw-r--r--   0 kapt       (501) kapt        (20)     1742 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
--rw-r--r--   0 kapt       (501) kapt        (20)     1361 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
--rw-r--r--   0 kapt       (501) kapt        (20)     1889 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
--rw-r--r--   0 kapt       (501) kapt        (20)     2549 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/views.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 08:14:36.603651 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda.egg-info/
--rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-05-22 08:14:36.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda.egg-info/PKG-INFO
--rw-r--r--   0 kapt       (501) kapt        (20)     1282 2024-05-22 08:14:36.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda.egg-info/SOURCES.txt
--rw-r--r--   0 kapt       (501) kapt        (20)        1 2024-05-22 08:14:36.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda.egg-info/dependency_links.txt
--rw-r--r--   0 kapt       (501) kapt        (20)       15 2024-05-22 08:14:36.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda.egg-info/requires.txt
--rw-r--r--   0 kapt       (501) kapt        (20)       22 2024-05-22 08:14:36.000000 djangocms_blog_agenda-0.6.1/djangocms_blog_agenda.egg-info/top_level.txt
--rw-r--r--   0 kapt       (501) kapt        (20)      786 2024-05-22 08:14:36.605651 djangocms_blog_agenda-0.6.1/setup.cfg
--rw-r--r--   0 kapt       (501) kapt        (20)       53 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.1/setup.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 14:12:16.028695 djangocms_blog_agenda-0.6.2/
+-rw-r--r--   0 kapt       (501) kapt        (20)       45 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/AUTHORS.md
+-rw-r--r--   0 kapt       (501) kapt        (20)     1318 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 kapt       (501) kapt        (20)    35149 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/LICENSE
+-rw-r--r--   0 kapt       (501) kapt        (20)      159 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/MANIFEST.in
+-rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-05-22 14:12:16.028695 djangocms_blog_agenda-0.6.2/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)     2682 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/README.md
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 14:12:16.021695 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     4389 2023-05-25 06:47:09.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/admin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1746 2023-03-31 09:10:44.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/apps.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     4035 2024-05-22 14:08:57.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/cms_plugins.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 14:12:16.014695 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/locale/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 14:12:16.014695 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/locale/fr/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 14:12:16.024695 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt       (501) kapt        (20)     2229 2024-05-22 08:01:11.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt       (501) kapt        (20)     3599 2024-05-22 08:01:04.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 14:12:16.026695 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/
+-rw-r--r--   0 kapt       (501) kapt        (20)     1076 2023-03-30 10:38:48.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0001_initial.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1139 2023-03-30 14:50:16.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      746 2023-11-13 16:05:40.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      651 2023-12-12 08:49:47.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     5530 2024-05-22 14:11:29.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0005_latestpostsplugin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      445 2024-05-22 14:11:28.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0006_rename.py
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      951 2024-04-18 15:57:53.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/misc.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     2977 2024-05-22 14:11:29.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/models.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1117 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/patched_urls.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 14:12:16.015695 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 14:12:16.027695 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501) kapt        (20)     1341 2023-03-30 10:37:22.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     1742 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     1361 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     1889 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     2549 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/views.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-22 14:12:16.028695 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda.egg-info/
+-rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-05-22 14:12:16.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda.egg-info/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)     1329 2024-05-22 14:12:16.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)        1 2024-05-22 14:12:16.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       15 2024-05-22 14:12:16.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda.egg-info/requires.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       22 2024-05-22 14:12:16.000000 djangocms_blog_agenda-0.6.2/djangocms_blog_agenda.egg-info/top_level.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)      786 2024-05-22 14:12:16.029695 djangocms_blog_agenda-0.6.2/setup.cfg
+-rw-r--r--   0 kapt       (501) kapt        (20)       53 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.6.2/setup.py
```

### Comparing `djangocms_blog_agenda-0.6.1/CONTRIBUTING.md` & `djangocms_blog_agenda-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/LICENSE` & `djangocms_blog_agenda-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/PKG-INFO` & `djangocms_blog_agenda-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.6.1
+Version: 0.6.2
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms_blog_agenda-0.6.1/README.md` & `djangocms_blog_agenda-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/admin.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/apps.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/cms_plugins.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/cms_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,15 @@
         fields.insert(2, "show_until_event_end")
         return fields
 
     def get_posts(self, instance, request, published_only=True):
         posts = instance.post_queryset(request, published_only)
 
         # Keep only posts with an event date in the futur
-        filters = Q(extension__event_end_date__isnull=True) & Q(
-            extension__event_start_date__gte=timezone.now()
-        )
+        filters = Q(extension__event_start_date__gte=timezone.now())
 
         if instance.show_until_event_end:
             filters |= Q(extension__event_end_date__isnull=False) & Q(
                 extension__event_end_date__gte=timezone.now()
             )
 
         posts = posts.order_by("extension__event_start_date").filter(filters)
```

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/0001_initial.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/misc.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/misc.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/patched_urls.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/patched_urls.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda/views.py` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda/views.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda.egg-info/PKG-INFO` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.6.1
+Version: 0.6.2
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms_blog_agenda-0.6.1/djangocms_blog_agenda.egg-info/SOURCES.txt` & `djangocms_blog_agenda-0.6.2/djangocms_blog_agenda.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,13 +20,14 @@
 djangocms_blog_agenda.egg-info/top_level.txt
 djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
 djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
 djangocms_blog_agenda/migrations/0001_initial.py
 djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
 djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py
 djangocms_blog_agenda/migrations/0004_pasteventsplugin.py
-djangocms_blog_agenda/migrations/0005_auto_20240521_1359.py
+djangocms_blog_agenda/migrations/0005_latestpostsplugin.py
+djangocms_blog_agenda/migrations/0006_rename.py
 djangocms_blog_agenda/migrations/__init__.py
 djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
 djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
 djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
 djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
```

### Comparing `djangocms_blog_agenda-0.6.1/setup.cfg` & `djangocms_blog_agenda-0.6.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangocms-blog-agenda
-version = 0.6.1
+version = 0.6.2
 description = Create an agenda on top of djangocms-blog!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 author = Corentin Bettiol
 author_email = dev@kapt.mobi
 classifiers =
```

