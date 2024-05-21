# Comparing `tmp/cs.app.playon-20240316.tar.gz` & `tmp/cs.app.playon-20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.app.playon-20240316.tar", last modified: Sat Mar 16 06:53:30 2024, max compression
+gzip compressed data, was "cs.app.playon-20240522.tar", last modified: Tue May 21 23:35:48 2024, max compression
```

## Comparing `cs.app.playon-20240316.tar` & `cs.app.playon-20240522.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:53:30.882673 cs.app.playon-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:53:19.000000 cs.app.playon-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     6933 2024-03-16 06:53:30.882368 cs.app.playon-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    13482 2024-03-16 06:53:23.000000 cs.app.playon-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:53:30.877681 cs.app.playon-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:53:30.878182 cs.app.playon-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:53:30.878324 cs.app.playon-20240316/lib/python/cs/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:53:30.881786 cs.app.playon-20240316/lib/python/cs/app/
--rw-r--r--   0 cameron    (501) cameron    (502)    33831 2024-03-16 06:53:10.000000 cs.app.playon-20240316/lib/python/cs/app/playon.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:53:30.881441 cs.app.playon-20240316/lib/python/cs.app.playon.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     6933 2024-03-16 06:53:30.000000 cs.app.playon-20240316/lib/python/cs.app.playon.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      354 2024-03-16 06:53:30.000000 cs.app.playon-20240316/lib/python/cs.app.playon.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:53:30.000000 cs.app.playon-20240316/lib/python/cs.app.playon.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       46 2024-03-16 06:53:30.000000 cs.app.playon-20240316/lib/python/cs.app.playon.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      329 2024-03-16 06:53:30.000000 cs.app.playon-20240316/lib/python/cs.app.playon.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:53:30.000000 cs.app.playon-20240316/lib/python/cs.app.playon.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     7760 2024-03-16 06:53:29.000000 cs.app.playon-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:53:30.882778 cs.app.playon-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:35:48.900094 cs.app.playon-20240522/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-21 23:35:36.000000 cs.app.playon-20240522/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15209 2024-05-21 23:35:48.899816 cs.app.playon-20240522/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    14404 2024-05-21 23:35:41.000000 cs.app.playon-20240522/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:35:48.896526 cs.app.playon-20240522/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:35:48.896768 cs.app.playon-20240522/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:35:48.896853 cs.app.playon-20240522/lib/python/cs/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:35:48.899380 cs.app.playon-20240522/lib/python/cs/app/
+-rw-r--r--   0 cameron    (501) cameron    (502)    38143 2024-05-21 23:35:23.000000 cs.app.playon-20240522/lib/python/cs/app/playon.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:35:48.899126 cs.app.playon-20240522/lib/python/cs.app.playon.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15209 2024-05-21 23:35:48.000000 cs.app.playon-20240522/lib/python/cs.app.playon.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      354 2024-05-21 23:35:48.000000 cs.app.playon-20240522/lib/python/cs.app.playon.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-21 23:35:48.000000 cs.app.playon-20240522/lib/python/cs.app.playon.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       46 2024-05-21 23:35:48.000000 cs.app.playon-20240522/lib/python/cs.app.playon.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      392 2024-05-21 23:35:48.000000 cs.app.playon-20240522/lib/python/cs.app.playon.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-21 23:35:48.000000 cs.app.playon-20240522/lib/python/cs.app.playon.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    16128 2024-05-21 23:35:47.000000 cs.app.playon-20240522/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-21 23:35:48.900173 cs.app.playon-20240522/setup.cfg
```

### Comparing `cs.app.playon-20240316/README.md` & `cs.app.playon-20240522/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,38 @@
+Metadata-Version: 2.1
+Name: cs.app.playon
+Version: 20240522
+Summary: PlayOn facilities, primarily access to the download API. Includes a nice command line tool.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python3
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 PlayOn facilities, primarily access to the download API.
 Includes a nice command line tool.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240522*:
+New superior tv-series/season/episode inference.
 
 ## Function `main(argv=None)`
 
 Playon command line mode;
 see the `PlayOnCommand` class below.
 
-## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI, cs.service_api.ServiceAPI, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI)`
 
 Access to the PlayOn API.
 
 *Method `PlayOnAPI.__getitem__(self, download_id: int)`*:
 Return the recording `TagSet` associated with the recording `download_id`.
 
 *Method `PlayOnAPI.account(self)`*:
