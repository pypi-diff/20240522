# Comparing `tmp/pydantic_pkgr-0.1.1.tar.gz` & `tmp/pydantic_pkgr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_pkgr-0.1.1.tar", last modified: Sat May 18 12:21:17 2024, max compression
+gzip compressed data, was "pydantic_pkgr-0.1.2.tar", last modified: Tue May 21 05:48:03 2024, max compression
```

## Comparing `pydantic_pkgr-0.1.1.tar` & `pydantic_pkgr-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1067 2024-05-18 10:31:28.160777 pydantic_pkgr-0.1.1/LICENSE
--rw-r--r--   0        0        0    16617 2024-05-18 12:19:51.423578 pydantic_pkgr-0.1.1/README.md
--rw-r--r--   0        0        0     6148 2024-05-18 10:59:52.992817 pydantic_pkgr-0.1.1/pydantic_pkgr/.DS_Store
--rw-r--r--   0        0        0    10365 2024-05-18 08:46:29.500191 pydantic_pkgr-0.1.1/pydantic_pkgr/README.md
--rw-r--r--   0        0        0      280 2024-05-18 10:55:38.562675 pydantic_pkgr-0.1.1/pydantic_pkgr/__init__.py
--rw-r--r--   0        0        0      958 2024-05-18 11:04:11.896491 pydantic_pkgr-0.1.1/pydantic_pkgr/admin.py
--rw-r--r--   0        0        0      157 2024-05-18 10:48:11.648219 pydantic_pkgr-0.1.1/pydantic_pkgr/apps.py
--rw-r--r--   0        0        0    11040 2024-05-18 12:19:51.428214 pydantic_pkgr-0.1.1/pydantic_pkgr/binary.py
--rw-r--r--   0        0        0    18423 2024-05-18 10:54:28.284898 pydantic_pkgr-0.1.1/pydantic_pkgr/binprovider.py
--rw-r--r--   0        0        0        0 2024-05-18 05:55:33.133304 pydantic_pkgr-0.1.1/pydantic_pkgr/migrations/__init__.py
--rw-r--r--   0        0        0      815 2024-05-18 11:07:50.379604 pydantic_pkgr-0.1.1/pydantic_pkgr/models.py
--rw-r--r--   0        0        0     5855 2024-05-18 10:54:18.838396 pydantic_pkgr-0.1.1/pydantic_pkgr/semver.py
--rw-r--r--   0        0        0       60 2024-05-18 05:55:33.133068 pydantic_pkgr-0.1.1/pydantic_pkgr/tests.py
--rw-r--r--   0        0        0     3117 2024-05-18 11:05:09.377160 pydantic_pkgr-0.1.1/pydantic_pkgr/views.py
--rw-r--r--   0        0        0     2378 2024-05-18 12:21:17.358375 pydantic_pkgr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-18 10:37:14.086350 pydantic_pkgr-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0    18111 1970-01-01 00:00:00.000000 pydantic_pkgr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-18 10:31:28.160777 pydantic_pkgr-0.1.2/LICENSE
+-rw-r--r--   0        0        0    19188 2024-05-21 05:42:03.899728 pydantic_pkgr-0.1.2/README.md
+-rw-r--r--   0        0        0     6148 2024-05-21 05:39:19.159621 pydantic_pkgr-0.1.2/pydantic_pkgr/.DS_Store
+-rw-r--r--   0        0        0      298 2024-05-21 05:42:03.908496 pydantic_pkgr-0.1.2/pydantic_pkgr/__init__.py
+-rw-r--r--   0        0        0      958 2024-05-18 11:04:11.896491 pydantic_pkgr-0.1.2/pydantic_pkgr/admin.py
+-rw-r--r--   0        0        0      157 2024-05-18 10:48:11.648219 pydantic_pkgr-0.1.2/pydantic_pkgr/apps.py
+-rw-r--r--   0        0        0    11622 2024-05-21 05:42:03.908758 pydantic_pkgr-0.1.2/pydantic_pkgr/binary.py
+-rw-r--r--   0        0        0    22084 2024-05-21 05:42:03.908974 pydantic_pkgr-0.1.2/pydantic_pkgr/binprovider.py
+-rw-r--r--   0        0        0        0 2024-05-18 05:55:33.133304 pydantic_pkgr-0.1.2/pydantic_pkgr/migrations/__init__.py
+-rw-r--r--   0        0        0      815 2024-05-18 11:07:50.379604 pydantic_pkgr-0.1.2/pydantic_pkgr/models.py
+-rw-r--r--   0        0        0     5961 2024-05-21 03:49:36.678700 pydantic_pkgr-0.1.2/pydantic_pkgr/semver.py
+-rw-r--r--   0        0        0     1041 2024-05-21 05:42:03.909403 pydantic_pkgr-0.1.2/pydantic_pkgr/settings.py
+-rw-r--r--   0        0        0       60 2024-05-18 05:55:33.133068 pydantic_pkgr-0.1.2/pydantic_pkgr/tests.py
+-rw-r--r--   0        0        0     2912 2024-05-21 05:42:03.909573 pydantic_pkgr-0.1.2/pydantic_pkgr/views.py
+-rw-r--r--   0        0        0     2483 2024-05-21 05:48:03.362758 pydantic_pkgr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    20682 1970-01-01 00:00:00.000000 pydantic_pkgr-0.1.2/PKG-INFO
```

### Comparing `pydantic_pkgr-0.1.1/LICENSE` & `pydantic_pkgr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_pkgr-0.1.1/README.md` & `pydantic_pkgr-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,90 @@
-<h1><a href="https://github.com/ArchiveBox/pydantic-pkgr"><code>pydantic-pkgr</code></a> &nbsp; &nbsp; &nbsp; &nbsp; 📦  <small><code>apt</code>&nbsp; <code>brew</code>&nbsp; <code>pip</code>&nbsp; <code>npm</code> &nbsp;++</small><br/><sub>A typed Python API wrapper for common system package managers.</sub></h1>
+<h1><a href="https://github.com/ArchiveBox/pydantic-pkgr"><code>pydantic-pkgr</code></a> &nbsp; &nbsp; &nbsp; &nbsp; 📦  <small><code>apt</code>&nbsp; <code>brew</code>&nbsp; <code>pip</code>&nbsp; <code>npm</code> &nbsp;₊₊₊</small><br/><sub>Simple Pydantic interfaces for package managers + installed binaries.</sub></h1>
 <br/>
 
 [![PyPI][pypi-badge]][pypi]
 [![Python Version][version-badge]][pypi]
 [![Django Version][django-badge]][pypi]
 [![GitHub][licence-badge]][licence]
 [![GitHub Last Commit][repo-badge]][repo]
 <!--[![Downloads][downloads-badge]][pypi]-->
 
 <br/>
 
