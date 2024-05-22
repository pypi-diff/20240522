# Comparing `tmp/django-model-helper-0.1.0.tar.gz` & `tmp/django-model-helper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-model-helper-0.1.0.tar", last modified: Fri Apr  5 00:45:16 2024, max compression
+gzip compressed data, was "django-model-helper-0.1.5.tar", last modified: Wed May 22 12:52:40 2024, max compression
```

## Comparing `django-model-helper-0.1.0.tar` & `django-model-helper-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-05 00:45:16.098592 django-model-helper-0.1.0/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-05 00:44:55.000000 django-model-helper-0.1.0/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      209 2024-04-04 12:16:10.000000 django-model-helper-0.1.0/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)      971 2024-04-05 00:45:16.098474 django-model-helper-0.1.0/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      403 2024-04-04 12:04:32.000000 django-model-helper-0.1.0/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-05 00:45:16.097464 django-model-helper-0.1.0/django_model_helper/
--rw-r--r--   0 test       (501) staff       (20)       45 2024-04-04 08:30:52.000000 django-model-helper-0.1.0/django_model_helper/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-04-04 03:34:59.000000 django-model-helper-0.1.0/django_model_helper/admin.py
--rw-r--r--   0 test       (501) staff       (20)      168 2024-04-04 03:34:59.000000 django-model-helper-0.1.0/django_model_helper/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-05 00:45:16.098312 django-model-helper-0.1.0/django_model_helper/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-04-04 03:34:59.000000 django-model-helper-0.1.0/django_model_helper/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)    16307 2024-04-04 12:31:03.000000 django-model-helper-0.1.0/django_model_helper/models.py
--rw-r--r--   0 test       (501) staff       (20)       60 2024-04-04 03:34:59.000000 django-model-helper-0.1.0/django_model_helper/tests.py
--rw-r--r--   0 test       (501) staff       (20)       18 2024-04-04 03:38:44.000000 django-model-helper-0.1.0/django_model_helper/version.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-04-04 03:34:59.000000 django-model-helper-0.1.0/django_model_helper/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-05 00:45:16.098186 django-model-helper-0.1.0/django_model_helper.egg-info/
--rw-r--r--   0 test       (501) staff       (20)      971 2024-04-05 00:45:16.000000 django-model-helper-0.1.0/django_model_helper.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      562 2024-04-05 00:45:16.000000 django-model-helper-0.1.0/django_model_helper.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-04-05 00:45:16.000000 django-model-helper-0.1.0/django_model_helper.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-04-05 00:45:16.000000 django-model-helper-0.1.0/django_model_helper.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       75 2024-04-05 00:45:16.000000 django-model-helper-0.1.0/django_model_helper.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       20 2024-04-05 00:45:16.000000 django-model-helper-0.1.0/django_model_helper.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       77 2024-04-04 10:36:00.000000 django-model-helper-0.1.0/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-04-05 00:45:16.098635 django-model-helper-0.1.0/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1439 2024-04-05 00:44:35.000000 django-model-helper-0.1.0/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:52:40.045859 django-model-helper-0.1.5/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-05 00:44:55.000000 django-model-helper-0.1.5/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      209 2024-04-04 12:16:10.000000 django-model-helper-0.1.5/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     1271 2024-05-22 12:52:40.045750 django-model-helper-0.1.5/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      681 2024-05-22 12:28:18.000000 django-model-helper-0.1.5/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:52:40.044836 django-model-helper-0.1.5/django_model_helper/
+-rw-r--r--   0 test       (501) staff       (20)       45 2024-04-04 08:30:52.000000 django-model-helper-0.1.5/django_model_helper/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      168 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:52:40.045613 django-model-helper-0.1.5/django_model_helper/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)    19162 2024-05-20 02:56:28.000000 django-model-helper-0.1.5/django_model_helper/models.py
+-rw-r--r--   0 test       (501) staff       (20)       60 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/tests.py
+-rw-r--r--   0 test       (501) staff       (20)       18 2024-05-20 02:56:37.000000 django-model-helper-0.1.5/django_model_helper/version.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:52:40.045500 django-model-helper-0.1.5/django_model_helper.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     1271 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      562 2024-05-22 12:52:40.000000 django-model-helper-0.1.5/django_model_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       75 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       20 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       77 2024-04-04 10:36:00.000000 django-model-helper-0.1.5/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-22 12:52:40.045899 django-model-helper-0.1.5/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1467 2024-04-05 00:47:30.000000 django-model-helper-0.1.5/setup.py
```

### Comparing `django-model-helper-0.1.0/LICENSE` & `django-model-helper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-model-helper-0.1.0/PKG-INFO` & `django-model-helper-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: django-model-helper
-Version: 0.1.0
+Version: 0.1.5
 Summary: Helpful django abstract models collection.
 Author: Li HuiTao