@@ -40,15 +59,15 @@
 
 *Method `PlayOnAPI.available(self)`*:
 Return the `TagSet` instances for the available recordings.
 
 *Method `PlayOnAPI.cdsurl_data(self, suburl, _method='GET', headers=None, **kw)`*:
 Wrapper for `suburl_data` using `CDS_BASE` as the base URL.
 
-*Method `PlayOnAPI.download(self, download_id: int, filename=None, *, runstate: cs.resources.RunState)`*:
+*Method `PlayOnAPI.download(self, download_id: int, filename=None, *, runstate: Optional[cs.resources.RunState] = <function uses_runstate.<locals>.<lambda> at 0x106a6dab0>)`*:
 Download the file with `download_id` to `filename_basis`.
 Return the `TagSet` for the recording.
 
 The default `filename` is the basename of the filename
 from the download.
 If the filename is supplied with a trailing dot (`'.'`)
 then the file extension will be taken from the filename
@@ -108,15 +127,17 @@
   result keys and returning `result['data']`
 Other keyword arguments are passed to the `HTTPServiceAPI.json` method.
 
 ## Class `PlayOnCommand(cs.cmdutils.BaseCommand)`
 
 Playon command line implementation.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: playon subcommand [args...]
 
         Environment:
           PLAYON_USER               PlayOn login name, default from $EMAIL.
           PLAYON_PASSWORD           PlayOn password.
                                     This is obtained from .netrc if omitted.
@@ -158,28 +179,33 @@
           This outputs the full help for the named subcommands,
           or the short help for all subcommands if no names are specified.
           -l  Long help even if no subcommand-names provided.
         ls [-l] [recordings...]
           List available downloads.
           -l        Long listing: list tags below each entry.
           -o format Format string for each entry.
-          Default format: {playon.ID} {playon.HumanSize} {resolution} {playon.Series} {playon.Name} {playon.ProviderID} {status:upper}
+          Default format: {playon.ID} {playon.HumanSize} {resolution} {nice_name} {playon.ProviderID} {status:upper}
         poll ...
         q [-l] [recordings...]
           List queued recordings.
           -l        Long listing: list tags below each entry.
           -o format Format string for each entry.
           Default format: {playon.ID} {playon.Series} {playon.Name} {playon.ProviderID}
         queue [-l] [recordings...]
           List queued recordings.
           -l        Long listing: list tags below each entry.
           -o format Format string for each entry.
           Default format: {playon.ID} {playon.Series} {playon.Name} {playon.ProviderID}
         refresh [queue] [recordings]
           Update the db state from the PlayOn service.
+        rename [-o filename_format] filenames...
+          Rename the filenames according to their fstags.
+          -n    No action, dry run.
+          -o filename_format
+                Format for the new filename, default '{series_prefix}{series_episode_name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}'.
         service [service_id]
           List services.
         shell
           Run a command prompt via cmd.Cmd using this command's subcommands.
 
 *`PlayOnCommand.Options`*
 
@@ -234,22 +260,38 @@
 -o format Format string for each entry.
 Default format: {QUEUE_FORMAT}
 
 *Method `PlayOnCommand.cmd_refresh(self, argv)`*:
 Usage: {cmd} [queue] [recordings]
 Update the db state from the PlayOn service.
 
+*Method `PlayOnCommand.cmd_rename(self, argv, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x105c65ea0>)`*:
+Usage: {cmd} [-o filename_format] filenames...
+Rename the filenames according to their fstags.
+-n    No action, dry run.
+-o filename_format
+      Format for the new filename, default {DEFAULT_FILENAME_FORMAT!r}.
+
 *Method `PlayOnCommand.cmd_service(self, argv, locale='en_US')`*:
 Usage: {cmd} [service_id]
 List services.
 
 *Method `PlayOnCommand.run_context(self)`*:
 Prepare the `PlayOnAPI` around each command invocation.
 