-**This is a [Python 3 library](https://pypi.org/project/pydantic-pkgr/) for installing & managing packages with a variety of package managers.**
+**This is a [Python library](https://pypi.org/project/pydantic-pkgr/) for installing & managing packages locally with a variety of package managers.**  
+It's designed to help Python apps check for and install local binaries at runtime.  
+
 
 ```shell
 pip install pydantic-pkgr
 ```
 
+
 > ✨ Built with [`pydantic`](https://pydantic-docs.helpmanual.io/) v2 for strong static typing guarantees and json import/export compatibility  
 > 📦 Provides consistent cross-platform interfaces for dependency resolution & installation at runtime  
 > 🌈 Supports [`django`](https://docs.djangoproject.com/en/5.0/) >= 4.0, [`django-ninja`](https://django-ninja.dev/), and OpenAPI + [`django-jsonform`](https://django-jsonform.readthedocs.io/) out-of-the-box  
-> 🦄 Plays well with [`pyinfra`](https://github.com/pyinfra-dev/pyinfra) and [`ansible`](https://github.com/ansible/ansible) for advanced orchestration use-cases
+> 🦄 Uses [`pyinfra`](https://github.com/pyinfra-dev/pyinfra) / [`ansible`](https://github.com/ansible/ansible) for the actual install operations whenever possible (with internal fallbacks)
 
 <sub><i>Built by <a href="https://github.com/ArchiveBox">ArchiveBox</a> to install & auto-update our extractor dependencies at runtime (<code>chrome</code>, <code>wget</code>, <code>curl</code>, etc.) on `macOS`/`Linux`/`Docker`.</i></sub>
 
 <br/>
 
+> [!WARNING]
+> This is [ALPHA] software under active development, not ready for production use yet.
+
+
 **Source Code**: [https://github.com/ArchiveBox/pydantic-pkgr/](https://github.com/ArchiveBox/pydantic-pkgr/)
 
 **Documentation**: [https://github.com/ArchiveBox/pydantic-pkgr/blob/main/README.md](https://github.com/ArchiveBox/pydantic-pkgr/blob/main/README.md)
 
 <br/>
 
 ```python
-from pydantic_pkgr import AptProvider
+from pydantic_pkgr import AptProvider, Binary
 
-# Example: Install curl using the apt provider
 apt = AptProvider()
 curl = apt.install('curl')
 
-print(curl.provider)                       # 'apt'
-print(curl.abspath)                        # Path('/usr/bin/curl')
-print(curl.version)                        # SemVer('7.81.0')
-curl.exec(['--version'])                   # curl 7.81.0 (x86_64-pc-linux-gnu) libcurl/7.81.0 ...
+print(curl.abspath, curl.version, curl.provider, curl.is_valid)  # Path('/usr/bin/curl') SemVer('7.81.0') 'apt' True
+
+proc = curl.exec(['-fsSL', 'https://example.com'])               # <!doctype html>...
 ```
 
 ```python
-from pydantic_pkgr import Binary, BinName, BinProvider
+from pydantic_pkgr import Binary, BinProvider, BrewProvider, EnvProvider
 
 # Example: Create a re-usable curl Binary object that defines its install methods
 curl = Binary(name='curl', providers=[BrewProvider(), EnvProvider()])
-curl = curl.install()
 
-print(curl.provider)                       # 'brew'
-print(curl.abspath)                        # Path('/opt/homebrew/bin/curl')
-print(curl.version)                        # SemVer('8.4.0')
-curl.exec(['--version'])                   # curl 8.4.0 (x86_64-apple-darwin23.0) libcurl/8.4.0 ...
+# or for nicer type checking ergonomics, use class-based definitions:
+class CurlBinary(Binary):
+    name: str = 'curl'
+    providers list[BinProvider] = [BrewProvider(), EnvProvider()]
+curl = CurlBinary()
+
+# it works the same either way
+curl = curl.install()
+print(curl.abspath, curl.version, curl.provider, curl.is_valid)  # Path('/opt/homebrew/bin/curl') SemVer('8.4.0') 'brew' True
+curl.exec(['--version'])                                         # curl 8.4.0 (x86_64-apple-darwin23.0) libcurl/8.4.0 ...
 ```
 
 ```python
-print(curl.model_dump_json())              # ... everything can also be dumped/loaded as json
-print(curl.model_json_schema())            # ... all types provide OpenAPI-ready JSON schemas
+from pyinfra.operations import apt
+from pydantic_pkgr import Binary
+
+# Example: Verify & use packages installed by other tools (e.g. pyinfra/ansible)
+apt.packages(name="Install ffmpeg", packages=['ffmpeg'], _sudo=True)
+
+# Load it as a Binary provides a nice type-checkable, validated, serializable handle for it
+ffmpeg = Binary(name='ffmpeg').load()
+ffmpeg.exec(['-i', 'input.mp4', 'output.avi'])
+
+print(ffmpeg)                       # name=ffmpeg abspath=/usr/bin/ffmpeg version=3.3.0 is_valid=True
+print(ffmpeg.model_dump_json())     # ... everything can also be dumped/loaded as json
+print(ffmpeg.model_json_schema())   # ... all types provide OpenAPI-ready JSON schemas
 ```
 
 ### Supported Package Managers
 
 **So far it supports `installing`/`finding installed`/~~`updating`/`removing`~~ packages on `Linux`/`macOS` with:**
 
 - `apt` (Ubuntu/Debian/etc.)
@@ -167,24 +188,24 @@
 class DockerBinary(Binary):
     name: BinName = 'docker'
 
     providers_supported: List[BinProvider] = [EnvProvider(), AptProvider()]
     
     provider_overrides: Dict[BinProviderName, ProviderLookupDict] = {
         'env': {
-            # prefer podman if installed (or fall back to docker)
+            # example: prefer podman if installed (falling back to docker)
             'abspath': lambda: os.which('podman') or os.which('docker') or os.which('docker-ce'),
         },
         'apt': {
-            # install docker OR docker-ce (varies based on CPU architecture)
+            # example: vary installed package name based on your CPU architecture
             'subdeps': lambda: {
                 'amd64': 'docker',
                 'armv7l': 'docker-ce',
                 'arm64': 'docker-ce',
-            }.get(platform.machine()) or 'docker',
+            }.get(platform.machine(), 'docker'),
         },
     }
 
 docker = DockerBinary().load_or_install()
 print(docker.provider)                    # 'env'
 print(docker.abspath)                     # Path('/usr/local/bin/podman')
 print(docker.version)                     # SemVer('6.0.2')
@@ -207,14 +228,19 @@
 
 ### Example: Use the SemVer type directly for parsing & verifying version strings
 SemVer.parse('Google Chrome 124.0.6367.208+beta_234. 234.234.123')  # SemVer(124, 0, 6367')
 SemVer.parse('2024.04.05)                                           # SemVer(2024, 4, 5)
 SemVer.parse('1.9+beta')                                            # SemVer(1, 9, 0)
 str(SemVer(1, 9, 0))                                                # '1.9.0'
 ```
+<br/>
+
+> These types are all meant to be used library-style to make writing your own apps easier.  
+> e.g. you can use it to build things like: [`playwright install --with-deps`](https://playwright.dev/docs/browsers#install-system-dependencies))
+
 
 <br/>
 
 ---
 
 <br/>
 
@@ -243,54 +269,60 @@
 
 
 Usage in your `models.py`:
 ```python
 from django.db import models
 from django_pydantic_field import SchemaField
 
-from pydantic_pkgr import BinProvider, EnvProvider, Binary
+from pydantic_pkgr import BinProvider, EnvProvider, Binary, SemVer
 
 DEFAULT_PROVIDER = EnvProvider()
 
-class MyModel(models.Model):
-    ...
-
-    # SchemaField supports storing a single BinProvider/Binary in a field...
-    favorite_binprovider: BinProvider = SchemaField(default=DEFAULT_PROVIDER)
+class Dependency(models.Model):
+    """Example model for storing information about a dependency"""
 
-    # ... or inside a collection type like list[...] dict[...]
-    optional_binaries: list[Binary] = SchemaField(default=[])
+    name = models.CharField(max_length=63)
+    min_version: SemVer = SchemaField(default=(0,0,1))
+    binaries: list[Binary] = SchemaField(default=[])
+    default_binprovider: BinProvider = SchemaField(default=DEFAULT_PROVIDER)
 
 curl = Binary(name='curl', providers=[DEFAULT_PROVIDER]).load()
 
-obj = MyModel(optional_binaries=[curl])
+obj = Dependency(default_binprovider=DEFAULT_PROVIDER, binaries=[curl], min_version=SemVer('0.1.5'))
 obj.save()
 
-assert obj.favorite_binprovider == DEFAULT_PROVIDER
-assert obj.optional_binaries[0].provider == DEFAULT_PROVIDER
+assert obj.default_binprovider == DEFAULT_PROVIDER
+assert obj.binaries[0].provider == DEFAULT_PROVIDER
 ```
+*For a full example see our provided [`django_example_project/`](https://github.com/ArchiveBox/pydantic-pkgr/tree/main/django_example_project)...*
 
 <br/>
 
 ### Django Admin Usage: Show read-only list of Binaries in Admin UI
 
+<img height="220" alt="Django Admin binaries list view" src="https://github.com/ArchiveBox/pydantic-pkgr/assets/511499/a9980217-f39e-434e-b266-20cd6feb17c3" align="top"><img height="220" alt="Django Admin binaries detail view" src="https://github.com/ArchiveBox/pydantic-pkgr/assets/511499/d4d9086e-c8f4-4b6e-8ee8-8c8a864715b0" align="top">
+
 ```bash
 pip install pydantic-pkgr django-admin-data-views
 ```
 *For more info see the [`django-admin-data-views`](https://github.com/MrThearMan/django-admin-data-views) docs...*
 
 Then add this to your `settings.py`:
 ```python
 INSTALLED_APPS = [
     # ...
     'admin_data_views'
     'pydantic_pkgr'
     # ...
 ]
 
+# point these to a function that gets the list of all binaries / a single binary
+PYDANTIC_PKGR_GET_ALL_BINARIES = 'pydantic_pkgr.views.get_all_binaries'
+PYDANTIC_PKGR_GET_BINARY = 'pydantic_pkgr.views.get_binary'
+
 ADMIN_DATA_VIEWS = {
     "NAME": "Environment",
     "URLS": [
         {
             "route": "binaries/",
             "view": "pydantic_pkgr.views.binaries_list_view",
             "name": "binaries",
@@ -300,14 +332,15 @@
                 "name": "binary",
             },
         },
         # Coming soon: binprovider_list_view + binprovider_detail_view ...
     ],
 }
 ```
+*For a full example see our provided [`django_example_project/`](https://github.com/ArchiveBox/pydantic-pkgr/tree/main/django_example_project)...*
 
 <details>
 <summary><i>Note: If you override the default site admin, you must register the views manually...</i></summary>
 <br/><br/>
 <b><code>admin.py</code>:</b>
 <br/>
 <pre><code>
@@ -321,17 +354,25 @@
 from pydantic_pkgr.admin import register_admin_views
 register_admin_views(custom_admin)
 </code></pre>
 </details>
 
 <br/>
 
-### Django Admin Usage: JSONFormWidget for editing `BinProvider` and `Binary` data
+### ~~Django Admin Usage: JSONFormWidget for editing `BinProvider` and `Binary` data~~
+
+<img src="https://github.com/ArchiveBox/pydantic-pkgr/assets/511499/63705a57-4f62-4dbe-9f3a-0515323d8b5e" width="600px"/>
+
+> [!IMPORTANT]
+> This feature is coming soon but is blocked on a few issues being fixed first:  
+> - https://github.com/surenkov/django-pydantic-field/issues/64
+> - https://github.com/surenkov/django-pydantic-field/issues/65
+> - https://github.com/surenkov/django-pydantic-field/issues/66
 
-Install `django-jsonform` to get auto-generated Forms for editing BinProvider, Binary, etc. data
+~~Install `django-jsonform` to get auto-generated Forms for editing BinProvider, Binary, etc. data~~
 ```bash
 pip install django-pydantic-field django-jsonform
 ```
 *For more info see the [`django-jsonform`](https://django-jsonform.readthedocs.io/) docs...*
 
 `admin.py`:
 ```python
@@ -340,14 +381,15 @@
 from django_pydantic_field.v2.fields import PydanticSchemaField
 
 class MyModelAdmin(admin.ModelAdmin):
     formfield_overrides = {PydanticSchemaField: {"widget": JSONFormWidget}}
 
 admin.site.register(MyModel, MyModelAdmin)
 ```
+*For a full example see our provided [`django_example_project/`](https://github.com/ArchiveBox/pydantic-pkgr/tree/main/django_example_project)...*
 
 <br/>
 
 ---
 
 <br/>
```

### Comparing `pydantic_pkgr-0.1.1/pydantic_pkgr/admin.py` & `pydantic_pkgr-0.1.2/pydantic_pkgr/admin.py`

 * *Files identical despite different names*

### Comparing `pydantic_pkgr-0.1.1/pydantic_pkgr/binary.py` & `pydantic_pkgr-0.1.2/pydantic_pkgr/binary.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__package__ = 'archivebox.plugantic'
+__package__ = 'pydantic_pkgr'
 
 import sys
 import inspect
 import importlib
 from pathlib import Path
 
 
@@ -16,48 +16,52 @@
 from pydantic import BaseModel, Field, model_validator, computed_field, field_validator, validate_call, field_serializer, ConfigDict
 
 from .semver import SemVer
 from .binprovider import (
     BinName,
     BinProviderName,
     HostBinPath,
+    ShallowBinary,
     BinProvider,
     EnvProvider,
     AptProvider,
     BrewProvider,
     PipProvider,
     ProviderLookupDict,
     bin_name,
     bin_abspath,
     path_is_script,
     path_is_executable,
 )
 
+DEFAULT_PROVIDER = EnvProvider()
 
-class Binary(BaseModel):
-    model_config = ConfigDict(extra='ignore', populate_by_name=True)
 
-    name: BinName
-    description: str = Field(default='')
+class Binary(ShallowBinary):
+    model_config = ConfigDict(extra='ignore', populate_by_name=True, validate_defaults=True)
 
-    providers_supported: List[BinProvider] = Field(default=[EnvProvider()], alias='providers')
+    name: BinName = ''
+    description: str = ''
+
+    providers_supported: List[BinProvider] = Field(default=[DEFAULT_PROVIDER], alias='providers')
     provider_overrides: Dict[BinProviderName, ProviderLookupDict] = Field(default={}, alias='overrides')
     
     loaded_provider: Optional[BinProviderName] = Field(default=None, alias='provider')
     loaded_abspath: Optional[HostBinPath] = Field(default=None, alias='abspath')
     loaded_version: Optional[SemVer] = Field(default=None, alias='version')
     
     # bin_filename:  see below
     # is_executable: see below
     # is_script
     # is_valid: see below
 
 
     @model_validator(mode='after')
     def validate(self):
+        # assert self.name, 'Binary.name must not be empty'
         self.loaded_abspath = bin_abspath(self.name) or self.name
         self.description = self.description or self.name
         
         assert self.providers_supported, f'No providers were given for package {self.name}'
 
         # pull in any overrides from the binproviders
         for provider in self.providers_supported:
@@ -127,80 +131,77 @@
             and self.loaded_abspath
             and self.loaded_version
             and (self.is_executable or self.is_script)
         )
 
     @validate_call
     def install(self) -> Self:
+        assert self.name, f'No binary name was provided! {self}'
+
         if not self.providers_supported:
             return self
 
-        exc = Exception('No providers were able to install binary', self.name, self.providers_supported)
+        outer_exc = Exception(f'None of the configured providers [{", ".join(p.name for p in self.providers_supported)}] were able to install binary: {self.name}')
+        inner_exc = Exception('No providers were available')
         for provider in self.providers_supported:
             try:
                 installed_bin = provider.install(self.name, overrides=self.provider_overrides.get(provider.name))
                 if installed_bin:
                     # print('INSTALLED', self.name, installed_bin)
-                    return self.model_copy(update={
-                        'loaded_provider': provider.name,
-                        'loaded_abspath': installed_bin.abspath,
-                        'loaded_version': installed_bin.version,
-                    })
+                    return self.model_copy(update=installed_bin.model_dump(exclude=('providers_supported',)))
             except Exception as err:
-                print(err)
-                exc = err
-        raise exc
+                # print(err)
+                inner_exc = err
+        raise outer_exc from inner_exc
 
     @validate_call
     def load(self, cache=True) -> Self:
+        assert self.name, f'No binary name was provided! {self}'
+
         if self.is_valid:
             return self
 
         if not self.providers_supported:
             return self
 
-        exc = Exception('No providers were able to install binary', self.name, self.providers_supported)
+        outer_exc = Exception(f'None of the configured providers [{", ".join(p.name for p in self.providers_supported)}] were able to load binary: {self.name}')
+        inner_exc = Exception('No providers were available')
         for provider in self.providers_supported:
             try:
                 installed_bin = provider.load(self.name, cache=cache, overrides=self.provider_overrides.get(provider.name))
                 if installed_bin:
                     # print('LOADED', provider, self.name, installed_bin)
-                    return self.model_copy(update={
-                        'loaded_provider': provider.name,
-                        'loaded_abspath': installed_bin.abspath,
-                        'loaded_version': installed_bin.version,
-                    })
+                    return self.model_copy(update=installed_bin.model_dump(exclude=('providers_supported',)))
             except Exception as err:
-                print(err)
-                exc = err
-        raise exc
+                # print(err)
+                inner_exc = err
+        raise outer_exc from inner_exc
 
     @validate_call
     def load_or_install(self, cache=True) -> Self:
+        assert self.name, f'No binary name was provided! {self}'
+
         if self.is_valid:
             return self
 
         if not self.providers_supported:
             return self
 
-        exc = Exception('No providers were able to install binary', self.name, self.providers_supported)
+        outer_exc = Exception(f'None of the configured providers [{", ".join(p.name for p in self.providers_supported)}] were able to find or install binary: {self.name}')
+        inner_exc = Exception('No providers were available')
         for provider in self.providers_supported:
             try:
                 installed_bin = provider.load_or_install(self.name, overrides=self.provider_overrides.get(provider.name), cache=cache)
                 if installed_bin:
                     # print('LOADED_OR_INSTALLED', self.name, installed_bin)
-                    return self.model_copy(update={
-                        'loaded_provider': provider.name,
-                        'loaded_abspath': installed_bin.abspath,
-                        'loaded_version': installed_bin.version,
-                    })
+                    return self.model_copy(update=installed_bin.model_dump(exclude=('providers_supported',)))
             except Exception as err:
-                print(err)
-                exc = err
-        raise exc
+                # print(err)
+                inner_exc = err
+        raise outer_exc from inner_exc
 
     @validate_call
     def exec(self, args=(), pwd='.') -> CompletedProcess:
         assert self.loaded_abspath
         assert self.loaded_version
         return run([self.loaded_abspath, *args], stdout=PIPE, stderr=PIPE, pwd=pwd)
 
@@ -319,7 +320,11 @@
 
 #     print('-------------------------------------DEFINING BINARIES---------------------------------')
 #     print(PYTHON_BINARY)
 #     print(SQLITE_BINARY)
 #     print(DJANGO_BINARY)
 #     print(WGET_BINARY)
 #     print(YTDLP_BINARY)
+
+# import json
+# print(json.dumps(EnvProvider().model_dump_json(), indent=4))            # ... everything can also be dumped/loaded as json
+# print(json.dumps(WgetBinary().model_json_schema(), indent=4))          # ... all types provide OpenAPI-ready JSON schemas
```

### Comparing `pydantic_pkgr-0.1.1/pydantic_pkgr/binprovider.py` & `pydantic_pkgr-0.1.2/pydantic_pkgr/binprovider.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 import os
+import sys
 import shutil
 import operator
 
-from typing import Callable, Any, Optional, Type, Dict, Annotated, ClassVar, Literal, cast, TYPE_CHECKING
+from typing import Callable, Any, Optional, Type, List, Dict, Annotated, ClassVar, Literal, cast, TYPE_CHECKING
 from typing_extensions import Self
-from abc import ABC, abstractmethod
 from collections import namedtuple
 from pathlib import Path
 from subprocess import run, PIPE, CompletedProcess
 
 from pydantic_core import core_schema, ValidationError
-from pydantic import BaseModel, Field, TypeAdapter, AfterValidator, validate_call, GetCoreSchemaHandler, ConfigDict
+from pydantic import BaseModel, Field, TypeAdapter, AfterValidator, validate_call, GetCoreSchemaHandler, ConfigDict, computed_field
+
+
+def validate_bin_provider_name(name: str) -> str:
+    assert 1 < len(name) < 16, 'BinProvider names must be between 1 and 16 characters long'
+    assert name.replace('_', '').isalnum(), 'BinProvider names can only contain a-Z0-9 and underscores'
+    assert name[0].isalpha(), 'BinProvider names must start with a letter'
+    return name
+
+BinProviderName = Annotated[str, AfterValidator(validate_bin_provider_name)]
+# in practice this is essentially BinProviderName: Literal['env', 'pip', 'apt', 'brew', 'npm', 'vendor']
+# but because users can create their own BinProviders we cant restrict it to a preset list of literal names
+
 
 from .semver import SemVer
 
 
 def func_takes_args_or_kwargs(lambda_func: Callable[..., Any]) -> bool:
     """returns True if a lambda func takes args/kwargs of any kind, otherwise false if it's pure/argless"""
     code = lambda_func.__code__
@@ -23,17 +35,18 @@
     has_varkw = code.co_flags & 0x08 != 0
     return has_args or has_varargs or has_varkw
 
 
 @validate_call
 def bin_name(bin_path_or_name: str | Path) -> str:
     name = Path(bin_path_or_name).name
-    assert len(name) > 1
+    assert 1 <= len(name) < 64, 'Binary names must be between 1 and 63 characters long'
     assert name.replace('-', '').replace('_', '').replace('.', '').isalnum(), (
         f'Binary name can only contain a-Z0-9-_.: {name}')
+    assert name[0].isalpha(), 'Binary names must start with a letter'
     return name
 
 BinName = Annotated[str, AfterValidator(bin_name)]
 
 @validate_call
 def path_is_file(path: Path | str) -> Path:
     path = Path(path) if isinstance(path, str) else path
@@ -53,56 +66,96 @@
     assert path.suffix.lower() in SCRIPT_EXTENSIONS, 'Path is not a script (does not end in {})'.format(', '.join(SCRIPT_EXTENSIONS))
     return path
 
 HostExecutablePath = Annotated[HostExistsPath, AfterValidator(path_is_executable)]
 
 @validate_call
 def path_is_abspath(path: Path) -> Path:
-    return path.resolve()
+    path = path.expanduser().absolute()   # resolve ~/ -> /home/<username/ and ../../
+    assert path.resolve()                 # make sure symlinks can be resolved, but dont return resolved link
+    return path
 
 HostAbsPath = Annotated[HostExistsPath, AfterValidator(path_is_abspath)]
-HostBinPath = Annotated[Path, AfterValidator(path_is_abspath), AfterValidator(path_is_file)]
-
+HostBinPath = Annotated[HostExistsPath, AfterValidator(path_is_abspath)] # removed: AfterValidator(path_is_executable)
+# not all bins need to be executable to be bins, some are scripts
 
 @validate_call
 def bin_abspath(bin_path_or_name: BinName | Path) -> HostBinPath | None:
     assert bin_path_or_name
 
     if str(bin_path_or_name).startswith('/'):
         # already a path, get its absolute form
-        abspath = Path(bin_path_or_name).resolve()
+        abspath = Path(bin_path_or_name).expanduser().absolute()
     else:
-        # not a path yet, get path using os.which
+        # not a path yet, get path using shutil.which
         binpath = shutil.which(bin_path_or_name)
         if not binpath:
             return None
-        abspath = Path(binpath).resolve()
+        abspath = Path(binpath).expanduser().absolute()
 
     try:
         return TypeAdapter(HostBinPath).validate_python(abspath)
     except ValidationError:
         return None
 
 
 @validate_call
 def bin_version(bin_path: HostBinPath, args=('--version',)) -> SemVer | None:
-    return SemVer(run([bin_path, *args], stdout=PIPE).stdout.strip().decode())
+    return SemVer(run([str(bin_path), *args], stdout=PIPE, text=True).stdout.strip())
 
 
-class InstalledBin(BaseModel):
+class ShallowBinary(BaseModel):
     """
     Shallow version of Binary used as a return type for BinProvider methods (e.g. load_or_install()).
     (doesn't implement full Binary interface, but can be used to populate a full loaded Binary instance)
     """
-    model_config = ConfigDict(extra='ignore', populate_by_name=True)
+    model_config = ConfigDict(extra='ignore', populate_by_name=True, validate_defaults=True)
+
 
+    name: BinName = ''
+
+    providers_supported: List['BinProvider'] = Field(default=[], alias='providers')
+
+    loaded_provider: BinProviderName = Field(default='env', alias='provider')
     loaded_abspath: HostBinPath = Field(alias='abspath')
     loaded_version: SemVer = Field(alias='version')
-    loaded_provider: 'BinProviderName' = Field(default='env', alias='provider')
-    
+
+    @computed_field                                                                                           # type: ignore[misc]  # see mypy issue #1362
+    @property
+    def is_executable(self) -> bool:
+        try:
+            assert self.loaded_abspath and path_is_executable(self.loaded_abspath)
+            return True
+        except (ValidationError, AssertionError):
+            return False
+
+    @computed_field                                                                                           # type: ignore[misc]  # see mypy issue #1362
+    @property
+    def is_script(self) -> bool:
+        try:
+            assert self.loaded_abspath and path_is_script(self.loaded_abspath)
+            return True
+        except (ValidationError, AssertionError):
+            return False
+
+    @computed_field                                                                                           # type: ignore[misc]  # see mypy issue #1362
+    @property
+    def is_valid(self) -> bool:
+        return bool(
+            self.name
+            and self.loaded_abspath
+            and self.loaded_version
+            and (self.is_executable or self.is_script)
+        )
+
+    @computed_field
+    @property
+    def loaded_respath(self) -> HostBinPath | None:
+        return self.loaded_abspath and self.loaded_abspath.resolve()
+
     def exec(self, args) -> CompletedProcess:
         return run([self.abspath, *args], stdout=PIPE, stderr=PIPE, text=True)
 
 
 def is_valid_install_string(pkgs_str: str) -> str:
     """Make sure a string is a valid install string for a package manager, e.g. 'yt-dlp ffmpeg'"""
     assert pkgs_str
@@ -128,19 +181,20 @@
 #     machine: str
 #     system: str
 #     platform: str
 #     in_docker: bool
 #     in_qemu: bool
 #     python: str
 
-BinProviderName = Literal['env', 'pip', 'apt', 'brew', 'npm', 'vendor']
 
 
-class BinProvider(ABC, BaseModel):
-    name: BinProviderName
+class BinProvider(BaseModel):
+    model_config = ConfigDict(extra='ignore', populate_by_name=True, validate_defaults=True)
+    
+    name: BinProviderName = ''
     
     abspath_provider: ProviderLookupDict = Field(default={'*': 'self.on_get_abspath'}, exclude=True)
     version_provider: ProviderLookupDict = Field(default={'*': 'self.on_get_version'}, exclude=True)
     subdeps_provider: ProviderLookupDict = Field(default={'*': 'self.on_get_subdeps'}, exclude=True)
     install_provider: ProviderLookupDict = Field(default={'*': 'self.on_install'}, exclude=True)
 
     _abspath_cache: ClassVar = {}
@@ -252,38 +306,38 @@
             return provider_func_without_args()
 
         provider_func = cast(Callable[..., Any], provider_func)
         return provider_func(bin_name, **kwargs)
 
 
 
-    def on_get_abspath(self, bin_name: BinName, **_) -> HostBinPath | None:
-        print(f'[*] {self.__class__.__name__}: Getting abspath for {bin_name}...')
+    def on_get_abspath(self, bin_name: BinName, **context) -> HostBinPath | None:
+        # print(f'[*] {self.__class__.__name__}: Getting abspath for {bin_name}...')
         try:
             return bin_abspath(bin_name)
         except ValidationError:
             return None
 
-    def on_get_version(self, bin_name: BinName, abspath: Optional[HostBinPath]=None, **_) -> SemVer | None:
+    def on_get_version(self, bin_name: BinName, abspath: Optional[HostBinPath]=None, **context) -> SemVer | None:
         abspath = abspath or self._abspath_cache.get(bin_name) or self.get_abspath(bin_name)
         if not abspath: return None
 
-        print(f'[*] {self.__class__.__name__}: Getting version for {bin_name}...')
+        # print(f'[*] {self.__class__.__name__}: Getting version for {bin_name}...')
         try:
             return bin_version(abspath)
         except ValidationError:
             return None
 
-    def on_get_subdeps(self, bin_name: BinName, **_) -> InstallStr:
-        print(f'[*] {self.__class__.__name__}: Getting subdependencies for {bin_name}')
+    def on_get_subdeps(self, bin_name: BinName, **context) -> InstallStr:
+        # print(f'[*] {self.__class__.__name__}: Getting subdependencies for {bin_name}')
         # ... subdependency calculation logic here
         return TypeAdapter(InstallStr).validate_python(bin_name)
 
-    @abstractmethod
-    def on_install(self, bin_name: BinName, subdeps: Optional[InstallStr]=None, **_):
+
+    def on_install(self, bin_name: BinName, subdeps: Optional[InstallStr]=None, **context):
         subdeps = subdeps or self.get_subdeps(bin_name)
         print(f'[*] {self.__class__.__name__}: Installing subdependencies for {bin_name} ({subdeps})')
         # ... install logic here
         assert True
 
 
     @validate_call
@@ -325,15 +379,15 @@
         )
         if not subdeps:
             subdeps = bin_name
         result = TypeAdapter(InstallStr).validate_python(subdeps)
         return result
 
     @validate_call
-    def install(self, bin_name: BinName, overrides: Optional[ProviderLookupDict]=None) -> InstalledBin | None:
+    def install(self, bin_name: BinName, overrides: Optional[ProviderLookupDict]=None) -> ShallowBinary | None:
         subdeps = self.get_subdeps(bin_name, overrides=overrides)
 
         self.call_provider_for_action(
             bin_name=bin_name,
             provider_type='install',
             default_provider=self.on_install,
             overrides=overrides,
@@ -342,20 +396,26 @@
 
         installed_abspath = self.get_abspath(bin_name)
         assert installed_abspath, f'Unable to find {bin_name} abspath after installing with {self.name}'
 
         installed_version = self.get_version(bin_name, abspath=installed_abspath)
         assert installed_version, f'Unable to find {bin_name} version after installing with {self.name}'
         
-        result = InstalledBin(provider=self.name, abspath=installed_abspath, version=installed_version)
+        result = ShallowBinary(
+            name=bin_name,
+            loaded_provider=self.name,
+            loaded_abspath=installed_abspath,
+            loaded_version=installed_version,
+            providers_supported=[self],
+        )
         self._install_cache[bin_name] = result
         return result
 
     @validate_call
-    def load(self, bin_name: BinName, overrides: Optional[ProviderLookupDict]=None, cache: bool=False) -> InstalledBin | None:
+    def load(self, bin_name: BinName, overrides: Optional[ProviderLookupDict]=None, cache: bool=False) -> ShallowBinary | None:
         installed_abspath = None
         installed_version = None
 
         if cache:
             installed_bin = self._install_cache.get(bin_name)
             if installed_bin:
                 return installed_bin
@@ -367,28 +427,34 @@
         if not installed_abspath:
             return None
 
         installed_version = installed_version or self.get_version(bin_name, abspath=installed_abspath, overrides=overrides)
         if not installed_version:
             return None
 
-        return InstalledBin(provider=self.name, abspath=installed_abspath, version=installed_version)
+        return ShallowBinary(
+            name=bin_name,
+            loaded_provider=self.name,
+            loaded_abspath=installed_abspath,
+            loaded_version=installed_version,
+            providers_supported=[self],
+        )
 
     @validate_call
-    def load_or_install(self, bin_name: BinName, overrides: Optional[ProviderLookupDict]=None, cache: bool=True) -> InstalledBin | None:
+    def load_or_install(self, bin_name: BinName, overrides: Optional[ProviderLookupDict]=None, cache: bool=True) -> ShallowBinary | None:
         installed = self.load(bin_name, overrides=overrides, cache=cache)
         if not installed:
             installed = self.install(bin_name, overrides=overrides)
         return installed
 
 
 class PipProvider(BinProvider):
     name: BinProviderName = 'pip'
 
-    def on_install(self, bin_name: str, subdeps: Optional[InstallStr]=None, **_):
+    def on_install(self, bin_name: str, subdeps: Optional[InstallStr]=None, **context):
         subdeps = subdeps or self.on_get_subdeps(bin_name)
         print(f'[*] {self.__class__.__name__}: Installing subdependencies for {bin_name} ({subdeps})')
         
         proc = run(['pip', 'install', '--upgrade', *subdeps.split(' ')], stdout=PIPE, stderr=PIPE)
         
         if proc.returncode != 0:
             print(proc.stdout.strip().decode())
@@ -396,33 +462,52 @@
             raise Exception(f'{self.__class__.__name__}: install got returncode {proc.returncode} while installing {subdeps}: {subdeps}')
 
 
 class AptProvider(BinProvider):
     name: BinProviderName = 'apt'
     
     subdeps_provider: ProviderLookupDict = {
+        **BinProvider.__fields__['subdeps_provider'].default,
         'yt-dlp': lambda: 'yt-dlp ffmpeg',
     }
 
-    def on_install(self, bin_name: BinName, subdeps: Optional[InstallStr]=None, **_):
+    def on_install(self, bin_name: BinName, subdeps: Optional[InstallStr]=None, **context):
         subdeps = subdeps or self.on_get_subdeps(bin_name)
         print(f'[*] {self.__class__.__name__}: Installing subdependencies for {bin_name} ({subdeps})')
         
-        run(['apt-get', 'update', '-qq'])
-        proc = run(['apt-get', 'install', '-y', *subdeps.split(' ')], stdout=PIPE, stderr=PIPE)
+        try:
+            # if pyinfra is installed, use it
+            
+            from pyinfra.operations import apt
+
+            apt.update(
+                name="Update apt repositories",
+                _sudo=True,
+                _sudo_user="pyinfra",
+            )
+
+            apt.packages(
+                name=f"Ensure {bin_name} is installed",
+                packages=subdeps.split(' '),
+                update=True,
+                _sudo=True,
+            )
+        except ImportError:
+            run(['apt-get', 'update', '-qq'])
+            proc = run(['apt-get', 'install', '-y', *subdeps.split(' ')], stdout=PIPE, stderr=PIPE)
         
-        if proc.returncode != 0:
-            print(proc.stdout.strip().decode())
-            print(proc.stderr.strip().decode())
-            raise Exception(f'{self.__class__.__name__} install got returncode {proc.returncode} while installing {subdeps}: {subdeps}')
+            if proc.returncode != 0:
+                print(proc.stdout.strip().decode())
+                print(proc.stderr.strip().decode())
+                raise Exception(f'{self.__class__.__name__} install got returncode {proc.returncode} while installing {subdeps}: {subdeps}')
 
 class BrewProvider(BinProvider):
     name: BinProviderName = 'brew'
 
-    def on_install(self, bin_name: str, subdeps: Optional[InstallStr]=None, **_):
+    def on_install(self, bin_name: str, subdeps: Optional[InstallStr]=None, **context):
         subdeps = subdeps or self.on_get_subdeps(bin_name)
         print(f'[*] {self.__class__.__name__}: Installing subdependencies for {bin_name} ({subdeps})')
         
         proc = run(['brew', 'install', *subdeps.split(' ')], stdout=PIPE, stderr=PIPE)
         
         if proc.returncode != 0:
             print(proc.stdout.strip().decode())
@@ -430,16 +515,27 @@
             raise Exception(f'{self.__class__.__name__} install got returncode {proc.returncode} while installing {subdeps}: {subdeps}')
 
 
 class EnvProvider(BinProvider):
     name: BinProviderName = 'env'
 
     abspath_provider: ProviderLookupDict = {
-        # 'python': lambda: Path('/opt/homebrew/Cellar/python@3.10/3.10.14/Frameworks/Python.framework/Versions/3.10/bin/python3.10'),
+        **BinProvider.__fields__['abspath_provider'].default,
+        'python': 'self.get_python_abspath',
     }
     version_provider: ProviderLookupDict = {
-        # 'python': lambda: '{}.{}.{}'.format(*sys.version_info[:3]),
+        **BinProvider.__fields__['version_provider'].default,
+        'python': 'self.get_python_version',
     }
 
-    def on_install(self, bin_name: BinName, subdeps: Optional[InstallStr]=None, **_):
+    @staticmethod
+    def get_python_abspath():
+        return Path(sys.executable)
+
+    @staticmethod
+    def get_python_version():
+        return '{}.{}.{}'.format(*sys.version_info[:3])
+
+
+    def on_install(self, bin_name: BinName, subdeps: Optional[InstallStr]=None, **context):
         """The env provider is ready-only and does not install any packages, so this is a no-op"""
         pass
```

### Comparing `pydantic_pkgr-0.1.1/pydantic_pkgr/models.py` & `pydantic_pkgr-0.1.2/pydantic_pkgr/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_pkgr-0.1.1/pydantic_pkgr/semver.py` & `pydantic_pkgr-0.1.2/pydantic_pkgr/semver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __package__ = 'archivebox.plugantic'
 
+import re
 import sys
 import inspect
 import importlib
 from pathlib import Path
 from collections import namedtuple
 
 
@@ -89,22 +90,22 @@
             version_stdout = str(version_stdout)
         
         # no text to work with, return None immediately
         if not version_stdout.strip():
             # raise Exception('Tried to parse semver from empty version output (is binary installed and available?)')
             return None
 
-        just_numbers = lambda col: col.lower().strip('v').split('+')[0].split('-')[0].split('_')[0]
+        just_numbers = lambda col: '.'.join(re.split(r'[\D]', col.lower().strip('v'), 4)[:3])  # split on any non-num character e.g. 5.2.26(1)-release -> ['5', '2', '26', '1', '', '', ...]
         contains_semver = lambda col: (
             col.count('.') in (1, 2, 3)
             and all(chunk.isdigit() for chunk in col.split('.')[:3])  # first 3 chunks can only be nums
         )
 
         full_text = version_stdout.split('\n')[0].strip()
-        first_line_columns = full_text.split()[:4]
+        first_line_columns = full_text.split()[:5]
         version_columns = list(filter(contains_semver, map(just_numbers, first_line_columns)))
         
         # could not find any column of first line that looks like a version number, despite there being some text
         if not version_columns:
             # raise Exception('Failed to parse semver from version command output: {}'.format(' '.join(first_line_columns)))
             return None
 
@@ -132,18 +133,18 @@
     #     )
 
 assert SemVer(None) == None
 assert SemVer('') == None
 assert SemVer.parse('') == None
 assert SemVer(1) == (1, 0, 0)
 assert SemVer(1, 2) == (1, 2, 0)
-assert SemVer('1.2+234234') == (1, 2, 0)
+assert SemVer('1.2+234234') == (1, 2, 234234)
 assert SemVer((1, 2, 3)) == (1, 2, 3)
 assert getattr(SemVer((1, 2, 3)), 'full_text') == '1.2.3'
 assert SemVer(('1', '2', '3')) == (1, 2, 3)
 assert SemVer.parse('5.6.7') == (5, 6, 7)
 assert SemVer.parse('124.0.6367.208') == (124, 0, 6367)
-assert SemVer.parse('Google Chrome 124.1+234.234') == (124, 1, 0)
+assert SemVer.parse('Google Chrome 124.1+234.234') == (124, 1, 234)
 assert SemVer.parse('Google Ch1rome 124.0.6367.208') == (124, 0, 6367)
 assert SemVer.parse('Google Chrome 124.0.6367.208+beta_234. 234.234.123\n123.456.324') == (124, 0, 6367)
 assert getattr(SemVer.parse('Google Chrome 124.0.6367.208+beta_234. 234.234.123\n123.456.324'), 'full_text') == 'Google Chrome 124.0.6367.208+beta_234. 234.234.123'
 assert SemVer.parse('Google Chrome') == None
```

### Comparing `pydantic_pkgr-0.1.1/pydantic_pkgr/views.py` & `pydantic_pkgr-0.1.2/pydantic_pkgr/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,76 +2,74 @@
 
 from django.http import HttpRequest
 from django.utils.html import format_html, mark_safe
 
 from admin_data_views.typing import TableContext, ItemContext
 from admin_data_views.utils import render_with_table_view, render_with_item_view, ItemLink
 
-from django.conf import settings
+from django.utils.module_loading import import_string
 
 from .binary import Binary
 
 
 def get_all_binaries() -> list[Binary]:
-    """Monkey patch this function implement getting the list of binaries to render"""
+    """Override this function implement getting the list of binaries to render"""
     return []
 
+def get_binary(name: str) -> Binary:
+    """Override this function implement getting the list of binaries to render"""
+
+    from . import settings
+
+    for binary in settings.PYDANTIC_PKGR_GET_ALL_BINARIES():
+        if binary.name == key:
+            return binary
+    return None
+
+
 
 @render_with_table_view
 def binaries_list_view(request: HttpRequest, **kwargs) -> TableContext:
 
     assert request.user.is_superuser, 'Must be a superuser to view configuration settings.'
 
+    from . import settings
+
     rows = {
         "Binary": [],
         "Found Version": [],
         "Provided By": [],
         "Found Abspath": [],
-        "Related Configuration": [],
         "Overrides": [],
         "Description": [],
     }
 
-    relevant_configs = {
-        key: val
-        for key, val in settings.CONFIG.items()
-        if '_BINARY' in key or '_VERSION' in key
-    }
-
-    for binary in get_all_binaries():
+    for binary in settings.get_all_pkgr_binaries():
         binary = binary.load_or_install()
 
         rows['Binary'].append(ItemLink(binary.name, key=binary.name))
         rows['Found Version'].append(binary.loaded_version)
         rows['Provided By'].append(binary.loaded_provider)
         rows['Found Abspath'].append(binary.loaded_abspath)
-        rows['Related Configuration'].append(mark_safe(', '.join(
-            f'<a href="/admin/environment/config/{config_key}/">{config_key}</a>'
-            for config_key, config_value in relevant_configs.items()
-                if binary.name.lower().replace('-', '').replace('_', '').replace('ytdlp', 'youtubedl') in config_key.lower()
-                # or binary.name.lower().replace('-', '').replace('_', '') in str(config_value).lower()
-        )))
         rows['Overrides'].append(str(binary.provider_overrides))
         rows['Description'].append(binary.description)
 
     return TableContext(
         title="Binaries",
         table=rows,
     )
 
 @render_with_item_view
 def binary_detail_view(request: HttpRequest, key: str, **kwargs) -> ItemContext:
 
     assert request.user.is_superuser, 'Must be a superuser to view configuration settings.'
 
-    binary = None
-    for loaded_binary in get_all_binaries():
-        if loaded_binary.name == key:
-            binary = loaded_binary
+    from . import settings
 
+    binary = settings.get_pkgr_binary(key)
 
     assert binary, f'Could not find a binary matching the specified name: {key}'
 
     binary = binary.load_or_install()
 
     return ItemContext(
         slug=key,
@@ -80,14 +78,17 @@
             {
                 "name": binary.name,
                 "description": binary.description,
                 "fields": {
                     'binprovider': binary.loaded_provider,
                     'abspath': binary.loaded_abspath,
                     'version': binary.loaded_version,
+                    'is_script': binary.is_script,
+                    'is_executable': binary.is_executable,
+                    'is_valid': binary.is_valid,
                     'overrides': str(binary.provider_overrides),
                     'providers': str(binary.providers_supported),
                 },
                 "help_texts": {
                     # TODO
                 },
             },
```

### Comparing `pydantic_pkgr-0.1.1/pyproject.toml` & `pydantic_pkgr-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydantic-pkgr"
-version = "0.1.1"
+version = "0.1.2"
 description = "System package manager APIs in strongly typed Python"
 authors = [
     { name = "Nick Sweeting", email = "pydantic-pkgr-pyproject-toml@sweeting.me" },
 ]
 requires-python = ">=3.10"
 platform = "py3-none-any"
 dependencies = [
@@ -69,18 +69,21 @@
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "django>=4.0",
     "mypy>=1.10.0",
     "pyright",
+    "django>=4.0",
     "django-stubs>=5.0.0",
+    "django-admin-data-views>=0.3.1",
+    "django-pydantic-field>=0.3.9",
+    "django-jsonform>=2.22.0",
 ]
 
 [tool.mypy]
 mypy_path = "pydantic_pkgr"
 python_version = "3.10"
 warn_return_any = "True"
 warn_unused_configs = "True"
```

### Comparing `pydantic_pkgr-0.1.1/PKG-INFO` & `pydantic_pkgr-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-pkgr
-Version: 0.1.1
+Version: 0.1.2
 Summary: System package manager APIs in strongly typed Python
 Keywords: pydantic,packagemanager,apt,brew,pip,system,dependencies
 Author-Email: Nick Sweeting <pydantic-pkgr-pyproject-toml@sweeting.me>
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -27,76 +27,97 @@
 Project-URL: Donate, https://github.com/ArchiveBox/ArchiveBox/wiki/Donations
 Requires-Python: >=3.10
 Requires-Dist: typing-extensions>=4.11.0
 Requires-Dist: pydantic>=2.7.1
 Requires-Dist: pydantic-core>=2.18.2
 Description-Content-Type: text/markdown
 
-<h1><a href="https://github.com/ArchiveBox/pydantic-pkgr"><code>pydantic-pkgr</code></a> &nbsp; &nbsp; &nbsp; &nbsp; 📦  <small><code>apt</code>&nbsp; <code>brew</code>&nbsp; <code>pip</code>&nbsp; <code>npm</code> &nbsp;++</small><br/><sub>A typed Python API wrapper for common system package managers.</sub></h1>
+<h1><a href="https://github.com/ArchiveBox/pydantic-pkgr"><code>pydantic-pkgr</code></a> &nbsp; &nbsp; &nbsp; &nbsp; 📦  <small><code>apt</code>&nbsp; <code>brew</code>&nbsp; <code>pip</code>&nbsp; <code>npm</code> &nbsp;₊₊₊</small><br/><sub>Simple Pydantic interfaces for package managers + installed binaries.</sub></h1>
 <br/>
 
 [![PyPI][pypi-badge]][pypi]
 [![Python Version][version-badge]][pypi]
 [![Django Version][django-badge]][pypi]
 [![GitHub][licence-badge]][licence]
 [![GitHub Last Commit][repo-badge]][repo]
 <!--[![Downloads][downloads-badge]][pypi]-->
 
 <br/>
 
-**This is a [Python 3 library](https://pypi.org/project/pydantic-pkgr/) for installing & managing packages with a variety of package managers.**
+**This is a [Python library](https://pypi.org/project/pydantic-pkgr/) for installing & managing packages locally with a variety of package managers.**  
+It's designed to help Python apps check for and install local binaries at runtime.  
+
 
 ```shell
 pip install pydantic-pkgr
 ```
 
+
 > ✨ Built with [`pydantic`](https://pydantic-docs.helpmanual.io/) v2 for strong static typing guarantees and json import/export compatibility  
 > 📦 Provides consistent cross-platform interfaces for dependency resolution & installation at runtime  
 > 🌈 Supports [`django`](https://docs.djangoproject.com/en/5.0/) >= 4.0, [`django-ninja`](https://django-ninja.dev/), and OpenAPI + [`django-jsonform`](https://django-jsonform.readthedocs.io/) out-of-the-box  
-> 🦄 Plays well with [`pyinfra`](https://github.com/pyinfra-dev/pyinfra) and [`ansible`](https://github.com/ansible/ansible) for advanced orchestration use-cases
+> 🦄 Uses [`pyinfra`](https://github.com/pyinfra-dev/pyinfra) / [`ansible`](https://github.com/ansible/ansible) for the actual install operations whenever possible (with internal fallbacks)
 
 <sub><i>Built by <a href="https://github.com/ArchiveBox">ArchiveBox</a> to install & auto-update our extractor dependencies at runtime (<code>chrome</code>, <code>wget</code>, <code>curl</code>, etc.) on `macOS`/`Linux`/`Docker`.</i></sub>
 
 <br/>
 
+> [!WARNING]
+> This is [ALPHA] software under active development, not ready for production use yet.
+
+
 **Source Code**: [https://github.com/ArchiveBox/pydantic-pkgr/](https://github.com/ArchiveBox/pydantic-pkgr/)
 
 **Documentation**: [https://github.com/ArchiveBox/pydantic-pkgr/blob/main/README.md](https://github.com/ArchiveBox/pydantic-pkgr/blob/main/README.md)
 
 <br/>
 
 ```python
-from pydantic_pkgr import AptProvider
+from pydantic_pkgr import AptProvider, Binary
 
-# Example: Install curl using the apt provider
 apt = AptProvider()
 curl = apt.install('curl')
 
-print(curl.provider)                       # 'apt'
-print(curl.abspath)                        # Path('/usr/bin/curl')
-print(curl.version)                        # SemVer('7.81.0')
-curl.exec(['--version'])                   # curl 7.81.0 (x86_64-pc-linux-gnu) libcurl/7.81.0 ...
+print(curl.abspath, curl.version, curl.provider, curl.is_valid)  # Path('/usr/bin/curl') SemVer('7.81.0') 'apt' True
+
+proc = curl.exec(['-fsSL', 'https://example.com'])               # <!doctype html>...
 ```
 
 ```python
-from pydantic_pkgr import Binary, BinName, BinProvider
+from pydantic_pkgr import Binary, BinProvider, BrewProvider, EnvProvider
 
 # Example: Create a re-usable curl Binary object that defines its install methods
 curl = Binary(name='curl', providers=[BrewProvider(), EnvProvider()])
-curl = curl.install()
 
-print(curl.provider)                       # 'brew'
-print(curl.abspath)                        # Path('/opt/homebrew/bin/curl')
-print(curl.version)                        # SemVer('8.4.0')
-curl.exec(['--version'])                   # curl 8.4.0 (x86_64-apple-darwin23.0) libcurl/8.4.0 ...
+# or for nicer type checking ergonomics, use class-based definitions:
+class CurlBinary(Binary):
+    name: str = 'curl'
+    providers list[BinProvider] = [BrewProvider(), EnvProvider()]
+curl = CurlBinary()
+
+# it works the same either way
+curl = curl.install()
+print(curl.abspath, curl.version, curl.provider, curl.is_valid)  # Path('/opt/homebrew/bin/curl') SemVer('8.4.0') 'brew' True
+curl.exec(['--version'])                                         # curl 8.4.0 (x86_64-apple-darwin23.0) libcurl/8.4.0 ...
 ```
 
 ```python
-print(curl.model_dump_json())              # ... everything can also be dumped/loaded as json
-print(curl.model_json_schema())            # ... all types provide OpenAPI-ready JSON schemas
+from pyinfra.operations import apt
+from pydantic_pkgr import Binary
+
+# Example: Verify & use packages installed by other tools (e.g. pyinfra/ansible)
+apt.packages(name="Install ffmpeg", packages=['ffmpeg'], _sudo=True)
+
+# Load it as a Binary provides a nice type-checkable, validated, serializable handle for it
+ffmpeg = Binary(name='ffmpeg').load()
+ffmpeg.exec(['-i', 'input.mp4', 'output.avi'])
+
+print(ffmpeg)                       # name=ffmpeg abspath=/usr/bin/ffmpeg version=3.3.0 is_valid=True
+print(ffmpeg.model_dump_json())     # ... everything can also be dumped/loaded as json
+print(ffmpeg.model_json_schema())   # ... all types provide OpenAPI-ready JSON schemas
 ```
 
 ### Supported Package Managers
 
 **So far it supports `installing`/`finding installed`/~~`updating`/`removing`~~ packages on `Linux`/`macOS` with:**
 
 - `apt` (Ubuntu/Debian/etc.)
@@ -200,24 +221,24 @@
 class DockerBinary(Binary):
     name: BinName = 'docker'
 
     providers_supported: List[BinProvider] = [EnvProvider(), AptProvider()]
     
     provider_overrides: Dict[BinProviderName, ProviderLookupDict] = {
         'env': {
-            # prefer podman if installed (or fall back to docker)
+            # example: prefer podman if installed (falling back to docker)
             'abspath': lambda: os.which('podman') or os.which('docker') or os.which('docker-ce'),
         },
         'apt': {
-            # install docker OR docker-ce (varies based on CPU architecture)
+            # example: vary installed package name based on your CPU architecture
             'subdeps': lambda: {
                 'amd64': 'docker',
                 'armv7l': 'docker-ce',
                 'arm64': 'docker-ce',
-            }.get(platform.machine()) or 'docker',
+            }.get(platform.machine(), 'docker'),
         },
     }
 
 docker = DockerBinary().load_or_install()
 print(docker.provider)                    # 'env'
 print(docker.abspath)                     # Path('/usr/local/bin/podman')
 print(docker.version)                     # SemVer('6.0.2')
@@ -240,14 +261,19 @@
 
 ### Example: Use the SemVer type directly for parsing & verifying version strings
 SemVer.parse('Google Chrome 124.0.6367.208+beta_234. 234.234.123')  # SemVer(124, 0, 6367')
 SemVer.parse('2024.04.05)                                           # SemVer(2024, 4, 5)
 SemVer.parse('1.9+beta')                                            # SemVer(1, 9, 0)
 str(SemVer(1, 9, 0))                                                # '1.9.0'
 ```
+<br/>
+
+> These types are all meant to be used library-style to make writing your own apps easier.  
+> e.g. you can use it to build things like: [`playwright install --with-deps`](https://playwright.dev/docs/browsers#install-system-dependencies))
+
 
 <br/>
 
 ---
 
 <br/>
 
@@ -276,54 +302,60 @@
 
 
 Usage in your `models.py`:
 ```python
 from django.db import models
 from django_pydantic_field import SchemaField
 
-from pydantic_pkgr import BinProvider, EnvProvider, Binary
+from pydantic_pkgr import BinProvider, EnvProvider, Binary, SemVer
 
 DEFAULT_PROVIDER = EnvProvider()
 
-class MyModel(models.Model):
-    ...
-
-    # SchemaField supports storing a single BinProvider/Binary in a field...
-    favorite_binprovider: BinProvider = SchemaField(default=DEFAULT_PROVIDER)
+class Dependency(models.Model):
+    """Example model for storing information about a dependency"""
 
-    # ... or inside a collection type like list[...] dict[...]
-    optional_binaries: list[Binary] = SchemaField(default=[])
+    name = models.CharField(max_length=63)
+    min_version: SemVer = SchemaField(default=(0,0,1))
+    binaries: list[Binary] = SchemaField(default=[])
+    default_binprovider: BinProvider = SchemaField(default=DEFAULT_PROVIDER)
 
 curl = Binary(name='curl', providers=[DEFAULT_PROVIDER]).load()
 
-obj = MyModel(optional_binaries=[curl])
+obj = Dependency(default_binprovider=DEFAULT_PROVIDER, binaries=[curl], min_version=SemVer('0.1.5'))
 obj.save()
 
-assert obj.favorite_binprovider == DEFAULT_PROVIDER
-assert obj.optional_binaries[0].provider == DEFAULT_PROVIDER
+assert obj.default_binprovider == DEFAULT_PROVIDER
+assert obj.binaries[0].provider == DEFAULT_PROVIDER
 ```
+*For a full example see our provided [`django_example_project/`](https://github.com/ArchiveBox/pydantic-pkgr/tree/main/django_example_project)...*
 
 <br/>
 
 ### Django Admin Usage: Show read-only list of Binaries in Admin UI
 
+<img height="220" alt="Django Admin binaries list view" src="https://github.com/ArchiveBox/pydantic-pkgr/assets/511499/a9980217-f39e-434e-b266-20cd6feb17c3" align="top"><img height="220" alt="Django Admin binaries detail view" src="https://github.com/ArchiveBox/pydantic-pkgr/assets/511499/d4d9086e-c8f4-4b6e-8ee8-8c8a864715b0" align="top">
+
 ```bash
 pip install pydantic-pkgr django-admin-data-views
 ```
 *For more info see the [`django-admin-data-views`](https://github.com/MrThearMan/django-admin-data-views) docs...*
 
 Then add this to your `settings.py`:
 ```python
 INSTALLED_APPS = [
     # ...
     'admin_data_views'
     'pydantic_pkgr'
     # ...
 ]
 
+# point these to a function that gets the list of all binaries / a single binary
+PYDANTIC_PKGR_GET_ALL_BINARIES = 'pydantic_pkgr.views.get_all_binaries'
+PYDANTIC_PKGR_GET_BINARY = 'pydantic_pkgr.views.get_binary'
+
 ADMIN_DATA_VIEWS = {
     "NAME": "Environment",
     "URLS": [
         {
             "route": "binaries/",
             "view": "pydantic_pkgr.views.binaries_list_view",
             "name": "binaries",
@@ -333,14 +365,15 @@
                 "name": "binary",
             },
         },
         # Coming soon: binprovider_list_view + binprovider_detail_view ...
     ],
 }
 ```
+*For a full example see our provided [`django_example_project/`](https://github.com/ArchiveBox/pydantic-pkgr/tree/main/django_example_project)...*
 
 <details>
 <summary><i>Note: If you override the default site admin, you must register the views manually...</i></summary>
 <br/><br/>
 <b><code>admin.py</code>:</b>
 <br/>
 <pre><code>
@@ -354,17 +387,25 @@
 from pydantic_pkgr.admin import register_admin_views
 register_admin_views(custom_admin)
 </code></pre>
 </details>
 
 <br/>
 
-### Django Admin Usage: JSONFormWidget for editing `BinProvider` and `Binary` data
+### ~~Django Admin Usage: JSONFormWidget for editing `BinProvider` and `Binary` data~~
+
+<img src="https://github.com/ArchiveBox/pydantic-pkgr/assets/511499/63705a57-4f62-4dbe-9f3a-0515323d8b5e" width="600px"/>
+
+> [!IMPORTANT]
+> This feature is coming soon but is blocked on a few issues being fixed first:  
+> - https://github.com/surenkov/django-pydantic-field/issues/64
+> - https://github.com/surenkov/django-pydantic-field/issues/65
+> - https://github.com/surenkov/django-pydantic-field/issues/66
 
-Install `django-jsonform` to get auto-generated Forms for editing BinProvider, Binary, etc. data
+~~Install `django-jsonform` to get auto-generated Forms for editing BinProvider, Binary, etc. data~~
 ```bash
 pip install django-pydantic-field django-jsonform
 ```
 *For more info see the [`django-jsonform`](https://django-jsonform.readthedocs.io/) docs...*
 
 `admin.py`:
 ```python
@@ -373,14 +414,15 @@
 from django_pydantic_field.v2.fields import PydanticSchemaField
 
 class MyModelAdmin(admin.ModelAdmin):
     formfield_overrides = {PydanticSchemaField: {"widget": JSONFormWidget}}
 
 admin.site.register(MyModel, MyModelAdmin)
 ```
+*For a full example see our provided [`django_example_project/`](https://github.com/ArchiveBox/pydantic-pkgr/tree/main/django_example_project)...*
 
 <br/>
 
 ---
 
 <br/>
```

