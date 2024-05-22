# Comparing `tmp/gceimgutils-0.12.0.tar.gz` & `tmp/gceimgutils-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gceimgutils-0.12.0.tar", last modified: Wed May 22 14:57:47 2024, max compression
+gzip compressed data, was "gceimgutils-0.9.1.tar", last modified: Mon Jul 19 21:31:53 2021, max compression
```

## Comparing `gceimgutils-0.12.0.tar` & `gceimgutils-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:47.128486 gceimgutils-0.12.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-22 14:57:47.128486 gceimgutils-0.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     3510 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/gcelistimg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4498 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/gceremoveimg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:47.120487 gceimgutils-0.12.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:47.124487 gceimgutils-0.12.0/lib/gceimgutils/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/lib/gceimgutils/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/lib/gceimgutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/lib/gceimgutils/gceimgutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/lib/gceimgutils/gceimgutilsExceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/lib/gceimgutils/gcelistimg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/lib/gceimgutils/gceremoveimg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/lib/gceimgutils/gceutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:47.128486 gceimgutils-0.12.0/lib/gceimgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-22 14:57:47.000000 gceimgutils-0.12.0/lib/gceimgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 14:57:47.000000 gceimgutils-0.12.0/lib/gceimgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:57:47.000000 gceimgutils-0.12.0/lib/gceimgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 14:57:47.000000 gceimgutils-0.12.0/lib/gceimgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 14:57:47.000000 gceimgutils-0.12.0/lib/gceimgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:47.120487 gceimgutils-0.12.0/man/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:47.128486 gceimgutils-0.12.0/man/man1/
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/man/man1/gcelistimg.1
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/man/man1/gceremoveimg.1
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 14:57:47.128486 gceimgutils-0.12.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2830 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:47.124487 gceimgutils-0.12.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:47.128486 gceimgutils-0.12.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/test/data/fake_credentials.json
--rw-r--r--   0 runner    (1001) docker     (127)    29717 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/test/data/image_data.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:57:47.128486 gceimgutils-0.12.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-22 14:57:39.000000 gceimgutils-0.12.0/test/unit/test_gceutils.py
+drwxr-xr-x   0 smarlow   (1000) users      (100)        0 2021-07-19 21:31:53.947007 gceimgutils-0.9.1/
+-rw-r--r--   0 smarlow   (1000) users      (100)    35149 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/LICENSE
+-rw-r--r--   0 smarlow   (1000) users      (100)      259 2021-07-19 16:39:35.000000 gceimgutils-0.9.1/MANIFEST.in
+-rw-r--r--   0 smarlow   (1000) users      (100)     1138 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/Makefile
+-rw-r--r--   0 smarlow   (1000) users      (100)     3571 2021-07-19 21:31:53.947007 gceimgutils-0.9.1/PKG-INFO
+-rw-r--r--   0 smarlow   (1000) users      (100)     1871 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/README.md
+-rwxr-xr-x   0 smarlow   (1000) users      (100)     3510 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/gcelistimg
+-rwxr-xr-x   0 smarlow   (1000) users      (100)     4498 2021-07-19 17:08:14.000000 gceimgutils-0.9.1/gceremoveimg
+drwxr-xr-x   0 smarlow   (1000) users      (100)        0 2021-07-19 21:31:53.943006 gceimgutils-0.9.1/lib/
+drwxr-xr-x   0 smarlow   (1000) users      (100)        0 2021-07-19 21:31:53.943006 gceimgutils-0.9.1/lib/gceimgutils/
+-rw-r--r--   0 smarlow   (1000) users      (100)        6 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/lib/gceimgutils/VERSION
+-rw-r--r--   0 smarlow   (1000) users      (100)        0 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/lib/gceimgutils/__init__.py
+-rw-r--r--   0 smarlow   (1000) users      (100)     1803 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/lib/gceimgutils/gceimgutils.py
+-rw-r--r--   0 smarlow   (1000) users      (100)      861 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/lib/gceimgutils/gceimgutilsExceptions.py
+-rw-r--r--   0 smarlow   (1000) users      (100)     3170 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/lib/gceimgutils/gcelistimg.py
+-rw-r--r--   0 smarlow   (1000) users      (100)     6043 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/lib/gceimgutils/gceremoveimg.py
+-rw-r--r--   0 smarlow   (1000) users      (100)     5799 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/lib/gceimgutils/gceutils.py
+drwxr-xr-x   0 smarlow   (1000) users      (100)        0 2021-07-19 21:31:53.947007 gceimgutils-0.9.1/lib/gceimgutils.egg-info/
+-rw-r--r--   0 smarlow   (1000) users      (100)     3571 2021-07-19 21:31:53.000000 gceimgutils-0.9.1/lib/gceimgutils.egg-info/PKG-INFO
+-rw-r--r--   0 smarlow   (1000) users      (100)      573 2021-07-19 21:31:53.000000 gceimgutils-0.9.1/lib/gceimgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 smarlow   (1000) users      (100)        1 2021-07-19 21:31:53.000000 gceimgutils-0.9.1/lib/gceimgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 smarlow   (1000) users      (100)      114 2021-07-19 21:31:53.000000 gceimgutils-0.9.1/lib/gceimgutils.egg-info/requires.txt
+-rw-r--r--   0 smarlow   (1000) users      (100)       12 2021-07-19 21:31:53.000000 gceimgutils-0.9.1/lib/gceimgutils.egg-info/top_level.txt
+drwxr-xr-x   0 smarlow   (1000) users      (100)        0 2021-07-19 21:31:53.943006 gceimgutils-0.9.1/man/
+drwxr-xr-x   0 smarlow   (1000) users      (100)        0 2021-07-19 21:31:53.947007 gceimgutils-0.9.1/man/man1/
+-rw-r--r--   0 smarlow   (1000) users      (100)     1857 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/man/man1/gcelistimg.1
+-rw-r--r--   0 smarlow   (1000) users      (100)     2198 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/man/man1/gceremoveimg.1
+-rw-r--r--   0 smarlow   (1000) users      (100)       52 2021-07-19 17:06:23.000000 gceimgutils-0.9.1/requirements-dev.txt
+-rw-r--r--   0 smarlow   (1000) users      (100)       76 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/requirements.txt
+-rw-r--r--   0 smarlow   (1000) users      (100)      226 2021-07-19 21:31:53.947007 gceimgutils-0.9.1/setup.cfg
+-rwxr-xr-x   0 smarlow   (1000) users      (100)     2774 2021-07-19 16:20:57.000000 gceimgutils-0.9.1/setup.py
```

### Comparing `gceimgutils-0.12.0/LICENSE` & `gceimgutils-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gceimgutils-0.12.0/Makefile` & `gceimgutils-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `gceimgutils-0.12.0/README.md` & `gceimgutils-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `gceimgutils-0.12.0/gcelistimg` & `gceimgutils-0.9.1/gcelistimg`

 * *Files identical despite different names*

### Comparing `gceimgutils-0.12.0/gceremoveimg` & `gceimgutils-0.9.1/gceremoveimg`

 * *Files identical despite different names*

### Comparing `gceimgutils-0.12.0/lib/gceimgutils/gceimgutils.py` & `gceimgutils-0.9.1/lib/gceimgutils/gceimgutils.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,42 +26,31 @@
     # ---------------------------------------------------------------------
     def __init__(
             self, project, credentials_path,
             log_level=logging.INFO, log_callback=None
     ):
 
         self.project = project