-## Class `PlayOnSQLTags(cs.sqltags.SQLTags, cs.tagset.BaseTagSets, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, collections.abc.MutableMapping, collections.abc.Mapping, collections.abc.Collection, collections.abc.Sized, collections.abc.Iterable, collections.abc.Container, cs.deco.Promotable)`
+## Class `PlayonSeriesEpisodeInfo(cs.mediainfo.SeriesEpisodeInfo)`
+
+A `SeriesEpisodeInfo` with a `from_Recording()` factory method to build 
+one from a PlayOn `Recording` instead or other mapping with `playon.*` keys.
+
+*Method `PlayonSeriesEpisodeInfo.from_Recording(R: Mapping[str, Any])`*:
+Infer series episode information from a `Recording`
+or any mapping with ".playon.*" keys.
+
+## Class `PlayOnSQLTags(cs.sqltags.SQLTags)`
 
 `SQLTags` subclass with PlayOn related methods.
 
 *Method `PlayOnSQLTags.__getitem__(self, index)`*:
 Override `SQLTags.__getitem__` to promote `int` indices
 to a `str` with value `f'recording.{index}'`.
 
@@ -269,18 +311,22 @@
 Convert a string to a list of recording ids.
 
 *Method `PlayOnSQLTags.recordings(self)`*:
 Yield recording `TagSet`s, those named `"recording.*"`.
 
 Note that this includes both recorded and queued items.
 
-## Class `Recording(cs.sqltags.SQLTagSet, cs.obj.SingletonMixin, cs.tagset.TagSet, builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin)`
+## Class `Recording(cs.sqltags.SQLTagSet)`
 
 An `SQLTagSet` with knowledge about PlayOn recordings.
 
+*Method `Recording.filename(self, filename_format=None) -> str`*:
+Return the computed filename per `filename_format`,
+default from `DEFAULT_FILENAME_FORMAT`: `'{series_prefix}{series_episode_name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}'`.
+
 *Method `Recording.is_available(self)`*:
 Is a recording available for download?
 
 *Method `Recording.is_downloaded(self)`*:
 Test whether this recording has been downloaded
 based on the presence of a `download_path` `Tag`
 or a true `downloaded` `Tag`.
@@ -321,14 +367,17 @@
 *Method `Recording.status(self)`*:
 Return a short status string.
 
 # Release Log
 
 
 
+*Release 20240522*:
+New superior tv-series/season/episode inference.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201.1*:
 Release with "playon" script.
 
 *Release 20240201*:
@@ -360,7 +409,8 @@
 * PlayOnCommand: new "poll" subcommand reporting the API notifications response.
 
 *Release 20220311*:
 Bugfix criteria for refreshing the PlayOn state.
 
 *Release 20211212*:
 Initial release.
+
```

### Comparing `cs.app.playon-20240316/lib/python/cs/app/playon.py` & `cs.app.playon-20240522/lib/python/cs/app/playon.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,52 +4,63 @@
 #
 
 ''' PlayOn facilities, primarily access to the download API.
     Includes a nice command line tool.
 '''
 
 from contextlib import contextmanager
-from dataclasses import dataclass, field
+from dataclasses import asdict, dataclass, field
 from datetime import datetime, timezone
+from functools import cached_property
 from getopt import getopt, GetoptError
 from netrc import netrc
 import os
 from os import environ
 from os.path import (
-    basename, exists as pathexists, expanduser, realpath, splitext
+    basename, exists as existspath, expanduser, realpath, samefile, splitext
 )
 from pprint import pformat, pprint
 import re
 import sys
 from threading import Semaphore
 import time
-from typing import Optional, Set
+from typing import Any, Mapping, Optional
 from urllib.parse import unquote as unpercent
 
 from icontract import require
 import requests
 from typeguard import typechecked
 
 from cs.cmdutils import BaseCommand
 from cs.context import stackattrs
-from cs.deco import fmtdoc
+from cs.deco import fmtdoc, promote, Promotable
 from cs.fileutils import atomic_filename
-from cs.lex import has_format_attributes, format_attribute, get_prefix_n
+from cs.fstags import FSTags, uses_fstags
+from cs.lex import (
+    cutprefix,
+    cutsuffix,
+    format_attribute,
+    get_prefix_n,
+    get_suffix_part,
+    has_format_attributes,
+)
 from cs.logutils import warning
+from cs.mediainfo import SeriesEpisodeInfo
 from cs.pfx import Pfx, pfx_method, pfx_call
 from cs.progress import progressbar
 from cs.resources import RunState, uses_runstate
 from cs.result import bg as bg_result, report as report_results, CancellationError
 from cs.service_api import HTTPServiceAPI, RequestsNoAuth
 from cs.sqltags import SQLTags, SQLTagSet
+from cs.tagset import TagSet
 from cs.threads import monitor, bg as bg_thread
 from cs.units import BINARY_BYTES_SCALE
