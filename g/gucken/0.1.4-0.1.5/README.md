# Comparing `tmp/gucken-0.1.4.tar.gz` & `tmp/gucken-0.1.5.tar.gz`

## Comparing `gucken-0.1.4.tar` & `gucken-0.1.5.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/__main__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/aniskip.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/custom_widgets.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/default_settings.toml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/gucken.css
--rw-r--r--   0        0        0    30111 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/gucken.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/rome.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/settings.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/skip.lua
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/update.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/hoster/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/hoster/_hosters.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/hoster/common.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/hoster/doodstream.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/hoster/streamtape.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/hoster/veo.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/hoster/vidoza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/player/__init__.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/player/_players.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/player/android.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/player/common.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/player/ffplay.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/player/flatpak.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/player/mpv.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/player/vlc.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/player/wmplayer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/provider/__init__.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/provider/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/provider/burningseries.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/provider/common.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/provider/crunchyroll.py
--rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/provider/serienstream.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/provider/streamcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/tracker/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/tracker/anilist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/tracker/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/tracker/common.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/tracker/myanimelist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.4/src/gucken/tracker/serienstream.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.4/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 gucken-0.1.4/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 gucken-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/__main__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/aniskip.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/custom_widgets.py
+-rw-r--r--   0        0        0    32791 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/gucken.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/rome.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/settings.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/update.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/_hosters.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/common.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/doodstream.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/streamtape.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/veo.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/vidoza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/__init__.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/_players.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/android.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/common.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/ffplay.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/flatpak.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/mpv.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/vlc.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/wmplayer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/__init__.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/burningseries.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/common.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/crunchyroll.py
+-rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/serienstream.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/streamcloud.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/resources/default_settings.toml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/resources/gucken.css
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/resources/mpv_skip.lua
+-rwxr-xr-x   0        0        0     3912 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/resources/vlc_skip.lua
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/anilist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/common.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/myanimelist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/serienstream.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 gucken-0.1.5/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 gucken-0.1.5/PKG-INFO
```

### Comparing `gucken-0.1.4/src/gucken/aniskip.py` & `gucken-0.1.5/src/gucken/aniskip.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/custom_widgets.py` & `gucken-0.1.5/src/gucken/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/default_settings.toml` & `gucken-0.1.5/src/gucken/resources/default_settings.toml`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/gucken.css` & `gucken-0.1.5/src/gucken/resources/gucken.css`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/gucken.py` & `gucken-0.1.5/src/gucken/gucken.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import logging
 from asyncio import gather
 from atexit import register as register_atexit
-from os import name as os_name
-from os import remove
+from os import remove, name as os_name
+from os.path import join
 from pathlib import Path
 from random import choice
 from shutil import which
 from subprocess import DEVNULL, PIPE, Popen
 from time import sleep, time
 from typing import ClassVar, List, Union
 
@@ -52,15 +52,15 @@
 from .player.mpv import MPVPlayer
 from .player.vlc import VLCPlayer
 from .provider.aniworld import AniWorldProvider
 from .provider.common import Episode, Language, SearchResult, Series
 from .provider.serienstream import SerienStreamProvider
 from .settings import gucken_settings_manager
 from .update import check
-from .utils import detect_player, is_android
+from .utils import detect_player, is_android, set_default_vlc_interface_cfg, get_vlc_intf_user_path
 
 
 def sort_favorite_lang(
         language_list: List[Language], pio_list: List[str]
 ) -> List[Language]:
     def lang_sort_key(hoster: Language) -> int:
         try:
@@ -203,15 +203,15 @@
 client_id = "1238219157464416266"
 
 
 class GuckenApp(App):
     TITLE = "Gucken TUI"
     # TODO: color theme https://textual.textualize.io/guide/design/#designing-with-colors
 
-    CSS_PATH = ["gucken.css"]
+    CSS_PATH = [join("resources", "gucken.css")]
     custom_css = user_config_path("gucken").joinpath("custom.css")
     if custom_css.exists():
         CSS_PATH.append(custom_css)
     BINDINGS: ClassVar[list[BindingType]] = [
         Binding("q", "quit", "Quit", show=True, priority=False),
     ]
 
@@ -308,27 +308,27 @@
                             available_players_keys,
                             id="player",
                             prompt="AutomaticPlayer",
                             value=(
                                 Select.BLANK if player == "AutomaticPlayer" else player
                             ),
                         )
