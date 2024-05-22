# Comparing `tmp/edge-tts-6.1.8.tar.gz` & `tmp/edge-tts-6.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge-tts-6.1.8.tar", last modified: Sat Aug 12 14:26:50 2023, max compression
+gzip compressed data, was "edge-tts-6.1.9.tar", last modified: Sat Nov  4 16:01:16 2023, max compression
```

## Comparing `edge-tts-6.1.8.tar` & `edge-tts-6.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-12 14:26:50.158575 edge-tts-6.1.8/
--rw-------   0 user      (1000) user      (1000)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.8/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     3994 2023-08-12 14:26:50.158575 edge-tts-6.1.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3477 2023-08-04 14:58:21.000000 edge-tts-6.1.8/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      834 2023-08-12 14:26:50.158575 edge-tts-6.1.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      223 2023-08-12 14:21:00.000000 edge-tts-6.1.8/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-12 14:26:50.158575 edge-tts-6.1.8/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-12 14:26:50.158575 edge-tts-6.1.8/src/edge_playback/
--rw-rw-r--   0 user      (1000) user      (1000)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.8/src/edge_playback/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2053 2023-06-18 15:33:31.000000 edge-tts-6.1.8/src/edge_playback/__main__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-12 14:26:50.158575 edge-tts-6.1.8/src/edge_tts/
--rw-rw-r--   0 user      (1000) user      (1000)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.8/src/edge_tts/__init__.py
--rw-------   0 user      (1000) user      (1000)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.8/src/edge_tts/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16995 2023-08-12 14:24:22.000000 edge-tts-6.1.8/src/edge_tts/communicate.py
--rw-rw-r--   0 user      (1000) user      (1000)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.8/src/edge_tts/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)      558 2023-04-05 13:39:33.000000 edge-tts-6.1.8/src/edge_tts/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2703 2023-08-12 14:25:02.000000 edge-tts-6.1.8/src/edge_tts/list_voices.py
--rw-rw-r--   0 user      (1000) user      (1000)     3823 2023-04-05 14:00:08.000000 edge-tts-6.1.8/src/edge_tts/submaker.py
--rw-rw-r--   0 user      (1000) user      (1000)     4369 2023-08-04 14:58:21.000000 edge-tts-6.1.8/src/edge_tts/util.py
--rw-rw-r--   0 user      (1000) user      (1000)      128 2023-08-12 14:25:42.000000 edge-tts-6.1.8/src/edge_tts/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-12 14:26:50.158575 edge-tts-6.1.8/src/edge_tts.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3994 2023-08-12 14:26:50.000000 edge-tts-6.1.8/src/edge_tts.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      543 2023-08-12 14:26:50.000000 edge-tts-6.1.8/src/edge_tts.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-12 14:26:50.000000 edge-tts-6.1.8/src/edge_tts.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       97 2023-08-12 14:26:50.000000 edge-tts-6.1.8/src/edge_tts.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       66 2023-08-12 14:26:50.000000 edge-tts-6.1.8/src/edge_tts.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       23 2023-08-12 14:26:50.000000 edge-tts-6.1.8/src/edge_tts.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-11-04 16:01:16.982850 edge-tts-6.1.9/
+-rw-------   0 user       (501) staff       (20)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     4055 2023-11-04 16:01:16.982921 edge-tts-6.1.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3538 2023-11-04 15:59:26.000000 edge-tts-6.1.9/README.md
+-rw-rw-r--   0 user       (501) staff       (20)      834 2023-11-04 16:01:16.983157 edge-tts-6.1.9/setup.cfg
+-rw-rw-r--   0 user       (501) staff       (20)      223 2023-08-12 14:21:00.000000 edge-tts-6.1.9/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-11-04 16:01:16.979620 edge-tts-6.1.9/src/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-11-04 16:01:16.980471 edge-tts-6.1.9/src/edge_playback/
+-rw-rw-r--   0 user       (501) staff       (20)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.9/src/edge_playback/__init__.py
+-rw-rw-r--   0 user       (501) staff       (20)     2053 2023-06-18 15:33:31.000000 edge-tts-6.1.9/src/edge_playback/__main__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-11-04 16:01:16.981800 edge-tts-6.1.9/src/edge_tts/
+-rw-rw-r--   0 user       (501) staff       (20)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.9/src/edge_tts/__init__.py
+-rw-------   0 user       (501) staff       (20)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.9/src/edge_tts/__main__.py
+-rw-r--r--   0 user       (501) staff       (20)    17313 2023-11-04 15:59:27.000000 edge-tts-6.1.9/src/edge_tts/communicate.py
+-rw-rw-r--   0 user       (501) staff       (20)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.9/src/edge_tts/constants.py
+-rw-rw-r--   0 user       (501) staff       (20)      558 2023-04-05 13:39:33.000000 edge-tts-6.1.9/src/edge_tts/exceptions.py
+-rw-rw-r--   0 user       (501) staff       (20)     2703 2023-08-12 14:25:02.000000 edge-tts-6.1.9/src/edge_tts/list_voices.py
+-rw-rw-r--   0 user       (501) staff       (20)     3823 2023-04-05 14:00:08.000000 edge-tts-6.1.9/src/edge_tts/submaker.py
+-rw-r--r--   0 user       (501) staff       (20)     4483 2023-11-04 15:59:27.000000 edge-tts-6.1.9/src/edge_tts/util.py
+-rw-rw-r--   0 user       (501) staff       (20)      128 2023-11-04 15:59:54.000000 edge-tts-6.1.9/src/edge_tts/version.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-11-04 16:01:16.982752 edge-tts-6.1.9/src/edge_tts.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     4055 2023-11-04 16:01:16.000000 edge-tts-6.1.9/src/edge_tts.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      543 2023-11-04 16:01:16.000000 edge-tts-6.1.9/src/edge_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-11-04 16:01:16.000000 edge-tts-6.1.9/src/edge_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       97 2023-11-04 16:01:16.000000 edge-tts-6.1.9/src/edge_tts.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       66 2023-11-04 16:01:16.000000 edge-tts-6.1.9/src/edge_tts.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       23 2023-11-04 16:01:16.000000 edge-tts-6.1.9/src/edge_tts.egg-info/top_level.txt
```

### Comparing `edge-tts-6.1.8/LICENSE` & `edge-tts-6.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.8/PKG-INFO` & `edge-tts-6.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.8
+Version: 6.1.9
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -75,25 +75,24 @@
 
     $ edge-tts --voice ar-EG-SalmaNeural --text "مرحبا كيف حالك؟" --write-media hello_in_arabic.mp3 --write-subtitles hello_in_arabic.vtt
 
 ### Custom SSML
 
 Support for custom SSML has been removed since 5.0.0 because Microsoft has taken the initiative to prevent it from working. You cannot use custom SSML anymore.
 