-from cs.upd import print  # pylint: disable=redefined-builtin
+from cs.upd import print, run_task  # pylint: disable=redefined-builtin
 
-__version__ = '20240316'
+__version__ = '20240522'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Programming Language :: Python",
@@ -62,22 +73,25 @@
         },
     },
     'install_requires': [
         'cs.cmdutils',
         'cs.context',
         'cs.deco',
         'cs.fileutils>=atomic_filename',
+        'cs.fstags',
         'cs.lex',
         'cs.logutils',
+        'cs.mediainfo',
         'cs.pfx>=pfx_call',
         'cs.progress',
         'cs.resources',
         'cs.result',
         'cs.service_api',
         'cs.sqltags',
+        'cs.tagset',
         'cs.threads',
         'cs.units',
         'cs.upd',
         'icontract',
         'requests',
         'typeguard',
     ],
@@ -103,15 +117,15 @@
 class PlayOnCommand(BaseCommand):
   ''' Playon command line implementation.
   '''
 
   # default "ls" output format
   LS_FORMAT = (
       '{playon.ID} {playon.HumanSize} {resolution}'
-      ' {playon.Series} {playon.Name} {playon.ProviderID} {status:upper}'
+      ' {nice_name} {playon.ProviderID} {status:upper}'
   )
 
   # default "queue" output format
   QUEUE_FORMAT = '{playon.ID} {playon.Series} {playon.Name} {playon.ProviderID}'
 
   USAGE_KEYWORDS = {
       'DEFAULT_DL_PARALLELISM': DEFAULT_DL_PARALLELISM,
@@ -151,15 +165,15 @@
         get('PLAYON_USER', environ.get('EMAIL'))
     )
     password: Optional[str] = field(
         default_factory=lambda: environ.get('PLAYON_PASSWORD')
     )
     filename_format: str = field(
         default_factory=lambda: environ.
-        get('PLAYON_FILENAME_FORMAT', DEFAULT_FILENAME_FORMAT)
+        get('FILENAME_FORMAT_ENVVAR', DEFAULT_FILENAME_FORMAT)
     )
 
   @contextmanager
   def run_context(self):
     ''' Prepare the `PlayOnAPI` around each command invocation.
     '''
     with super().run_context():
@@ -214,24 +228,69 @@
       raise GetoptError("extra arguments: %r" % (argv,))
     api = self.options.api
     lstate = api.login_state
     pprint(lstate)
     result = api.cdsurl_data(suburl)
     pprint(result)
 
+  @uses_fstags
+  def cmd_rename(self, argv, *, fstags: FSTags):
+    ''' Usage: {cmd} [-o filename_format] filenames...
+          Rename the filenames according to their fstags.
+          -n    No action, dry run.
+          -o filename_format
+                Format for the new filename, default {DEFAULT_FILENAME_FORMAT!r}.
+    '''
+    options = self.options
+    options.popopts(argv, n='dry_run', o_='filename_format')
+    api = options.api
+    doit = options.doit
+    filename_format = options.filename_format
+    if not argv:
+      raise GetoptError("missing filenames")
+    xit = 0
+    for fspath in argv:
+      with Pfx(fspath):
+        if not existspath(fspath):
+          warning("does not exist")
+          xit = 1
+          continue
+        _, ext = splitext(basename(fspath))
+        playon_id = fstags[fspath].get('playon.ID')
+        if not playon_id:
+          warning("no playon.ID, skipping")
+          xit = 1
+          continue
+        recording = api[playon_id]
+        new_filename = recording.filename(filename_format)
+        new_pfx, new_ext = splitext(new_filename)
+        new_filename = new_pfx + ext
+        if new_filename in (fspath, basename(fspath)):
+          continue
+        with Pfx("-> %s", new_filename):
+          if existspath(new_filename):
+            warning("already exists")
+            if not samefile(fspath, new_filename):
+              xit = 1
+            continue
+          print("mv", fspath, new_filename)
+          if doit:
+            fstags.mv(fspath, new_filename)
+            fstags[new_filename].update(recording)
+    return xit
+
   # pylint: disable=too-many-locals,too-many-branches,too-many-statements
   def cmd_dl(self, argv):
     ''' Usage: {cmd} [-j jobs] [-n] [recordings...]
           Download the specified recordings, default "pending".
           -j jobs   Run this many downloads in parallel.
                     The default is {DEFAULT_DL_PARALLELISM}.
           -n        No download. List the specified recordings.
     '''
     options = self.options
