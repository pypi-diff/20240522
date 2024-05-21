# Comparing `tmp/osu-1.4.7.tar.gz` & `tmp/osu-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu-1.4.7.tar", last modified: Sat Mar 23 18:04:42 2024, max compression
+gzip compressed data, was "osu-1.4.8.tar", last modified: Tue May 21 23:26:44 2024, max compression
```

## Comparing `osu-1.4.7.tar` & `osu-1.4.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:04:42.743684 osu-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-23 18:04:38.000000 osu-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-23 18:04:42.743684 osu-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-23 18:04:38.000000 osu-1.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:04:42.739684 osu-1.4.7/osu/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-23 18:04:38.000000 osu-1.4.7/osu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:04:42.739684 osu-1.4.7/osu/api/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-23 18:04:38.000000 osu-1.4.7/osu/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16326 2024-03-23 18:04:38.000000 osu-1.4.7/osu/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-23 18:04:38.000000 osu-1.4.7/osu/api/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:04:42.743684 osu-1.4.7/osu/bancho/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-23 18:04:38.000000 osu-1.4.7/osu/bancho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-03-23 18:04:38.000000 osu-1.4.7/osu/bancho/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15611 2024-03-23 18:04:38.000000 osu-1.4.7/osu/bancho/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    16165 2024-03-23 18:04:38.000000 osu-1.4.7/osu/bancho/packets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-03-23 18:04:38.000000 osu-1.4.7/osu/bancho/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-23 18:04:38.000000 osu-1.4.7/osu/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-03-23 18:04:38.000000 osu-1.4.7/osu/game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:04:42.743684 osu-1.4.7/osu/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/beatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/replays.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/score.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-23 18:04:38.000000 osu-1.4.7/osu/objects/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-03-23 18:04:38.000000 osu-1.4.7/osu/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:04:42.743684 osu-1.4.7/osu/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-23 18:04:38.000000 osu-1.4.7/osu/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-23 18:04:38.000000 osu-1.4.7/osu/tcp/bancho.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-03-23 18:04:38.000000 osu-1.4.7/osu/tcp/game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:04:42.743684 osu-1.4.7/osu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-23 18:04:42.000000 osu-1.4.7/osu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-23 18:04:42.000000 osu-1.4.7/osu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 18:04:42.000000 osu-1.4.7/osu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-23 18:04:42.000000 osu-1.4.7/osu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-23 18:04:42.000000 osu-1.4.7/osu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 18:04:42.743684 osu-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-23 18:04:38.000000 osu-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.733149 osu-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-21 23:26:37.000000 osu-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-21 23:26:44.733149 osu-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-21 23:26:37.000000 osu-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.729149 osu-1.4.8/osu/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-21 23:26:37.000000 osu-1.4.8/osu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.729149 osu-1.4.8/osu/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 23:26:37.000000 osu-1.4.8/osu/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16326 2024-05-21 23:26:37.000000 osu-1.4.8/osu/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-21 23:26:37.000000 osu-1.4.8/osu/api/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.729149 osu-1.4.8/osu/bancho/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15611 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16165 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/packets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-21 23:26:37.000000 osu-1.4.8/osu/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-21 23:26:37.000000 osu-1.4.8/osu/game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.733149 osu-1.4.8/osu/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/beatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/replays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-21 23:26:37.000000 osu-1.4.8/osu/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.733149 osu-1.4.8/osu/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 23:26:37.000000 osu-1.4.8/osu/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-21 23:26:37.000000 osu-1.4.8/osu/tcp/bancho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-21 23:26:37.000000 osu-1.4.8/osu/tcp/game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.733149 osu-1.4.8/osu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:26:44.733149 osu-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 23:26:37.000000 osu-1.4.8/setup.py
```

### Comparing `osu-1.4.7/LICENSE` & `osu-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/PKG-INFO` & `osu-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: osu
-Version: 1.4.7
+Version: 1.4.8
 Summary: A python library that emulates the osu! stable client
 Author: Lekuru
 Author-email: contact@lekuru.xyz
 Keywords: osu,osugame,python,bancho
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: wmi; platform_system == "Windows"
 
 # osu.py
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Lekuruu/osu.py/blob/main/LICENSE)
```

### Comparing `osu-1.4.7/README.md` & `osu-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/api/client.py` & `osu-1.4.8/osu/api/client.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/api/constants.py` & `osu-1.4.8/osu/api/constants.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/bancho/client.py` & `osu-1.4.8/osu/bancho/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,18 @@
 
         `game`: osu.game.Game
 
         `connected`: bool
 
         `retry`: bool
 
