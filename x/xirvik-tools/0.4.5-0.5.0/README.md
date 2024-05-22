# Comparing `tmp/xirvik_tools-0.4.5.tar.gz` & `tmp/xirvik_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xirvik_tools-0.4.5.tar", max compression
+gzip compressed data, was "xirvik_tools-0.5.0.tar", max compression
```

## Comparing `xirvik_tools-0.4.5.tar` & `xirvik_tools-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1072 2015-04-05 10:25:34.116301 xirvik_tools-0.4.5/LICENSE.txt
--rw-r--r--   0        0        0      628 2023-04-11 15:59:06.810994 xirvik_tools-0.4.5/LaunchAgents/README.md
--rw-r--r--   0        0        0      733 2023-04-14 20:37:57.649077 xirvik_tools-0.4.5/LaunchAgents/sh.tat.XirvikStartTorrents.plist
--rw-r--r--   0        0        0      664 2023-09-16 22:36:44.976043 xirvik_tools-0.4.5/README.md
--rw-r--r--   0        0        0    11887 2023-09-15 19:04:19.610324 xirvik_tools-0.4.5/man/xirvik.1
--rw-r--r--   0        0        0     4263 2023-09-16 22:36:44.976043 xirvik_tools-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      815 2020-02-20 00:53:15.113538 xirvik_tools-0.4.5/systemd/README.md
--rw-r--r--   0        0        0      140 2021-09-12 02:01:33.922925 xirvik_tools-0.4.5/systemd/xirvik-start-torrents.service
--rw-r--r--   0        0        0      128 2020-02-20 00:53:15.113538 xirvik_tools-0.4.5/systemd/xirvik-start-torrents.timer
--rw-r--r--   0        0        0       95 2020-10-29 09:51:37.765849 xirvik_tools-0.4.5/xirvik/__init__.py
--rw-r--r--   0        0        0    14975 2023-07-08 10:51:42.433718 xirvik_tools-0.4.5/xirvik/client.py
--rw-r--r--   0        0        0       71 2021-09-14 05:10:34.682258 xirvik_tools-0.4.5/xirvik/commands/__init__.py
--rw-r--r--   0        0        0     4039 2023-09-15 18:13:47.244534 xirvik_tools-0.4.5/xirvik/commands/delete_old.py
--rw-r--r--   0        0        0     3756 2023-09-15 19:15:29.886294 xirvik_tools-0.4.5/xirvik/commands/move_by_label.py
--rw-r--r--   0        0        0     2820 2023-09-15 18:13:47.244534 xirvik_tools-0.4.5/xirvik/commands/move_erroneous.py
--rw-r--r--   0        0        0     1662 2023-09-15 18:13:47.244534 xirvik_tools-0.4.5/xirvik/commands/root.py
--rw-r--r--   0        0        0    18451 2023-09-15 18:13:47.244534 xirvik_tools-0.4.5/xirvik/commands/simple.py
--rw-r--r--   0        0        0     7076 2023-09-15 18:14:02.778523 xirvik_tools-0.4.5/xirvik/commands/util.py
--rw-r--r--   0        0        0     2412 2023-04-14 20:37:57.649077 xirvik_tools-0.4.5/xirvik/typing.py
--rw-r--r--   0        0        0     1032 2023-09-15 18:14:02.780523 xirvik_tools-0.4.5/xirvik/utils.py
--rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 xirvik_tools-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2015-04-05 10:25:34.116301 xirvik_tools-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      637 2023-11-29 03:19:51.032951 xirvik_tools-0.5.0/LaunchAgents/README.md
+-rw-r--r--   0        0        0      734 2023-11-29 03:19:08.815010 xirvik_tools-0.5.0/LaunchAgents/sh.tat.XirvikStartTorrents.plist
+-rw-r--r--   0        0        0     1143 2024-05-22 02:55:16.601014 xirvik_tools-0.5.0/README.md
+-rw-r--r--   0        0        0    11887 2024-05-22 02:54:54.442501 xirvik_tools-0.5.0/man/xirvik.1
+-rw-r--r--   0        0        0     5976 2024-05-22 02:55:16.601014 xirvik_tools-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      831 2023-11-29 03:20:18.854913 xirvik_tools-0.5.0/systemd/README.md
+-rw-r--r--   0        0        0      140 2021-09-12 02:01:33.922925 xirvik_tools-0.5.0/systemd/xirvik-start-torrents.service
+-rw-r--r--   0        0        0      128 2020-02-20 00:53:15.113538 xirvik_tools-0.5.0/systemd/xirvik-start-torrents.timer
+-rw-r--r--   0        0        0       95 2020-10-29 09:51:37.765849 xirvik_tools-0.5.0/xirvik/__init__.py
+-rw-r--r--   0        0        0    15181 2024-05-22 02:55:03.786718 xirvik_tools-0.5.0/xirvik/client.py
+-rw-r--r--   0        0        0       71 2021-09-14 05:10:34.682258 xirvik_tools-0.5.0/xirvik/commands/__init__.py
+-rw-r--r--   0        0        0     3897 2024-02-17 06:33:44.070469 xirvik_tools-0.5.0/xirvik/commands/delete_old.py
+-rw-r--r--   0        0        0     3916 2024-05-22 02:55:03.786718 xirvik_tools-0.5.0/xirvik/commands/move_by_label.py
+-rw-r--r--   0        0        0     2832 2024-05-22 02:55:03.786718 xirvik_tools-0.5.0/xirvik/commands/move_erroneous.py
+-rw-r--r--   0        0        0     1662 2023-09-15 18:13:47.244534 xirvik_tools-0.5.0/xirvik/commands/root.py
+-rw-r--r--   0        0        0    18556 2023-11-29 03:42:58.661923 xirvik_tools-0.5.0/xirvik/commands/simple.py
+-rw-r--r--   0        0        0     7171 2023-11-29 03:48:34.485442 xirvik_tools-0.5.0/xirvik/commands/util.py
+-rw-r--r--   0        0        0     2500 2023-11-29 03:24:16.655576 xirvik_tools-0.5.0/xirvik/typing.py
+-rw-r--r--   0        0        0     1041 2023-11-29 02:51:05.884463 xirvik_tools-0.5.0/xirvik/utils.py
+-rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 xirvik_tools-0.5.0/PKG-INFO
```

### Comparing `xirvik_tools-0.4.5/LICENSE.txt` & `xirvik_tools-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.5/LaunchAgents/README.md` & `xirvik_tools-0.5.0/LaunchAgents/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # To use
 
 1. For easiness, install lunchy: `gem install lunchy`
-2. Edit a copy of this file for use filling in the path to Python, the script, server host, and path to search
+2. Edit a copy of this file for use filling in the path to Python, the script, server host, and path
+   to search
 3. Add the port argument (`-P`) if necessary
