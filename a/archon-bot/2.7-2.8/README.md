# Comparing `tmp/archon-bot-2.7.tar.gz` & `tmp/archon_bot-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archon-bot-2.7.tar", last modified: Tue Jan 16 08:11:05 2024, max compression
+gzip compressed data, was "archon_bot-2.8.tar", last modified: Wed May 22 08:32:21 2024, max compression
```

## Comparing `archon-bot-2.7.tar` & `archon_bot-2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-01-16 08:11:05.024235 archon-bot-2.7/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     4499 2024-01-16 08:11:04.000000 archon-bot-2.7/CHANGELOG.rst
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2024-01-16 08:11:04.000000 archon-bot-2.7/LICENSE
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      209 2024-01-16 08:11:04.000000 archon-bot-2.7/MANIFEST.in
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    24754 2024-01-16 08:11:05.024129 archon-bot-2.7/PKG-INFO
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    23509 2024-01-16 08:11:04.000000 archon-bot-2.7/README.md
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-01-16 08:11:05.022801 archon-bot-2.7/archon_bot/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)       35 2024-01-16 08:11:04.000000 archon-bot-2.7/archon_bot/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)       27 2024-01-16 08:11:04.000000 archon-bot-2.7/archon_bot/__main__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     9630 2024-01-16 08:11:04.000000 archon-bot-2.7/archon_bot/bot.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)   155927 2024-01-16 08:11:04.000000 archon-bot-2.7/archon_bot/commands.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     7153 2024-01-16 08:11:04.000000 archon-bot-2.7/archon_bot/db.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1098 2024-01-16 08:11:04.000000 archon-bot-2.7/archon_bot/permissions.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    39917 2024-01-16 08:11:04.000000 archon-bot-2.7/archon_bot/tournament.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2128 2024-01-16 08:11:04.000000 archon-bot-2.7/archon_bot/utils.py
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-01-16 08:11:05.023598 archon-bot-2.7/archon_bot.egg-info/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      284 2024-01-16 08:11:05.000000 archon-bot-2.7/archon_bot.egg-info/SOURCES.txt
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-01-16 08:11:05.023134 archon-bot-2.7/images/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)   264772 2024-01-16 08:11:04.000000 archon-bot-2.7/images/integrations.png
--rw-r--r--   0 lpanhaleux   (501) staff       (20)   111417 2024-01-16 08:11:04.000000 archon-bot-2.7/images/permissions.png
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1423 2024-01-16 08:11:05.024605 archon-bot-2.7/setup.cfg
--rw-r--r--   0 lpanhaleux   (501) staff       (20)       39 2024-01-16 08:11:04.000000 archon-bot-2.7/setup.py
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-05-22 08:32:21.664471 archon_bot-2.8/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     4618 2024-05-22 08:32:21.000000 archon_bot-2.8/CHANGELOG.rst
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2024-05-22 08:32:21.000000 archon_bot-2.8/LICENSE
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      209 2024-05-22 08:32:21.000000 archon_bot-2.8/MANIFEST.in
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    24754 2024-05-22 08:32:21.663724 archon_bot-2.8/PKG-INFO
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    23509 2024-05-22 08:32:21.000000 archon_bot-2.8/README.md
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-05-22 08:32:21.661510 archon_bot-2.8/archon_bot/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)       35 2024-05-22 08:32:21.000000 archon_bot-2.8/archon_bot/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)       27 2024-05-22 08:32:21.000000 archon_bot-2.8/archon_bot/__main__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     9631 2024-05-22 08:32:21.000000 archon_bot-2.8/archon_bot/bot.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   156959 2024-05-22 08:32:21.000000 archon_bot-2.8/archon_bot/commands.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     7153 2024-05-22 08:32:21.000000 archon_bot-2.8/archon_bot/db.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1098 2024-05-22 08:32:21.000000 archon_bot-2.8/archon_bot/permissions.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    39917 2024-05-22 08:32:21.000000 archon_bot-2.8/archon_bot/tournament.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2129 2024-05-22 08:32:21.000000 archon_bot-2.8/archon_bot/utils.py
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-05-22 08:32:21.663045 archon_bot-2.8/archon_bot.egg-info/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      284 2024-05-22 08:32:21.000000 archon_bot-2.8/archon_bot.egg-info/SOURCES.txt
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-05-22 08:32:21.662514 archon_bot-2.8/images/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   264772 2024-05-22 08:32:21.000000 archon_bot-2.8/images/integrations.png
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   111417 2024-05-22 08:32:21.000000 archon_bot-2.8/images/permissions.png
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1423 2024-05-22 08:32:21.665118 archon_bot-2.8/setup.cfg
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)       39 2024-05-22 08:32:21.000000 archon_bot-2.8/setup.py
```

### Comparing `archon-bot-2.7/CHANGELOG.rst` & `archon_bot-2.8/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2.8 (2024-05-22)
+----------------
+
+- BUGIFX: `download-reports` now works even with more than 10 files (many rounds)
+
+
 2.7 (2024-01-16)
 ----------------
 
 - BUGIFX: `standings` now displays the correct rank
 
 
 2.6 (2024-01-09)
