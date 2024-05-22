# Comparing `tmp/django_post_deploy-2.3.1.tar.gz` & `tmp/django_post_deploy-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_post_deploy-2.3.1.tar", last modified: Thu Jan 12 14:26:52 2023, max compression
+gzip compressed data, was "django_post_deploy-2.4.0.tar", last modified: Wed May 22 14:27:04 2024, max compression
```

## Comparing `django_post_deploy-2.3.1.tar` & `django_post_deploy-2.4.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.026335 django_post_deploy-2.3.1/
--rw-r--r--   0 erlend     (501) staff       (20)      237 2022-05-22 19:01:38.000000 django_post_deploy-2.3.1/MANIFEST.in
--rw-r--r--   0 erlend     (501) staff       (20)     6690 2023-01-12 14:26:52.026455 django_post_deploy-2.3.1/PKG-INFO
--rw-r--r--   0 erlend     (501) staff       (20)     6033 2022-11-10 09:37:22.000000 django_post_deploy-2.3.1/README.md
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.016533 django_post_deploy-2.3.1/django_post_deploy.egg-info/
--rw-r--r--   0 erlend     (501) staff       (20)     6690 2023-01-12 14:26:51.000000 django_post_deploy-2.3.1/django_post_deploy.egg-info/PKG-INFO
--rw-r--r--   0 erlend     (501) staff       (20)      913 2023-01-12 14:26:51.000000 django_post_deploy-2.3.1/django_post_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 erlend     (501) staff       (20)        1 2023-01-12 14:26:51.000000 django_post_deploy-2.3.1/django_post_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 erlend     (501) staff       (20)        7 2023-01-12 14:26:51.000000 django_post_deploy-2.3.1/django_post_deploy.egg-info/requires.txt
--rw-r--r--   0 erlend     (501) staff       (20)       12 2023-01-12 14:26:51.000000 django_post_deploy-2.3.1/django_post_deploy.egg-info/top_level.txt
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.020391 django_post_deploy-2.3.1/post_deploy/
--rw-r--r--   0 erlend     (501) staff       (20)    20137 2022-05-22 19:24:58.000000 django_post_deploy-2.3.1/post_deploy/LICENSE.txt
--rw-r--r--   0 erlend     (501) staff       (20)       82 2023-01-12 14:25:13.000000 django_post_deploy-2.3.1/post_deploy/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)       56 2022-05-16 18:03:30.000000 django_post_deploy-2.3.1/post_deploy/errors.py
--rw-r--r--   0 erlend     (501) staff       (20)     2120 2022-11-10 14:42:25.000000 django_post_deploy-2.3.1/post_deploy/local_utils.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.012385 django_post_deploy-2.3.1/post_deploy/management/
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.020827 django_post_deploy-2.3.1/post_deploy/management/commands/
--rw-r--r--   0 erlend     (501) staff       (20)     6796 2022-11-15 16:20:58.000000 django_post_deploy-2.3.1/post_deploy/management/commands/deploy.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.022276 django_post_deploy-2.3.1/post_deploy/migrations/
--rw-r--r--   0 erlend     (501) staff       (20)     1122 2022-05-20 21:04:36.000000 django_post_deploy-2.3.1/post_deploy/migrations/0001_initial.py
--rw-r--r--   0 erlend     (501) staff       (20)     1870 2023-01-12 14:25:13.000000 django_post_deploy-2.3.1/post_deploy/migrations/0002_postdeploylog.py
--rw-r--r--   0 erlend     (501) staff       (20)        0 2022-05-16 18:03:30.000000 django_post_deploy-2.3.1/post_deploy/migrations/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)     4533 2022-11-15 16:20:58.000000 django_post_deploy-2.3.1/post_deploy/models.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.022503 django_post_deploy-2.3.1/post_deploy/plugins/
--rw-r--r--   0 erlend     (501) staff       (20)        0 2022-05-16 18:11:09.000000 django_post_deploy-2.3.1/post_deploy/plugins/__init__.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.023198 django_post_deploy-2.3.1/post_deploy/plugins/context/
--rw-r--r--   0 erlend     (501) staff       (20)      280 2022-05-20 20:10:51.000000 django_post_deploy-2.3.1/post_deploy/plugins/context/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)      438 2022-05-20 21:02:34.000000 django_post_deploy-2.3.1/post_deploy/plugins/context/tenant.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.024232 django_post_deploy-2.3.1/post_deploy/plugins/scheduler/
--rw-r--r--   0 erlend     (501) staff       (20)      291 2022-11-10 09:28:43.000000 django_post_deploy-2.3.1/post_deploy/plugins/scheduler/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)     1312 2022-11-10 09:28:43.000000 django_post_deploy-2.3.1/post_deploy/plugins/scheduler/celery.py
--rw-r--r--   0 erlend     (501) staff       (20)      369 2022-11-10 09:28:43.000000 django_post_deploy-2.3.1/post_deploy/tasks.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2023-01-12 14:26:52.025951 django_post_deploy-2.3.1/post_deploy/tests/
--rw-r--r--   0 erlend     (501) staff       (20)        0 2022-05-22 18:25:46.000000 django_post_deploy-2.3.1/post_deploy/tests/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)     2472 2022-11-10 09:28:43.000000 django_post_deploy-2.3.1/post_deploy/tests/test_decorator.py
--rw-r--r--   0 erlend     (501) staff       (20)     5323 2022-11-15 16:29:32.000000 django_post_deploy-2.3.1/post_deploy/tests/test_log_queryset.py
--rw-r--r--   0 erlend     (501) staff       (20)     7158 2022-11-15 07:58:12.000000 django_post_deploy-2.3.1/post_deploy/tests/test_management_command.py
--rw-r--r--   0 erlend     (501) staff       (20)     1665 2022-11-15 16:23:36.000000 django_post_deploy-2.3.1/post_deploy/utils.py
--rw-r--r--   0 erlend     (501) staff       (20)       79 2023-01-12 14:26:52.026843 django_post_deploy-2.3.1/setup.cfg
--rw-r--r--   0 erlend     (501) staff       (20)     1075 2022-05-21 22:05:12.000000 django_post_deploy-2.3.1/setup.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.303012 django_post_deploy-2.4.0/
+-rw-r--r--   0 erlend     (501) staff       (20)      237 2024-05-22 13:15:43.000000 django_post_deploy-2.4.0/MANIFEST.in
+-rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-22 14:27:04.302965 django_post_deploy-2.4.0/PKG-INFO
+-rw-r--r--   0 erlend     (501) staff       (20)     5701 2024-05-22 13:17:21.000000 django_post_deploy-2.4.0/README.md
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.302747 django_post_deploy-2.4.0/django_post_deploy.egg-info/
+-rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-22 14:27:04.000000 django_post_deploy-2.4.0/django_post_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 erlend     (501) staff       (20)      935 2024-05-22 14:27:04.000000 django_post_deploy-2.4.0/django_post_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 erlend     (501) staff       (20)        1 2024-05-22 14:27:04.000000 django_post_deploy-2.4.0/django_post_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 erlend     (501) staff       (20)        7 2024-05-22 14:27:04.000000 django_post_deploy-2.4.0/django_post_deploy.egg-info/requires.txt
+-rw-r--r--   0 erlend     (501) staff       (20)       12 2024-05-22 14:27:04.000000 django_post_deploy-2.4.0/django_post_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.301087 django_post_deploy-2.4.0/post_deploy/
+-rw-r--r--   0 erlend     (501) staff       (20)    20137 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/LICENSE.txt
+-rw-r--r--   0 erlend     (501) staff       (20)      121 2024-05-22 14:17:09.000000 django_post_deploy-2.4.0/post_deploy/README.md
+-rw-r--r--   0 erlend     (501) staff       (20)       82 2024-05-22 13:08:35.000000 django_post_deploy-2.4.0/post_deploy/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)       56 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/errors.py
+-rw-r--r--   0 erlend     (501) staff       (20)     2120 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/local_utils.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.298861 django_post_deploy-2.4.0/post_deploy/management/
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.301191 django_post_deploy-2.4.0/post_deploy/management/commands/
+-rw-r--r--   0 erlend     (501) staff       (20)     6666 2024-05-22 13:04:35.000000 django_post_deploy-2.4.0/post_deploy/management/commands/deploy.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.301602 django_post_deploy-2.4.0/post_deploy/migrations/
+-rw-r--r--   0 erlend     (501) staff       (20)     1123 2024-05-22 13:04:35.000000 django_post_deploy-2.4.0/post_deploy/migrations/0001_initial.py
+-rw-r--r--   0 erlend     (501) staff       (20)     1871 2024-05-22 13:04:35.000000 django_post_deploy-2.4.0/post_deploy/migrations/0002_postdeploylog.py
+-rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/migrations/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)     4533 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/models.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.301681 django_post_deploy-2.4.0/post_deploy/plugins/
+-rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/plugins/__init__.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.301873 django_post_deploy-2.4.0/post_deploy/plugins/context/
+-rw-r--r--   0 erlend     (501) staff       (20)      280 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/plugins/context/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)      439 2024-05-22 13:04:35.000000 django_post_deploy-2.4.0/post_deploy/plugins/context/tenant.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.302081 django_post_deploy-2.4.0/post_deploy/plugins/scheduler/
+-rw-r--r--   0 erlend     (501) staff       (20)      291 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/plugins/scheduler/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)     1311 2024-05-22 13:04:35.000000 django_post_deploy-2.4.0/post_deploy/plugins/scheduler/celery.py
+-rw-r--r--   0 erlend     (501) staff       (20)      369 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/tasks.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 14:27:04.302557 django_post_deploy-2.4.0/post_deploy/tests/
+-rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/tests/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)     2472 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/tests/test_decorator.py
+-rw-r--r--   0 erlend     (501) staff       (20)     5323 2024-05-22 12:55:59.000000 django_post_deploy-2.4.0/post_deploy/tests/test_log_queryset.py
+-rw-r--r--   0 erlend     (501) staff       (20)     7172 2024-05-22 13:04:35.000000 django_post_deploy-2.4.0/post_deploy/tests/test_management_command.py
+-rw-r--r--   0 erlend     (501) staff       (20)     2091 2024-05-22 13:04:35.000000 django_post_deploy-2.4.0/post_deploy/utils.py
+-rw-r--r--   0 erlend     (501) staff       (20)       76 2024-05-22 14:27:04.303209 django_post_deploy-2.4.0/setup.cfg
+-rw-r--r--   0 erlend     (501) staff       (20)     1045 2024-05-22 14:15:07.000000 django_post_deploy-2.4.0/setup.py
```

### Comparing `django_post_deploy-2.3.1/PKG-INFO` & `django_post_deploy-2.4.0/django_post_deploy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: django_post_deploy
-Version: 2.3.1
+Name: django-post-deploy
+Version: 2.4.0
 Summary: A generic way to have post-deploy actions done.
 Home-page: https://github.com/erlendgit/django_post_deploy
+Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.0.tar.gz
 Author: Erlend ter Maat
 Author-email: erwitema@gmail.com
 License: cc-by-4.0
-Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.3.1.tar.gz
 Keywords: Django,Deployment,Management,CLI
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Requires-Dist: Django
 
 Django Post Deploy
 ===
 
 This module adds a way automate release-specific post-deploy/post-migrate actions to your Django project.
 
 ### Features
@@ -198,21 +198,14 @@
         # Do 'public' specific operations.
         pass
 
     # else, proceed as required.
     ...
 ```
 
-## Technical details
-
-* This module provides a model, and therefore require a common relational database to be installed. There are however no relations between multiple models in
-  this module, so it may be possible that it works with a non-relational database too. But it is not tested in non-relational database configurations.
-
 ## License information
 
 django_post_deploy (c) by Erlend ter Maat
 
 django_post_deploy is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.
 
 You should have received a copy of the license along with this work. If not, see <http://creativecommons.org/licenses/by-sa/4.0/>.
-
-
```

### Comparing `django_post_deploy-2.3.1/README.md` & `django_post_deploy-2.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -181,19 +181,14 @@
         # Do 'public' specific operations.
         pass
 
     # else, proceed as required.
     ...
 ```
 
-## Technical details
-
-* This module provides a model, and therefore require a common relational database to be installed. There are however no relations between multiple models in
-  this module, so it may be possible that it works with a non-relational database too. But it is not tested in non-relational database configurations.
-
 ## License information
 
 django_post_deploy (c) by Erlend ter Maat
 
 django_post_deploy is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.
 
 You should have received a copy of the license along with this work. If not, see <http://creativecommons.org/licenses/by-sa/4.0/>.
```