-    runstate = options.runstate
     sqltags = options.sqltags
     dl_jobs = DEFAULT_DL_PARALLELISM
     no_download = False
     opts, argv = getopt(argv, 'j:n')
     for opt, val in opts:
       with Pfx(opt):
         if opt == '-j':
@@ -242,26 +301,22 @@
           no_download = True
         else:
           raise RuntimeError("unhandled option")
     if not argv:
       argv = ['pending']
     api = options.api
     filename_format = options.filename_format
+    runstate = options.runstate
     sem = Semaphore(dl_jobs)
 
     @typechecked
     def _dl(dl_id: int, sem):
       try:
         with sqltags:
-          filename = api[dl_id].format_as(filename_format)
-          filename = (
-              filename.lower().replace(' - ', '--').replace(' ', '-')
-              .replace('_', ':').replace(os.sep, ':') + '.'
-          )
-          filename = re.sub('---+', '--', filename)
+          filename = api[dl_id].filename(filename_format)
           try:
             api.download(dl_id, filename=filename, runstate=runstate)
           except ValueError as e:
             warning("download fails: %s", e)
             return None
           return filename
       finally:
@@ -313,25 +368,23 @@
 
     return xit
 
   def _refresh_sqltags_data(self, api, sqltags, max_age=None):
     ''' Refresh the queue and recordings if any unexpired records are stale
         or if all records are expired.
     '''
-    options = self.options
-    upd = options.upd
     recordings = set(sqltags.recordings())
     need_refresh = (
         # any current recordings whose state is stale
         any(recording.is_stale(max_age=max_age) for recording in recordings) or
         # no recording is current
         all(recording.is_expired() for recording in recordings)
     )
     if need_refresh:
-      with upd.run_task("refresh queue and recordings"):
+      with run_task("refresh queue and recordings"):
         Ts = [bg_thread(api.queue), bg_thread(api.recordings)]
         for T in Ts:
           T.join()
 
   @staticmethod
   def _list(argv, options, default_argv, default_format):
     ''' Inner workings of "ls" and "queue".
@@ -356,15 +409,14 @@
       argv = list(default_argv)
     xit = 0
     for arg in argv:
       with Pfx(arg):
         recording_ids = sqltags.recording_ids_from_str(arg)
         if not recording_ids:
           warning("no recording ids")
-          xit = 1
           continue
         for dl_id in sorted(recording_ids):
           recording = sqltags[dl_id]
           with Pfx(recording.name):
             recording.ls(ls_format=listing_format, long_mode=long_mode)
     return xit
 
@@ -384,26 +436,23 @@
           xit = 1
           continue
         for dl_id in recording_ids:
           with Pfx("%s", dl_id):
             recording = sqltags[dl_id]
             print(dl_id, '+ downloaded')
             recording.add("downloaded")
+    return xit
 
   def cmd_feature(self, argv, locale='en_US'):
     ''' Usage: {cmd} [feature_id]
           List features.
     '''
     long_mode = False
-    opts, argv = getopt(argv, 'l', '')
-    for opt, val in opts:
-      if opt == '-l':
-        long_mode = True
-      else:
-        raise RuntimeError("unhandled option: %r" % (opt,))
+    opts = self.popopts(argv, l='long_mode')
+    long_mode = opts['long_mode']
     if argv:
       feature_id = argv.pop(0)
     else:
       feature_id = None
     if argv:
       raise GetoptError("extra arguments: %r" % (argv,))
     api = self.options.api
@@ -481,15 +530,16 @@
       raise GetoptError("extra arguments: %r" % (argv,))
     api = self.options.api
     for service in sorted(api.services(), key=lambda svc: svc['playon.ID']):
       playon = service.subtags('playon')
       if service_id is not None and playon.ID != service_id:
         print("skip", playon.ID)
         continue
-      print(playon.ID, playon.Name, playon.LoginMetadata["URL"])
+      login_meta = playon.LoginMetadata
+      print(playon.ID, playon.Name, login_meta['URL'] if login_meta else {})
       if service_id is None:
         continue
       for tag in playon:
         print(" ", tag)
 
 # pylint: disable=too-many-ancestors
 @has_format_attributes
@@ -515,23 +565,32 @@
 
   @format_attribute
   def recording_id(self):
     ''' The recording id or `None`.
     '''
     return self.get('playon.ID')
 
+  @cached_property
+  def sei(self):
+    ''' A `PlayonSeriesEpisodeInfo` inferred from this `Recording`.
+    '''
+    return PlayonSeriesEpisodeInfo.from_Recording(self)
+
   @format_attribute
   def nice_name(self):
     ''' A nice name for the recording: the PlayOn series and name,
         omitting the series if `None`.
     '''
-    playon_tags = self.subtags('playon')
-    citation = playon_tags.Name
-    if playon_tags.Series and playon_tags.Series != 'none':
-      citation = playon_tags.Series + " - " + citation
+    sei = self.sei
+    if sei.series:
+      citation = f'{sei.series} - s{sei.season:02d}e{sei.episode:02d} - {sei.episode_title}'
+      if sei.episode_part:
+        citation += f' - pt{sei.episode_part:02d}'
+    else:
+      citation = sei.episode_title
     return citation
 
   @format_attribute
   def status(self):
     ''' Return a short status string.
     '''
     for status_label in 'queued', 'expired', 'downloaded', 'pending':
@@ -540,49 +599,36 @@
     raise RuntimeError("cannot infer a status string: %s" % (self,))
 
   @format_attribute
   def series_prefix(self):
     ''' Return a series prefix for recording containing the series name
         and season and episode, or `''`.
     '''
+    sei = self.sei
     sep = '--'
     parts = []
-    if self.playon.Series:
-      parts.append(self.playon.Series)
+    if sei.series:
+      parts.append(sei.series)
       se_parts = []
-      if self.playon.get('Season'):
-        se_parts.append(f's{self.playon.Season:02d}')
-      if self.playon.get('Episode'):
-        se_parts.append(f'e{self.playon.Episode:02d}')
+      if sei.season:
+        se_parts.append(f's{sei.season:02d}')
+      if sei.episode is not None:
+        se_parts.append(f'e{sei.episode:02d}')
       if se_parts:
         parts.append(''.join(se_parts))
     if not parts:
       return ''
     return sep.join(parts) + sep
 
   @format_attribute
   def series_episode_name(self):
-    name = self.playon.Name
-    name = name.strip()
-    if self.playon.get('Season'):
-      spfx, n, offset = get_prefix_n(name, 's', n=self.playon.Season)
-      if spfx is not None:
-        assert name.startswith(f's{self.playon.Season:02d}')
-        name = name[offset:]
-    if self.playon.get('Episode'):
-      epfx, n, offset = get_prefix_n(name, 'e', n=self.playon.Episode)
-      if epfx is not None:
-        assert name.startswith(f'e{self.playon.Episode:02d}')
-        name = name[offset:]
-      name = name.lstrip()
-      epfx, n, offset = get_prefix_n(
-          name.lower(), 'episode ', n=self.playon.Episode
-      )
-      if epfx is not None:
-        name = name[offset:]
+    sei = self.sei
+    name = sei.episode_title
+    if sei.episode_part:
+      name += f'--pt{sei.episode_part:02d}'
     return name.strip()
 
   @format_attribute
   def is_available(self):
     ''' Is a recording available for download?
     '''
     return not self.is_expired() and not self.is_queued()
@@ -624,26 +670,98 @@
         service.
     '''
     if self.is_expired():
       # expired recording will never become unstale
       return False
     return super().is_stale(max_age=max_age)
 
+  @fmtdoc
+  def filename(self, filename_format=None) -> str:
+    ''' Return the computed filename per `filename_format`,
+        default from `DEFAULT_FILENAME_FORMAT`: `{DEFAULT_FILENAME_FORMAT!r}`.
+    '''
+    if filename_format is None:
+      filename_format = DEFAULT_FILENAME_FORMAT
+    filename = self.format_as(filename_format)
+    filename = (
+        filename.lower().replace(' - ', '--').replace(' ', '-')
+        .replace('_', ':').replace(os.sep, ':') + '.'
+    )
+    filename = re.sub('---+', '--', filename)
+    return filename
+
   def ls(self, ls_format=None, long_mode=False, print_func=None):
     ''' List a recording.
     '''
     if ls_format is None:
       ls_format = PlayOnCommand.LS_FORMAT
     if print_func is None:
       print_func = print
     print_func(self.format_as(ls_format))
     if long_mode:
       for tag in sorted(self):
         print_func(" ", tag)
 
