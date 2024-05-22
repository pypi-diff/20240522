# Comparing `tmp/netbox-nas-1.0.1.tar.gz` & `tmp/netbox_nas-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-nas-1.0.1.tar", last modified: Wed Aug 30 21:09:43 2023, max compression
+gzip compressed data, was "netbox_nas-1.0.2.tar", last modified: Wed May 22 15:53:40 2024, max compression
```

## Comparing `netbox-nas-1.0.1.tar` & `netbox_nas-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 21:09:43.584297 netbox-nas-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (999)       46 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)      740 2023-08-30 21:09:43.584297 netbox-nas-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      609 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 21:09:43.580297 netbox-nas-1.0.1/netbox_nas/
--rw-r--r--   0 runner    (1001) docker     (999)      276 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 21:09:43.584297 netbox-nas-1.0.1/netbox_nas/api/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5708 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (999)      355 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (999)     1085 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/api/views.py
--rw-r--r--   0 runner    (1001) docker     (999)      995 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (999)     4753 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 21:09:43.584297 netbox-nas-1.0.1/netbox_nas/migrations/
--rw-r--r--   0 runner    (1001) docker     (999)     7432 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6506 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/models.py
--rw-r--r--   0 runner    (1001) docker     (999)     1505 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/navigation.py
--rw-r--r--   0 runner    (1001) docker     (999)      969 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/search.py
--rw-r--r--   0 runner    (1001) docker     (999)     2400 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 21:09:43.580297 netbox-nas-1.0.1/netbox_nas/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 21:09:43.584297 netbox-nas-1.0.1/netbox_nas/templates/netbox_nas/
--rw-r--r--   0 runner    (1001) docker     (999)     1766 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/templates/netbox_nas/nascluster.html
--rw-r--r--   0 runner    (1001) docker     (999)     1857 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/templates/netbox_nas/nasmount.html
--rw-r--r--   0 runner    (1001) docker     (999)     2426 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/templates/netbox_nas/nasshare.html
--rw-r--r--   0 runner    (1001) docker     (999)     2421 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/templates/netbox_nas/nasvolume.html
--rw-r--r--   0 runner    (1001) docker     (999)     3610 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/urls.py
--rw-r--r--   0 runner    (1001) docker     (999)     4854 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/netbox_nas/views.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 21:09:43.584297 netbox-nas-1.0.1/netbox_nas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      740 2023-08-30 21:09:43.000000 netbox-nas-1.0.1/netbox_nas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      757 2023-08-30 21:09:43.000000 netbox-nas-1.0.1/netbox_nas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 21:09:43.000000 netbox-nas-1.0.1/netbox_nas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 21:09:43.000000 netbox-nas-1.0.1/netbox_nas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-30 21:09:43.000000 netbox-nas-1.0.1/netbox_nas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-30 21:09:43.584297 netbox-nas-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      353 2023-08-30 21:09:32.000000 netbox-nas-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.442907 netbox_nas-1.0.2/netbox_nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.442907 netbox_nas-1.0.2/netbox_nas/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.442907 netbox_nas-1.0.2/netbox_nas/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.438907 netbox_nas-1.0.2/netbox_nas/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nascluster.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasmount.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasshare.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasvolume.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/netbox_nas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/setup.py
```

### Comparing `netbox-nas-1.0.1/PKG-INFO` & `netbox_nas-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-nas
-Version: 1.0.1
+Version: 1.0.2
 Summary: Add NAS entities to NetBox
 Description-Content-Type: text/markdown
 
 ## netbox-nas
 
 A plugin to enable managment of NAS resources.
```

### Comparing `netbox-nas-1.0.1/README.md` & `netbox_nas-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/api/serializers.py` & `netbox_nas-1.0.2/netbox_nas/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/api/views.py` & `netbox_nas-1.0.2/netbox_nas/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/filtersets.py` & `netbox_nas-1.0.2/netbox_nas/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/forms.py` & `netbox_nas-1.0.2/netbox_nas/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/migrations/0001_initial.py` & `netbox_nas-1.0.2/netbox_nas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/models.py` & `netbox_nas-1.0.2/netbox_nas/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from django.contrib.contenttypes.fields import GenericRelation
 from django.contrib.postgres.fields import ArrayField
 from django.db import models
 from django.urls import reverse
 from netbox.models import NetBoxModel
+from netbox.models.features import ContactsMixin
 from tenancy.models import Tenant, ContactAssignment
 from ipam.models import Prefix, IPAddress
 from dcim.models import Device
 from utilities.choices import ChoiceSet
 from utilities.forms.fields import CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField
 
 class NASVolumeSecurityStyleChoices(ChoiceSet):