+        `min_idletime`: int (Minimum time between requests)
+
+        `max_idletime`: int (Maximum time between requests)
+
     Functions:
         `enqueue`: Send a bancho packet to the server
 
         `ping`: Send a ping packet
 
         `request_presence`: Request a presence update for a list of players
 
@@ -121,15 +125,15 @@
         self.last_action = datetime.now().timestamp()
         self.fast_read = False
 
         self.silenced = False
         self.in_lobby = False
 
         self.min_idletime = 1
-        self.max_idletime = 4
+        self.max_idletime = 2.5
 
     @property
     def status(self) -> Status:
         """Status of the connected player"""
         if not self.player:
             return Status()
         return self.player.status
@@ -144,34 +148,31 @@
         """Time between requests"""
 
         if self.fast_read:
             return 0
 
         interval = 1
 
-        if self.game.tourney:
-            return interval
-
         if not self.spectating:
             interval *= 1 + self.idle_time / 10
-            interval *= 1 + self.ping_count
+            interval *= self.ping_count
 
         interval = min(self.max_idletime, max(self.min_idletime, interval))
 
         return interval
 
     def run(self):
         """Run the client loop"""
         self.connect()
 
         while self.connected:
             try:
+                time.sleep(self.request_interval)
                 self.dequeue()
                 self.game.tasks.execute()
-                time.sleep(self.request_interval)
             except KeyboardInterrupt:
                 raise
             except Exception as exc:
                 self.logger.fatal(f"Unhandled Exception: {exc}", exc_info=exc)
 
         if self.retry:
             self.logger.error("Retrying in 15 seconds...")
@@ -212,15 +213,16 @@
         if not self.connected:
             return
 
         if self.queue.empty():
             # Queue is empty, sending ping
             self.ping_count += 1
             return self.ping()
-        else:
+
+        if self.queue.qsize() > 1:
             self.ping_count = 0
 
         data = b""
 
         while not self.queue.empty():
             data += self.queue.get()
```

### Comparing `osu-1.4.7/osu/bancho/constants.py` & `osu-1.4.8/osu/bancho/constants.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/bancho/packets.py` & `osu-1.4.8/osu/bancho/packets.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/bancho/streams.py` & `osu-1.4.8/osu/bancho/streams.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/events.py` & `osu-1.4.8/osu/events.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/game.py` & `osu-1.4.8/osu/game.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/objects/beatmap.py` & `osu-1.4.8/osu/objects/beatmap.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/objects/channel.py` & `osu-1.4.8/osu/objects/channel.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/objects/client.py` & `osu-1.4.8/osu/objects/client.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/objects/collections.py` & `osu-1.4.8/osu/objects/collections.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/objects/lists.py` & `osu-1.4.8/osu/objects/lists.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/objects/player.py` & `osu-1.4.8/osu/objects/player.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/objects/replays.py` & `osu-1.4.8/osu/objects/replays.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/objects/score.py` & `osu-1.4.8/osu/objects/score.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/objects/status.py` & `osu-1.4.8/osu/objects/status.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/tasks.py` & `osu-1.4.8/osu/tasks.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/tcp/bancho.py` & `osu-1.4.8/osu/tcp/bancho.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu/tcp/game.py` & `osu-1.4.8/osu/tcp/game.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/osu.egg-info/PKG-INFO` & `osu-1.4.8/osu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: osu
-Version: 1.4.7
+Version: 1.4.8
 Summary: A python library that emulates the osu! stable client
 Author: Lekuru
 Author-email: contact@lekuru.xyz
 Keywords: osu,osugame,python,bancho
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: wmi; platform_system == "Windows"
 
 # osu.py
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Lekuruu/osu.py/blob/main/LICENSE)
```

### Comparing `osu-1.4.7/osu.egg-info/SOURCES.txt` & `osu-1.4.8/osu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osu-1.4.7/setup.py` & `osu-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 with open(os.path.join(current_directory, "requirements.txt"), "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="osu",
-    version="1.4.7",
+    version="1.4.8",
     author="Lekuru",
     author_email="contact@lekuru.xyz",
     description="A python library that emulates the osu! stable client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