-4. Add any other arguments you would like _except_ `-d` (debug) or `-v` (verbose), unless you add keys `StandardOutPath` and `StandardErrorPath` with paths to valid files to write to.
+4. Add any other arguments you would like _except_ `-d` (debug) or `-v` (verbose), unless you add
+   keys `StandardOutPath` and `StandardErrorPath` with paths to valid files to write to.
 5. Put your copy of the plist file into `~/Library/LaunchAgents`
-6. If you kept the name of the agent the same, you can enable and start it with: `lunchy start -w sh.tat.XirvikStartTorrents`, otherwise fix the service name.
+6. If you kept the name of the agent the same, you can enable and start it with:
+   `lunchy start -w sh.tat.XirvikStartTorrents`, otherwise fix the service name.
```

### Comparing `xirvik_tools-0.4.5/LaunchAgents/sh.tat.XirvikStartTorrents.plist` & `xirvik_tools-0.5.0/LaunchAgents/sh.tat.XirvikStartTorrents.plist`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 203f 3e0a 3c21 444f 4354 5950  F-8" ?>.<!DOCTYP
 00000030: 4520 706c 6973 7420 5055 424c 4943 2022  E plist PUBLIC "
 00000040: 2d2f 2f41 7070 6c65 2f2f 4454 4420 504c  -//Apple//DTD PL
-00000050: 4953 5420 312e 302f 2f45 4e22 0a09 2268  IST 1.0//EN".."h
-00000060: 7474 703a 2f2f 7777 772e 6170 706c 652e  ttp://www.apple.
-00000070: 636f 6d2f 4454 4473 2f50 726f 7065 7274  com/DTDs/Propert
-00000080: 794c 6973 742d 312e 302e 6474 6422 3e0a  yList-1.0.dtd">.
-00000090: 3c70 6c69 7374 2076 6572 7369 6f6e 3d22  <plist version="
-000000a0: 312e 3022 3e0a 2020 3c64 6963 743e 0a20  1.0">.  <dict>. 
-000000b0: 2020 203c 6b65 793e 4c61 6265 6c3c 2f6b     <key>Label</k
-000000c0: 6579 3e0a 2020 2020 3c73 7472 696e 673e  ey>.    <string>
-000000d0: 7368 2e74 6174 2e58 6972 7669 6b53 7461  sh.tat.XirvikSta
-000000e0: 7274 546f 7272 656e 7473 3c2f 7374 7269  rtTorrents</stri
-000000f0: 6e67 3e0a 2020 2020 3c6b 6579 3e50 726f  ng>.    <key>Pro
-00000100: 6772 616d 4172 6775 6d65 6e74 733c 2f6b  gramArguments</k
-00000110: 6579 3e0a 2020 2020 3c61 7272 6179 3e0a  ey>.    <array>.
-00000120: 2020 2020 2020 3c73 7472 696e 673e 4655        <string>FU
-00000130: 4c4c 2050 4154 4820 544f 2050 7974 686f  LL PATH TO Pytho
-00000140: 6e20 332c 2069 2e65 202f 5573 6572 732f  n 3, i.e /Users/
-00000150: 7461 7473 682f 2e76 6972 7475 616c 656e  tatsh/.virtualen
-00000160: 7673 2f78 6972 7669 6b2d 746f 6f6c 732f  vs/xirvik-tools/
-00000170: 6269 6e2f 7079 7468 6f6e 333c 2f73 7472  bin/python3</str
-00000180: 696e 673e 0a20 2020 2020 203c 7374 7269  ing>.      <stri
-00000190: 6e67 3e46 554c 4c20 5041 5448 2054 4f20  ng>FULL PATH TO 
-000001a0: 7869 7276 696b 2c20 692e 6520 2f55 7365  xirvik, i.e /Use
-000001b0: 7273 2f74 6174 7368 2f2e 7669 7274 7561  rs/tatsh/.virtua
-000001c0: 6c65 6e76 732f 7869 7276 696b 2d74 6f6f  lenvs/xirvik-too
-000001d0: 6c73 2f62 696e 2f78 6972 7669 6b3c 2f73  ls/bin/xirvik</s
-000001e0: 7472 696e 673e 0a20 2020 2020 203c 7374  tring>.      <st
-000001f0: 7269 6e67 3e72 746f 7272 656e 743c 2f73  ring>rtorrent</s
-00000200: 7472 696e 673e 0a20 2020 2020 203c 7374  tring>.      <st
-00000210: 7269 6e67 3e61 6464 3c2f 7374 7269 6e67  ring>add</string
-00000220: 3e0a 2020 2020 2020 3c73 7472 696e 673e  >.      <string>
-00000230: 484f 5354 4e41 4d45 3c2f 7374 7269 6e67  HOSTNAME</string
-00000240: 3e0a 2020 2020 2020 3c73 7472 696e 673e  >.      <string>
-00000250: 2f46 554c 4c2f 5041 5448 3c2f 7374 7269  /FULL/PATH</stri
-00000260: 6e67 3e0a 2020 2020 3c2f 6172 7261 793e  ng>.    </array>
-00000270: 0a20 2020 203c 6b65 793e 5374 6172 7449  .    <key>StartI
-00000280: 6e74 6572 7661 6c3c 2f6b 6579 3e0a 2020  nterval</key>.  
-00000290: 2020 3c21 2d2d 2052 756e 2065 7665 7279    <!-- Run every
-000002a0: 2032 206d 696e 7574 6573 202d 2d3e 0a20   2 minutes -->. 
-000002b0: 2020 203c 696e 7465 6765 723e 3132 303c     <integer>120<
-000002c0: 2f69 6e74 6567 6572 3e0a 2020 3c2f 6469  /integer>.  </di
-000002d0: 6374 3e0a 3c2f 706c 6973 743e 0a         ct>.</plist>.
+00000050: 4953 5420 312e 302f 2f45 4e22 0a20 2022  IST 1.0//EN".  "
+00000060: 6874 7470 3a2f 2f77 7777 2e61 7070 6c65  http://www.apple
+00000070: 2e63 6f6d 2f44 5444 732f 5072 6f70 6572  .com/DTDs/Proper
+00000080: 7479 4c69 7374 2d31 2e30 2e64 7464 223e  tyList-1.0.dtd">
+00000090: 0a3c 706c 6973 7420 7665 7273 696f 6e3d  .<plist version=
+000000a0: 2231 2e30 223e 0a20 203c 6469 6374 3e0a  "1.0">.  <dict>.
+000000b0: 2020 2020 3c6b 6579 3e4c 6162 656c 3c2f      <key>Label</
+000000c0: 6b65 793e 0a20 2020 203c 7374 7269 6e67  key>.    <string
+000000d0: 3e73 682e 7461 742e 5869 7276 696b 5374  >sh.tat.XirvikSt
+000000e0: 6172 7454 6f72 7265 6e74 733c 2f73 7472  artTorrents</str
+000000f0: 696e 673e 0a20 2020 203c 6b65 793e 5072  ing>.    <key>Pr
+00000100: 6f67 7261 6d41 7267 756d 656e 7473 3c2f  ogramArguments</
+00000110: 6b65 793e 0a20 2020 203c 6172 7261 793e  key>.    <array>
+00000120: 0a20 2020 2020 203c 7374 7269 6e67 3e46  .      <string>F
+00000130: 554c 4c20 5041 5448 2054 4f20 5079 7468  ULL PATH TO Pyth
+00000140: 6f6e 2033 2c20 692e 6520 2f55 7365 7273  on 3, i.e /Users
+00000150: 2f74 6174 7368 2f2e 7669 7274 7561 6c65  /tatsh/.virtuale
+00000160: 6e76 732f 7869 7276 696b 2d74 6f6f 6c73  nvs/xirvik-tools
+00000170: 2f62 696e 2f70 7974 686f 6e33 3c2f 7374  /bin/python3</st
+00000180: 7269 6e67 3e0a 2020 2020 2020 3c73 7472  ring>.      <str
+00000190: 696e 673e 4655 4c4c 2050 4154 4820 544f  ing>FULL PATH TO
+000001a0: 2078 6972 7669 6b2c 2069 2e65 202f 5573   xirvik, i.e /Us
+000001b0: 6572 732f 7461 7473 682f 2e76 6972 7475  ers/tatsh/.virtu
+000001c0: 616c 656e 7673 2f78 6972 7669 6b2d 746f  alenvs/xirvik-to
+000001d0: 6f6c 732f 6269 6e2f 7869 7276 696b 3c2f  ols/bin/xirvik</
+000001e0: 7374 7269 6e67 3e0a 2020 2020 2020 3c73  string>.      <s
+000001f0: 7472 696e 673e 7274 6f72 7265 6e74 3c2f  tring>rtorrent</
+00000200: 7374 7269 6e67 3e0a 2020 2020 2020 3c73  string>.      <s
+00000210: 7472 696e 673e 6164 643c 2f73 7472 696e  tring>add</strin
+00000220: 673e 0a20 2020 2020 203c 7374 7269 6e67  g>.      <string
+00000230: 3e48 4f53 544e 414d 453c 2f73 7472 696e  >HOSTNAME</strin
+00000240: 673e 0a20 2020 2020 203c 7374 7269 6e67  g>.      <string
+00000250: 3e2f 4655 4c4c 2f50 4154 483c 2f73 7472  >/FULL/PATH</str
+00000260: 696e 673e 0a20 2020 203c 2f61 7272 6179  ing>.    </array
+00000270: 3e0a 2020 2020 3c6b 6579 3e53 7461 7274  >.    <key>Start
+00000280: 496e 7465 7276 616c 3c2f 6b65 793e 0a20  Interval</key>. 
+00000290: 2020 203c 212d 2d20 5275 6e20 6576 6572     <!-- Run ever
+000002a0: 7920 3220 6d69 6e75 7465 7320 2d2d 3e0a  y 2 minutes -->.
+000002b0: 2020 2020 3c69 6e74 6567 6572 3e31 3230      <integer>120
+000002c0: 3c2f 696e 7465 6765 723e 0a20 203c 2f64  </integer>.  </d
+000002d0: 6963 743e 0a3c 2f70 6c69 7374 3e0a       ict>.</plist>.
```