### Comparing `django_post_deploy-2.3.1/django_post_deploy.egg-info/PKG-INFO` & `django_post_deploy-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: django-post-deploy
-Version: 2.3.1
+Name: django_post_deploy
+Version: 2.4.0
 Summary: A generic way to have post-deploy actions done.
 Home-page: https://github.com/erlendgit/django_post_deploy
+Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.0.tar.gz
 Author: Erlend ter Maat
 Author-email: erwitema@gmail.com
 License: cc-by-4.0
-Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.3.1.tar.gz
 Keywords: Django,Deployment,Management,CLI
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Requires-Dist: Django
 
 Django Post Deploy
 ===
 
 This module adds a way automate release-specific post-deploy/post-migrate actions to your Django project.
 
 ### Features
@@ -198,21 +198,14 @@
         # Do 'public' specific operations.
         pass
 
     # else, proceed as required.
     ...
 ```
 
-## Technical details
-
-* This module provides a model, and therefore require a common relational database to be installed. There are however no relations between multiple models in
-  this module, so it may be possible that it works with a non-relational database too. But it is not tested in non-relational database configurations.
-
 ## License information
 
 django_post_deploy (c) by Erlend ter Maat
 
 django_post_deploy is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.
 
 You should have received a copy of the license along with this work. If not, see <http://creativecommons.org/licenses/by-sa/4.0/>.
-
-
```