-### Changing rate and volume
+### Changing rate, volume and pitch
 
 It is possible to make minor changes to the generated speech.
 
     $ edge-tts --rate=-50% --text "Hello, world!" --write-media hello_with_rate_halved.mp3 --write-subtitles hello_with_rate_halved.vtt
     $ edge-tts --volume=-50% --text "Hello, world!" --write-media hello_with_volume_halved.mp3 --write-subtitles hello_with_volume_halved.vtt
+    $ edge-tts --pitch=-50Hz --text "Hello, world!" --write-media hello_with_pitch_halved.mp3 --write-subtitles hello_with_pitch_halved.vtt
 
 In addition, it is required to use `--rate=-50%` instead of `--rate -50%` (note the lack of an equal sign) otherwise the `-50%` would be interpreted as just another argument.
 
-**NOTE**: `--pitch` was removed in 6.0.3 as it no longer appears to have any effect.
-
 ### Note on the `edge-playback` command
 
 `edge-playback` is just a wrapper around `edge-tts` that plays back the generated speech. It takes the same arguments as the `edge-tts` option.
 
 ## Python module
 
 It is possible to use the `edge-tts` module directly from Python. For a list of example applications:
```

### Comparing `edge-tts-6.1.8/README.md` & `edge-tts-6.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,25 +59,24 @@
 
     $ edge-tts --voice ar-EG-SalmaNeural --text "مرحبا كيف حالك؟" --write-media hello_in_arabic.mp3 --write-subtitles hello_in_arabic.vtt
 
 ### Custom SSML
 
 Support for custom SSML has been removed since 5.0.0 because Microsoft has taken the initiative to prevent it from working. You cannot use custom SSML anymore.
 
-### Changing rate and volume
+### Changing rate, volume and pitch
 
 It is possible to make minor changes to the generated speech.
 
     $ edge-tts --rate=-50% --text "Hello, world!" --write-media hello_with_rate_halved.mp3 --write-subtitles hello_with_rate_halved.vtt
     $ edge-tts --volume=-50% --text "Hello, world!" --write-media hello_with_volume_halved.mp3 --write-subtitles hello_with_volume_halved.vtt