-                    with Collapsible(title="ani-skip (only for MPV)", collapsed=False):
+                    with Collapsible(title="ani-skip (only for MPV and VLC)", collapsed=False):
                         yield RadioButton(
                             "Skip opening",
                             id="ani_skip_opening",
                             value=settings["ani_skip"]["skip_opening"],
                         )
                         yield RadioButton(
                             "Skip ending",
                             id="ani_skip_ending",
                             value=settings["ani_skip"]["skip_ending"],
                         )
                         yield RadioButton(
-                            "Get chapters",
+                            "Get chapters (only MPV)",
                             id="ani_skip_chapters",
                             value=settings["ani_skip"]["chapters"],
                         )
         with Footer():
             with Center():
                 yield Label("Made by Commandcracker with [red]:heart:[/red]")
 
@@ -456,15 +456,16 @@
             await self.RPC.clear()
             # close without closing event loop
             self.RPC.send_data(2, {"v": 1, "client_id": self.RPC.client_id})
             self.RPC.sock_writer.close()
             self.RPC = None
 
     # TODO: https://textual.textualize.io/guide/workers/#thread-workers
-    @work(exclusive=True)
+    # TODO: Exit on error when debug = true
+    @work(exclusive=True, exit_on_error=False)
     async def lookup_anime(self, keyword: str) -> None:
         search_providers = []
         if self.query_one("#aniworld_to", Checkbox).value:
             search_providers.append(AniWorldProvider.search(keyword))
 
         if self.query_one("#serienstream_to", Checkbox).value:
             search_providers.append(SerienStreamProvider.search(keyword))
@@ -655,52 +656,97 @@
                     # small_text="ff 15",
                     # start=time.time(), # for paused
                     # end=time.time() + timedelta(minutes=20).seconds   # for time left
                 )
 
             self.app.call_later(update)
 
+        if self._debug:
+            logs_path = user_log_path("gucken", ensure_exists=True)
+            if isinstance(_player, MPVPlayer):
+                args.append("--log-file=" + str(logs_path.joinpath("mpv.log")))
+            elif isinstance(_player, VLCPlayer):
+                args.append("--file-logging")
+                args.append("--log-verbose=3")
+                args.append("--logfile=" + str(logs_path.joinpath("vlc.log")))
+
         chapters_file = None
 
         # TODO: cache more
         # TODO: Support based on mpv
         # TODO: recover start --start=00:56
-        if isinstance(_player, MPVPlayer):
+        if isinstance(_player, MPVPlayer) or isinstance(_player, VLCPlayer):
             ani_skip_opening = self.query_one("#ani_skip_opening", RadioButton).value
             ani_skip_ending = self.query_one("#ani_skip_ending", RadioButton).value
             ani_skip_chapters = self.query_one("#ani_skip_chapters", RadioButton).value
 
             if ani_skip_opening or ani_skip_ending or ani_skip_chapters:
                 timings = await get_timings_from_search(
                     series_search_result.name, index + 1
                 )
                 if timings:
-                    if ani_skip_chapters:
-                        chapters_file = generate_chapters_file(timings)
+                    if isinstance(_player, MPVPlayer):
+                        if ani_skip_chapters:
+                            chapters_file = generate_chapters_file(timings)
+
+                            def delete_chapters_file():
+                                try:
+                                    remove(chapters_file.name)
+                                except FileNotFoundError:
+                                    pass
+
+                            register_atexit(delete_chapters_file)
+
+                            args.append(get_chapters_file_mpv_option(chapters_file.name))
+
+                        if ani_skip_opening:
+                            args.append(opening_timings_to_mpv_option(timings))
+
+                        if ani_skip_ending:
+                            args.append(ending_timings_to_mpv_option(timings))
+
+                        args.append("--script=" + str(Path(__file__).parent.joinpath("resources", "mpv_skip.lua")))
+
+                    if isinstance(_player, VLCPlayer):
+                        # cant use --lua-config because it would override syncplay cfg
+                        # cant use --extraintf and --lua-intf because it is already used by syncplay
+                        """
+                            args = [
+                                "vlc",
+                                "--extraintf=luaintf",
+                                "--lua-intf=skip",
+                                "--lua-config=skip={" + f"op_start={op_start},op_end={op_end},ed_start={ed_start},ed_end={ed_end}" +"}",
+                                url
+                            ]
+                        """
+                        prepend_data = ["-- Generated"]
+
+                        if ani_skip_opening:
+                            prepend_data.append(set_default_vlc_interface_cfg("op_start", timings["op_start_time"]))
+                            prepend_data.append(set_default_vlc_interface_cfg("op_end", timings["op_end_time"]))
+
+                        if ani_skip_ending:
+                            prepend_data.append(set_default_vlc_interface_cfg("ed_start", timings["ed_start_time"]))
+                            prepend_data.append(set_default_vlc_interface_cfg("ed_end", timings["ed_end_time"]))
 
-                        def delete_chapters_file():
-                            try:
-                                remove(chapters_file.name)
-                            except FileNotFoundError:
-                                pass
+                        prepend_data.append("-- Generated\n")
 