```

### Comparing `archon-bot-2.7/LICENSE` & `archon_bot-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `archon-bot-2.7/PKG-INFO` & `archon_bot-2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archon-bot
-Version: 2.7
+Version: 2.8
 Summary: "Discord bot for VTES tournaments",
 Home-page: http://github.com/lionel-panhaleux/archon-bot
 Author: lionelpx
 Author-email: lionel.panhaleux@gmail.com
 License: "MIT"
 Keywords: vampire vtes ccg discord bot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `archon-bot-2.7/README.md` & `archon_bot-2.8/README.md`

 * *Files identical despite different names*

### Comparing `archon-bot-2.7/archon_bot/bot.py` & `archon_bot-2.8/archon_bot/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Discord Bot."""
+
 import asyncio
 import logging
 import os
 
 import hikari
 import krcg.vtes
```

### Comparing `archon-bot-2.7/archon_bot/commands.py` & `archon_bot-2.8/archon_bot/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import io
 import json
 import logging
 import random
 import re
 from dataclasses import dataclass, field, asdict
 from typing import Iterable, List, Optional, Union
-
+import zipfile
 
 import hikari
 import hikari.channels
 import hikari.guilds
 import hikari.users
 from hikari.interactions.base_interactions import ResponseType
 from hikari.interactions.command_interactions import CommandInteraction
@@ -982,40 +982,48 @@
             COMPONENTS.pop("multideck", None)
             COMPONENTS.pop("register-between", None)
             COMPONENTS.pop("validate", None)
         else:
             components = [
                 self.bot.rest.build_message_action_row()
                 .add_interactive_button(
-                    hikari.ButtonStyle.SECONDARY
-                    if vekn_required
-                    else hikari.ButtonStyle.PRIMARY,
+                    (
+                        hikari.ButtonStyle.SECONDARY
+                        if vekn_required
+                        else hikari.ButtonStyle.PRIMARY
+                    ),
                     "vekn-required",
                     label=("No VEKN" if vekn_required else "Require VEKN"),
                 )
                 .add_interactive_button(
-                    hikari.ButtonStyle.SECONDARY
-                    if decklist_required
-                    else hikari.ButtonStyle.PRIMARY,
+                    (
+                        hikari.ButtonStyle.SECONDARY
+                        if decklist_required
+                        else hikari.ButtonStyle.PRIMARY
+                    ),
                     "decklist-required",
                     label=("No Decklist" if decklist_required else "Require Decklist"),
                 )
                 .add_interactive_button(
-                    hikari.ButtonStyle.SECONDARY
-                    if checkin_each_round
-                    else hikari.ButtonStyle.PRIMARY,
+                    (
+                        hikari.ButtonStyle.SECONDARY
+                        if checkin_each_round
+                        else hikari.ButtonStyle.PRIMARY
+                    ),
                     "checkin-each-round",
                     label=(
                         "Checkin once" if checkin_each_round else "Checkin each round"
                     ),
                 )
                 .add_interactive_button(
-                    hikari.ButtonStyle.SECONDARY
-                    if multideck
-                    else hikari.ButtonStyle.PRIMARY,
+                    (
+                        hikari.ButtonStyle.SECONDARY
+                        if multideck
+                        else hikari.ButtonStyle.PRIMARY
+                    ),
                     "multideck",
                     label=("Single Deck" if multideck else "Multideck"),
                 ),
                 self.bot.rest.build_message_action_row().add_interactive_button(
                     hikari.ButtonStyle.SUCCESS, "validate", label="OK"
                 ),
             ]
@@ -1023,17 +1031,19 @@
             COMPONENTS["decklist-required"] = ConfigureTournament
             COMPONENTS["checkin-each-round"] = ConfigureTournament
             COMPONENTS["multideck"] = ConfigureTournament
             COMPONENTS["validate"] = ConfigureTournament
             # only allow to activate the register-between option if not staggered
             if not self.tournament.flags & tournament.TournamentFlag.STAGGERED:
                 components[0].add_interactive_button(
-                    hikari.ButtonStyle.SECONDARY
-                    if between
-                    else hikari.ButtonStyle.PRIMARY,
+                    (
+                        hikari.ButtonStyle.SECONDARY
+                        if between
+                        else hikari.ButtonStyle.PRIMARY
+                    ),
                     "register-between",
                     label=("No late joiners" if between else "Join anytime"),
                 )
                 COMPONENTS["register-between"] = ConfigureTournament
         # main embed
         embed = hikari.Embed(
             title=f"Configuration - {self.tournament.name}",
@@ -1745,15 +1755,16 @@
         elif (
             self.tournament.flags & tournament.TournamentFlag.DECKLIST_REQUIRED
             and not player.deck
         ):
             description += (
                 "\n\n**Deck list required**\n"
                 "A decklist is required to participate, please use "
-                f"{UploadDeckFor.mention} to provide one before the tournament begins."
+                f"{UploadDeckFor.mention()} "
+                "to provide one before the tournament begins."
             )
         elif (
             self.tournament.max_rounds
             and self.player_rounds_played(player) >= self.max_rounds
         ):
             description += (
                 "\n\n**Maximum number of rounds**\n"
@@ -2649,17 +2660,19 @@
         vekn = vekn or self.discord.get_vekn(user)
         self.tournament.report(vekn, vp, round)
         await self.update()
         await self.create_or_edit_response(
             content=(
                 f"Result registered: {vp:.2g} VPs for {self._player_display(vekn)}"
             ),
-            flags=hikari.UNDEFINED
-            if self._is_judge_channel()
-            else hikari.MessageFlag.EPHEMERAL,
+            flags=(
+                hikari.UNDEFINED
+                if self._is_judge_channel()
+                else hikari.MessageFlag.EPHEMERAL
+            ),
         )
         if round is not None:
             return
         info = self.tournament.player_info(vekn)
         if not info.table:
             return
         embed = hikari.Embed(
@@ -2707,17 +2720,19 @@
     async def __call__(
         self, table: int, note: str, round: Optional[int] = None
     ) -> None:
         self.tournament.validate_score(table, self.author.id, note, round)
         await self.update()
         await self.create_or_edit_response(
             content=f"Score validated for table {table}: {note}",
-            flags=hikari.UNDEFINED
-            if self._is_judge_channel()
-            else hikari.MessageFlag.EPHEMERAL,
+            flags=(
+                hikari.UNDEFINED
+                if self._is_judge_channel()
+                else hikari.MessageFlag.EPHEMERAL
+            ),
         )
 
 
 def note_level_int(level: tournament.NoteLevel) -> int:
     """Note level as int. The higher the penalty, the higher the int."""
     return list(tournament.NoteLevel.__members__.values()).index(level)
 
@@ -3715,15 +3730,14 @@
         tournament.PlayerStatus.WAITING: "",
         tournament.PlayerStatus.CHECKED_OUT: "❌",  # red cross
         tournament.PlayerStatus.DROPPED_OUT: "🛑",  # red octogon
     }[status]
 
 
 class PlayersList(BaseCommand):
-
     """Players list with status icon - useful to sheperd the flock."""
 
     UPDATE = db.UpdateLevel.READ_ONLY
     ACCESS = CommandAccess.JUDGE
     DESCRIPTION = "JUDGE: Display the list of players"
     OPTIONS = [
         hikari.CommandOption(
@@ -3774,42 +3788,54 @@
         if self.tournament.flags & tournament.TournamentFlag.DECKLIST_REQUIRED:
             reports.append(self._build_decks_json())
         if self.tournament.flags & tournament.TournamentFlag.VEKN_REQUIRED:
             reports.append(self._build_methuselahs_csv())
             reports.extend(f for f in self._build_rounds_csvs())
             if self.tournament.state == tournament.TournamentState.FINISHED:
                 reports.append(self._build_finals_csv())
+        # Discord limits to 10 attachments: zip if there are more (eg. league)
+        if len(reports) > 10:
+            tmp = io.BytesIO()
+            with zipfile.ZipFile(tmp, "w") as archive:
+                for r in reports:
+                    archive.writestr(r.filename, r.data)
+                tmp.seek(0)
+            reports = [
+                hikari.Bytes(tmp.getvalue(), "reports.zip", mimetype="application/zip")
+            ]
         await self.create_or_edit_response(
             embed=hikari.Embed(
                 title="Reports",
                 description=(
                     "Download those file and store them safely before you close "
                     "the tournament."
                 ),
             ),
             attachments=reports,
             flags=hikari.MessageFlag.EPHEMERAL,
         )
 
-    def _build_csv(self, filename: str, it: Iterable[str], columns=None):
+    def _build_csv(
+        self, filename: str, it: Iterable[str], columns=None
+    ) -> hikari.Bytes:
         buffer = io.StringIO()
         writer = csv.writer(buffer)
         if columns:
             writer.writerow(columns)
         writer.writerows(it)
         buffer = io.BytesIO(buffer.getvalue().encode("utf-8"))
         return hikari.Bytes(buffer, filename, mimetype="text/csv")
 
-    def _build_json(self, filename: str, data: str):
+    def _build_json(self, filename: str, data: str) -> hikari.Bytes:
         buffer = io.StringIO()
         json.dump(data, buffer, indent=2)
         buffer = io.BytesIO(buffer.getvalue().encode("utf-8"))
         return hikari.Bytes(buffer, filename, mimetype="application/json")
 
-    def _build_results_csv(self):
+    def _build_results_csv(self) -> hikari.Bytes:
         _winner, ranking = self.tournament.standings()
         data = []
         report_number = 1
         for rank, vekn, score in ranking:
             if vekn in self.tournament.dropped:
                 rank = "DQ"
             info = self.tournament.player_info(vekn)
@@ -3841,15 +3867,15 @@
                 "Games Won",
                 "Total VPs",
                 "Finals Position",
                 "Rank",
             ],
         )
 
-    def _build_decks_json(self):
+    def _build_decks_json(self) -> hikari.Bytes:
         """List of decks."""
         data = []
         for player in sorted(
             self.tournament.players.values(),
             key=lambda p: self._report_number.get(p.vekn, 0),
         ):
             info = self.tournament.player_info(player.vekn)
@@ -3875,15 +3901,15 @@
         else:
             name = player.name
         name = name.split(" ", 1)
         if len(name) < 2:
             name.append("")
         return name
 
-    def _build_methuselahs_csv(self):
+    def _build_methuselahs_csv(self) -> hikari.Bytes:
         data = []
         for player in sorted(
             self.tournament.players.values(),
             key=lambda p: self._report_number.get(p.vekn, 0),
         ):
             if not self._report_number.get(player.vekn, None):
                 continue
@@ -3893,26 +3919,28 @@
                 [
                     self._report_number[player.vekn],
                     name[0],
                     name[1],
                     "",  # country
                     player.vekn,
                     info.rounds,
-                    "DQ"
-                    if info.status
-                    in [
-                        tournament.PlayerStatus.DISQUALIFIED
-                        or tournament.PlayerStatus.DROPPED_OUT
-                    ]
-                    else "",
+                    (
+                        "DQ"
+                        if info.status
+                        in [
+                            tournament.PlayerStatus.DISQUALIFIED
+                            or tournament.PlayerStatus.DROPPED_OUT
+                        ]
+                        else ""
+                    ),
                 ]
             )
         return self._build_csv("Methuselahs.csv", data)
 
-    def _build_rounds_csvs(self):
+    def _build_rounds_csvs(self) -> hikari.Bytes:
         for i, round in enumerate(self.tournament.rounds, 1):
             if not round.results:
                 break
             if round.finals:
                 break
             data = []
             for j, table in enumerate(round.seating, 1):
@@ -3928,15 +3956,15 @@
                             round.results.get(player.vekn, tournament.Score()).vp,
                         ]
                     )
                 if len(table) < 5:
                     data.append(["", "", "", "", ""])
             yield self._build_csv(f"Round-{i}.csv", data)
 
-    def _build_finals_csv(self):
+    def _build_finals_csv(self) -> hikari.Bytes:
         data = []
         round = self.tournament.rounds[-1]
         if not round.finals:
             raise RuntimeError("No finals")
         players = sorted(
             [self.tournament.players[n] for n in round.seating[0]], key=lambda p: p.seed
         )
```

### Comparing `archon-bot-2.7/archon_bot/db.py` & `archon_bot-2.8/archon_bot/db.py`

 * *Files identical despite different names*

### Comparing `archon-bot-2.7/archon_bot/permissions.py` & `archon_bot-2.8/archon_bot/permissions.py`

 * *Files identical despite different names*

### Comparing `archon-bot-2.7/archon_bot/tournament.py` & `archon_bot-2.8/archon_bot/tournament.py`

 * *Files identical despite different names*

### Comparing `archon-bot-2.7/archon_bot/utils.py` & `archon_bot-2.8/archon_bot/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Useful generic tools
 """
+
 import logging
 from dataclasses import is_dataclass
 from typing import get_args, get_origin, Union, TypeVar
 
 # TODO: remove conditional on upgrade
 # python 3.9 backward compatibility
 try:
```

### Comparing `archon-bot-2.7/images/integrations.png` & `archon_bot-2.8/images/integrations.png`

 * *Files identical despite different names*

### Comparing `archon-bot-2.7/images/permissions.png` & `archon_bot-2.8/images/permissions.png`

 * *Files identical despite different names*

### Comparing `archon-bot-2.7/setup.cfg` & `archon_bot-2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = archon-bot
-version = 2.7
+version = 2.8
 author = lionelpx
 author_email = lionel.panhaleux@gmail.com
 url = http://github.com/lionel-panhaleux/archon-bot
 description = "Discord bot for VTES tournaments",
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = "MIT"
```