@@ -25,15 +25,15 @@
 
 class NASShareAccessLevelChoices(ChoiceSet):
     CHOICES = [
         ('rw', 'Read/Write'),
         ('ro', 'Read-Only'),
     ]
 
-class NASCluster(NetBoxModel):
+class NASCluster(ContactsMixin, NetBoxModel):
     name = models.CharField(
         max_length=100,
         unique=True
     )
 
     devices = models.ManyToManyField(
         to='dcim.Device',
@@ -54,18 +54,14 @@
         blank=True
     )
 
     comments = models.TextField(
         blank=True
     )
 
-    contacts = GenericRelation(
-        to=ContactAssignment
-    )
-
     tenant = models.ForeignKey(
         to=Tenant,
         on_delete=models.PROTECT,
         related_name='nas_clusters',
         blank = True,
         null = True
     )
@@ -75,15 +71,15 @@
 
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_nas:nascluster', args=[self.pk])
 
-class NASVolume(NetBoxModel):
+class NASVolume(ContactsMixin, NetBoxModel):
     nas_cluster = models.ForeignKey(
         to=NASCluster,
         on_delete=models.PROTECT,
         related_name='volumes'
     )
 
     name = models.CharField(
@@ -122,18 +118,14 @@
         blank=True
     )
 
     comments = models.TextField(
         blank=True
     )
 
-    contacts = GenericRelation(
-        to=ContactAssignment
-    )
-
     tenant = models.ForeignKey(
         to=Tenant,
         on_delete=models.PROTECT,
         related_name='nas_volumes',
         blank = True,
         null = True
     )
@@ -147,15 +139,15 @@
 
     def __str__(self):
         return f'{self.nas_cluster}: {self.local_directory}'
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_nas:nasvolume', args=[self.pk])
 
-class NASShare(NetBoxModel):
+class NASShare(ContactsMixin, NetBoxModel):
     nas_volume = models.ForeignKey(
         to=NASVolume,
         on_delete=models.PROTECT,
         related_name='shares'
     )
 
     name = models.CharField(
@@ -202,18 +194,14 @@
         blank=True
     )
 
     comments = models.TextField(
         blank=True
     )
 
-    contacts = GenericRelation(
-        to=ContactAssignment
-    )
-
     tenant = models.ForeignKey(
         to=Tenant,
         on_delete=models.PROTECT,
         related_name='nas_shares',
         blank = True,
         null = True
     )
@@ -224,15 +212,15 @@
 
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_nas:nasshare', args=[self.pk])
 
-class NASMount(NetBoxModel):
+class NASMount(ContactsMixin, NetBoxModel):
     nas_share = models.ForeignKey(
         to=NASShare,
         on_delete=models.PROTECT,
         related_name='mounts'
     )
 
     devices = models.ManyToManyField(
@@ -263,18 +251,14 @@
         blank=True
     )
 
     comments = models.TextField(
         blank=True
     )
 
-    contacts = GenericRelation(
-        to=ContactAssignment
-    )
-
     tenant = models.ForeignKey(
         to=Tenant,
         on_delete=models.PROTECT,
         related_name='nas_mounts',
         blank = True,
         null = True
     )
```

### Comparing `netbox-nas-1.0.1/netbox_nas/search.py` & `netbox_nas-1.0.2/netbox_nas/search.py`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/tables.py` & `netbox_nas-1.0.2/netbox_nas/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/templates/netbox_nas/nascluster.html` & `netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nascluster.html`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/templates/netbox_nas/nasmount.html` & `netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasmount.html`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/templates/netbox_nas/nasshare.html` & `netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasshare.html`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/templates/netbox_nas/nasvolume.html` & `netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasvolume.html`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/urls.py` & `netbox_nas-1.0.2/netbox_nas/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas/views.py` & `netbox_nas-1.0.2/netbox_nas/views.py`

 * *Files identical despite different names*

### Comparing `netbox-nas-1.0.1/netbox_nas.egg-info/PKG-INFO` & `netbox_nas-1.0.2/netbox_nas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-nas
-Version: 1.0.1
+Version: 1.0.2
 Summary: Add NAS entities to NetBox
 Description-Content-Type: text/markdown
 
 ## netbox-nas
 
 A plugin to enable managment of NAS resources.
```

### Comparing `netbox-nas-1.0.1/netbox_nas.egg-info/SOURCES.txt` & `netbox_nas-1.0.2/netbox_nas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

