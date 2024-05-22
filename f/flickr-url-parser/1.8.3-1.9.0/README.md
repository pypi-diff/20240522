# Comparing `tmp/flickr_url_parser-1.8.3.tar.gz` & `tmp/flickr_url_parser-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr_url_parser-1.8.3.tar", last modified: Tue Apr 30 14:43:35 2024, max compression
+gzip compressed data, was "flickr_url_parser-1.9.0.tar", last modified: Wed May 22 15:17:16 2024, max compression
```

## Comparing `flickr_url_parser-1.8.3.tar` & `flickr_url_parser-1.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.813903 flickr_url_parser-1.8.3/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-10-03 13:54:10.000000 flickr_url_parser-1.8.3/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-10-03 13:54:10.000000 flickr_url_parser-1.8.3/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3835 2024-04-30 14:43:35.813669 flickr_url_parser-1.8.3/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2991 2023-12-18 15:24:26.000000 flickr_url_parser-1.8.3/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1890 2023-12-18 15:19:07.000000 flickr_url_parser-1.8.3/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-30 14:43:35.813953 flickr_url_parser-1.8.3/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.808774 flickr_url_parser-1.8.3/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.811503 flickr_url_parser-1.8.3/src/flickr_url_parser/
--rw-r--r--   0 alexwlchan   (501) staff       (20)      371 2024-04-30 14:43:31.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      878 2023-10-31 12:00:36.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/base58.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      649 2023-12-18 15:19:07.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/cli.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      309 2023-12-18 15:19:07.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      481 2023-12-12 14:58:59.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/matcher.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    16783 2024-04-30 14:43:31.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/parser.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 09:20:42.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/py.typed
--rw-r--r--   0 alexwlchan   (501) staff       (20)      796 2024-04-30 09:55:09.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/types.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.813381 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3835 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      653 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       65 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/entry_points.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       16 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.813056 flickr_url_parser-1.8.3/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1323 2023-12-18 15:15:45.000000 flickr_url_parser-1.8.3/tests/test_cli.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    16854 2024-04-30 14:43:31.000000 flickr_url_parser-1.8.3/tests/test_flickr_url_parser.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1786 2023-12-12 14:58:59.000000 flickr_url_parser-1.8.3/tests/test_matcher.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-22 15:17:16.244036 flickr_url_parser-1.9.0/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-10-03 13:54:10.000000 flickr_url_parser-1.9.0/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-10-03 13:54:10.000000 flickr_url_parser-1.9.0/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3835 2024-05-22 15:17:16.243541 flickr_url_parser-1.9.0/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2991 2023-12-18 15:24:26.000000 flickr_url_parser-1.9.0/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1890 2023-12-18 15:19:07.000000 flickr_url_parser-1.9.0/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-05-22 15:17:16.244098 flickr_url_parser-1.9.0/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-22 15:17:16.239079 flickr_url_parser-1.9.0/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-22 15:17:16.241618 flickr_url_parser-1.9.0/src/flickr_url_parser/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      371 2024-05-22 15:17:08.000000 flickr_url_parser-1.9.0/src/flickr_url_parser/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      878 2023-10-31 12:00:36.000000 flickr_url_parser-1.9.0/src/flickr_url_parser/base58.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      649 2023-12-18 15:19:07.000000 flickr_url_parser-1.9.0/src/flickr_url_parser/cli.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      309 2023-12-18 15:19:07.000000 flickr_url_parser-1.9.0/src/flickr_url_parser/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      481 2023-12-12 14:58:59.000000 flickr_url_parser-1.9.0/src/flickr_url_parser/matcher.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    17582 2024-05-22 15:17:08.000000 flickr_url_parser-1.9.0/src/flickr_url_parser/parser.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 09:20:42.000000 flickr_url_parser-1.9.0/src/flickr_url_parser/py.typed
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1037 2024-05-22 15:17:08.000000 flickr_url_parser-1.9.0/src/flickr_url_parser/types.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-22 15:17:16.243274 flickr_url_parser-1.9.0/src/flickr_url_parser.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3835 2024-05-22 15:17:16.000000 flickr_url_parser-1.9.0/src/flickr_url_parser.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      653 2024-05-22 15:17:16.000000 flickr_url_parser-1.9.0/src/flickr_url_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-05-22 15:17:16.000000 flickr_url_parser-1.9.0/src/flickr_url_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       65 2024-05-22 15:17:16.000000 flickr_url_parser-1.9.0/src/flickr_url_parser.egg-info/entry_points.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       16 2024-05-22 15:17:16.000000 flickr_url_parser-1.9.0/src/flickr_url_parser.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-05-22 15:17:16.000000 flickr_url_parser-1.9.0/src/flickr_url_parser.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-22 15:17:16.242923 flickr_url_parser-1.9.0/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1414 2024-05-22 15:17:08.000000 flickr_url_parser-1.9.0/tests/test_cli.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    20484 2024-05-22 15:17:08.000000 flickr_url_parser-1.9.0/tests/test_flickr_url_parser.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1786 2023-12-12 14:58:59.000000 flickr_url_parser-1.9.0/tests/test_matcher.py
```

### Comparing `flickr_url_parser-1.8.3/LICENSE-APACHE` & `flickr_url_parser-1.9.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr_url_parser-1.8.3/LICENSE-MIT` & `flickr_url_parser-1.9.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr_url_parser-1.8.3/PKG-INFO` & `flickr_url_parser-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-url-parser
-Version: 1.8.3
+Version: 1.9.0
 Summary: Enter a Flickr URL, and find out what sort of URL it is (single photo, album, gallery, etc.)
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-url-parser
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-url-parser/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_url_parser-1.8.3/README.md` & `flickr_url_parser-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `flickr_url_parser-1.8.3/pyproject.toml` & `flickr_url_parser-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flickr_url_parser-1.8.3/src/flickr_url_parser/base58.py` & `flickr_url_parser-1.9.0/src/flickr_url_parser/base58.py`

 * *Files identical despite different names*