-                        register_atexit(delete_chapters_file)
+                        vlc_intf_user_path = get_vlc_intf_user_path(_player.executable).vlc_intf_user_path
+                        Path(vlc_intf_user_path).mkdir(mode=0o755, parents=True, exist_ok=True)
 
-                        args.append(get_chapters_file_mpv_option(chapters_file.name))
+                        vlc_skip_plugin = Path(__file__).parent.joinpath("resources", "vlc_skip.lua")
+                        copyTo = join(vlc_intf_user_path, "vlc_skip.lua")
 
-                    if ani_skip_opening:
-                        args.append(opening_timings_to_mpv_option(timings))
+                        with open(vlc_skip_plugin, 'r') as f:
+                            original_content = f.read()
 
-                    if ani_skip_ending:
-                        args.append(ending_timings_to_mpv_option(timings))
+                        with open(copyTo, 'w') as f:
+                            f.write("\n".join(prepend_data) + original_content)
 
-                    args.append("--script=" + str(Path(__file__).parent.joinpath("skip.lua")))
-                    if self._debug:
-                        logs_path = user_log_path("gucken", ensure_exists=True)
-                        args.append("--log-file=" + str(logs_path.joinpath("mpv.log")))
+                        args.append("--control=luaintf{intf=vlc_skip}")
 
         if syncplay:
             # TODO: make work with flatpak
             # TODO: make work with android
             syncplay_path = None
             if which("syncplay"):
                 syncplay_path = "syncplay"
@@ -742,15 +788,15 @@
         # if child_pid == 0:
         process = Popen(args, stderr=PIPE, stdout=DEVNULL, stdin=DEVNULL)
         while not self.app._exit:
             sleep(0.1)
 
             resume_time = None
 
-            # only if mpv
+            # only if mpv WIP
             while not self.app._exit:
                 output = process.stderr.readline()
                 if process.poll() is not None:
                     break
                 if output:
                     out_s = output.strip().decode()
                     # AV: 00:11:57 / 00:24:38 (49%) A-V:  0.000 Cache: 89s/22MB
```

### Comparing `gucken-0.1.4/src/gucken/rome.py` & `gucken-0.1.5/src/gucken/rome.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/settings.py` & `gucken-0.1.5/src/gucken/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,10 +75,10 @@
 
 
 class GuckenSettingsManager(Singleton, SettingsManager):
     pass
 
 
 gucken_settings_manager = GuckenSettingsManager(
-    default_settings_file=Path(__file__).parent.joinpath("default_settings.toml"),
+    default_settings_file=Path(__file__).parent.joinpath("resources", "default_settings.toml"),
     settings_file=user_config_path("gucken").joinpath("settings.toml"),
 )
```

### Comparing `gucken-0.1.4/src/gucken/skip.lua` & `gucken-0.1.5/src/gucken/resources/mpv_skip.lua`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 local mpv_utils = require("mp.utils")
 
 -- Stop script if skip.lua is inside scripts folder
 local scripts_dir = mp.find_config_file("scripts")
 if mpv_utils.file_info(mpv_utils.join_path(scripts_dir, "skip.lua")) ~= nil then
-    mp.msg.info("Disabling, another skip.lua is already present in scripts dir")
-    return
+	mp.msg.info("Disabling, another skip.lua is already present in scripts dir")
+	return
 end
 
 local mpv_options = require("mp.options")
 
 local options = {
-    op_start = 0,
-    op_end = 0,
-    ed_start = 0,
-    ed_end = 0
+	op_start = 0,
+	op_end = 0,
+	ed_start = 0,
+	ed_end = 0,
 }
 mpv_options.read_options(options, "skip")
 
 local skipped_op = false
 local skipped_ed = false
 
 local function check_skip()
-    local current_time = mp.get_property_number("time-pos")
-    if not current_time then return end
-
-    -- Opening
-    if not skipped_op and current_time >= options.op_start and current_time < options.op_end then
-        mp.set_property_number("time-pos", options.op_end)
-        skipped_op = true
-    end
-    
-    -- Ending
-    if not skipped_ed and current_time >= options.ed_start and current_time < options.ed_end then
-        mp.set_property_number("time-pos", options.ed_end)
-        skipped_ed = true
-    end
+	local current_time = mp.get_property_number("time-pos")
+	if not current_time then
+		return
+	end
+
+	-- Opening
+	if not skipped_op and current_time >= options.op_start and current_time < options.op_end then
+		mp.set_property_number("time-pos", options.op_end)
+		skipped_op = true
+	end
+
+	-- Ending
+	if not skipped_ed and current_time >= options.ed_start and current_time < options.ed_end then
+		mp.set_property_number("time-pos", options.ed_end)
+		skipped_ed = true
+	end
 end
 
 mp.observe_property("time-pos", "number", check_skip)
```

