# Comparing `tmp/datanommer_commands-1.2.0.tar.gz` & `tmp/datanommer_commands-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanommer_commands-1.2.0.tar", max compression
+gzip compressed data, was "datanommer_commands-1.3.0.tar", max compression
```

## Comparing `datanommer_commands-1.2.0.tar` & `datanommer_commands-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_commands-1.2.0/LICENSE
--rw-r--r--   0        0        0      392 2021-07-05 15:27:34.000000 datanommer_commands-1.2.0/README.rst
--rw-r--r--   0        0        0     1734 2022-07-06 08:10:03.000000 datanommer_commands-1.2.0/config.toml.example
--rw-r--r--   0        0        0    11417 2024-04-15 09:57:21.426639 datanommer_commands-1.2.0/datanommer/commands/__init__.py
--rw-r--r--   0        0        0     5020 2024-04-15 09:57:21.426639 datanommer_commands-1.2.0/datanommer/commands/extract_users.py
--rw-r--r--   0        0        0     2321 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      595 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0    18298 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/test_commands.py
--rw-r--r--   0        0        0     5905 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/test_extract_users.py
--rw-r--r--   0        0        0     1224 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/utils.py
--rw-r--r--   0        0        0      633 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tox.ini
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 datanommer_commands-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_commands-1.3.0/LICENSE
+-rw-r--r--   0        0        0      392 2021-07-05 15:27:34.000000 datanommer_commands-1.3.0/README.rst
+-rw-r--r--   0        0        0     1734 2022-07-06 08:10:03.000000 datanommer_commands-1.3.0/config.toml.example
+-rw-r--r--   0        0        0    11421 2024-05-16 13:59:37.493021 datanommer_commands-1.3.0/datanommer/commands/__init__.py
+-rw-r--r--   0        0        0     5498 2024-05-22 15:36:27.837287 datanommer_commands-1.3.0/datanommer/commands/extract_users.py
+-rw-r--r--   0        0        0     2321 2024-05-22 17:27:32.051456 datanommer_commands-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 09:57:21.427639 datanommer_commands-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      595 2024-05-16 13:59:37.495021 datanommer_commands-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0    18298 2024-05-16 13:59:37.495021 datanommer_commands-1.3.0/tests/test_commands.py
+-rw-r--r--   0        0        0     6419 2024-05-22 15:32:42.478014 datanommer_commands-1.3.0/tests/test_extract_users.py
+-rw-r--r--   0        0        0     1224 2024-05-06 15:52:35.235265 datanommer_commands-1.3.0/tests/utils.py
+-rw-r--r--   0        0        0      633 2024-04-15 09:57:21.427639 datanommer_commands-1.3.0/tox.ini
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 datanommer_commands-1.3.0/PKG-INFO
```

### Comparing `datanommer_commands-1.2.0/LICENSE` & `datanommer_commands-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datanommer_commands-1.2.0/config.toml.example` & `datanommer_commands-1.3.0/config.toml.example`

 * *Files identical despite different names*

### Comparing `datanommer_commands-1.2.0/datanommer/commands/__init__.py` & `datanommer_commands-1.3.0/datanommer/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     is_flag=True,
     help="When combined with --timestamp or --timesince,show a human readable date.",
 )
 def latest(config_path, topic, category, overall, timestamp, timesince, human):
     """Print the latest message(s) ingested by datanommer.
 
     The default is to display the latest message in each message category. The
-    latest in only a specified category or topic can also be returned:
+    latest in only a specified category or topic can also be returned::
 
         $ datanommer-latest --category bodhi
         [{"bodhi": {
           "topic": "org.fedoraproject.stg.bodhi.update.comment",
           "msg": {
             "comment": {
               "group": null,
@@ -231,15 +231,15 @@
               "timestamp": 1360349639.0,
               "update_title": "xmonad-0.10-10.fc17"
             },
             "agent": "ralph"
           },
         }}]
 
-    Or to display the latest, regardless of the topic or category:
+    Or to display the latest, regardless of the topic or category::
 
         $ datanommer-latest --overall
         [{"bodhi": {
           "topic": "org.fedoraproject.stg.bodhi.update.comment",
           "msg": {
             "comment": {
               "group": null,
@@ -251,24 +251,24 @@
               "update_title": "xmonad-0.10-10.fc17"
             },
             "agent": "ralph"
           },
         }}]
 
     You can combine either a --topic, --category or --overall argument while
-    requesting information about the timestamp of the latest:
+    requesting information about the timestamp of the latest::
 
         $ datanommer-latest --category wiki --timestamp
         [1361166918.0]
 
         # February 18, 2013 at 5:55AM
         $ datanommer-latest --category wiki --timestamp --human
         ["2013-02-18 05:55:18"]
 
-    Or how recent that timestamp is:
+    Or how recent that timestamp is::
 
         # 49250 seconds ago
         $ datanommer-latest --category wiki --timesince
         [49250]
 
         # 13 hours, 40 minutes, 59.52 seconds ago
         $ datanommer-latest --category wiki --timesince --human
```

### Comparing `datanommer_commands-1.2.0/datanommer/commands/extract_users.py` & `datanommer_commands-1.3.0/datanommer/commands/extract_users.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import datetime
 import logging
 
 import click
 from fedora_messaging.exceptions import ValidationError
 from fedora_messaging.message import load_message as load_message
-from sqlalchemy import and_, func, select
+from sqlalchemy import and_, func, not_, select
 
 import datanommer.models as m
 
 from . import config_option, get_config
 
 
-# Go trough messages these many days at a time
-CHUNK_DAYS = 30
+# Go trough messages these at a time
+CHUNK_SIZE = 10000
 log = logging.getLogger(__name__)
 
+SKIP_TOPICS = [
+    "%.anitya.%",
+    "%.discourse.%",
+    "%.hotness.update.bug.file",
+    "%.koschei.%",
+    "%.mdapi.%",
+]
+
 
 @click.command()
 @config_option
 @click.option("--topic", default=None, help="Only extract users for messages of a specific topic.")
 @click.option(
     "--category",
     default=None,
@@ -41,26 +49,26 @@
     default=None,
     help=(
         "Force usage of this schema name to extract usernames. This is the key in the "
         "exposed entry point / plugin, for example: wiki.article.edit.v1"
     ),
 )
 @click.option(
-    "--chunk-size-days",
-    default=CHUNK_DAYS,
+    "--chunk-size",
+    default=CHUNK_SIZE,
     type=int,
     show_default=True,
-    help="Go through messages these many days at a time (lower is slower but saves memory).",
+    help="Go through messages these many at a time (lower is slower but saves memory).",
 )
 @click.option(
     "--debug",
     is_flag=True,
     help="Show more information.",
 )
-def main(config_path, topic, category, start, end, force_schema, chunk_size_days, debug):
+def main(config_path, topic, category, start, end, force_schema, chunk_size, debug):
     """Go over old messages, extract users and store them.
 
     This is useful when a message schema has been added and we want to populate the users table
     with the new information.
     """
     config = get_config(config_path)
     m.init(
@@ -72,24 +80,31 @@
         raise click.UsageError("can't use both --topic and --category, choose one.")
 
     query = select(m.Message)
     if topic:
         query = query.where(m.Message.topic == topic)
     elif category:
         query = query.where(m.Message.category == category)
+    else:
+        query = query.where(and_(*[not_(m.Message.topic.like(skipped)) for skipped in SKIP_TOPICS]))
     if start:
         query = query.where(m.Message.timestamp >= start)
     else:
         start = m.session.execute(
             select(m.Message.timestamp).order_by(m.Message.timestamp).limit(1)
         ).scalar_one()
     if end:
         query = query.where(m.Message.timestamp < end)
     else:
         end = datetime.datetime.now()
+    if force_schema is None:
+        query = query.where(
+            m.Message.headers.has_key("fedora_messaging_schema"),
+            m.Message.headers["fedora_messaging_schema"].astext != "base.message",
+        )
 
     query = query.join(
         m.users_assoc_table,
         and_(
             m.Message.id == m.users_assoc_table.c.msg_id,
             m.Message.timestamp == m.users_assoc_table.c.msg_timestamp,
         ),
@@ -100,36 +115,38 @@
     if not total:
         click.echo("No messages matched.")
         return
 
     click.echo(f"Considering {total} message{'s' if total > 1 else ''}")
 
     query = query.order_by(m.Message.timestamp)
-    chunk_timedelta = datetime.timedelta(days=chunk_size_days)
     with click.progressbar(length=total) as bar:
-        chunk_start = start - chunk_timedelta
-        chunk_end = start
-        while chunk_end < end:
-            chunk_start += chunk_timedelta
-            chunk_end += chunk_timedelta
-            chunk_query = query.where(
-                m.Message.timestamp >= chunk_start, m.Message.timestamp < chunk_end
-            )
+        has_messages = True
+        chunk_start = start
+        first_run = True
+        while has_messages:
+            chunk_query = query.where(m.Message.timestamp >= chunk_start).limit(chunk_size)
+            if not first_run:
+                chunk_query = chunk_query.offset(1)
+            has_messages = False
             for message in m.session.scalars(chunk_query):
                 bar.update(1)
+                has_messages = True
                 usernames = get_usernames(message, force_schema=force_schema)
                 if not usernames:
                     m.session.expunge(message)
                     continue
                 message._insert_list(m.User, m.users_assoc_table, usernames)
                 if debug:
                     click.echo(
                         f"Usernames for message {message.msg_id} of topic {message.topic}"
                         f": {', '.join(usernames)}"
                     )
+            chunk_start = message.timestamp
+            first_run = False
             m.session.commit()
             m.session.expunge_all()
 
 
 def get_usernames(db_message, force_schema):
     headers = db_message.headers
     if force_schema and headers is not None:
```

### Comparing `datanommer_commands-1.2.0/pyproject.toml` & `datanommer_commands-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datanommer.commands"
-version = "1.2.0"
+version = "1.3.0"
 description = "Console commands for datanommer"
 authors = [
   "Fedora Infrastructure <admin@fedoraproject.org>"
 ]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 repository = "https://github.com/fedora-infra/datanommer"
```

### Comparing `datanommer_commands-1.2.0/tests/conftest.py` & `datanommer_commands-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datanommer_commands-1.2.0/tests/test_commands.py` & `datanommer_commands-1.3.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `datanommer_commands-1.2.0/tests/test_extract_users.py` & `datanommer_commands-1.3.0/tests/test_extract_users.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,16 +92,31 @@
 def test_extract_users_topic_and_category(mock_config, mock_init):
     runner = CliRunner()
     result = runner.invoke(extract_users, ["--category", "bodhi", "--topic", "some.topic"])
     assert result.exit_code != 0, result.output
     assert "Error: can't use both --topic and --category, choose one." in result.output
 
 
+def test_extract_users_skipped_topic(bodhi_message_db, mock_config, mock_init):
+    bodhi_message_db.topic = "org.release-monitoring.prod.anitya.project.version.update"
+    m.session.commit()
+
+    runner = CliRunner()
+    result = runner.invoke(extract_users)
+
+    assert result.exit_code == 0, result.output
+
+    m.session.refresh(bodhi_message_db)
+    assert len(bodhi_message_db.users) == 0
+
+
 def test_extract_users_no_users(datanommer_models, mock_config, mock_init):
     msg = generate_message()
+    # change the schema header or the script won't pick it up
+    msg._headers["fedora_messaging_schema"] = "testing"
     m.add(msg)
     runner = CliRunner()
     result = runner.invoke(extract_users)
 
     assert result.exit_code == 0, result.output
     users_count = m.session.scalar(sa.select(sa.func.count(m.users_assoc_table.c.msg_id)))
     assert users_count == 0
```

### Comparing `datanommer_commands-1.2.0/tests/utils.py` & `datanommer_commands-1.3.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datanommer_commands-1.2.0/tox.ini` & `datanommer_commands-1.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `datanommer_commands-1.2.0/PKG-INFO` & `datanommer_commands-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datanommer.commands
-Version: 1.2.0
+Version: 1.3.0
 Summary: Console commands for datanommer
 Home-page: https://github.com/fedora-infra/datanommer
 License: GPL-3.0-or-later
 Author: Fedora Infrastructure
 Author-email: admin@fedoraproject.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