-        self.credentials_path = credentials_path
-        self._credentials = None
-        self._compute_driver = None
+        self.credentials = None
 
         if log_callback:
             self.log = log_callback
         else:
             logger = logging.getLogger('gceimgutils')
             logger.setLevel(log_level)
             self.log = logger
 
         try:
             self.log_level = self.log.level
         except AttributeError:
             self.log_level = self.log.logger.level  # LoggerAdapter
 
-    # ---------------------------------------------------------------------
-    @property
-    def compute_driver(self):
-        """Get an authenticated compute driver"""
-        if not self._compute_driver:
-            self._compute_driver = utils.get_compute_api(self.credentials)
-
-        return self._compute_driver
+        try:
+            self.credentials = utils.get_credentials(project, credentials_path)
+        except Exception as err:
+            self.log.error(format(err))
 
     # ---------------------------------------------------------------------
-    @property
-    def credentials(self):
-        if not self._credentials:
-            self._credentials = utils.get_credentials(
-                self.project,
-                self.credentials_path
-            )
+    def _get_api(self):
+        """Set up the API"""
 
-        return self._credentials
+        return utils.get_compute_api(self.credentials)
```

### Comparing `gceimgutils-0.12.0/lib/gceimgutils/gceimgutilsExceptions.py` & `gceimgutils-0.9.1/lib/gceimgutils/gceimgutilsExceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,21 +12,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with gceimgutils.  If not, see <http://www.gnu.org/licenses/>.
 
 
-class GCEImgUtilsException(Exception):
+class GCEProjectCredentialsException(Exception):
     pass
 
 