### Comparing `xirvik_tools-0.4.5/man/xirvik.1` & `xirvik_tools-0.5.0/man/xirvik.1`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.5/systemd/README.md` & `xirvik_tools-0.5.0/systemd/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
 # To use
 
-1. Edit a copy of this file for use filling in the path to the script (with full path to Python 3.4+ if necessary), server host, and path to search.
+1. Edit a copy of this file for use filling in the path to the script (with full path to Python 3.11+
+   if necessary), server host, and path to search.
 2. Add the port argument (`-P`) if necessary.
 3. Add any other arguments you would like _except_ `-d` (debug) or `-v` (verbose).
-4. If you plan to use this as a user and not as a system service, copy both the timer and service file to `~/.config/systemd/user/`. If you plan to use this as a system service, copy both the timer and service file to `/etc/systemd/system/` (must be root).
-5. To enable and start a user: `systemctl --user enable xirvik-start-torrents.timer`, `systemctl --user start xirvik-start-torrents.timer`. If as system, run as root and use: `systemctl enable xirvik-start-torrents.timer`, `systemctl start xirvik-start-torrents.timer`.
+4. If you plan to use this as a user and not as a system service, copy both the timer and service
+   file to `~/.config/systemd/user/`. If you plan to use this as a system service, copy both the
+   timer and service file to `/etc/systemd/system/` (must be root).
+5. To enable and start a user: `systemctl --user enable xirvik-start-torrents.timer`,
+   `systemctl --user start xirvik-start-torrents.timer`. If as system, run as root and use:
+   `systemctl enable xirvik-start-torrents.timer`, `systemctl start xirvik-start-torrents.timer`.
```

### Comparing `xirvik_tools-0.4.5/xirvik/client.py` & `xirvik_tools-0.5.0/xirvik/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Client for ruTorrent."""
-from datetime import datetime
+from datetime import UTC, datetime
 from enum import IntEnum
+from functools import cached_property
 from netrc import netrc
-from os.path import expanduser
-from typing import Any, Final, Iterator, cast
+from pathlib import Path
+from typing import Any, Final, cast
+from collections.abc import Iterator
 from urllib.parse import quote
 import logging
 import xmlrpc.client as xmlrpc
 
-from cached_property import cached_property
 from requests.adapters import HTTPAdapter
 from urllib3.util import Retry
 import requests
 
 from .typing import FileDownloadStrategy, FilePriority, TorrentInfo, TorrentTrackedFile
 from .utils import parse_header
 
@@ -26,14 +27,17 @@
     """Raised when an unexpected error occurs."""
 
 
 class ListTorrentsError(Exception):
     """Raised when ruTorrentClient.list_torrents() has an exception."""
 
 
+FIRST_YEAR_XIRVIK: Final[int] = 2009
+
+
 class ruTorrentClient:
     """
     ruTorrent client class.
 
     `Reference on RPC returned fields.`_
 
     .. _Reference on RPC returned fields.: https://goo.gl/DvmW4c