+    $ edge-tts --pitch=-50Hz --text "Hello, world!" --write-media hello_with_pitch_halved.mp3 --write-subtitles hello_with_pitch_halved.vtt
 
 In addition, it is required to use `--rate=-50%` instead of `--rate -50%` (note the lack of an equal sign) otherwise the `-50%` would be interpreted as just another argument.
 
-**NOTE**: `--pitch` was removed in 6.0.3 as it no longer appears to have any effect.
-
 ### Note on the `edge-playback` command
 
 `edge-playback` is just a wrapper around `edge-tts` that plays back the generated speech. It takes the same arguments as the `edge-tts` option.
 
 ## Python module
 
 It is possible to use the `edge-tts` module directly from Python. For a list of example applications:
```

### Comparing `edge-tts-6.1.8/setup.cfg` & `edge-tts-6.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.8/src/edge_playback/__main__.py` & `edge-tts-6.1.9/src/edge_playback/__main__.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.8/src/edge_tts/communicate.py` & `edge-tts-6.1.9/src/edge_tts/communicate.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,27 +148,27 @@
         text = text[split_at:]
 
     new_text = text.strip()
     if new_text:
         yield new_text
 
 
-def mkssml(text: Union[str, bytes], voice: str, rate: str, volume: str) -> str:
+def mkssml(text: Union[str, bytes], voice: str, rate: str, volume: str, pitch: str) -> str:
     """
     Creates a SSML string from the given parameters.
 
     Returns:
         str: The SSML string.
     """
     if isinstance(text, bytes):
         text = text.decode("utf-8")
 
     ssml = (
         "<speak version='1.0' xmlns='http://www.w3.org/2001/10/synthesis' xml:lang='en-US'>"
-        f"<voice name='{voice}'><prosody pitch='+0Hz' rate='{rate}' volume='{volume}'>"
+        f"<voice name='{voice}'><prosody pitch='{pitch}' rate='{rate}' volume='{volume}'>"
         f"{text}</prosody></voice></speak>"
     )
     return ssml
 
 
 def date_to_string() -> str:
     """
@@ -199,27 +199,27 @@
         "Content-Type:application/ssml+xml\r\n"
         f"X-Timestamp:{timestamp}Z\r\n"  # This is not a mistake, Microsoft Edge bug.
         "Path:ssml\r\n\r\n"
         f"{ssml}"
     )
 
 
-def calc_max_mesg_size(voice: str, rate: str, volume: str) -> int:
+def calc_max_mesg_size(voice: str, rate: str, volume: str, pitch: str) -> int:
     """Calculates the maximum message size for the given voice, rate, and volume.
 
     Returns:
         int: The maximum message size.
     """
     websocket_max_size: int = 2**16
     overhead_per_message: int = (
         len(
             ssml_headers_plus_data(
                 connect_id(),
                 date_to_string(),
-                mkssml("", voice, rate, volume),
+                mkssml("", voice, rate, volume, pitch),
             )
         )
         + 50  # margin of error
     )
     return websocket_max_size - overhead_per_message
 
 
@@ -231,14 +231,15 @@
     def __init__(
         self,
         text: str,
         voice: str = "Microsoft Server Speech Text to Speech Voice (en-US, AriaNeural)",
         *,
         rate: str = "+0%",
         volume: str = "+0%",
+        pitch: str = "+0Hz",
         proxy: Optional[str] = None,
     ):
         """
         Initializes the Communicate class.
 
         Raises:
             ValueError: If the voice is not valid.
@@ -285,24 +286,30 @@
 
         if not isinstance(volume, str):
             raise TypeError("volume must be str")
         if re.match(r"^[+-]\d+%$", volume) is None:
             raise ValueError(f"Invalid volume '{volume}'.")
         self.volume: str = volume
 
+        if not isinstance(pitch, str):
+            raise TypeError("pitch must be str")
+        if re.match(r"^[+-]\d+Hz$", pitch) is None:
+            raise ValueError(f"Invalid pitch '{pitch}'.")
+        self.pitch: str = pitch
+
         if proxy is not None and not isinstance(proxy, str):
             raise TypeError("proxy must be str")
         self.proxy: Optional[str] = proxy
 
     async def stream(self) -> AsyncGenerator[Dict[str, Any], None]:
         """Streams audio and metadata from the service."""
 
         texts = split_text_by_byte_length(
             escape(remove_incompatible_characters(self.text)),
-            calc_max_mesg_size(self.voice, self.rate, self.volume),
+            calc_max_mesg_size(self.voice, self.rate, self.volume, self.pitch),
         )
         final_utterance: Dict[int, int] = {}
         prev_idx = -1
         shift_time = -1
 
         ssl_ctx = ssl.create_default_context(cafile=certifi.where())
         for idx, text in enumerate(texts):
