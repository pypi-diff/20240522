# Comparing `tmp/rebootpy-0.0.1.tar.gz` & `tmp/rebootpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rebootpy-0.0.1.tar", last modified: Mon May 20 10:29:50 2024, max compression
+gzip compressed data, was "rebootpy-0.0.2.tar", last modified: Wed May 22 13:56:53 2024, max compression
```

## Comparing `rebootpy-0.0.1.tar` & `rebootpy-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-20 10:29:50.074390 rebootpy-0.0.1/
--rw-r--r--   0 oli        (501) staff       (20)     1068 2024-05-17 03:38:25.000000 rebootpy-0.0.1/LICENSE
--rw-r--r--   0 oli        (501) staff       (20)     3732 2024-05-20 10:29:50.073811 rebootpy-0.0.1/PKG-INFO
--rw-r--r--   0 oli        (501) staff       (20)     2381 2024-05-20 09:49:15.000000 rebootpy-0.0.1/README.md
-drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-20 10:29:50.063531 rebootpy-0.0.1/rebootpy/
--rw-rw-r--   0 oli        (501) staff       (20)     2289 2024-05-20 03:54:25.000000 rebootpy-0.0.1/rebootpy/__init__.py
--rw-rw-r--   0 oli        (501) staff       (20)    40394 2024-05-20 03:21:44.000000 rebootpy-0.0.1/rebootpy/auth.py
--rw-rw-r--   0 oli        (501) staff       (20)     1742 2022-12-18 00:25:45.000000 rebootpy-0.0.1/rebootpy/avatar.py
--rw-rw-r--   0 oli        (501) staff       (20)   125925 2024-05-20 08:46:28.000000 rebootpy-0.0.1/rebootpy/client.py
--rw-rw-r--   0 oli        (501) staff       (20)     9316 2024-05-20 06:46:15.000000 rebootpy-0.0.1/rebootpy/enums.py
--rw-rw-r--   0 oli        (501) staff       (20)     7758 2024-05-16 14:14:46.000000 rebootpy-0.0.1/rebootpy/errors.py
-drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-20 10:29:50.051787 rebootpy-0.0.1/rebootpy/ext/
-drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-20 10:29:50.072052 rebootpy-0.0.1/rebootpy/ext/commands/
--rw-rw-r--   0 oli        (501) staff       (20)      195 2022-12-18 00:25:45.000000 rebootpy-0.0.1/rebootpy/ext/commands/__init__.py
--rw-rw-r--   0 oli        (501) staff       (20)     1130 2022-12-18 00:25:45.000000 rebootpy-0.0.1/rebootpy/ext/commands/_types.py
--rw-rw-r--   0 oli        (501) staff       (20)    32166 2024-05-16 14:14:59.000000 rebootpy-0.0.1/rebootpy/ext/commands/bot.py
--rw-rw-r--   0 oli        (501) staff       (20)    15372 2024-05-16 14:16:32.000000 rebootpy-0.0.1/rebootpy/ext/commands/cog.py
--rw-rw-r--   0 oli        (501) staff       (20)    11670 2024-05-16 14:16:36.000000 rebootpy-0.0.1/rebootpy/ext/commands/context.py
--rw-rw-r--   0 oli        (501) staff       (20)     6099 2024-05-16 14:16:38.000000 rebootpy-0.0.1/rebootpy/ext/commands/converter.py
--rw-rw-r--   0 oli        (501) staff       (20)     8382 2024-05-16 14:16:39.000000 rebootpy-0.0.1/rebootpy/ext/commands/cooldown.py
--rw-rw-r--   0 oli        (501) staff       (20)    60249 2024-05-16 14:16:40.000000 rebootpy-0.0.1/rebootpy/ext/commands/core.py
--rw-rw-r--   0 oli        (501) staff       (20)    14399 2024-05-16 14:16:42.000000 rebootpy-0.0.1/rebootpy/ext/commands/errors.py
--rw-rw-r--   0 oli        (501) staff       (20)    50683 2024-05-16 14:16:45.000000 rebootpy-0.0.1/rebootpy/ext/commands/help.py
--rw-rw-r--   0 oli        (501) staff       (20)     1212 2024-05-16 14:16:49.000000 rebootpy-0.0.1/rebootpy/ext/commands/typedefs.py
--rw-rw-r--   0 oli        (501) staff       (20)     6204 2022-12-18 00:25:45.000000 rebootpy-0.0.1/rebootpy/ext/commands/view.py
--rw-rw-r--   0 oli        (501) staff       (20)    18921 2024-05-16 14:15:37.000000 rebootpy-0.0.1/rebootpy/friend.py
--rw-rw-r--   0 oli        (501) staff       (20)    62083 2024-05-19 20:51:08.000000 rebootpy-0.0.1/rebootpy/http.py
--rw-rw-r--   0 oli        (501) staff       (20)     3852 2024-05-16 14:15:45.000000 rebootpy-0.0.1/rebootpy/message.py
--rw-rw-r--   0 oli        (501) staff       (20)     2670 2024-05-16 14:15:48.000000 rebootpy-0.0.1/rebootpy/news.py
--rw-rw-r--   0 oli        (501) staff       (20)   155598 2024-05-20 09:07:00.000000 rebootpy-0.0.1/rebootpy/party.py
--rw-rw-r--   0 oli        (501) staff       (20)     3748 2024-05-16 14:15:54.000000 rebootpy-0.0.1/rebootpy/playlist.py
--rw-rw-r--   0 oli        (501) staff       (20)    12625 2024-05-16 14:15:56.000000 rebootpy-0.0.1/rebootpy/presence.py
--rw-rw-r--   0 oli        (501) staff       (20)    10138 2024-05-20 07:06:08.000000 rebootpy-0.0.1/rebootpy/stats.py
--rw-rw-r--   0 oli        (501) staff       (20)     8894 2024-05-20 04:12:04.000000 rebootpy-0.0.1/rebootpy/store.py
--rw-rw-r--   0 oli        (501) staff       (20)     1361 2024-05-16 14:16:04.000000 rebootpy-0.0.1/rebootpy/typedefs.py
--rw-rw-r--   0 oli        (501) staff       (20)    22856 2024-05-16 14:16:43.000000 rebootpy-0.0.1/rebootpy/user.py
--rw-rw-r--   0 oli        (501) staff       (20)     4414 2024-05-16 14:16:09.000000 rebootpy-0.0.1/rebootpy/utils.py
--rw-rw-r--   0 oli        (501) staff       (20)    58925 2024-05-20 02:17:38.000000 rebootpy-0.0.1/rebootpy/xmpp.py
-drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-20 10:29:50.072650 rebootpy-0.0.1/rebootpy.egg-info/
--rw-r--r--   0 oli        (501) staff       (20)     3732 2024-05-20 10:29:50.000000 rebootpy-0.0.1/rebootpy.egg-info/PKG-INFO
--rw-r--r--   0 oli        (501) staff       (20)      922 2024-05-20 10:29:50.000000 rebootpy-0.0.1/rebootpy.egg-info/SOURCES.txt
--rw-r--r--   0 oli        (501) staff       (20)        1 2024-05-20 10:29:50.000000 rebootpy-0.0.1/rebootpy.egg-info/dependency_links.txt
--rw-r--r--   0 oli        (501) staff       (20)      114 2024-05-20 10:29:50.000000 rebootpy-0.0.1/rebootpy.egg-info/requires.txt
--rw-r--r--   0 oli        (501) staff       (20)        9 2024-05-20 10:29:50.000000 rebootpy-0.0.1/rebootpy.egg-info/top_level.txt
--rw-r--r--   0 oli        (501) staff       (20)       38 2024-05-20 10:29:50.074489 rebootpy-0.0.1/setup.cfg
--rw-r--r--   0 oli        (501) staff       (20)     1889 2024-05-20 08:34:30.000000 rebootpy-0.0.1/setup.py
+drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-22 13:56:53.484225 rebootpy-0.0.2/
+-rw-r--r--   0 oli        (501) staff       (20)     1068 2024-05-17 03:38:25.000000 rebootpy-0.0.2/LICENSE
+-rw-r--r--   0 oli        (501) staff       (20)     3728 2024-05-22 13:56:53.483693 rebootpy-0.0.2/PKG-INFO
+-rw-r--r--   0 oli        (501) staff       (20)     2377 2024-05-20 10:38:52.000000 rebootpy-0.0.2/README.md
+drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-22 13:56:53.474032 rebootpy-0.0.2/rebootpy/
+-rw-rw-r--   0 oli        (501) staff       (20)     2289 2024-05-22 13:56:06.000000 rebootpy-0.0.2/rebootpy/__init__.py
+-rw-rw-r--   0 oli        (501) staff       (20)    40394 2024-05-20 03:21:44.000000 rebootpy-0.0.2/rebootpy/auth.py
+-rw-rw-r--   0 oli        (501) staff       (20)     1742 2022-12-18 00:25:45.000000 rebootpy-0.0.2/rebootpy/avatar.py
+-rw-rw-r--   0 oli        (501) staff       (20)   125925 2024-05-20 08:46:28.000000 rebootpy-0.0.2/rebootpy/client.py
+-rw-rw-r--   0 oli        (501) staff       (20)     9316 2024-05-20 06:46:15.000000 rebootpy-0.0.2/rebootpy/enums.py
+-rw-rw-r--   0 oli        (501) staff       (20)     7758 2024-05-16 14:14:46.000000 rebootpy-0.0.2/rebootpy/errors.py
+drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-22 13:56:53.462722 rebootpy-0.0.2/rebootpy/ext/
+drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-22 13:56:53.482012 rebootpy-0.0.2/rebootpy/ext/commands/
+-rw-rw-r--   0 oli        (501) staff       (20)      195 2022-12-18 00:25:45.000000 rebootpy-0.0.2/rebootpy/ext/commands/__init__.py
+-rw-rw-r--   0 oli        (501) staff       (20)     1130 2022-12-18 00:25:45.000000 rebootpy-0.0.2/rebootpy/ext/commands/_types.py
+-rw-rw-r--   0 oli        (501) staff       (20)    32166 2024-05-16 14:14:59.000000 rebootpy-0.0.2/rebootpy/ext/commands/bot.py
+-rw-rw-r--   0 oli        (501) staff       (20)    15372 2024-05-16 14:16:32.000000 rebootpy-0.0.2/rebootpy/ext/commands/cog.py
+-rw-rw-r--   0 oli        (501) staff       (20)    11670 2024-05-16 14:16:36.000000 rebootpy-0.0.2/rebootpy/ext/commands/context.py
+-rw-rw-r--   0 oli        (501) staff       (20)     6099 2024-05-16 14:16:38.000000 rebootpy-0.0.2/rebootpy/ext/commands/converter.py
+-rw-rw-r--   0 oli        (501) staff       (20)     8382 2024-05-16 14:16:39.000000 rebootpy-0.0.2/rebootpy/ext/commands/cooldown.py
+-rw-rw-r--   0 oli        (501) staff       (20)    60249 2024-05-16 14:16:40.000000 rebootpy-0.0.2/rebootpy/ext/commands/core.py
+-rw-rw-r--   0 oli        (501) staff       (20)    14399 2024-05-16 14:16:42.000000 rebootpy-0.0.2/rebootpy/ext/commands/errors.py
+-rw-rw-r--   0 oli        (501) staff       (20)    50683 2024-05-16 14:16:45.000000 rebootpy-0.0.2/rebootpy/ext/commands/help.py
+-rw-rw-r--   0 oli        (501) staff       (20)     1212 2024-05-16 14:16:49.000000 rebootpy-0.0.2/rebootpy/ext/commands/typedefs.py
+-rw-rw-r--   0 oli        (501) staff       (20)     6204 2022-12-18 00:25:45.000000 rebootpy-0.0.2/rebootpy/ext/commands/view.py
+-rw-rw-r--   0 oli        (501) staff       (20)    18921 2024-05-16 14:15:37.000000 rebootpy-0.0.2/rebootpy/friend.py
+-rw-rw-r--   0 oli        (501) staff       (20)    62083 2024-05-19 20:51:08.000000 rebootpy-0.0.2/rebootpy/http.py
+-rw-rw-r--   0 oli        (501) staff       (20)     3852 2024-05-16 14:15:45.000000 rebootpy-0.0.2/rebootpy/message.py
+-rw-rw-r--   0 oli        (501) staff       (20)     2670 2024-05-16 14:15:48.000000 rebootpy-0.0.2/rebootpy/news.py
+-rw-rw-r--   0 oli        (501) staff       (20)   155598 2024-05-20 09:07:00.000000 rebootpy-0.0.2/rebootpy/party.py
+-rw-rw-r--   0 oli        (501) staff       (20)     3748 2024-05-16 14:15:54.000000 rebootpy-0.0.2/rebootpy/playlist.py
+-rw-rw-r--   0 oli        (501) staff       (20)    12639 2024-05-22 13:55:12.000000 rebootpy-0.0.2/rebootpy/presence.py
+-rw-rw-r--   0 oli        (501) staff       (20)    10138 2024-05-20 07:06:08.000000 rebootpy-0.0.2/rebootpy/stats.py
+-rw-rw-r--   0 oli        (501) staff       (20)     8894 2024-05-20 04:12:04.000000 rebootpy-0.0.2/rebootpy/store.py
+-rw-rw-r--   0 oli        (501) staff       (20)     1361 2024-05-16 14:16:04.000000 rebootpy-0.0.2/rebootpy/typedefs.py
+-rw-rw-r--   0 oli        (501) staff       (20)    22856 2024-05-16 14:16:43.000000 rebootpy-0.0.2/rebootpy/user.py
+-rw-rw-r--   0 oli        (501) staff       (20)     4414 2024-05-16 14:16:09.000000 rebootpy-0.0.2/rebootpy/utils.py
+-rw-rw-r--   0 oli        (501) staff       (20)    58925 2024-05-20 02:17:38.000000 rebootpy-0.0.2/rebootpy/xmpp.py
+drwxr-xr-x   0 oli        (501) staff       (20)        0 2024-05-22 13:56:53.482578 rebootpy-0.0.2/rebootpy.egg-info/
+-rw-r--r--   0 oli        (501) staff       (20)     3728 2024-05-22 13:56:53.000000 rebootpy-0.0.2/rebootpy.egg-info/PKG-INFO
+-rw-r--r--   0 oli        (501) staff       (20)      922 2024-05-22 13:56:53.000000 rebootpy-0.0.2/rebootpy.egg-info/SOURCES.txt
+-rw-r--r--   0 oli        (501) staff       (20)        1 2024-05-22 13:56:53.000000 rebootpy-0.0.2/rebootpy.egg-info/dependency_links.txt
+-rw-r--r--   0 oli        (501) staff       (20)      114 2024-05-22 13:56:53.000000 rebootpy-0.0.2/rebootpy.egg-info/requires.txt
+-rw-r--r--   0 oli        (501) staff       (20)        9 2024-05-22 13:56:53.000000 rebootpy-0.0.2/rebootpy.egg-info/top_level.txt
+-rw-r--r--   0 oli        (501) staff       (20)       38 2024-05-22 13:56:53.484324 rebootpy-0.0.2/setup.cfg
+-rw-r--r--   0 oli        (501) staff       (20)     1889 2024-05-20 08:34:30.000000 rebootpy-0.0.2/setup.py
```

### Comparing `rebootpy-0.0.1/LICENSE` & `rebootpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/PKG-INFO` & `rebootpy-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rebootpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for interacting with fortnite services
 Home-page: https://github.com/xMistt/rebootpy
 Author: xMistt
 License: MIT
 Project-URL: Documentation, https://rebootpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/xMistt/rebootpy/issues
 Classifier: License :: OSI Approved :: MIT License