### Comparing `django_post_deploy-2.3.1/django_post_deploy.egg-info/SOURCES.txt` & `django_post_deploy-2.4.0/django_post_deploy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 django_post_deploy.egg-info/PKG-INFO
 django_post_deploy.egg-info/SOURCES.txt
 django_post_deploy.egg-info/dependency_links.txt
 django_post_deploy.egg-info/requires.txt
 django_post_deploy.egg-info/top_level.txt
 post_deploy/LICENSE.txt
+post_deploy/README.md
 post_deploy/__init__.py
 post_deploy/errors.py
 post_deploy/local_utils.py
 post_deploy/models.py
 post_deploy/tasks.py
 post_deploy/utils.py
 post_deploy/management/commands/deploy.py
```

### Comparing `django_post_deploy-2.3.1/post_deploy/LICENSE.txt` & `django_post_deploy-2.4.0/post_deploy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.3.1/post_deploy/local_utils.py` & `django_post_deploy-2.4.0/post_deploy/local_utils.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.3.1/post_deploy/management/commands/deploy.py` & `django_post_deploy-2.4.0/post_deploy/management/commands/deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from django.core.management.base import BaseCommand
 from django.utils import timezone
 from django.utils.timezone import get_current_timezone as ltz
 
-from post_deploy.local_utils import initialize_actions, get_context_manager, get_scheduler_manager, model_ok
-
+from post_deploy.local_utils import (get_context_manager,
+                                     get_scheduler_manager, initialize_actions,
+                                     model_ok)
 from post_deploy.models import PostDeployLog
+from post_deploy.utils import run_task
 
 
 def strftime(datetime: timezone.datetime):
     return datetime.astimezone(ltz()).strftime("%Y-%m-%d %H:%M")
 
 
 class Command(BaseCommand):
@@ -148,11 +150,9 @@
                 actions.append(name)
 
         if len(actions) == 0:
             self.stdout.write(f"No actions scheduled.")
             return
 
         for import_name in actions:
-            action_log = PostDeployLog.objects.register_action(import_name)
-            task_id = get_scheduler_manager().schedule([action_log], self.context_manager.default_parameters())
-            PostDeployLog.objects.filter(import_name=import_name).update(task_id=task_id)
+            run_task(import_name)
             self.stdout.write(f"Scheduled {import_name}")
```

### Comparing `django_post_deploy-2.3.1/post_deploy/migrations/0001_initial.py` & `django_post_deploy-2.4.0/post_deploy/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Generated by Django 4.0.4 on 2022-05-20 21:04
 
-from django.db import migrations, models
 import uuid
 
+from django.db import migrations, models
+
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
     ]
```

### Comparing `django_post_deploy-2.3.1/post_deploy/migrations/0002_postdeploylog.py` & `django_post_deploy-2.4.0/post_deploy/migrations/0002_postdeploylog.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 4.0.4 on 2022-11-07 16:19
 