@@ -63,19 +67,19 @@
         Factor used to calculate back-off time when retrying requests.
     """
     def __init__(self,
                  host: str,
                  name: str | None = None,
                  password: str | None = None,
                  max_retries: int = 10,
-                 netrc_path: str | None = None,
+                 netrc_path: str | Path | None = None,
                  backoff_factor: int = 1):
         if not name and not password:
             if not netrc_path:
-                netrc_path = expanduser('~/.netrc')
+                netrc_path = Path('~/.netrc').expanduser()
             netrc_data = netrc(netrc_path).authenticators(host)
             assert netrc_data is not None
             name, _, password = netrc_data
         assert name is not None
         assert password is not None
         self.name = name
         self.password = password
@@ -138,25 +142,27 @@
         """Get all torrent information."""
         r = self._session.post(self.multirpc_action_uri,
                                data=dict(mode='list', cmd='d.custom=seedingtime'),
                                auth=self.auth)
         r.raise_for_status()
         possible_dict = cast(dict[str, list[Any]], r.json()['t'])
         if not hasattr(possible_dict, 'items'):
+            self._log.debug('Returned: %s', possible_dict)
             raise ListTorrentsError('Unexpected type in response: ' + str(type(possible_dict)))
         for hash_, x in possible_dict.items():
             del x[34]  # Delete unknown field
             for i, (type_cls, val) in enumerate(
                     zip((t[1] for t in list(TorrentInfo.__annotations__.items())[1:]),
-                        (y.strip() for y in x))):
+                        (y.strip() for y in x),
+                        strict=False)):
                 if getattr(type_cls, '__args__', [None])[0] == datetime:
                     try:
-                        x[i] = datetime.fromtimestamp(float(val or '0'))
+                        x[i] = datetime.fromtimestamp(float(val or '0'), UTC)
                         # First year xirvik.com existed
-                        if x[i].year < 2009:
+                        if x[i].year < FIRST_YEAR_XIRVIK:
                             x[i] = None
                     except ValueError:  # pragma no cover
                         x[i] = None
                 elif type_cls == bool or issubclass(type_cls, IntEnum):
                     x[i] = type_cls(int(val))
                 else:
                     x[i] = type_cls(val)
@@ -226,16 +232,16 @@
         # twice in a dictionary.
         hashes = kwargs.pop('hashes', [])
         label = kwargs.pop('label', None)
         allow_recursive_fix = kwargs.pop('allow_recursive_fix', True)
         recursion_limit = kwargs.pop('recursion_limit', 5)
         recursion_attempt = kwargs.pop('recursion_attempt', 0)
         if not hashes or not label:
-            raise TypeError('"hashes" (list) and "label" (str) keyword '
-                            'arguments are required')
+            raise TypeError(  # noqa: TRY003
+                '"hashes" (list) and "label" (str) keyword arguments are required')
         data = b'mode=setlabel'
         for hash_ in hashes:
             data += f'&hash={hash_}'.encode()
         data += f'&v={label}'.encode() * len(hashes)
         data += b'&s=label' * len(hashes)
         self._log.debug('set_labels() with data: %s', data.decode())
         r = self._session.post(self.multirpc_action_uri, data=data, auth=self.auth)
@@ -313,15 +319,15 @@
         for x in r.json():
             # Fix the numeric values which come as strings
             x[1] = int(x[1])  # total number of pieces
             x[2] = int(x[2])  # downloaded pieces
             x[3] = int(x[3])  # size in bytes
             x[4] = FilePriority(int(x[4]))  # priority ID
             x[5] = FileDownloadStrategy(int(x[5]))  # download strategy ID
-            # x[6] = int(x[6])  # Not used
+            # x[6] = int(x[6])  # Not used  # noqa: ERA001
             yield TorrentTrackedFile(*x[:6])
 
     def list_all_files(self) -> Iterator[TorrentTrackedFile]:
         """
         list all files tracked by rTorrent.
 
         If there are thousands of torrents, this may take well over 10 minutes.
```

### Comparing `xirvik_tools-0.4.5/xirvik/commands/delete_old.py` & `xirvik_tools-0.5.0/xirvik/commands/delete_old.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-#!/usr/bin/env python
 """
 Deletes old torrents based on specified criteria.
 """
-from datetime import datetime, timedelta
-from os.path import expanduser
+from datetime import UTC, datetime, timedelta
+from pathlib import Path
 from time import sleep
-from typing import Callable
+from collections.abc import Callable
 import xmlrpc.client as xmlrpc
 
 from loguru import logger
 from requests.exceptions import HTTPError
 import click
 
 from xirvik.typing import TorrentInfo
@@ -19,24 +18,22 @@
 
 TestCallable = Callable[[TorrentInfo], tuple[str, bool]]
 TestsDict = dict[str, tuple[bool, TestCallable]]
 
 
 def _test_date_cb(days: int = 14) -> TestCallable:
     def test_date(info: TorrentInfo) -> tuple[str, bool]:
-        condition1 = info.creation_date
-        condition2 = info.state_changed
-        expect = datetime.now() - timedelta(days=days)
-        logger.debug(f'creation date: {condition1}')
-        logger.debug(f'state changed: {condition2}')
+        condition1 = info.state_changed
+        expect = datetime.now(UTC) - timedelta(days=days)
+        logger.debug(f'state changed: {condition1}')
         logger.debug(f'{condition1} <= {expect} or')
-        logger.debug(f'    {condition2} <= {expect}')
+        logger.debug(f'    {condition1} <= {expect}')
         return (
             f'over {days} days seeded',
-            bool((condition1 and condition1 <= expect) or (condition2 and condition2 <= expect)),
+            bool(condition1 and condition1 <= expect),
         )
 
     return test_date
 
 
 def _test_ratio(info: TorrentInfo) -> tuple[str, bool]:
     logger.debug(f'ratio: {info.ratio:.2f}')
@@ -69,20 +66,20 @@
          config: str | None = None) -> None:
     """Delete torrents based on certain criteria."""
     setup_logging(debug)
     client = ruTorrentClient(host,
                              name=username,
                              password=password,
                              max_retries=max_retries,
-                             netrc_path=netrc or expanduser('~/.netrc'))
+                             netrc_path=netrc or Path('~/.netrc').expanduser())
     try:
         torrents = client.list_torrents()
     except HTTPError as e:
         logger.error('Connection failed on list_torrents() call')
-        raise click.Abort() from e
+        raise click.Abort from e
     tests = dict(
         ratio=(ignore_ratio, _test_ratio),
         date=(ignore_date, _test_date_cb(days)),
     )
     for info in torrents:
         if info.left_bytes != 0 or info.custom1 != label:
             continue
```

### Comparing `xirvik_tools-0.4.5/xirvik/commands/move_by_label.py` & `xirvik_tools-0.5.0/xirvik/commands/move_by_label.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-#!/usr/bin/env python
 """Organise torrents based on labels assigned in ruTorrent."""
-from os.path import expanduser
+from collections.abc import Callable, Sequence
+from pathlib import Path
 from time import sleep
-from typing import Callable, Sequence
 
+import click
 from loguru import logger
 from requests.exceptions import HTTPError
-import click
 
 from xirvik.typing import TorrentInfo
 
 from ..client import ruTorrentClient
 from .util import command_with_config_file, common_options_and_arguments, setup_logging
 
 PREFIX = '/downloads/{}'
@@ -20,28 +19,30 @@
                      lower_label: bool) -> Callable[[TorrentInfo], bool]:
     def maybe_lower(x: str) -> str:
         if lower_label:
             return str.lower(x)
         return x
 
     def bpc(info: TorrentInfo) -> bool:
-        return (not info.base_path.startswith(f'{PREFIX.format(completed_dir)}'
-                                              f'/{maybe_lower(info.custom1 or "")}')
-                # Old style paths
-                and not info.base_path.startswith(f'/torrents/{username}/'))
+        return bool(info.base_path.strip()
+                    and not info.base_path.startswith(f'{PREFIX.format(completed_dir)}'
+                                                      f'/{maybe_lower(info.custom1 or "")}')
+                    # Old style paths
+                    and not info.base_path.startswith(f'/torrents/{username}/'))
 
     return bpc
 
 
 def _key_check(info: TorrentInfo) -> bool:
     return not info.is_hash_checking and info.left_bytes == 0
 
 
 @click.command(cls=command_with_config_file('config', 'move-by-label'))
 @common_options_and_arguments
+@click.option('-b', '--batch-size', default=10, help='Batch size.')
 @click.option('-c',
               '--completed-dir',
               default='_completed',
               help='Top directory where moved torrent data will be placed')
 @click.option('-t',
               '--sleep-time',
               default=10,
@@ -60,41 +61,42 @@
          password: str | None = None,
          completed_dir: str = '_completed',
          sleep_time: int = 10,
          lower_label: bool | None = None,
          max_retries: int = 10,
          debug: bool = False,
          backoff_factor: int = 1,
-         config: str | None = None) -> None:
+         config: str | None = None,
+         batch_size: int = 10) -> None:
     """Move torrents according to labels assigned."""
     setup_logging(debug)
     logger.debug(f'Host: {host}')
     logger.debug(f'Configuration file: {config}')
     logger.debug(f'Use lowercase labels: {lower_label}')
     logger.debug(f'Ignoring labels: {", ".join(ignore_labels)}')
     client = ruTorrentClient(host,
                              name=username,
                              password=password,
                              max_retries=max_retries,
-                             netrc_path=netrc or expanduser('~/.netrc'),
+                             netrc_path=netrc or Path('~/.netrc').expanduser(),
                              backoff_factor=backoff_factor)
     username = client.name
     assert username is not None
     try:
         torrents = client.list_torrents()
     except (ValueError, HTTPError) as e:
         logger.error('Connection failed on list_torrents() call')
-        raise click.Abort() from e
+        raise click.Abort from e
     count = 0
     for info in (y for y in (x for x in torrents if _key_check(x))
                  if _base_path_check(username, completed_dir, lower_label or False)(y)):
         label = info.custom1
         if not label or label in ignore_labels:
             continue
         if lower_label:
             label = label.lower()
         move_to = f'{PREFIX.format(completed_dir)}/{label}'
         logger.info(f'Moving {info.name} from {info.base_path} to {move_to}/')
         client.move_torrent(info.hash, move_to)
         count += 1
-        if count > 0 and (count % 10) == 0:
+        if count > 0 and (count % batch_size) == 0:
             sleep(sleep_time)
```

### Comparing `xirvik_tools-0.4.5/xirvik/commands/move_erroneous.py` & `xirvik_tools-0.5.0/xirvik/commands/move_erroneous.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Move torrents in error state to another location."""
 from time import sleep
-from typing import Any, Final, Iterable, TypeVar
+from typing import Any, Final, TypeVar
+from collections.abc import Iterable
 
 from loguru import logger
 import click
 
 from ..client import ruTorrentClient
 from ..typing import TorrentInfo
 from .util import command_with_config_file, common_options_and_arguments, setup_logging
@@ -55,19 +56,17 @@
                              name=username,
                              password=password,
                              max_retries=max_retries,
                              netrc_path=netrc)
     prefix = PREFIX.format(client.name)
     to_delete: list[tuple[str, str]] = []
     items = [info for info in client.list_torrents() if _should_process(info)]
-    count = 0
-    for info in items:
+    for count, info in enumerate(items):
         logger.info(f'Stopping {info.name}')
         client.stop(info.hash)
-        count += 1
         if count > 0 and (count % 10) == 0:
             sleep(sleep_time)
     count = 0
     for info in items:
         move_to = _make_move_to(prefix, info.custom1.lower())
         to_delete.append((info.hash, info.name))
         logger.info(f'Moving {info.name} to {move_to}/')
```

### Comparing `xirvik_tools-0.4.5/xirvik/commands/root.py` & `xirvik_tools-0.5.0/xirvik/commands/root.py`

 * *Files identical despite different names*

### Comparing `xirvik_tools-0.4.5/xirvik/commands/simple.py` & `xirvik_tools-0.5.0/xirvik/commands/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Mirror (copy data from remote to local) helper."""
 from base64 import b64encode
-from datetime import datetime
+from datetime import MINYEAR, UTC, datetime
 from logging.handlers import SysLogHandler
-from os import listdir, makedirs, remove as rm
-from os.path import basename, expanduser, isdir, join as path_join, realpath, splitext
+from os import listdir
+from os.path import realpath
+from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import Any, Iterator, NoReturn, Sequence, cast
+from typing import Any, NoReturn, cast
+from collections.abc import Iterator, Sequence
 import json
 import logging
 import signal
 import subprocess as sp
 import sys
 
 from bs4 import BeautifulSoup as Soup
@@ -23,15 +25,15 @@
 from ..client import ruTorrentClient
 from ..typing import TorrentInfo, TorrentTrackedFile
 from .util import command_with_config_file, complete_hosts, complete_ports, setup_logging
 
 
 def _ctrl_c_handler(_: int, __: Any) -> NoReturn:  # pragma: no cover
     """Used as a TERM signal handler. Arguments are ignored."""
-    raise SystemExit('Signal raised')
+    raise SystemExit('Signal raised')  # noqa: TRY003
 
 
 @click.command(cls=command_with_config_file('config', 'add-torrents'))
 @click.option('-p', '--port', type=int, default=443, shell_complete=complete_ports)
 @click.option('-d', '--debug', is_flag=True)
 @click.option('--start-stopped', is_flag=True)
 @click.option('-s', '--syslog', is_flag=True)
@@ -39,27 +41,26 @@
 @click.option('-C', '--config', help='Configuration file')
 @click.option('--no-verify',
               default=False,
               is_flag=True,
               help='Disable TLS verification (not recommended)')
 @click.argument('directories', type=click.Path(exists=True, file_okay=False), nargs=-1)
 def start_torrents(host: str,
-                   directories: str,
+                   directories: list[str],
                    port: int = 443,
                    debug: bool = False,
                    start_stopped: bool = False,
                    syslog: bool = False,
                    config: str | None = None,
                    no_verify: bool = False) -> None:
     """Uploads torrent files to the server."""
     signal.signal(signal.SIGINT, _ctrl_c_handler)
     setup_logging(debug)