@@ -30,16 +30,16 @@
 Provides-Extra: docs
 Requires-Dist: sphinxcontrib_trio==1.1.2; extra == "docs"
 Requires-Dist: furo==2021.4.11b34; extra == "docs"
 Requires-Dist: Jinja2<3.1; extra == "docs"
 
  # rebootpy
 
-[![Supported py versions](https://img.shields.io/pypi/pyversions/fortnitepy.svg)](https://pypi.org/project/rebootpy/)
-[![Current pypi version](https://img.shields.io/pypi/v/fortnitepy.svg)](https://pypi.org/project/rebootpy/)
+[![Supported py versions](https://img.shields.io/pypi/pyversions/rebootpy.svg)](https://pypi.org/project/rebootpy/)
+[![Current pypi version](https://img.shields.io/pypi/v/rebootpy.svg)](https://pypi.org/project/rebootpy/)
 [![Donate link](https://img.shields.io/badge/paypal-donate-blue.svg)](https://www.paypal.me/terbau)
 
 Asynchronous library for interacting with Fortnite and EpicGames' API and XMPP services.
 
 This library is a fork of [Terbau](https://github.com/Terbau/)'s [fortnitepy](https://github.com/Terbau/fortnitepy) which was abandoned.
 
 **Note:** This library is still under developement so breaking changes might happen at any time.
```

### Comparing `rebootpy-0.0.1/README.md` & `rebootpy-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
  # rebootpy
 
-[![Supported py versions](https://img.shields.io/pypi/pyversions/fortnitepy.svg)](https://pypi.org/project/rebootpy/)
-[![Current pypi version](https://img.shields.io/pypi/v/fortnitepy.svg)](https://pypi.org/project/rebootpy/)
+[![Supported py versions](https://img.shields.io/pypi/pyversions/rebootpy.svg)](https://pypi.org/project/rebootpy/)
+[![Current pypi version](https://img.shields.io/pypi/v/rebootpy.svg)](https://pypi.org/project/rebootpy/)
 [![Donate link](https://img.shields.io/badge/paypal-donate-blue.svg)](https://www.paypal.me/terbau)
 
 Asynchronous library for interacting with Fortnite and EpicGames' API and XMPP services.
 
 This library is a fork of [Terbau](https://github.com/Terbau/)'s [fortnitepy](https://github.com/Terbau/fortnitepy) which was abandoned.
 
 **Note:** This library is still under developement so breaking changes might happen at any time.
```

### Comparing `rebootpy-0.0.1/rebootpy/__init__.py` & `rebootpy-0.0.2/rebootpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 from .client import (BasicClient, Client, run_multiple, start_multiple,
                      close_multiple)
 from .auth import (Auth, DeviceCodeAuth, ExchangeCodeAuth,
                    AuthorizationCodeAuth, DeviceAuth, RefreshTokenAuth,
                    AdvancedAuth)
 from .friend import Friend, IncomingPendingFriend, OutgoingPendingFriend
```

### Comparing `rebootpy-0.0.1/rebootpy/auth.py` & `rebootpy-0.0.2/rebootpy/auth.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/avatar.py` & `rebootpy-0.0.2/rebootpy/avatar.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/client.py` & `rebootpy-0.0.2/rebootpy/client.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/enums.py` & `rebootpy-0.0.2/rebootpy/enums.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/errors.py` & `rebootpy-0.0.2/rebootpy/errors.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/_types.py` & `rebootpy-0.0.2/rebootpy/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/bot.py` & `rebootpy-0.0.2/rebootpy/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/cog.py` & `rebootpy-0.0.2/rebootpy/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/context.py` & `rebootpy-0.0.2/rebootpy/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/converter.py` & `rebootpy-0.0.2/rebootpy/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/cooldown.py` & `rebootpy-0.0.2/rebootpy/ext/commands/cooldown.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/core.py` & `rebootpy-0.0.2/rebootpy/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/errors.py` & `rebootpy-0.0.2/rebootpy/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/help.py` & `rebootpy-0.0.2/rebootpy/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/typedefs.py` & `rebootpy-0.0.2/rebootpy/ext/commands/typedefs.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/ext/commands/view.py` & `rebootpy-0.0.2/rebootpy/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/friend.py` & `rebootpy-0.0.2/rebootpy/friend.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/http.py` & `rebootpy-0.0.2/rebootpy/http.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/message.py` & `rebootpy-0.0.2/rebootpy/message.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/news.py` & `rebootpy-0.0.2/rebootpy/news.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/party.py` & `rebootpy-0.0.2/rebootpy/party.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/playlist.py` & `rebootpy-0.0.2/rebootpy/playlist.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/presence.py` & `rebootpy-0.0.2/rebootpy/presence.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
                 raw_properties['FortGameplayStats_j'],
                 players_alive
             )
         else:
             self.gameplay_stats = None
 
         key = "party.joininfodata.286331153_j"
-        if key is None:
+        if key not in raw_properties:
             self.party = None
         else:
             self.party = PresenceParty(self.client, raw_properties[key])
 
     def __repr__(self) -> str:
         return ('<Presence friend={0.friend!r} available={0.available} '
                 'received_at={0.received_at!r}>'.format(self))
```

### Comparing `rebootpy-0.0.1/rebootpy/stats.py` & `rebootpy-0.0.2/rebootpy/stats.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/store.py` & `rebootpy-0.0.2/rebootpy/store.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/typedefs.py` & `rebootpy-0.0.2/rebootpy/typedefs.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/user.py` & `rebootpy-0.0.2/rebootpy/user.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/utils.py` & `rebootpy-0.0.2/rebootpy/utils.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy/xmpp.py` & `rebootpy-0.0.2/rebootpy/xmpp.py`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/rebootpy.egg-info/PKG-INFO` & `rebootpy-0.0.2/rebootpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rebootpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for interacting with fortnite services
 Home-page: https://github.com/xMistt/rebootpy
 Author: xMistt
 License: MIT
 Project-URL: Documentation, https://rebootpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/xMistt/rebootpy/issues
 Classifier: License :: OSI Approved :: MIT License
@@ -30,16 +30,16 @@
 Provides-Extra: docs
 Requires-Dist: sphinxcontrib_trio==1.1.2; extra == "docs"
 Requires-Dist: furo==2021.4.11b34; extra == "docs"
 Requires-Dist: Jinja2<3.1; extra == "docs"
 
  # rebootpy
 
-[![Supported py versions](https://img.shields.io/pypi/pyversions/fortnitepy.svg)](https://pypi.org/project/rebootpy/)
-[![Current pypi version](https://img.shields.io/pypi/v/fortnitepy.svg)](https://pypi.org/project/rebootpy/)
+[![Supported py versions](https://img.shields.io/pypi/pyversions/rebootpy.svg)](https://pypi.org/project/rebootpy/)
+[![Current pypi version](https://img.shields.io/pypi/v/rebootpy.svg)](https://pypi.org/project/rebootpy/)
 [![Donate link](https://img.shields.io/badge/paypal-donate-blue.svg)](https://www.paypal.me/terbau)
 
 Asynchronous library for interacting with Fortnite and EpicGames' API and XMPP services.
 
 This library is a fork of [Terbau](https://github.com/Terbau/)'s [fortnitepy](https://github.com/Terbau/fortnitepy) which was abandoned.
 
 **Note:** This library is still under developement so breaking changes might happen at any time.
```

### Comparing `rebootpy-0.0.1/rebootpy.egg-info/SOURCES.txt` & `rebootpy-0.0.2/rebootpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rebootpy-0.0.1/setup.py` & `rebootpy-0.0.2/setup.py`

 * *Files identical despite different names*