-from django.db import migrations, models
-import django.utils.timezone
 import uuid
 
+import django.utils.timezone
+from django.db import migrations, models
+
 
 def library_to_id(key):
     module, method = key.split('.')
     class_path = '.'.join([module, 'post_deploy', method])
     return class_path
```

### Comparing `django_post_deploy-2.3.1/post_deploy/models.py` & `django_post_deploy-2.4.0/post_deploy/models.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.3.1/post_deploy/plugins/scheduler/celery.py` & `django_post_deploy-2.4.0/post_deploy/plugins/scheduler/celery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from celery import Celery
 from celery.result import AsyncResult
-
 from django.conf import settings
 from django.utils.module_loading import import_string
 
 from post_deploy.errors import PostDeployConfigurationError
 from post_deploy.plugins.scheduler import DefaultScheduler
```

### Comparing `django_post_deploy-2.3.1/post_deploy/tests/test_decorator.py` & `django_post_deploy-2.4.0/post_deploy/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.3.1/post_deploy/tests/test_log_queryset.py` & `django_post_deploy-2.4.0/post_deploy/tests/test_log_queryset.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.3.1/post_deploy/tests/test_management_command.py` & `django_post_deploy-2.4.0/post_deploy/tests/test_management_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import uuid
 from unittest import mock
 
 from django.test.testcases import TestCase
 from django.utils import timezone
 
+from post_deploy.local_utils import get_context_manager
 from post_deploy.models import PostDeployLog
 from post_deploy.plugins.scheduler import DefaultScheduler
-from post_deploy.local_utils import get_context_manager
 
 
 class TestManagementCommandTestCase(TestCase):
     def setUp(self):
         super().setUp()
 
         self.initialize_actions = mock.patch("post_deploy.management.commands.deploy.initialize_actions").start()
@@ -53,15 +53,16 @@
             started_at=timezone.localtime(),
         )
         PostDeployLog.objects.create(
             import_name='custom_still_running_action',
             started_at=timezone.localtime(),
         )
 
-        from post_deploy.management.commands.deploy import Command as DeployCommand
+        from post_deploy.management.commands.deploy import \
+            Command as DeployCommand
         self.command = DeployCommand()
         self.command.stdout = mock.MagicMock()
         self.command.stderr = mock.MagicMock()
 
     def tearDown(self):
         mock.patch.stopall()
         super().tearDown()
```

### Comparing `django_post_deploy-2.3.1/post_deploy/utils.py` & `django_post_deploy-2.4.0/post_deploy/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from collections import OrderedDict
-from functools import update_wrapper, partial
+from functools import partial, update_wrapper
 from inspect import isfunction
 
+from django.utils.translation import gettext as _
+
 
 class register_post_deploy():
     bindings = OrderedDict()
 
     decorated = None
 
     def __init__(self, *args, **kwargs):
@@ -42,13 +44,21 @@
         register_post_deploy.bindings[key] = {
             "auto": self.auto,
             "description": self.description,
         }
 
 
 def skip_all_tasks(reason):
-    from post_deploy.models import PostDeployLog
     from post_deploy.local_utils import initialize_actions
+    from post_deploy.models import PostDeployLog
 
     actions = initialize_actions()
     for import_name in actions.keys():
         PostDeployLog.objects.skip_action(import_name, reason)
+
+
+def run_task(import_name):
+    assert not PostDeployLog.objects.is_running(import_name), _("Task is already running")
+
+    action_log = PostDeployLog.objects.register_action(import_name)
+    task_id = get_scheduler_manager().schedule([action_log], self.context_manager.default_parameters())
+    PostDeployLog.objects.filter(import_name=import_name).update(task_id=task_id)
```

### Comparing `django_post_deploy-2.3.1/setup.py` & `django_post_deploy-2.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import io
 from distutils.core import setup
 from os.path import exists
 
 from setuptools import find_packages
+
 from post_deploy import VERSION
 
 setup(
-    name='django_post_deploy',
     packages=find_packages(),
     version=VERSION[1:],
     license='cc-by-4.0',
     description='A generic way to have post-deploy actions done.',
     long_description=io.open("README.md", encoding='utf-8').read() if exists("README.md") else "",
     long_description_content_type='text/markdown',
     author='Erlend ter Maat',
```