-    cache_dir = realpath(expanduser('~/.cache/xirvik'))
-    if not isdir(cache_dir):
-        makedirs(cache_dir)
+    cache_dir = Path(realpath(Path('~/.cache/xirvik').expanduser()))
+    cache_dir.mkdir(parents=True, exist_ok=True)
     if syslog:  # pragma: no cover
         try:
             syslog_handle = SysLogHandler(address='/dev/log')
         except OSError:
             syslog_handle = SysLogHandler(address='/var/run/syslog',
                                           facility=SysLogHandler.LOG_USER)
             syslog_handle.ident = 'xirvik-start-torrents'
@@ -71,46 +72,45 @@
     form_data = {}
     # rtorrent2/3 params
     # dir_edit - ?
     # tadd_label - Label for the torrents, more param: label=
     # torrent_file - Torrent file blob data
     if start_stopped:
         form_data['torrents_start_stopped'] = 'on'
-    for d in directories:
+    for d in (Path(x) for x in directories):
         for item in listdir(d):
             if not item.lower().endswith('.torrent'):
                 continue
-            item_inner = path_join(d, item)
+            item_inner = d / item
             # Workaround for surrogates not allowed error, rename the file
-            prefix = f'{splitext(basename(item_inner))[0]:s}-'
+            prefix = f'{item_inner.name:s}-'
             with NamedTemporaryFile(prefix=prefix, suffix='.torrent', dir=cache_dir,
                                     delete=False) as w:
                 with open(item_inner, 'rb') as r:
                     w.write(r.read())
                 old = item_inner
-                item_inner = w.name
-            with open(item_inner, 'rb') as torrent_file:
+            with open(w.name, 'rb') as torrent_file:
                 # Because the server does not understand filename*=UTF8 syntax
                 # https://github.com/kennethreitz/requests/issues/2117
                 # This is not a huge concern, as the API's "Get .torrent"
                 # does not return the file with its original name either
                 filename = unidecode(torrent_file.name)
-                logger.info(f'Uploading torrent {basename(item)} (actual '
-                            f'name: "{basename(filename)}")')
+                logger.info(f'Uploading torrent {Path(item).name} (actual '
+                            f'name: "{Path(filename).name}")')
                 resp = requests.post(post_url,
                                      data=form_data,
                                      files=dict(torrent_file=(filename, torrent_file)),
                                      verify=not no_verify,
                                      timeout=30)
                 if not resp.ok:
                     logger.error(f'Error uploading {old}')
                     continue
                 # Delete original only after successful upload
                 logger.debug(f'Deleting {old}')
-                rm(old)
+                Path(old).unlink()
 
 
 @click.command(cls=command_with_config_file('config', 'list-ftp-users'))
 @click.option('-p', '--port', type=int, default=443, shell_complete=complete_ports)
 @click.option('-d', '--debug', is_flag=True)
 @click.option('-H', '--host', help='Xirvik host (without protocol)', shell_complete=complete_hosts)
 @click.option('-C', '--config', help='Configuration file')
@@ -120,15 +120,15 @@
                    config: str | None = None) -> None:
     """Lists FTP users."""
     setup_logging(debug)
     r = requests.get(f'https://{host}:{port:d}/userpanel/index.php/ftp_users', timeout=30)
     try:
         r.raise_for_status()
     except HTTPError as e:
-        raise click.Abort() from e
+        raise click.Abort from e
     content = Soup(r.text, 'html5lib').select('.gradeX td')
     click.echo(
         tabulate(((user.text, read_only.text == 'Yes', root_dir.text)
                   for user, read_only, root_dir, _ in (content[i:i + 4]
                                                        for i in range(0, len(content), 4))),
                  headers=('Username', 'Read-only', 'Root directory')))
 
@@ -159,15 +159,15 @@
                                 password_1=password,
                                 root_folder=root_dir,
                                 read_only='no'),
                       timeout=30)
     try:
         r.raise_for_status()
     except HTTPError as e:
-        raise click.Abort() from e
+        raise click.Abort from e
 
 
 @click.command(cls=command_with_config_file('config', 'delete-ftp-user'))
 @click.option('-p', '--port', type=int, default=443, shell_complete=complete_ports)
 @click.option('-d', '--debug', is_flag=True)
 @click.option('-H', '--host', help='Xirvik host (without protocol)', shell_complete=complete_hosts)
 @click.option('-C', '--config', help='Configuration file')
@@ -182,15 +182,15 @@
     user = b64encode(username.encode()).decode()
     uri = (f'https://{host}:{port:d}/userpanel/index.php/ftp_users/'
            f'delete/{user}')
     r = requests.get(uri, timeout=30)
     try:
         r.raise_for_status()
     except HTTPError as e:
-        raise click.Abort() from e
+        raise click.Abort from e
 
 
 @click.command(cls=command_with_config_file('config', 'authorize-ip'))
 @click.option('-p', '--port', type=int, default=443, shell_complete=complete_ports)
 @click.option('-d', '--debug', is_flag=True)
 @click.option('-H', '--host', help='Xirvik host (without protocol)', shell_complete=complete_hosts)
 @click.option('-C', '--config', help='Configuration file')
@@ -202,15 +202,15 @@
     setup_logging(debug)
     uri = (f'https://{host}:{port:d}/userpanel/index.php/virtual_machine/'
            'authorize_ip')
     r = requests.get(uri, timeout=30)
     try:
         r.raise_for_status()
     except HTTPError as e:
-        raise click.Abort() from e
+        raise click.Abort from e
 
 
 @click.command(cls=command_with_config_file('config', 'fix-rtorrent'))
 @click.option('-H', '--host', help='Xirvik host (without protocol)', shell_complete=complete_hosts)
 @click.option('-C', '--config', help='Configuration file')
 @click.option('-p', '--port', type=int, default=443, shell_complete=complete_ports)
 @click.option('-d', '--debug', is_flag=True)
@@ -223,18 +223,18 @@
     logger.info('No guarantees this will work!')
     uri = (f'https://{host}:{port:d}/userpanel/index.php/services/'
            'restart/rtorrent')
     r = requests.get(uri, timeout=30)
     try:
         r.raise_for_status()
     except HTTPError as e:
-        raise click.Abort() from e
+        raise click.Abort from e
 
 
-STATES_FOR_SORTING = set(('finished', 'creation_date', 'state_changed'))
+STATES_FOR_SORTING = {'finished', 'creation_date', 'state_changed'}
 
 
 @click.command(cls=command_with_config_file('config', 'list-torrents'))
 @click.option('-H', '--host', help='Xirvik host (without protocol)', shell_complete=complete_hosts)
 @click.option('-C', '--config', help='Configuration file')
 @click.option('-p', '--port', type=int, default=443, shell_complete=complete_ports)
 @click.option('-d', '--debug', is_flag=True)
@@ -253,19 +253,21 @@
                   debug: bool = False,
                   config: str | None = None,
                   no_headers: bool = False,
                   table_format: str = 'plain',
                   sort: str | None = None,
                   reverse_order: bool | None = None) -> None:
     """list torrents in a given format."""