@@ -358,15 +365,15 @@
                     "}}}}\r\n"
                 )
 
                 await websocket.send_str(
                     ssml_headers_plus_data(
                         connect_id(),
                         date,
-                        mkssml(text, self.voice, self.rate, self.volume),
+                        mkssml(text, self.voice, self.rate, self.volume, self.pitch),
                     )
                 )
 
                 async for received in websocket:
                     if received.type == aiohttp.WSMsgType.TEXT:
                         parameters, data = get_headers_and_data(received.data)
                         path = parameters.get(b"Path")
```

### Comparing `edge-tts-6.1.8/src/edge_tts/exceptions.py` & `edge-tts-6.1.9/src/edge_tts/exceptions.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.8/src/edge_tts/list_voices.py` & `edge-tts-6.1.9/src/edge_tts/list_voices.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.8/src/edge_tts/submaker.py` & `edge-tts-6.1.9/src/edge_tts/submaker.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.8/src/edge_tts/util.py` & `edge-tts-6.1.9/src/edge_tts/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     tts: Communicate = Communicate(
         args.text,
         args.voice,
         proxy=args.proxy,
         rate=args.rate,
         volume=args.volume,
+        pitch=args.pitch,
     )
     subs: SubMaker = SubMaker()
     with open(
         args.write_media, "wb"
     ) if args.write_media else sys.stdout.buffer as audio_file:
         async for chunk in tts.stream():
             if chunk["type"] == "audio":
@@ -93,14 +94,15 @@
         "-l",
         "--list-voices",
         help="lists available voices and exits",
         action="store_true",
     )
     parser.add_argument("--rate", help="set TTS rate. Default +0%%.", default="+0%")
     parser.add_argument("--volume", help="set TTS volume. Default +0%%.", default="+0%")
+    parser.add_argument("--pitch", help="set TTS pitch. Default +0Hz.", default="+0Hz")
     parser.add_argument(
         "--words-in-cue",
         help="number of words in a subtitle cue. Default: 10.",
         default=10,
         type=float,
     )
     parser.add_argument(
```

### Comparing `edge-tts-6.1.8/src/edge_tts.egg-info/PKG-INFO` & `edge-tts-6.1.9/src/edge_tts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.8
+Version: 6.1.9
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -75,25 +75,24 @@
 
     $ edge-tts --voice ar-EG-SalmaNeural --text "مرحبا كيف حالك؟" --write-media hello_in_arabic.mp3 --write-subtitles hello_in_arabic.vtt
 
 ### Custom SSML
 
 Support for custom SSML has been removed since 5.0.0 because Microsoft has taken the initiative to prevent it from working. You cannot use custom SSML anymore.
 
-### Changing rate and volume
+### Changing rate, volume and pitch
 
 It is possible to make minor changes to the generated speech.
 
     $ edge-tts --rate=-50% --text "Hello, world!" --write-media hello_with_rate_halved.mp3 --write-subtitles hello_with_rate_halved.vtt
     $ edge-tts --volume=-50% --text "Hello, world!" --write-media hello_with_volume_halved.mp3 --write-subtitles hello_with_volume_halved.vtt
+    $ edge-tts --pitch=-50Hz --text "Hello, world!" --write-media hello_with_pitch_halved.mp3 --write-subtitles hello_with_pitch_halved.vtt
 
 In addition, it is required to use `--rate=-50%` instead of `--rate -50%` (note the lack of an equal sign) otherwise the `-50%` would be interpreted as just another argument.
 
-**NOTE**: `--pitch` was removed in 6.0.3 as it no longer appears to have any effect.
-
 ### Note on the `edge-playback` command
 
 `edge-playback` is just a wrapper around `edge-tts` that plays back the generated speech. It takes the same arguments as the `edge-tts` option.
 
 ## Python module
 
 It is possible to use the `edge-tts` module directly from Python. For a list of example applications:
```

### Comparing `edge-tts-6.1.8/src/edge_tts.egg-info/SOURCES.txt` & `edge-tts-6.1.9/src/edge_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