+Maintainer: Li HuiTao
 License: MIT
 Keywords: django-model-helper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,27 +15,39 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-model-helper
 
 Helpful django abstract models collection.
 
-## Abstract Models
+## 抽象类列表
 
-- WithAddModTimeFields
-- WithConfigFields
-- WithCountFields
-- WithDeletedStatusFields
-- WithDisplayOrderFields
-- WithEnabledStatusFields
-- WithExpireTimeFields
-- WithJsonDataFields
-- WithLockStatusFields
-- WithSimpleResultFields
-- WithSimpleNRRDStatusFields
-- WithUidFields
+1. WithAddModTimeFields
+1. WithConfigFields
+1. WithCountFields
+1. WithDeletedStatusFields
+1. WithDisplayOrderFields
+1. WithEnabledStatusFields
+1. WithExpireTimeFields
+1. WithHotspotFields
+1. WithJsonDataFields
+1. WithLockStatusFields
+1. WithSimpleResultFields
+1. WithSimpleNRRDStatusFields
+1. WithUidFields
+1. WithVisibleFields
 
-## Releases
+## 版本记录
 
 ### v0.1.0
 
-- First release.
+- 版本首发。
+
+### v0.1.1
+
+- WithExpireTimeFields添加default_expires属性。
+- WithUidFields添加uidgen属性，用于生成uid默认值。
+
+### v0.1.5
+
+- 添加WithVisibleFields抽象类。
+- 添加WithHotspotFields抽象类。
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-model-helper-0.1.0/django_model_helper/models.py` & `django-model-helper-0.1.5/django_model_helper/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -270,27 +270,32 @@
     def set_data(self, value):
         self.data_raw = jsonutils.simple_json_dumps(value, ensure_ascii=False)
 
     data = property(get_data, set_data)
 
 
 class WithUidFields(models.Model):
+
     uid = models.CharField(
         max_length=64,
         null=True,
         blank=True,
         verbose_name="唯一码",
     )
 
     class Meta:
         abstract = True
 
+    @classmethod
+    def uidgen(cls):
+        return uuid.uuid4().hex
+
     def save(self, *args, **kwargs):
         if not self.uid:
-            self.uid = str(uuid.uuid4())
+            self.uid = self.uidgen()
         return super().save(*args, **kwargs)
 
 
 class WithSimpleNRRDStatusFields(models.Model):
     """添加简易流程状态。
 
     状态列表：
@@ -548,14 +553,15 @@
             if lock.is_locked:
                 self.count -= delta
                 self.save()
         return self.count
 
 
 class WithExpireTimeFields(models.Model):
+
     EXPIRES_UNIT_SECOND = 10
     EXPIRES_UNIT_MINUTE = 20
     EXPIRES_UNIT_HOUR = 30
     EXPIRES_UNIT_DAY = 40
     EXPIRES_UNITS = [
         (EXPIRES_UNIT_SECOND, "秒"),
         (EXPIRES_UNIT_MINUTE, "分钟"),
@@ -579,33 +585,38 @@
         default=EXPIRES_UNIT_SECOND,
         verbose_name="过期时长单位",
     )
     expire_time = models.DateTimeField(
         null=True,
         blank=True,
         verbose_name="过期时间",
-        help_text="如果未设置过期时间，表示永久有效。",
     )
 
+    default_expires = None
+    default_expires_unit = EXPIRES_UNIT_SECOND
+
     class Meta:
         abstract = True
 
     def clean_expire_time(self, save=True):
         self.expires = None
-        self.expires_unit = self.EXPIRES_UNIT_SECOND
+        self.expires_unit = None
         self.expire_time = None
         if save:
             self.save()
 
-    def set_expire_time(self, expires, expires_unit=None, nowtime=None, save=True):
+    def set_expire_time(self, expires=None, expires_unit=None, nowtime=None, save=True):
         if nowtime is None:
             nowtime = timezone.now()
+        if expires is None:
+            expires = self.default_expires
         if expires_unit is None:
-            self.expires_unit = self.EXPIRES_UNIT_SECOND
+            expires_unit = self.default_expires_unit
         self.expires = expires
+        self.expires_unit = expires_unit
         self.expire_time = nowtime + datetime.timedelta(
             seconds=self.get_expire_seconds()
         )
         if save:
             self.save()
 
     def get_expire_seconds(self):
@@ -617,13 +628,111 @@
         nowtime = timezone.now()
         if self.expire_time:
             if self.expire_time < nowtime:
                 return True
         return False
 
     def save(self, *args, **kwargs):
+        if self.expires is None:
+            if self.default_expires:
+                self.expires = self.default_expires
+        if self.expires_unit is None:
+            if self.default_expires_unit:
+                self.expires_unit = self.default_expires_unit
         if self.expires:
             if self.expire_time is None:
                 self.expire_time = timezone.now() + datetime.timedelta(
                     seconds=self.get_expire_seconds()
                 )
         return super().save(*args, **kwargs)
+
+
+class WithVisibleFields(models.Model):
+    visible = models.BooleanField(
+        null=True,
+        verbose_name="是否显示",
+    )
+    hidden_time = models.DateTimeField(
+        null=True,
+        blank=True,
+        verbose_name="隐藏时间",
+    )
+    visible_time = models.DateTimeField(
+        null=True,
+        blank=True,
+        verbose_name="显示时间",
+    )
+
+    class Meta:
+        abstract = True
+
+    def save(self, *args, **kwargs):
+        if self.visible:
+            if self.hidden_time is not None:
+                self.hidden_time = None
+            if self.visible_time is None:
+                self.visible_time = timezone.now()
+        else:
+            if self.hidden_time is None:
+                self.hidden_time = timezone.now()
+            if self.visible_time is not None:
+                self.visible_time = None
+        return super().save(*args, **kwargs)
+
+    def set_hidden(self, save=True):
+        self.visible = False
+        if self.save:
+            self.save()
+
+    def set_visible(self, save=True):
+        self.visible = True
+        if self.save:
+            self.save()
+
+
+class WithHotspotFields(models.Model):
+    hotspot = models.BooleanField(
+        null=True,
+        verbose_name="是否热点",
+    )
+    hotspot_weight = models.IntegerField(
+        null=True,
+        blank=True,
+        default=100,
+        verbose_name="热度",
+    )
+    hotspot_time = models.DateTimeField(
+        null=True,
+        blank=True,
+        verbose_name="设置热点时间",
+    )
+    non_hotspot_time = models.DateTimeField(
+        null=True,
+        blank=True,
+        verbose_name="取消热点时间",
+    )
+
+    class Meta:
+        abstract = True
+
+    def save(self, *args, **kwargs):
+        if self.hotspot:
+            if self.hotspot_time is None:
+                self.hotspot_time = timezone.now()
+            if self.non_hotspot_time is not None:
+                self.non_hotspot_time = None
+        else:
+            if self.hotspot_time is not None:
+                self.hotspot_time = None
+            if self.non_hotspot_time is None:
+                self.non_hotspot_time = timezone.now()
+        return super().save(*args, **kwargs)
+
+    def set_hotspot(self, save=True):
+        self.hotspot = True
+        if save:
+            self.save()
+
+    def set_non_hotspot(self, save=True):
+        self.hotspot = False
+        if save:
+            self.save()
```

### Comparing `django-model-helper-0.1.0/django_model_helper.egg-info/PKG-INFO` & `django-model-helper-0.1.5/django_model_helper.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: django-model-helper
-Version: 0.1.0
+Version: 0.1.5
 Summary: Helpful django abstract models collection.
 Author: Li HuiTao
+Maintainer: Li HuiTao
 License: MIT
 Keywords: django-model-helper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,27 +15,39 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-model-helper
 
 Helpful django abstract models collection.
 
-## Abstract Models
+## 抽象类列表
 
-- WithAddModTimeFields
-- WithConfigFields
-- WithCountFields
-- WithDeletedStatusFields
-- WithDisplayOrderFields
-- WithEnabledStatusFields
-- WithExpireTimeFields
-- WithJsonDataFields
-- WithLockStatusFields
-- WithSimpleResultFields
-- WithSimpleNRRDStatusFields
-- WithUidFields
+1. WithAddModTimeFields
+1. WithConfigFields
+1. WithCountFields
+1. WithDeletedStatusFields
+1. WithDisplayOrderFields
+1. WithEnabledStatusFields
+1. WithExpireTimeFields
+1. WithHotspotFields
+1. WithJsonDataFields
+1. WithLockStatusFields
+1. WithSimpleResultFields
+1. WithSimpleNRRDStatusFields
+1. WithUidFields
+1. WithVisibleFields
 
-## Releases
+## 版本记录
 
 ### v0.1.0
 
-- First release.
+- 版本首发。
+
+### v0.1.1
+
+- WithExpireTimeFields添加default_expires属性。
+- WithUidFields添加uidgen属性，用于生成uid默认值。
+
+### v0.1.5
+
+- 添加WithVisibleFields抽象类。
+- 添加WithHotspotFields抽象类。
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-model-helper-0.1.0/django_model_helper.egg-info/SOURCES.txt` & `django-model-helper-0.1.5/django_model_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-model-helper-0.1.0/setup.py` & `django-model-helper-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 setup(
     name="django-model-helper",
     version=version.VERSION,
     description="Helpful django abstract models collection.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Li HuiTao",
+    maintainer="Li HuiTao",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