+    min_tz_aware = datetime(MINYEAR, 1, 1, tzinfo=UTC)
+
     def sorter(x: TorrentInfo) -> Any:
         assert sort is not None
         if ((val := getattr(x, sort if sort != 'label' else 'custom1', None)) is None
                 and sort in STATES_FOR_SORTING):
-            return datetime.min
+            return min_tz_aware
         return val or ''
 
     setup_logging(debug)
     torrents = cast(Iterator[TorrentInfo] | Sequence[TorrentInfo],
                     ruTorrentClient(host).list_torrents())
     if sort:
         torrents = sorted(torrents, key=sorter)
@@ -282,15 +284,16 @@
                 dict(hash=x.hash,
                      name=x.name,
                      label=x.custom1,
                      finished=x.finished.isoformat() if x.finished else None,
                      base_path=x.base_path) for x in torrents
             ]))
     else:  # pragma no cover
-        raise click.Abort('Invalid table format specified')
+        click.echo('Invalid table format specified.', err=True)
+        raise click.Abort
 
 
 @click.command(cls=command_with_config_file('config', 'list-files'))
 @click.option('-H', '--host', help='Xirvik host (without protocol)', shell_complete=complete_hosts)
 @click.option('-C', '--config', help='Configuration file')
 @click.option('-p', '--port', type=int, default=443, shell_complete=complete_ports)
 @click.option('-d', '--debug', is_flag=True)
@@ -298,23 +301,24 @@
 @click.option('-F',
               '--table-format',
               type=click.Choice(tabulate_formats + ['json']),
               default='plain')
 @click.option('-S', '--sort', type=click.Choice(('name', 'size_bytes', 'priority')), default='name')
 @click.option('-R', '--reverse-order', is_flag=True)
 @click.argument('hash')
-def list_files(hash: str,
-               host: str,
-               port: int,
-               debug: bool = False,
-               config: str | None = None,
-               no_headers: bool = False,
-               table_format: str = 'plain',
-               sort: str = 'name',
-               reverse_order: bool | None = None) -> None:
+def list_files(
+        hash: str,  # noqa: A002
+        host: str,
+        port: int,
+        debug: bool = False,
+        config: str | None = None,
+        no_headers: bool = False,
+        table_format: str = 'plain',
+        sort: str = 'name',
+        reverse_order: bool | None = None) -> None:
     """list a torrent's files in a given format."""
     setup_logging(debug)
     files = sorted(cast(Iterator[TorrentTrackedFile] | Sequence[TorrentTrackedFile],
                         ruTorrentClient(host).list_files(hash)),
                    key=lambda x: getattr(x, sort))
     if reverse_order:
         files = list(reversed(list(files)))
@@ -325,15 +329,16 @@
                  for f in files),
                 headers=() if no_headers else
                 ('Name', 'Size', 'Downloaded Pieces', 'Number of Pieces', 'Priority ID'),
                 tablefmt=table_format))
     elif table_format == 'json':
         click.echo(json.dumps([x._asdict() for x in files]))
     else:  # pragma no cover
-        raise click.Abort('Invalid table format specified')
+        click.echo('Invalid table format specified.', err=True)
+        raise click.Abort
 
 
 def _resolve_single_file_torrent_path(info: TorrentInfo, filename: str) -> str:
     if not info.base_path.endswith(filename):
         return f'{info.base_path}/{filename}'
     return info.base_path
 
@@ -364,15 +369,15 @@
 @click.command(cls=command_with_config_file('config', 'list-untracked-files'),
                help='list untracked file paths.')
 @click.option('-H', '--host', help='Xirvik host (without protocol)', shell_complete=complete_hosts)
 @click.option('-L',
               '--server-list-command',
               help=('This should be a command that outputs lines where each line is a '
                     'complete file path that matches the "torrents/<username>/..." output '
-                    'from ruTorrent\'s API. An example using SSH:\n\n    '
+                    "from ruTorrent's API. An example using SSH:\n\n    "
                     "ssh name-of-server 'find /media/sf_hostshare -type f' | "
                     "sed -re 's|^/media/sf_hostshare|/torrents/username|g'"))
 @click.option('-d', '--debug', is_flag=True)
 def list_untracked_files(host: str,
                          server_list_command: str,
                          debug: bool = False,
                          config: str | None = None) -> None:
@@ -406,12 +411,16 @@
             files = list(client.list_files(info.hash))
             if len(files) == 1:
                 tracked_files.add(_resolve_single_file_torrent_path(info, files[0].name))
             else:
                 for file in (f'{info.base_path}/{y.name}' for y in files):
                     tracked_files.add(file)
     click.echo('Getting server-side file list', file=sys.stderr)
-    with sp.Popen(server_list_command, shell=True, text=True, stdout=sp.PIPE) as process:
+    with sp.Popen(
+            server_list_command,
+            shell=True,  # noqa: S602
+            text=True,
+            stdout=sp.PIPE) as process:
         assert process.stdout is not None
         while (line := process.stdout.readline().strip()):
             if line not in tracked_files:
                 click.echo(line)
```

### Comparing `xirvik_tools-0.4.5/xirvik/commands/util.py` & `xirvik_tools-0.5.0/xirvik/commands/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Utility functions for CLI commands."""
-from os.path import expanduser
-from types import FrameType
-from typing import Any, Callable, Iterator, Sequence, Type
+from pathlib import Path
+from typing import TYPE_CHECKING, Any
+from collections.abc import Callable, Iterator, Sequence
 import functools
 import itertools
 import logging
-import pathlib
 import re
 import sys
 import warnings
 
 from click.core import ParameterSource
 from loguru import logger
 import click
 import xdg.BaseDirectory
 import yaml
 
+if TYPE_CHECKING:  # pragma no cover
+    from types import FrameType
+
 __all__ = ('common_options_and_arguments', 'complete_hosts', 'complete_ports',
            'setup_log_intercept_handler', 'setup_logging')
 
 
 def setup_logging(debug: bool | None = False) -> None:
     """Shared function to enable logging."""
     if debug:  # pragma: no cover
@@ -47,15 +49,15 @@
                   help='Number of retries for each request (passed to client)')
     @click.option('-d', '--debug', is_flag=True, help='Enable debug level logging')
     @click.option('--backoff-factor',
                   default=5,
                   type=int,
                   help=('Back-off factor used when calculating time to wait to retry '
                         'a failed request'))
-    @click.option('--netrc', default=expanduser('~/.netrc'), help='netrc file path')
+    @click.option('--netrc', default=Path('~/.netrc').expanduser, help='netrc file path')
     @click.option('-C', '--config', help='Configuration file')
     @click.option('-H',
                   '--host',
                   help='Xirvik host (without protocol)',
                   shell_complete=complete_hosts)
     @functools.wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
@@ -70,28 +72,28 @@
         return host
     # Remove brackets and remove port at end
     return re.sub(r'[\[\]]', '', re.sub(r'\:[0-9]+$', '', host))
 
 
 def _read_ssh_known_hosts() -> Iterator[str]:
     try:
-        with open(expanduser('~/.ssh/known_hosts')) as f:
+        with open(Path('~/.ssh/known_hosts').expanduser()) as f:
             for line in f.readlines():
                 host_part = line.split()[0]
                 if ',' in host_part:
                     yield from (_clean_host(x) for x in host_part.split(','))
                 else:
                     yield _clean_host(host_part)
     except FileNotFoundError:
         pass
 
 
 def _read_netrc_hosts() -> Iterator[str]:
     try:
-        with open(expanduser('~/.netrc')) as f:
+        with open(Path('~/.netrc').expanduser()) as f:
             yield from (x.split()[1] for x in f.readlines())
     except FileNotFoundError:
         pass
 
 
 def complete_hosts(_: Any, __: Any, incomplete: str) -> Sequence[str]:
     """