-class GCEProjectCredentialsException(GCEImgUtilsException):
+class GCERemoveImgException(Exception):
     pass
 
 
-class GCERemoveImgException(GCEImgUtilsException):
-    pass
-
-
-class GCEListImgException(GCEImgUtilsException):
+class GCEListImgException(Exception):
     pass
```

### Comparing `gceimgutils-0.12.0/lib/gceimgutils/gcelistimg.py` & `gceimgutils-0.9.1/lib/gceimgutils/gcelistimg.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,17 +49,15 @@
         self.image_name_match = image_name_match
         self.detail = detail
 
     # ---------------------------------------------------------------------
     def get_images(self):
         """Get images from sdk"""
         owned_images = utils.get_project_images(
-            self.compute_driver,
-            self.project,
-            True
+            self.project, self.credentials, True
         )
 
         if self.image_name:
             return utils.find_images_by_name(
                 owned_images,
                 self.image_name,
                 self.log
@@ -78,22 +76,22 @@
                     self.log
                 )
             except Exception:
                 msg = 'Unable to complie regular expression "%s"'
                 msg = msg % self.image_name_match
                 raise GCEListImgException(msg)
         else:
-            return owned_images
+            return(owned_images)
 
     # ---------------------------------------------------------------------
     def list_images(self):
         """List the images"""
         images = self.get_images()
 
         if not images:
             raise GCEListImgException('No Images found')
 
         for image in images:
             if self.detail or self.image_name:
-                self.log.info(json.dumps(image, indent=4))
+                print(json.dumps(image, indent=4))
             else:
-                self.log.info(image['name'])
+                print(image['name'])
```

### Comparing `gceimgutils-0.12.0/lib/gceimgutils/gceremoveimg.py` & `gceimgutils-0.9.1/lib/gceimgutils/gceremoveimg.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,17 +72,15 @@
 
         return True
 
     # ---------------------------------------------------------------------
     def _get_images_to_remove(self):
         """Find the images to remove"""
         owned_images = utils.get_project_images(
-            self.compute_driver,
-            self.project,
-            True
+            self.project, self.credentials, True
         )
         if self.image_name:
             return utils.find_images_by_name(
                 owned_images,
                 self.image_name,
                 self.log
             )
@@ -128,45 +126,36 @@
             self.log.info('\t\t%s' % image.get('name'))
 
         return True
 
     # ---------------------------------------------------------------------
     def remove_images(self):
         """Remove the images"""
+        api = self._get_api()
         images = self._get_images_to_remove()
         images_ok = self._check_images_boundary_condition(images)
 
         if not images_ok:
             raise GCERemoveImgException('Image ambiguity')
 
         for image in images:
-            try:
-                self.remove_image(image.get('name'))
-            except GCERemoveImgException:
-                pass  # If an image fails it is logged
-
-    # ---------------------------------------------------------------------
-    def remove_image(self, image_name):
-        """Remove the image"""
-        delete = True
-        if self.confirm:
-            delete = self._query_yes_no(image_name)
-
-        if delete:
-            try:
-                self.compute_driver.images().delete(
-                    project=self.project, image=image_name
-                ).execute()
-            except HttpError as error:
-                msg = 'Unable to remove image: "{image}". {error}'.format(
-                    image=image_name,
-                    error=error
-                )
-                self.log.error(msg)
-                raise GCERemoveImgException(msg) from error
+            delete = True
+            if self.confirm:
+                delete = self._query_yes_no(image)
+
+            if delete:
+                image_name = image.get('name')
+                try:
+                    api.images().delete(
+                        project=self.project, image=image_name
+                    ).execute()
+                except HttpError:
+                    self.log.error('Unable to remove image: "%s"' % image_name)
+            else:
+                continue
 
     # ---------------------------------------------------------------------
     def _query_yes_no(self, image):
         yes = {'yes', 'y', 'ye', ''}
         no = {'no', 'n'}
 
         while True:
```

### Comparing `gceimgutils-0.12.0/lib/gceimgutils/gceutils.py` & `gceimgutils-0.9.1/lib/gceimgutils/gceutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # along with gceimgutils.ase.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import os
 import re
 
 from google.oauth2 import service_account