### Comparing `gucken-0.1.4/src/gucken/update.py` & `gucken-0.1.5/src/gucken/update.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/hoster/common.py` & `gucken-0.1.5/src/gucken/hoster/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/hoster/doodstream.py` & `gucken-0.1.5/src/gucken/hoster/doodstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/hoster/streamtape.py` & `gucken-0.1.5/src/gucken/hoster/streamtape.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/hoster/veo.py` & `gucken-0.1.5/src/gucken/hoster/veo.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/hoster/vidoza.py` & `gucken-0.1.5/src/gucken/hoster/vidoza.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/player/_players.py` & `gucken-0.1.5/src/gucken/player/_players.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/player/android.py` & `gucken-0.1.5/src/gucken/player/android.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/player/common.py` & `gucken-0.1.5/src/gucken/player/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/player/ffplay.py` & `gucken-0.1.5/src/gucken/player/ffplay.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/player/flatpak.py` & `gucken-0.1.5/src/gucken/player/flatpak.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/player/mpv.py` & `gucken-0.1.5/src/gucken/player/mpv.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/player/vlc.py` & `gucken-0.1.5/src/gucken/player/vlc.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/player/wmplayer.py` & `gucken-0.1.5/src/gucken/player/wmplayer.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/provider/aniworld.py` & `gucken-0.1.5/src/gucken/provider/aniworld.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/provider/common.py` & `gucken-0.1.5/src/gucken/provider/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/provider/serienstream.py` & `gucken-0.1.5/src/gucken/provider/serienstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/src/gucken/tracker/anilist.py` & `gucken-0.1.5/src/gucken/tracker/anilist.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/LICENSE.txt` & `gucken-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gucken-0.1.4/README.md` & `gucken-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,16 @@
 - [ ] BIG CODE CLEANUP
 - [ ] Translation
 - [ ] detect existing chapters and use them for skip
 - [ ] Better settings design
 - [ ] FIX TYPING SOMETIMES CAUSES CRASH
 - [ ] Syncplay on Android
 - [ ] More CLI args
+- [ ] reverse proxy
+- [ ] Chapters for VLC
 
 [Anime4k]: https://github.com/bloc97/Anime4K
 [MPV]: https://mpv.io/
 [VLC]: https://www.videolan.org/vlc/
 [AniWorld.to]: https://aniworld.to
 [SerienStream.to]: https://186.2.175.5
 [Python]: https://www.python.org/downloads/
```

### Comparing `gucken-0.1.4/pyproject.toml` & `gucken-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 dynamic = ["version"]
 description = "Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style."
 authors = [{name="Commandcracker"}]
 maintainers = [{name="Commandcracker"}]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 dependencies = [
-  "textual>=0.60.1",
+  "textual>=0.62.0",
   "beautifulsoup4>=4.12.3",
   "httpx>=0.27.0",
   "pypresence>=4.3.0",
   "packaging>=24.0",
   "platformdirs>=4.2.2",
   "toml>=0.10.2"
   #"yt-dlp>=2024.4.9",
```

### Comparing `gucken-0.1.4/PKG-INFO` & `gucken-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gucken
-Version: 0.1.4
+Version: 0.1.5
 Summary: Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style.
 Project-URL: Repository, https://github.com/Commandcracker/gucken
 Author: Commandcracker
 Maintainer: Commandcracker
 License: MIT License
         
         Copyright (c) 2024 Commandcracker
@@ -45,15 +45,15 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: packaging>=24.0
 Requires-Dist: platformdirs>=4.2.2
 Requires-Dist: pypresence>=4.3.0
-Requires-Dist: textual>=0.60.1
+Requires-Dist: textual>=0.62.0
 Requires-Dist: toml>=0.10.2
 Description-Content-Type: text/markdown
 
 # Gucken
 
 Project state: **Pre-Alpha**
 
@@ -286,14 +286,16 @@
 - [ ] BIG CODE CLEANUP
 - [ ] Translation
 - [ ] detect existing chapters and use them for skip
 - [ ] Better settings design
 - [ ] FIX TYPING SOMETIMES CAUSES CRASH
 - [ ] Syncplay on Android
 - [ ] More CLI args
+- [ ] reverse proxy
+- [ ] Chapters for VLC
 
 [Anime4k]: https://github.com/bloc97/Anime4K
 [MPV]: https://mpv.io/
 [VLC]: https://www.videolan.org/vlc/
 [AniWorld.to]: https://aniworld.to
 [SerienStream.to]: https://186.2.175.5
 [Python]: https://www.python.org/downloads/
```