@@ -128,29 +130,29 @@
 
 def setup_log_intercept_handler() -> None:  # pragma: no cover
     """Sets up Loguru to intercept records from the logging module."""
     logging.basicConfig(handlers=(InterceptHandler(),), level=0)
 
 
 def command_with_config_file(config_file_param_name: str = 'config',
-                             default_section: str | None = None) -> Type[click.Command]:
+                             default_section: str | None = None) -> type[click.Command]:
     """
     Returns a custom command class that can read from a configuration file
     in place of missing arguments.
 
     Parameters
     ----------
     config_file_param_name : str
         The name of the parameter given to Click in ``click.option``.
 
     default_section : str | None
         Default top key of YAML to read from.
     """
-    home = pathlib.Path.home()
-    default_config_file_path = pathlib.Path(xdg.BaseDirectory.xdg_config_home) / 'xirvik.yml'
+    home = Path.home()
+    default_config_file_path = Path(xdg.BaseDirectory.xdg_config_home) / 'xirvik.yml'
     if sys.platform == 'win32':  # pragma: no cover
         default_config_file_path = home / 'AppData/Roaming/xirvik-tools/config.yml'
     elif sys.platform == 'darwin':  # pragma: no cover
         default_config_file_path = home / 'Library/Application Support/xirvik-tools/config.yml'
 
     class _ConfigFileCommand(click.Command):
         def invoke(self, ctx: click.Context) -> Any:
@@ -162,25 +164,26 @@
                 with open(config_file_path) as f:
                     config_data = yaml.safe_load(f)
             except FileNotFoundError:  # pragma no cover
                 pass
             if isinstance(config_data, dict):
                 alt_data = (config_data.get(default_section, {})
                             if default_section is not None else {})
-                for param in ctx.params.keys():
+                for param in ctx.params:
                     if ctx.get_parameter_source(param) == ParameterSource.DEFAULT:
                         yaml_param = param.replace('_', '-')
                         if yaml_param in alt_data:
                             ctx.params[param] = alt_data[yaml_param]
                         elif yaml_param in config_data:
                             ctx.params[param] = config_data[yaml_param]
                 ctx.params[config_file_param_name] = config_file_path
             else:  # pragma no cover
-                warnings.warn(f'Unexpected type in {config_file_path}: ' + str(type(config_data)))
+                warnings.warn(f'Unexpected type in {config_file_path}: ' + str(type(config_data)),
+                              stacklevel=1)
             try:
                 return super().invoke(ctx)
             except Exception as e:
                 if debug:  # pragma no cover
                     logger.exception(str(e))
-                raise click.Abort() from e
+                raise click.Abort from e
 
     return _ConfigFileCommand
```

### Comparing `xirvik_tools-0.4.5/xirvik/typing.py` & `xirvik_tools-0.5.0/xirvik/typing.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,92 +17,94 @@
     HASHING = 2
     #:
     REHASHING = 3
 
 
 class State(IntEnum):
     """State of the torrent."""
-    #:
     STOPPED = 0
-    #:
+    ''''''
     STARTED_OR_PAUSED = 1
+    ''''''
 
 
 class TorrentInfo(NamedTuple):
     """Torrent information."""
-    hash: str
+    hash: str  # noqa: A003
     is_open: bool
     is_hash_checking: bool
     is_hash_checked: bool
     state: State
     name: str
     size_bytes: int
     completed_chunks: int
     size_chunks: int
     bytes_done: int
     up_total: int
     ratio: float
     up_rate: int
     down_rate: int
-    #: Chunk size (usually a power of 2).
     chunk_size: int
-    #: Usually contains the assigned label.
+    '''Chunk size (usually a power of 2).'''
     custom1: str
+    '''Usually contains the assigned label.'''
     peers_accounted: int
     peers_not_connected: int
     peers_connected: int
     peers_complete: int
     left_bytes: int
     priority: int
     state_changed: datetime | None
     skip_total: int
     hashing: HashingState
     chunks_hashed: int
-    #: Path before the torrent directory or file.
     base_path: str
-    #: Date torrent was added to the client. Can be ``None`` if this was not
-    #: captured, or possibly due to a crash.
+    '''Path before the torrent directory or file.'''
     creation_date: datetime | None
+    '''
+    Date torrent was added to the client. Can be ``None`` if this was not captured, or possibly due
+    to a crash.
+    '''
     tracker_focus: int
     is_active: bool
-    #: Message from the server.
     message: str
+    '''Message from the server.'''
     custom2: str
     free_diskspace: int
     is_private: bool
     is_multi_file: bool
-    # unk1: str
+    # unk1: str  # noqa: ERA001
     finished: datetime | None
 
 
 class FilePriority(IntEnum):
     """
     Single file priority. These are based on ruTorrent's code, not
     rTorrent's.
     """
-    #:
     DO_NOT_DOWNLOAD = 0
-    #:
+    ''''''
     NORMAL = 1
-    #:
+    ''''''
     HIGH = 2
+    ''''''
 
 
 class FileDownloadStrategy(IntEnum):
     """Single file download strategy."""
-    #: Also known as 'trailing chunk first'.
     NORMAL = 0
-    #:
+    '''Also known as 'trailing chunk first'.'''
     LEADING_CHUNK_FIRST = 1
+    ''''''
 
 
 class TorrentTrackedFile(NamedTuple):
     """Contains information about a single file within a torrent."""
-    #: File name without path.
     name: str
+    '''File name without path.'''
     number_of_pieces: int
     downloaded_pieces: int
     size_bytes: int
-    #: Download priority.
     priority_id: FilePriority
-    #: Download strategy.
+    '''Download priority.'''
     download_strategy_id: FileDownloadStrategy
+    '''Download strategy.'''
```

### Comparing `xirvik_tools-0.4.5/xirvik/utils.py` & `xirvik_tools-0.5.0/xirvik/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterator
+from collections.abc import Iterator
 
 __all__ = ('parse_header',)
 
 
 def _parseparam(param: str) -> Iterator[str]:
     while param[:1] == ';':
         param = param[1:]
```