+@dataclass
+class PlayonSeriesEpisodeInfo(SeriesEpisodeInfo, Promotable):
+  ''' A `SeriesEpisodeInfo` with a `from_Recording()` factory method to build 
+      one from a PlayOn `Recording` instead or other mapping with `playon.*` keys.
+  '''
+
+  @classmethod
+  def from_Recording(cls, R: Mapping[str, Any]):
+    ''' Infer series episode information from a `Recording`
+        or any mapping with ".playon.*" keys.
+    '''
+    # get a basic SEI from the title
+    episode_title = R.get('playon.Name')
+    playon_series = R.get('playon.Series')
+    playon_season = R.get('playon.Season')
+    playon_episode = R.get('playon.Episode')
+    self = cls.from_str(episode_title, series=playon_series)
+    # now override various fields from the playon tags
+    ###############################################################
+    # match a Playon browse path like "... | The Flash | Season 9"
+    browse_path = R['playon.BrowsePath']
+    browse_re_s = r'\|\s+(?P<series_s>[^|\s][^|]*[^|\s])\s+\|\s+season\s+(?P<season_s>\d+)$'
+    m = re.search(
+        browse_re_s,
+        browse_path,
+        re.I,
+    )
+    browse_series = m and m.group('series_s')
+    browse_season = m and int(m.group('season_s'))
+    # ignore the series "None", still unsure if this is some furphy
+    # from a genuine None value
+    if playon_series and playon_series.lower() == 'none':
+      playon_series = None
+    # sometimes the series is prepended to the episode title
+    if playon_series:
+      episode_title = cutprefix(episode_title, f'{playon_series} - ')
+    # strip the trailing part info eg ": Part One"
+    part_suffix, episode_part = get_suffix_part(episode_title)
+    if part_suffix:
+      episode_title = cutsuffix(episode_title, part_suffix)
+    # strip leading "sSSeEE - " prefix
+    spfx, episode_title_season, offset = get_prefix_n(
+        episode_title.lower(), 's', n=playon_season
+    )
+    epfx, episode_title_episode, offset = get_prefix_n(
+        episode_title.lower(), 'e', n=playon_episode, offset=offset
+    )
+    if offset > 0:
+      # strip the sSSeEE and any following spaces or dashes
+      episode_title = episode_title[offset:].lstrip(' -')
+    # fall back from provided stuff to inferred stuff
+    self.series = playon_series or self.series or browse_series
+    self.season = playon_season or self.season or episode_title_season or browse_season
+    self.episode = playon_episode or self.episode or episode_title_episode
+    self.episode_part = episode_part
+    return self
+
 class LoginState(SQLTagSet):
 
   @property
   def expiry(self):
     ''' Expiry unixtime of the login state information.
         `-1` if the `'exp'` field is not present.
     '''
@@ -1044,15 +1162,15 @@
     dl_url = dl_data['url']
     dl_basename = unpercent(basename(dl_url))
     if filename is None:
       filename = dl_basename
     elif filename.endswith('.'):
       _, dl_ext = splitext(dl_basename)
       filename = filename[:-1] + dl_ext
-    if pathexists(filename):
+    if existspath(filename):
       warning(
           "SKIPPING download of %r: already exists, just tagging", filename
       )
       dl_rsp = None
     else:
       dl_cookies = dl_data['data']
       jar = self.cookies
@@ -1072,16 +1190,15 @@
             dl_rsp.iter_content(chunk_size=131072),
             label=filename,
             total=dl_length,
             units_scale=BINARY_BYTES_SCALE,
             itemlenfunc=len,
             report_print=True,
         ):
-          if runstate.cancelled:
-            raise CancellationError
+          runstate.raiseif()
           offset = 0
           length = len(chunk)
           while offset < length:
             with Pfx("write %d bytes", length - offset):
               written = f.write(chunk[offset:])
               if written < 1:
                 warning("fewer than 1 bytes written: %s", written)
@@ -1090,12 +1207,15 @@
                 assert offset <= length
           assert offset == length
     fullpath = realpath(filename)
     recording = self[download_id]
     if dl_rsp is not None:
       recording.set('download_path', fullpath)
     # apply the SQLTagSet to the FSTags TagSet
-    self.fstags[fullpath].update(recording.subtags('playon'), prefix='playon')
+    tagged = self.fstags[fullpath]
+    tagged.update(recording.subtags('playon'), prefix='playon')
+    # and also the Series/Season/Episode info
+    tagged.update(recording.sei.as_dict())
     return recording
 
 if __name__ == '__main__':
   sys.exit(main(sys.argv))
```