-from google.auth.exceptions import RefreshError
-from google.auth.transport.requests import AuthorizedSession
 from googleapiclient import discovery
 
 from gceimgutils.gceimgutilsExceptions import (
     GCEProjectCredentialsException
 )
 
 from googleapiclient.errors import HttpError
 
+compute_api = None
+
 
 # ----------------------------------------------------------------------------
 def find_images_by_name(images, image_name, log_callback):
     """Return a list of images that match the given name."""
     matching_images = []
     for image in images:
         if not image.get('name'):
@@ -98,33 +98,17 @@
                 '"%s" credentials not found' % credentials_file
             )
 
     try:
         credentials = service_account.Credentials.from_service_account_file(
             credentials_file
         )
-    except Exception as error:
-        raise GCEProjectCredentialsException(
-            'Could not extract credentials from "{credentials_file}": '
-            '{error}'.format(credentials_file=credentials_file, error=error)
-        )
-
-    try:
-        # https://developers.google.com/identity/protocols/oauth2/scopes#google-sign-in
-        scoped_credentials = credentials.with_scopes(['profile'])
-        authed_session = AuthorizedSession(scoped_credentials)
-        authed_session.get('https://www.googleapis.com/oauth2/v2/userinfo')
-    except RefreshError:
-        raise GCEProjectCredentialsException(
-            'The provided credentials are invalid or expired: '
-            '{creds_file}'.format(creds_file=credentials_file)
-        )
-    except Exception as error:
+    except Exception:
         raise GCEProjectCredentialsException(
-            'GCP authentication failed: {error}'.format(error=error)
+            'Could not extract credentials from "%s"' % credentials_file
         )
 
     return credentials
 
 
 # ----------------------------------------------------------------------------
 def get_logger(verbose):
@@ -144,20 +128,20 @@
     console_handler.setFormatter(logging.Formatter('%(message)s'))
 
     logger.addHandler(console_handler)
     return logger
 
 
 # ----------------------------------------------------------------------------
-def get_project_images(compute_driver, project_name, deprecated=False):
+def get_project_images(project_name, credentials, deprecated=False):
     """Get the images owned by the given project"""
 
     current_images = []
     try:
-        response = compute_driver.images().list(
+        response = get_compute_api(credentials).images().list(
             project=project_name).execute()
     except HttpError:
         return current_images
 
     for image in response.get('items'):
         if not deprecated and image.get('deprecated'):
             continue
@@ -173,16 +157,20 @@
     version = open(os.path.join(base_path, version_file_name), 'r').read()
     return version.rstrip('\n')
 
 
 # ----------------------------------------------------------------------------
 def get_compute_api(credentials):
     """Build the compute API"""
+    global compute_api
+
+    if not compute_api:
+        compute_api = discovery.build('compute', 'v1', credentials=credentials)
 
-    return discovery.build('compute', 'v1', credentials=credentials)
+    return compute_api
 
 
 # ----------------------------------------------------------------------------
 def _no_name_warning(image, log_callback):
     """Print a warning for images that have no name"""
     msg = 'WARNING: Found image with no name, ignoring for search results. '
     msg += 'Image ID: %s' % image['ImageId']
```

### Comparing `gceimgutils-0.12.0/man/man1/gcelistimg.1` & `gceimgutils-0.9.1/man/man1/gcelistimg.1`

 * *Files identical despite different names*

### Comparing `gceimgutils-0.12.0/man/man1/gceremoveimg.1` & `gceimgutils-0.9.1/man/man1/gceremoveimg.1`

 * *Files identical despite different names*

### Comparing `gceimgutils-0.12.0/setup.py` & `gceimgutils-0.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,17 +65,16 @@
             'Development Status :: 4 - Beta',
             'Intended Audience :: Developers',
             'Natural Language :: English',
             'License :: OSI Approved :: '
             'GNU General Public License v3 or later (GPLv3+)',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
+            'Programming Language :: Python :: 3.4',
+            'Programming Language :: Python :: 3.5',
+            'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
-            'Programming Language :: Python :: 3.9',
-            'Programming Language :: Python :: 3.10',
-            'Programming Language :: Python :: 3.11',
-            'Programming Language :: Python :: 3.12',
             'Programming Language :: Python :: Implementation :: CPython',
             'Programming Language :: Python :: Implementation :: PyPy',
         ]
     )
```