### Comparing `flickr_url_parser-1.8.3/src/flickr_url_parser/cli.py` & `flickr_url_parser-1.9.0/src/flickr_url_parser/cli.py`

 * *Files identical despite different names*

### Comparing `flickr_url_parser-1.8.3/src/flickr_url_parser/parser.py` & `flickr_url_parser-1.9.0/src/flickr_url_parser/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 
 import httpx
 import hyperlink
 
 from .base58 import is_base58, base58_decode
 from .exceptions import NotAFlickrUrl, UnrecognisedUrl
-from .types import ParseResult
+from .types import anonymous_single_photo, ParseResult
 
 
 def get_page(url: hyperlink.URL) -> int:
     """
     Flickr does pagination by appending a `pageXX` component to the end of URLs, e.g.
 
         https://www.flickr.com/photos/belindavick/
@@ -246,18 +246,28 @@
     # https://www.flickr.com/photos/coast_guard/32812033543/
     if (
         is_long_url
         and len(u.path) >= 3
         and u.path[0] == "photos"
         and is_digits(u.path[2])
     ):
-        return {
-            "type": "single_photo",
-            "photo_id": u.path[2],
-        }
+        if is_flickr_user_id(u.path[1].upper()):
+            return {
+                "type": "single_photo",
+                "photo_id": u.path[2],
+                "user_url": f"https://www.flickr.com/photos/{u.path[1].upper()}/",
+                "user_id": u.path[1].upper(),
+            }
+        else:
+            return {
+                "type": "single_photo",
+                "photo_id": u.path[2],
+                "user_url": f"https://www.flickr.com/photos/{u.path[1]}/",
+                "user_id": None,
+            }
 
     # Old-style URLs for a single photo, e.g.
     # http://flickr.com/photo/17277074@N00/2619974961
     #
     # This is a variant of Flickr photo URL that appears fairly
     # regularly in e.g. Wikimedia Commons – it no longer resolves, but
     # there are enough of these both on WMC and around the general web
@@ -267,27 +277,37 @@
     # parse it, even if new URLs like this are no longer created.
     if (
         is_long_url
         and len(u.path) >= 3
         and u.path[0] == "photo"
         and is_digits(u.path[2])
     ):
-        return {
-            "type": "single_photo",
-            "photo_id": u.path[2],
-        }
+        if is_flickr_user_id(u.path[1].upper()):
+            return {
+                "type": "single_photo",
+                "photo_id": u.path[2],
+                "user_url": f"https://www.flickr.com/photos/{u.path[1].upper()}/",
+                "user_id": u.path[1].upper(),
+            }
+        else:
+            return {
+                "type": "single_photo",
+                "photo_id": u.path[2],
+                "user_url": f"https://www.flickr.com/photos/{u.path[1]}/",
+                "user_id": None,
+            }
 
     # The URL for a single photo, e.g.
     #
     #     https://flic.kr/p/2p4QbKN
     #
     # Here the final path component is a base-58 conversion of the photo ID.
     # See https://www.flickr.com/groups/51035612836@N01/discuss/72157616713786392/
     if is_short_url and len(u.path) == 2 and u.path[0] == "p" and is_base58(u.path[1]):
-        return {"type": "single_photo", "photo_id": base58_decode(u.path[1])}
+        return anonymous_single_photo(photo_id=base58_decode(u.path[1]))
 
     # Another variant of URL for a single photo, e.g.
     #
     #     https://www.flickr.com/photo_zoom.gne?id=196155401&size=m
     #     https://www.flickr.com/photo_exif.gne?id=1427904898
     #     www.flickr.com/photo.gne?id=105
     #     https://www.flickr.com/photo.gne?short=2ouuqFT
@@ -300,26 +320,26 @@
         and u.path[0].startswith(("photo", "video"))
         and u.path[0].endswith(".gne")
         and len(u.get("id")) == 1
     ):
         photo_id = u.get("id")[0]
 
         if isinstance(photo_id, str) and is_digits(photo_id):
-            return {"type": "single_photo", "photo_id": photo_id}
+            return anonymous_single_photo(photo_id)
 
     if (
         is_long_url
         and len(u.path) == 1
         and u.path[0] == "photo.gne"
         and len(u.get("short")) == 1
     ):
         short_id = u.get("short")[0]
 
         if isinstance(short_id, str) and is_base58(short_id):
-            return {"type": "single_photo", "photo_id": base58_decode(short_id)}
+            return anonymous_single_photo(photo_id=base58_decode(short_id))
 
     # The URL for an actual file, e.g.
     #
     #     https://live.staticflickr.com/65535/53381630964_63d765ee92_s.jpg
     #     http://static.flickr.com/63/155697786_0125559b4e.jpg
     #     http://farm1.static.flickr.com/82/241708183_dd0847d5c7_o.jpg
     #     https://farm5.staticflickr.com/4586/37767087695_bb4ecff5f4_o.jpg
@@ -335,55 +355,55 @@
             or re.match(r"^farm\d+\.static\.flickr\.com$", u.host)
         )
         and len(u.path) >= 2
         and is_digits(u.path[0])
     ):
         photo_id, *_ = u.path[1].split("_")
         if is_digits(photo_id):
-            return {"type": "single_photo", "photo_id": photo_id}
+            return anonymous_single_photo(photo_id)
 
     # The URL for a static video file, e.g.
     #
     #     https://live.staticflickr.com/video/52868534222/346a41e5a9/1080p.mp4
     #
     if (
         is_static_url
         and u.host == "live.staticflickr.com"
         and len(u.path) >= 2
         and u.path[0] == "video"
         and is_digits(u.path[1])
     ):
-        return {"type": "single_photo", "photo_id": u.path[1]}
+        return anonymous_single_photo(photo_id=u.path[1])
 
     # The URL for a static file, e.g.
     #
     #     https://photos12.flickr.com/16159487_3a6615a565_b.jpg
     #
     if (
         is_static_url
         and re.match(r"^photos\d+\.flickr\.com$", u.host)
         and len(u.path) >= 1
     ):
         photo_id, *_ = u.path[0].split("_")
         if is_digits(photo_id):
-            return {"type": "single_photo", "photo_id": photo_id}
+            return anonymous_single_photo(photo_id)
 
     # The URL for a static file, e.g.
     #
     #     https://c8.staticflickr.com/6/5159/14288803431_7cf094b085_b.jpg
     #
     if is_static_url and (
         re.match(r"^c\d+\.staticflickr\.com$", u.host)
         and len(u.path) == 3
         and is_digits(u.path[0])
         and is_digits(u.path[1])
     ):
         photo_id, *_ = u.path[2].split("_")
         if is_digits(photo_id):
-            return {"type": "single_photo", "photo_id": photo_id}
+            return anonymous_single_photo(photo_id)
 
     # The URL for an album, e.g.
     #
     #     https://www.flickr.com/photos/cat_tac/albums/72157666833379009
     #     https://www.flickr.com/photos/cat_tac/sets/72157666833379009
     #     https://www.flickr.com/photos/andygocher/albums/72157648252420622/page3
     #
@@ -491,10 +511,10 @@
         is_long_url
         and u.path == ("apps", "video", "stewart.swf")
         and len(u.get("photo_id")) == 1
     ):
         photo_id = u.get("photo_id")[0]
 
         if isinstance(photo_id, str) and is_digits(photo_id):
-            return {"type": "single_photo", "photo_id": photo_id}
+            return anonymous_single_photo(photo_id)
 
     raise UnrecognisedUrl(f"Unrecognised URL: {url}")
```

### Comparing `flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/PKG-INFO` & `flickr_url_parser-1.9.0/src/flickr_url_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-url-parser
-Version: 1.8.3
+Version: 1.9.0
 Summary: Enter a Flickr URL, and find out what sort of URL it is (single photo, album, gallery, etc.)
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-url-parser
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-url-parser/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/SOURCES.txt` & `flickr_url_parser-1.9.0/src/flickr_url_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flickr_url_parser-1.8.3/tests/test_cli.py` & `flickr_url_parser-1.9.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
     assert rc == 0
 
     captured = capsys.readouterr()
     assert json.loads(captured.out) == {
         "type": "single_photo",
         "photo_id": "32812033543",
+        "user_url": "https://www.flickr.com/photos/coast_guard/",
+        "user_id": None,
     }
     assert captured.err == ""
 
 
 def test_run_cli_shows_help(capsys: CaptureFixture[str]) -> None:
     rc = run_cli(argv=["flickr_url_parser", "--help"])
```

### Comparing `flickr_url_parser-1.8.3/tests/test_flickr_url_parser.py` & `flickr_url_parser-1.9.0/tests/test_flickr_url_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from flickr_url_parser import (
     is_flickr_user_id,
     parse_flickr_url,
     NotAFlickrUrl,
     UnrecognisedUrl,
 )
-from flickr_url_parser.types import Album, Gallery, Group, Tag
+from flickr_url_parser.types import Album, Gallery, Group, SinglePhoto, Tag
 
 
 @pytest.mark.parametrize(
     ["text", "result"], [("47265398@N04", True), ("blueminds", False), ("", False)]
 )
 def test_is_flickr_user_id(text: str, result: bool) -> None:
     assert is_flickr_user_id(text) == result
@@ -71,21 +71,22 @@
     [
         "https://www.flickr.com/photos/coast_guard/32812033543",
         "http://www.flickr.com/photos/coast_guard/32812033543",
         "https://flickr.com/photos/coast_guard/32812033543",
         "http://flickr.com/photos/coast_guard/32812033543",
         "www.flickr.com/photos/coast_guard/32812033543",
         "flickr.com/photos/coast_guard/32812033543",
-        "live.staticflickr.com/2903/32812033543_c1b3784192_w_d.jpg",
     ],
 )
 def test_it_can_parse_urls_even_if_the_host_is_a_bit_unusual(url: str) -> None:
     assert parse_flickr_url(url) == {
         "type": "single_photo",
         "photo_id": "32812033543",
+        "user_url": "https://www.flickr.com/photos/coast_guard/",
+        "user_id": None,
     }
 
 
 @pytest.mark.parametrize(
     "url",
     [
         "https://www.flickr.com",
@@ -101,47 +102,158 @@
     ],
 )
 def test_it_can_parse_the_homepage(url: str) -> None:
     assert parse_flickr_url(url) == {"type": "homepage"}
 
 
 @pytest.mark.parametrize(
-    ["url", "photo_id"],
+    ["url", "single_photo"],
     [
-        ("https://www.flickr.com/photos/coast_guard/32812033543", "32812033543"),
+        (
+            "https://www.flickr.com/photos/coast_guard/32812033543",
+            {
+                "type": "single_photo",
+                "photo_id": "32812033543",
+                "user_url": "https://www.flickr.com/photos/coast_guard/",
+                "user_id": None,
+            },
+        ),
         (
             "https://www.flickr.com/photos/coast_guard/32812033543/in/photolist-RZufqg-ebEcP7-YvCkaU-2dKrfhV-6o5anp-7ZjJuj-fxZTiu-2c1pGwi-JbqooJ-TaNkv5-ehrqn7-2aYFaRh-QLDxJX-2dKrdip-JB7iUz-ehrsNh-2aohZ14-Rgeuo3-JRwKwE-ksAR6U-dZVQ3m-291gkvk-26ynYWn-pHMQyE-a86UD8-9Tpmru-hamg6T-8ZCRFU-QY8amt-2eARQfP-qskFkD-2c1pG1Z-jbCpyF-fTBQDa-a89xfd-a7kYMs-dYjL51-5XJgXY-8caHdL-a89HZd-9GBmft-xy7PBo-sai77d-Vs8YPG-RgevC7-Nv5CF6-e4ZLn9-cPaxqS-9rnjS9-8Y7mhm",
-            "32812033543",
+            {
+                "type": "single_photo",
+                "photo_id": "32812033543",
+                "user_url": "https://www.flickr.com/photos/coast_guard/",
+                "user_id": None,
+            },
         ),
         (
             "https://www.flickr.com/photos/britishlibrary/13874001214/in/album-72157644007437024/",
-            "13874001214",
+            {
+                "type": "single_photo",
+                "photo_id": "13874001214",
+                "user_url": "https://www.flickr.com/photos/britishlibrary/",
+                "user_id": None,
+            },
+        ),
+        (
+            "https://www.Flickr.com/photos/techiedog/44257407",
+            {
+                "type": "single_photo",
+                "photo_id": "44257407",
+                "user_url": "https://www.flickr.com/photos/techiedog/",
+                "user_id": None,
+            },
+        ),
+        (
+            "www.Flickr.com/photos/techiedog/44257407",
+            {
+                "type": "single_photo",
+                "photo_id": "44257407",
+                "user_url": "https://www.flickr.com/photos/techiedog/",
+                "user_id": None,
+            },
         ),
-        ("https://www.Flickr.com/photos/techiedog/44257407", "44257407"),
-        ("www.Flickr.com/photos/techiedog/44257407", "44257407"),
         (
             "https://www.flickr.com/photos/tanaka_juuyoh/1866762301/sizes/o/in/set-72157602201101937",
-            "1866762301",
+            {
+                "type": "single_photo",
+                "photo_id": "1866762301",
+                "user_url": "https://www.flickr.com/photos/tanaka_juuyoh/",
+                "user_id": None,
+            },
+        ),
+        #
+        # Strictly speaking this URL is invalid, because of the lowercase @n02,
+        # which should be uppercase.  But we know what you meant, so parse it anyway.
+        (
+            "https://www.flickr.com/photos/11588490@n02/2174280796/sizes/l",
+            {
+                "type": "single_photo",
+                "photo_id": "2174280796",
+                "user_url": "https://www.flickr.com/photos/11588490@N02/",
+                "user_id": "11588490@N02",
+            },
+        ),
+        (
+            "https://www.flickr.com/photos/nrcs_south_dakota/8023844010/in",
+            {
+                "type": "single_photo",
+                "photo_id": "8023844010",
+                "user_url": "https://www.flickr.com/photos/nrcs_south_dakota/",
+                "user_id": None,
+            },
         ),
-        ("https://www.flickr.com/photos/11588490@n02/2174280796/sizes/l", "2174280796"),
-        ("https://www.flickr.com/photos/nrcs_south_dakota/8023844010/in", "8023844010"),
         (
             "https://www.flickr.com/photos/chucksutherland/6738252077/player/162ed63802",
-            "6738252077",
+            {
+                "type": "single_photo",
+                "photo_id": "6738252077",
+                "user_url": "https://www.flickr.com/photos/chucksutherland/",
+                "user_id": None,
+            },
         ),
         (
+            "http://flickr.com/photo/17277074@N00/2619974961",
+            {
+                "type": "single_photo",
+                "photo_id": "2619974961",
+                "user_url": "https://www.flickr.com/photos/17277074@N00/",
+                "user_id": "17277074@N00",
+            },
+        ),
+        (
+            "http://flickr.com/photo/art-sarah/2619974961",
+            {
+                "type": "single_photo",
+                "photo_id": "2619974961",
+                "user_url": "https://www.flickr.com/photos/art-sarah/",
+                "user_id": None,
+            },
+        ),
+        (
+            "https://www.flickr.com/photos/gracewong/196155401/meta/",
+            {
+                "type": "single_photo",
+                "photo_id": "196155401",
+                "user_url": "https://www.flickr.com/photos/gracewong/",
+                "user_id": None,
+            },
+        ),
+        #
+        # From https://commons.wikimedia.org/wiki/File:75016-75017_Avenues_Foch_et_de_la_Grande_Armée_20050919.jpg
+        # Retrieved 12 December 2023
+        (
+            "https://www.flickr.com/photos/joyoflife//44627174",
+            {
+                "type": "single_photo",
+                "photo_id": "44627174",
+                "user_url": "https://www.flickr.com/photos/joyoflife/",
+                "user_id": None,
+            },
+        ),
+    ],
+)
+def test_it_parses_a_single_photo_with_user_info(
+    url: str, single_photo: SinglePhoto
+) -> None:
+    assert parse_flickr_url(url) == single_photo
+
+
+@pytest.mark.parametrize(
+    ["url", "photo_id"],
+    [
+        (
             "https://live.staticflickr.com/65535/53381630964_63d765ee92_s.jpg",
             "53381630964",
         ),
         ("photos12.flickr.com/16159487_3a6615a565_b.jpg", "16159487"),
         ("http://farm1.static.flickr.com/82/241708183_dd0847d5c7_o.jpg", "241708183"),
         ("farm1.static.flickr.com/82/241708183_dd0847d5c7_o.jpg", "241708183"),
-        ("http://flickr.com/photo/17277074@N00/2619974961", "2619974961"),
         ("https://www.flickr.com/photo_zoom.gne?id=196155401&size=m", "196155401"),
-        ("https://www.flickr.com/photos/gracewong/196155401/meta/", "196155401"),
         ("https://www.flickr.com/photo_exif.gne?id=1427904898", "1427904898"),
         # This URL is linked from https://commons.wikimedia.org/wiki/File:Adriaen_Brouwer_-_The_slaughter_feast.jpg
         (
             "https://farm5.staticflickr.com/4586/37767087695_bb4ecff5f4_o.jpg",
             "37767087695",
         ),
         #
@@ -154,18 +266,14 @@
         # Retrieved 12 December 2023
         ("www.flickr.com/photo.gne?id=105", "105"),
         #
         # From https://commons.wikimedia.org/wiki/File:IgnazioDanti.jpg
         # Retrieved 12 December 2023
         ("c8.staticflickr.com/6/5159/14288803431_7cf094b085_b.jpg", "14288803431"),
         #
-        # From https://commons.wikimedia.org/wiki/File:75016-75017_Avenues_Foch_et_de_la_Grande_Armée_20050919.jpg
-        # Retrieved 12 December 2023
-        ("https://www.flickr.com/photos/joyoflife//44627174", "44627174"),
-        #
         # From https://commons.wikimedia.org/wiki/File:The_Peace_Hat_and_President_Chester_Arthur,_1829_-_1886_(3435827496).jpg
         # Retrieved 20 December 2023
         ("www.flickr.com/photo_edit.gne?id=3435827496", "3435827496"),
         #
         # From https://commons.wikimedia.org/wiki/File:Mars_-_Valles_Marineris,_Melas_Chasma_-_ESA_Mars_Express_(52830681359).png
         # Retrieved 20 December 2023
         ("https://www.flickr.com/photo.gne?short=2ouuqFT", "52830949513"),
@@ -187,18 +295,20 @@
         # Retrieved 2 January 2024
         (
             "https://www.flickr.com/apps/video/stewart.swf?v=2968162862&photo_id=53262935176&photo_secret=06c382eee3",
             "53262935176",
         ),
     ],
 )
-def test_it_parses_a_single_photo(url: str, photo_id: str) -> None:
+def test_it_parses_a_single_photo_without_user_info(url: str, photo_id: str) -> None:
     assert parse_flickr_url(url) == {
         "type": "single_photo",
         "photo_id": photo_id,
+        "user_url": None,
+        "user_id": None,
     }
 
 
 @pytest.mark.parametrize(
     ["url", "album"],
     [
         (
@@ -431,14 +541,16 @@
     assert parse_flickr_url(url) == tag
 
 
 def test_it_parses_a_short_flickr_url() -> None:
     assert parse_flickr_url(url="https://flic.kr/p/2p4QbKN") == {
         "type": "single_photo",
         "photo_id": "53208249252",
+        "user_url": None,
+        "user_id": None,
     }
 
 
 # Note: Guest Pass URLs are used to give somebody access to content
 # on Flickr, even if (1) the content is private or (2) the person
 # looking at the content isn't logged in.
 #
@@ -460,15 +572,20 @@
                 "page": 1,
             },
             id="M195SLkj98",
         ),
         # one of mine (Alex's)
         pytest.param(
             "https://www.flickr.com/gp/199246608@N02/nSN80jZ64E",
-            {"type": "single_photo", "photo_id": "53279364618"},
+            {
+                "type": "single_photo",
+                "photo_id": "53279364618",
+                "user_url": "https://www.flickr.com/photos/199246608@N02/",
+                "user_id": "199246608@N02",
+            },
             id="nSN80jZ64E",
         ),
     ],
 )
 def test_it_parses_guest_pass_urls(
     vcr_cassette: str, url: str, expected: dict[str, str]
 ) -> None:
```

### Comparing `flickr_url_parser-1.8.3/tests/test_matcher.py` & `flickr_url_parser-1.9.0/tests/test_matcher.py`

 * *Files identical despite different names*

