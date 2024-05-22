# Comparing `tmp/nonebot_plugin_mystool-2.4.0.tar.gz` & `tmp/nonebot_plugin_mystool-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-2.4.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-2.5.0.tar", max compression
```

## Comparing `nonebot_plugin_mystool-2.4.0.tar` & `nonebot_plugin_mystool-2.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1065 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/LICENSE
--rw-r--r--   0        0        0     2679 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/README.md
--rw-r--r--   0        0        0     1850 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     2316 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0       23 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/_version.py
--rw-r--r--   0        0        0       61 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/__init__.py
--rw-r--r--   0        0        0    85119 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/common.py
--rw-r--r--   0        0        0    11733 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/game_sign_api.py
--rw-r--r--   0        0        0    23943 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/myb_missions_api.py
--rw-r--r--   0        0        0     5365 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/weibo.py
--rw-r--r--   0        0        0      179 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/__init__.py
--rw-r--r--   0        0        0     4372 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/address.py
--rw-r--r--   0        0        0      662 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/common.py
--rw-r--r--   0        0        0    24207 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/exchange.py
--rw-r--r--   0        0        0     2739 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/help.py
--rw-r--r--   0        0        0    12213 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/login.py
--rw-r--r--   0        0        0    36439 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/plan.py
--rw-r--r--   0        0        0    14755 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/setting.py
--rw-r--r--   0        0        0    12523 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/user_check.py
--rw-r--r--   0        0        0       64 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/__init__.py
--rw-r--r--   0        0        0    17494 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/common.py
--rw-r--r--   0        0        0    11248 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/config.py
--rw-r--r--   0        0        0    17776 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/data.py
--rw-r--r--   0        0        0       22 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/__init__.py
--rw-r--r--   0        0        0     5004 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/common.py
--rw-r--r--   0        0        0     9484 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/configV2.py
--rw-r--r--   0        0        0    16456 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/dataV2.py
--rw-r--r--   0        0        0       48 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/__init__.py
--rw-r--r--   0        0        0    16124 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/common.py
--rw-r--r--   0        0        0     5622 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/good_image.py
--rw-r--r--   0        0        0     4438 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-22 13:01:02.456653 nonebot_plugin_mystool-2.5.0/LICENSE
+-rw-r--r--   0        0        0     2895 2024-05-22 13:01:02.456653 nonebot_plugin_mystool-2.5.0/README.md
+-rw-r--r--   0        0        0     1675 2024-05-22 13:01:02.456653 nonebot_plugin_mystool-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2806 2024-05-22 13:01:02.456653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-22 13:01:02.456653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/_version.py
+-rw-r--r--   0        0        0       61 2024-05-22 13:01:02.456653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/api/__init__.py
+-rw-r--r--   0        0        0    85119 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/api/common.py
+-rw-r--r--   0        0        0    11733 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/api/game_sign_api.py
+-rw-r--r--   0        0        0    23983 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/api/myb_missions_api.py
+-rw-r--r--   0        0        0    11454 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/api/weibo.py
+-rw-r--r--   0        0        0      179 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/__init__.py
+-rw-r--r--   0        0        0     4372 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/address.py
+-rw-r--r--   0        0        0      662 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/common.py
+-rw-r--r--   0        0        0    24400 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/exchange.py
+-rw-r--r--   0        0        0     2739 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/help.py
+-rw-r--r--   0        0        0    12213 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/login.py
+-rw-r--r--   0        0        0    37699 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/plan.py
+-rw-r--r--   0        0        0    15048 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/setting.py
+-rw-r--r--   0        0        0    12523 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/user_check.py
+-rw-r--r--   0        0        0       64 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/__init__.py
+-rw-r--r--   0        0        0    17494 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/common.py
+-rw-r--r--   0        0        0    11278 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/config.py
+-rw-r--r--   0        0        0    17704 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/data.py
+-rw-r--r--   0        0        0       22 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/upgrade/__init__.py
+-rw-r--r--   0        0        0     5004 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/upgrade/common.py
+-rw-r--r--   0        0        0     9484 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/upgrade/configV2.py
+-rw-r--r--   0        0        0    16456 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/upgrade/dataV2.py
+-rw-r--r--   0        0        0       48 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/utils/__init__.py
+-rw-r--r--   0        0        0    16281 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/utils/common.py
+-rw-r--r--   0        0        0     5622 2024-05-22 13:01:02.460653 nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/utils/good_image.py
+-rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-2.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-2.4.0/LICENSE` & `nonebot_plugin_mystool-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/README.md` & `nonebot_plugin_mystool-2.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -56,113 +56,126 @@
 00000370: 6164 6765 295d 2868 7474 7073 3a2f 2f67  adge)](https://g
 00000380: 6974 6875 622e 636f 6d2f 4c6a 7a64 2d50  ithub.com/Ljzd-P
 00000390: 524f 2f6e 6f6e 6562 6f74 2d70 6c75 6769  RO/nonebot-plugi
 000003a0: 6e2d 6d79 7374 6f6f 6c2f 636f 6d6d 6974  n-mystool/commit
 000003b0: 732f 6465 7629 0a0a 2320 6d79 7354 6f6f  s/dev)..# mysToo
 000003c0: 6c20 2d20 e7b1 b3e6 b8b8 e7a4 bee8 be85  l - ............
 000003d0: e58a a9e5 b7a5 e585 b7e6 8f92 e4bb b60a  ................
-000003e0: 0a23 2320 e29a a120 e58a 9fe8 83bd e592  .## ... ........
-000003f0: 8ce7 89b9 e680 a70a 0a2d 20e6 94af e68c  .........- .....
-00000400: 8151 51e8 818a e5a4 a9e5 928c 5151 e9a2  .QQ.........QQ..
-00000410: 91e9 8193 0a2d 20e7 9fad e4bf a1e9 aa8c  .....- .........
-00000420: e8af 81e7 99bb e5bd 95ef bc8c e585 8de6  ................
-00000430: 8a93 e58c 85e8 8eb7 e58f 9620 436f 6f6b  ........... Cook
-00000440: 6965 0a2d 20e8 87aa e58a a8e5 ae8c e688  ie.- ...........
-00000450: 90e6 af8f e697 a5e7 b1b3 e6b8 b8e5 b881  ................
-00000460: e4bb bbe5 8aa1 0a2d 20e8 87aa e58a a8e8  .......- .......
-00000470: bf9b e8a1 8ce6 b8b8 e688 8fe7 adbe e588  ................
-00000480: b00a 2d20 e58f afe5 88b6 e5ae 9ae7 b1b3  ..- ............
-00000490: e6b8 b8e5 b881 e595 86e5 9381 e585 91e6  ................
-000004a0: 8da2 e8ae a1e5 8892 efbc 8ce5 88b0 e782  ................
-000004b0: b9e5 8591 e68d a2ef bc88 e59b a0e5 8aa0  ................
-000004c0: e585 a5e4 ba86 e4ba bae6 9cba e9aa 8ce8  ................
-000004d0: af81 efbc 8ce6 8890 e58a 9fe7 8e87 e8be  ................
-000004e0: 83e4 bd8e efbc 890a 2d20 e58f afe6 94af  ........- ......
-000004f0: e68c 81e5 a49a e4b8 aa20 5151 20e8 b4a6  ......... QQ ...
-00000500: e58f b7ef bc8c e6af 8fe4 b8aa 2051 5120  ............ QQ 
-00000510: e8b4 a6e5 8fb7 e58f afe7 bb91 e5ae 9ae5  ................
-00000520: a49a e4b8 aae7 b1b3 e593 88e6 b8b8 e8b4  ................
-00000530: a6e6 88b7 0a2d 2051 5120 e68e a8e9 8081  .....- QQ ......
-00000540: e689 a7e8 a18c e7bb 93e6 9e9c e980 9ae7  ................
-00000550: 9fa5 0a2d 20e5 8e9f e7a5 9ee3 8081 e5b4  ...- ...........
-00000560: a9e5 9d8f efbc 9ae6 989f e7a9 b9e9 9381  ................
-00000570: e981 93e7 8ab6 e680 81e4 bebf e7ac bae9  ................
-00000580: 809a e79f a50a 2d20 e58f afe4 b8ba e799  ......- ........
-00000590: bbe5 bd95 e380 81e6 af8f e697 a5e7 b1b3  ................
-000005a0: e6b8 b8e5 b881 e4bb bbe5 8aa1 e380 81e6  ................
-000005b0: b8b8 e688 8fe7 adbe e588 b0e9 858d e7bd  ................
-000005c0: aee4 baba e69c bae9 aa8c e8af 81e6 8993  ................
-000005d0: e7a0 81e5 b9b3 e58f b00a 2d20 e58f afe9  ..........- ....
-000005e0: 858d e7bd aee7 94a8 e688 b7e9 bb91 e590  ................
-000005f0: 8de5 8d95 2fe7 99bd e590 8de5 8d95 0a0a  ..../...........
-00000600: 2323 20f0 9f93 9620 e4bd bfe7 94a8 e8af  ## .... ........
-00000610: b4e6 988e 0a0a 2323 2320 f09f 9ba0 efb8  ......### ......
-00000620: 8f20 4e6f 6e65 426f 7432 20e6 9cba e599  . NoneBot2 .....
-00000630: a8e4 baba e983 a8e7 bdb2 e592 8ce6 8f92  ................
-00000640: e4bb b6e5 ae89 e8a3 850a 0ae8 afb7 e69f  ................
-00000650: a5e7 9c8b 202d 3e20 5bf0 9f94 9749 6e73  .... -> [....Ins
-00000660: 7461 6c6c 6174 696f 6e5d 2868 7474 7073  tallation](https
-00000670: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c6a  ://github.com/Lj
-00000680: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
-00000690: 6c75 6769 6e2d 6d79 7374 6f6f 6c2f 7769  lugin-mystool/wi
-000006a0: 6b69 2f49 6e73 7461 6c6c 6174 696f 6e29  ki/Installation)
-000006b0: 0a0a 2323 2320 f09f 9396 20e6 8f92 e4bb  ..### .... .....
-000006c0: b6e5 85b7 e4bd 93e4 bdbf e794 a8e8 afb4  ................
-000006d0: e698 8e0a 0ae8 afb7 e69f a5e7 9c8b 202d  .............. -
-000006e0: 3e20 5bf0 9f94 9757 696b 6920 e696 87e6  > [....Wiki ....
-000006f0: a1a3 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
-00000700: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
-00000710: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-00000720: 7973 746f 6f6c 2f77 696b 6929 0a0a 2323  ystool/wiki)..##
-00000730: 2320 e29d 9320 e88e b7e5 8f96 e68f 92e4  # ... ..........
-00000740: bbb6 e5b8 aee5 8aa9 e4bf a1e6 81af 0a0a  ................
-00000750: 2323 2323 20e6 8f92 e4bb b6e5 91bd e4bb  #### ...........
-00000760: a40a 0a60 6060 0a2f e5b8 aee5 8aa9 0a60  ...```./.......`
-00000770: 6060 0a0a 3e20 5b21 4e4f 5445 5d0a 3e20  ``..> [!NOTE].> 
-00000780: e6ad a4e5 a484 e6b2 a1e6 9c89 e4bd bfe7  ................
-00000790: 94a8 205b f09f 9497 20e6 8f92 e4bb b6e5  .. [.... .......
-000007a0: 91bd e4bb a4e5 a4b4 5d28 6874 7470 733a  ........](https:
-000007b0: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
-000007c0: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
-000007d0: 7567 696e 2d6d 7973 746f 6f6c 2f77 696b  ugin-mystool/wik
-000007e0: 692f 436f 6e66 6967 7572 6174 696f 6e2d  i/Configuration-
-000007f0: 5072 6566 6572 656e 6365 2363 6f6d 6d61  Preference#comma
-00000800: 6e64 5f73 7461 7274 290a 0a23 2320 e585  nd_start)..## ..
-00000810: b6e4 bb96 0a0a 2323 2320 e8b4 a1e7 8cae  ......### ......
-00000820: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00000830: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
-00000840: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
-00000850: 7567 696e 2d6d 7973 746f 6f6c 2f67 7261  ugin-mystool/gra
-00000860: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
-00000870: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
-00000880: 7474 7073 3a2f 2f63 6f6e 7472 6962 2e72  ttps://contrib.r
-00000890: 6f63 6b73 2f69 6d61 6765 3f72 6570 6f3d  ocks/image?repo=
-000008a0: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
-000008b0: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c26  -plugin-mystool&
-000008c0: 6d61 783d 3130 3030 2220 616c 743d 22e8  max=1000" alt=".
-000008d0: b4a1 e78c aee8 8085 222f 3e0a 3c2f 613e  ........"/>.</a>
-000008e0: 0a0a 2323 2320 f09f 94a8 20e5 bc80 e58f  ..### .... .....
-000008f0: 91e7 8988 e588 86e6 94af 0a5b 2a2a f09f  ...........[**..
-00000900: 94a8 6465 762a 2a5d 2868 7474 7073 3a2f  ..dev**](https:/
-00000910: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
-00000920: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
-00000930: 6769 6e2d 6d79 7374 6f6f 6c2f 7472 6565  gin-mystool/tree
-00000940: 2f64 6576 290a 0a23 2323 20f0 9f93 8320  /dev)..### .... 
-00000950: e6ba 90e7 a081 e8af b4e6 988e 0a5b f09f  .............[..
-00000960: 9383 536f 7572 6365 2d53 7472 7563 7475  ..Source-Structu
-00000970: 7265 5d28 6874 7470 733a 2f2f 6769 7468  re](https://gith
-00000980: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
-00000990: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-000009a0: 7973 746f 6f6c 2f77 696b 692f 536f 7572  ystool/wiki/Sour
-000009b0: 6365 2d53 7472 7563 7475 7265 290a 0a23  ce-Structure)..#
-000009c0: 2323 20e9 8082 e985 8d20 5be7 bbaa e5b1  ## ...... [.....
-000009d0: b1e7 9c9f e5af bb42 6f74 5d28 6874 7470  .......Bot](http
-000009e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f48  s://github.com/H
-000009f0: 6962 694b 6965 722f 7a68 656e 7875 6e5f  ibiKier/zhenxun_
-00000a00: 626f 7429 20e7 9a84 e588 86e6 94af 0a2d  bot) ..........-
-00000a10: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000a20: 636f 6d2f 4d57 544a 432f 7a68 656e 7875  com/MWTJC/zhenxu
-00000a30: 6e2d 706c 7567 696e 2d6d 7973 746f 6f6c  n-plugin-mystool
-00000a40: 0a2d 2068 7474 7073 3a2f 2f67 6974 6875  .- https://githu
-00000a50: 622e 636f 6d2f 6179 616b 6173 756b 692f  b.com/ayakasuki/
-00000a60: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-00000a70: 7973 746f 6f6c 0a                        ystool.
+000003e0: 0a3e 205b 214e 6f74 655d 0a3e 20e7 9bae  .> [!Note].> ...
+000003f0: e589 8de6 9cac e9a1 b9e7 9bae e59f bae6  ................
+00000400: 9cac e4b8 8de5 868d e696 b0e5 a29e e58a  ................
+00000410: 9fe8 83bd efbc 8ce9 97ae e9a2 98e4 bfae  ................
+00000420: e5a4 8de5 8faf e883 bde4 b99f e4bc 9ae6  ................
+00000430: af94 e8be 83e8 bf9f efbc 8ce4 b8bb e8a6  ................
+00000440: 81e6 98af e794 b1e4 ba8e e5bd 93e5 898d  ................
+00000450: e9a1 b9e7 9bae e4bb a3e7 a081 e58f afe7  ................
+00000460: bbb4 e68a a4e6 80a7 e8be 83e5 b7ae efbc  ................
+00000470: 885c 0a3e 20e4 bba5 e58f 8ae4 b8aa e4ba  .\.> ...........
+00000480: bae6 97b6 e997 b4e5 ae89 e68e 92e7 ad89  ................
+00000490: e380 82e6 9caa e69d a5e5 8faf e883 bde8  ................
+000004a0: 8083 e899 91e5 bdbb e5ba 95e9 878d e581  ................
+000004b0: 9ae4 b880 e6ac a10a 0a23 2320 e29a a120  .........## ... 
+000004c0: e58a 9fe8 83bd e592 8ce7 89b9 e680 a70a  ................
+000004d0: 0a2d 20e6 94af e68c 8151 51e8 818a e5a4  .- ......QQ.....
+000004e0: a9e5 928c 5151 e9a2 91e9 8193 0a2d 20e7  ....QQ.......- .
+000004f0: 9fad e4bf a1e9 aa8c e8af 81e7 99bb e5bd  ................
+00000500: 95ef bc8c e585 8de6 8a93 e58c 85e8 8eb7  ................
+00000510: e58f 9620 436f 6f6b 6965 0a2d 20e8 87aa  ... Cookie.- ...
+00000520: e58a a8e5 ae8c e688 90e6 af8f e697 a5e7  ................
+00000530: b1b3 e6b8 b8e5 b881 e4bb bbe5 8aa1 0a2d  ...............-
+00000540: 20e8 87aa e58a a8e8 bf9b e8a1 8ce6 b8b8   ...............
+00000550: e688 8fe7 adbe e588 b00a 2d20 e58f afe5  ..........- ....
+00000560: 88b6 e5ae 9ae7 b1b3 e6b8 b8e5 b881 e595  ................
+00000570: 86e5 9381 e585 91e6 8da2 e8ae a1e5 8892  ................
+00000580: efbc 8ce5 88b0 e782 b9e5 8591 e68d a2ef  ................
+00000590: bc88 e59b a0e5 8aa0 e585 a5e4 ba86 e4ba  ................
+000005a0: bae6 9cba e9aa 8ce8 af81 efbc 8ce6 8890  ................
+000005b0: e58a 9fe7 8e87 e8be 83e4 bd8e efbc 890a  ................
+000005c0: 2d20 e58f afe6 94af e68c 81e5 a49a e4b8  - ..............
+000005d0: aa20 5151 20e8 b4a6 e58f b7ef bc8c e6af  . QQ ...........
+000005e0: 8fe4 b8aa 2051 5120 e8b4 a6e5 8fb7 e58f  .... QQ ........
+000005f0: afe7 bb91 e5ae 9ae5 a49a e4b8 aae7 b1b3  ................
+00000600: e593 88e6 b8b8 e8b4 a6e6 88b7 0a2d 2051  .............- Q
+00000610: 5120 e68e a8e9 8081 e689 a7e8 a18c e7bb  Q ..............
+00000620: 93e6 9e9c e980 9ae7 9fa5 0a2d 20e5 8e9f  ...........- ...
+00000630: e7a5 9ee3 8081 e5b4 a9e5 9d8f efbc 9ae6  ................
+00000640: 989f e7a9 b9e9 9381 e981 93e7 8ab6 e680  ................
+00000650: 81e4 bebf e7ac bae9 809a e79f a50a 2d20  ..............- 
+00000660: e58f afe4 b8ba e799 bbe5 bd95 e380 81e6  ................
+00000670: af8f e697 a5e7 b1b3 e6b8 b8e5 b881 e4bb  ................
+00000680: bbe5 8aa1 e380 81e6 b8b8 e688 8fe7 adbe  ................
+00000690: e588 b0e9 858d e7bd aee4 baba e69c bae9  ................
+000006a0: aa8c e8af 81e6 8993 e7a0 81e5 b9b3 e58f  ................
+000006b0: b00a 2d20 e58f afe9 858d e7bd aee7 94a8  ..- ............
+000006c0: e688 b7e9 bb91 e590 8de5 8d95 2fe7 99bd  ............/...
+000006d0: e590 8de5 8d95 0a0a 2323 20f0 9f93 9620  ........## .... 
+000006e0: e4bd bfe7 94a8 e8af b4e6 988e 0a0a 2323  ..............##
+000006f0: 2320 f09f 9ba0 efb8 8f20 4e6f 6e65 426f  # ....... NoneBo
+00000700: 7432 20e6 9cba e599 a8e4 baba e983 a8e7  t2 .............
+00000710: bdb2 e592 8ce6 8f92 e4bb b6e5 ae89 e8a3  ................
+00000720: 850a 0ae8 afb7 e69f a5e7 9c8b 202d 3e20  ............ -> 
+00000730: 5bf0 9f94 9749 6e73 7461 6c6c 6174 696f  [....Installatio
+00000740: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
+00000750: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+00000760: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00000770: 7374 6f6f 6c2f 7769 6b69 2f49 6e73 7461  stool/wiki/Insta
+00000780: 6c6c 6174 696f 6e29 0a0a 2323 2320 f09f  llation)..### ..
+00000790: 9396 20e6 8f92 e4bb b6e5 85b7 e4bd 93e4  .. .............
+000007a0: bdbf e794 a8e8 afb4 e698 8e0a 0ae8 afb7  ................
+000007b0: e69f a5e7 9c8b 202d 3e20 5bf0 9f94 9757  ...... -> [....W
+000007c0: 696b 6920 e696 87e6 a1a3 5d28 6874 7470  iki ......](http
+000007d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+000007e0: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
+000007f0: 706c 7567 696e 2d6d 7973 746f 6f6c 2f77  plugin-mystool/w
+00000800: 696b 6929 0a0a 2323 2320 e29d 9320 e88e  iki)..### ... ..
+00000810: b7e5 8f96 e68f 92e4 bbb6 e5b8 aee5 8aa9  ................
+00000820: e4bf a1e6 81af 0a0a 2323 2323 20e6 8f92  ........#### ...
+00000830: e4bb b6e5 91bd e4bb a40a 0a60 6060 0a2f  ...........```./
+00000840: e5b8 aee5 8aa9 0a60 6060 0a0a 3e20 5b21  .......```..> [!
+00000850: 4e4f 5445 5d0a 3e20 e6ad a4e5 a484 e6b2  NOTE].> ........
+00000860: a1e6 9c89 e4bd bfe7 94a8 205b f09f 9497  .......... [....
+00000870: 20e6 8f92 e4bb b6e5 91bd e4bb a4e5 a4b4   ...............
+00000880: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000890: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
+000008a0: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+000008b0: 746f 6f6c 2f77 696b 692f 436f 6e66 6967  tool/wiki/Config
+000008c0: 7572 6174 696f 6e2d 5072 6566 6572 656e  uration-Preferen
+000008d0: 6365 2363 6f6d 6d61 6e64 5f73 7461 7274  ce#command_start
+000008e0: 290a 0a23 2320 e585 b6e4 bb96 0a0a 2323  )..## ........##
+000008f0: 2320 e8b4 a1e7 8cae 0a3c 6120 6872 6566  # .......<a href
+00000900: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000910: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
+00000920: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00000930: 746f 6f6c 2f67 7261 7068 732f 636f 6e74  tool/graphs/cont
+00000940: 7269 6275 746f 7273 223e 0a20 203c 696d  ributors">.  <im
+00000950: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
+00000960: 6f6e 7472 6962 2e72 6f63 6b73 2f69 6d61  ontrib.rocks/ima
+00000970: 6765 3f72 6570 6f3d 4c6a 7a64 2d50 524f  ge?repo=Ljzd-PRO
+00000980: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
+00000990: 6d79 7374 6f6f 6c26 6d61 783d 3130 3030  mystool&max=1000
+000009a0: 2220 616c 743d 22e8 b4a1 e78c aee8 8085  " alt=".........
+000009b0: 222f 3e0a 3c2f 613e 0a0a 2323 2320 f09f  "/>.</a>..### ..
+000009c0: 94a8 20e5 bc80 e58f 91e7 8988 e588 86e6  .. .............
+000009d0: 94af 0a5b 2a2a f09f 94a8 6465 762a 2a5d  ...[**....dev**]
+000009e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000009f0: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
+00000a00: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
+00000a10: 6f6f 6c2f 7472 6565 2f64 6576 290a 0a23  ool/tree/dev)..#
+00000a20: 2323 20f0 9f93 8320 e6ba 90e7 a081 e8af  ## .... ........
+00000a30: b4e6 988e 0a5b f09f 9383 536f 7572 6365  .....[....Source
+00000a40: 2d53 7472 7563 7475 7265 5d28 6874 7470  -Structure](http
+00000a50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+00000a60: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
+00000a70: 706c 7567 696e 2d6d 7973 746f 6f6c 2f77  plugin-mystool/w
+00000a80: 696b 692f 536f 7572 6365 2d53 7472 7563  iki/Source-Struc
+00000a90: 7475 7265 290a 0a23 2323 20e9 8082 e985  ture)..### .....
+00000aa0: 8d20 5be7 bbaa e5b1 b1e7 9c9f e5af bb42  . [............B
+00000ab0: 6f74 5d28 6874 7470 733a 2f2f 6769 7468  ot](https://gith
+00000ac0: 7562 2e63 6f6d 2f48 6962 694b 6965 722f  ub.com/HibiKier/
+00000ad0: 7a68 656e 7875 6e5f 626f 7429 20e7 9a84  zhenxun_bot) ...
+00000ae0: e588 86e6 94af 0a2d 2068 7474 7073 3a2f  .......- https:/
+00000af0: 2f67 6974 6875 622e 636f 6d2f 4d57 544a  /github.com/MWTJ
+00000b00: 432f 7a68 656e 7875 6e2d 706c 7567 696e  C/zhenxun-plugin
+00000b10: 2d6d 7973 746f 6f6c 0a2d 2068 7474 7073  -mystool.- https
+00000b20: 3a2f 2f67 6974 6875 622e 636f 6d2f 6179  ://github.com/ay
+00000b30: 616b 6173 756b 692f 6e6f 6e65 626f 742d  akasuki/nonebot-
+00000b40: 706c 7567 696e 2d6d 7973 746f 6f6c 0a    plugin-mystool.
```

### Comparing `nonebot_plugin_mystool-2.4.0/pyproject.toml` & `nonebot_plugin_mystool-2.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v2.4.0"
+version = "v2.5.0"
 description = "QQ聊天、频道机器人插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神崩铁便笺提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.asia>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
@@ -35,19 +35,14 @@
 tenacity = "^8.2.3"
 qrcode = "^7.4.2"
 pydantic = "^1.10.14"
 nonebot2 = ">=2.0.0"
 pytz = ">=2023.4,<2025.0"
 
 [tool.poetry.group.test.dependencies]
-nonebot2 = { version = "^2.0.1", extras = ["fastapi", "httpx", "websockets"] }
-nonebug = "^0.3.4"
-pytest = "^7.4.0"
-pytest-html = ">=3.2,<5.0"
-pytest-asyncio = ">=0.21,<0.24"
 flake8 = ">=6.1,<8.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Ljzd-PRO/nonebot-plugin-mystool/issues"
```

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/common.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/api/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/game_sign_api.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/api/game_sign_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/myb_missions_api.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/api/myb_missions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         self.headers = HEADERS_BASE.copy()
         self.headers["x-rpc-device_id"] = account.device_id_android
 
     async def sign(self, user: UserData, retry: bool = True) -> Tuple[MissionStatus, Optional[int]]:
         """
         签到
 
+        :param user: 用户数据对象
         :param retry: 是否允许重试
         :return: (BaseApiStatus, 签到获得的米游币数量)
         """
         content = {"gids": self.gids}
         try:
             async for attempt in get_async_retry(retry):
                 with attempt:
```

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/address.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/address.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/common.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/exchange.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,19 @@
         plans = PluginDataManager.plugin_data.users[event.get_user_id()].exchange_plans
         if plans:
             for plan in plans:
                 if plan.good.goods_id == good_id:
                     plans.discard(plan)
                     PluginDataManager.write_plugin_data()
                     for i in range(plugin_config.preference.exchange_thread_count):
-                        scheduler.remove_job(job_id=f"exchange-plan-{hash(plan)}-{i}")
+                        try:
+                            scheduler.remove_job(job_id=f"exchange-plan-{hash(plan)}-{i}")
+                        except scheduler.JobLookupError:
+                            # TODO: 原因不明，暂时忽略异常
+                            pass
                     await matcher.finish('兑换计划删除成功')
             await matcher.finish(f"您没有设置商品ID为 {good_id} 的兑换哦~")
         else:
             await matcher.finish("您还没有配置兑换计划哦~")
 
     else:
         await matcher.reject(
```

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/help.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/login.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/plan.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_saa import Image
 from pydantic import BaseModel
 
 from ..api import BaseGameSign
 from ..api import BaseMission, get_missions_state
 from ..api.common import genshin_note, get_game_record, starrail_note
-from ..api.weibo import WeiboCode
+from ..api.weibo import WeiboCode, WeiboSign
 from ..command.common import CommandRegistry
 from ..command.exchange import generate_image
 from ..model import (MissionStatus, PluginDataManager, plugin_config, UserData, CommandUsage, GenshinNoteNotice,
                      StarRailNoteNotice)
 from ..utils import get_file, logger, COMMAND_BEGIN, GeneralMessageEvent, GeneralGroupMessageEvent, \
     send_private_msg, get_all_bind, \
     get_unique_users, get_validate, read_admin_list
 
 __all__ = [
     "manually_game_sign", "manually_bbs_sign", "manually_genshin_note_check",
-    "manually_starrail_note_check", "manually_weibo_check"
+    "manually_starrail_note_check", "manually_weibo_code_check", "manually_weibo_sign_check"
 ]
 
 manually_game_sign = on_command(plugin_config.preference.command_start + '签到', priority=5, block=True)
 
 CommandRegistry.set_usage(
     manually_game_sign,
     CommandUsage(
@@ -645,47 +645,88 @@
             if matcher:
                 await matcher.send(msg)
             else:
                 for user_id in user_ids:
                     await send_private_msg(user_id=user_id, message=msg)
 
 
+manually_weibo_code_check = on_command(plugin_config.preference.command_start + 'wb兑换', priority=5, block=True)
+
+
+@manually_weibo_code_check.handle()
+async def weibo_code(event: Union[GeneralMessageEvent], matcher: Matcher):
+    if isinstance(event, GeneralGroupMessageEvent):
+        await matcher.send("⚠️为了保护您的隐私，请私聊进行查询。")
+    else:
+        user_id = event.get_user_id()
+        user = PluginDataManager.plugin_data.users.get(user_id)
+        await weibo_code_check(user=user, user_ids=[user_id], matcher=matcher)
+
+
+manually_weibo_sign_check = on_command(plugin_config.preference.command_start + 'wb签到', priority=5, block=True)
+
+
+@manually_weibo_sign_check.handle()
+async def weibo_sign(event: Union[GeneralMessageEvent], matcher: Matcher):
+    user_id = event.get_user_id()
+    user = PluginDataManager.plugin_data.users.get(user_id)
+    await weibo_sign_check(user=user, user_ids=[user_id], matcher=matcher)
+
+
+async def weibo_sign_check(user: UserData, user_ids: Iterable[str], matcher: Matcher = None):
+    """
+    :param user: 用户对象
+    :param user_ids: 发送通知的所有用户ID
+    :param matcher: nonebot ``Matcher``
+    """
+    for user_data in user.weibo:
+        msg = await WeiboSign.sign(user_data)
+        if matcher:
+            await matcher.send(message=msg)
+        else:
+            for user_id in user_ids:
+                await send_private_msg(user_id=user_id, message=msg)
+
+
 async def weibo_code_check(user: UserData, user_ids: Iterable[str], matcher: Matcher = None):
     """
     是否开启微博兑换码功能的函数，并发送给用户任务执行消息。
 
     :param user: 用户对象
     :param user_ids: 发送通知的所有用户ID
     :param matcher: nonebot ``Matcher``
     """
-    msg, img = None, None
+
     if user.enable_weibo:
         # account = UserAccount(account) 
-        weibo = WeiboCode(user)
-        result = await weibo.get_code_list()
-        try:
-            if isinstance(result, tuple):
-                msg, img = result
-            else:
-                msg = result
-        except Exception:
-            pass
-        if matcher:
-            if img:
-                onebot_img_msg = OneBotV11MessageSegment.image(await get_file(img))
-                messages = msg + onebot_img_msg
-            else:
-                messages = msg
-            await matcher.send(messages)
-        else:
-            if img and '无' not in msg:
-                saa_img = Image(await get_file(img))
-                messages = msg + saa_img
-                for user_id in user_ids:
-                    await send_private_msg(user_id=user_id, message=messages)
+        for user_data in user.weibo:
+            msg, img = None, None
+            weibo = WeiboCode(user_data)
+            result = await weibo.get_code_list()
+            try:
+                if isinstance(result, tuple):
+                    msg, img = result
+                else:
+                    msg = result
+            except Exception:
+                pass
+            if matcher:
+                if img:
+                    onebot_img_msg = OneBotV11MessageSegment.image(await get_file(img))
+                    messages = msg + onebot_img_msg
+                else:
+                    messages = msg
+                await matcher.send(messages)
+            else:
+                if img and '无' not in msg:
+                    saa_img = Image(await get_file(img))
+                    messages = msg + saa_img
+                    for user_id in user_ids:
+                        logger.info(f"检测到当前超话有兑换码，正在给{user_id}推送信息中")
+                        await send_private_msg(user_id=user_id, message=messages)
     else:
         message = "未开启微博功能"
         if matcher:
             await matcher.send(message)
 
 
 @scheduler.scheduled_job("cron", hour='0', minute='0', id="daily_goodImg_update")
@@ -730,27 +771,15 @@
 
 @scheduler.scheduled_job("cron",
                          hour=str(int(plugin_config.preference.plan_time.split(':')[0]) + 1),
                          minute=plugin_config.preference.plan_time.split(':')[1],
                          id="weibo_schedule")
 async def auto_weibo_check():
     """
-    每日检查微博活动签到兑换码函数
+    每日检查微博超话签到及兑换码函数
     """
     logger.info(f"{plugin_config.preference.log_head}开始执行微博自动任务")
     for user_id, user in get_unique_users():
         user_ids = [user_id] + list(get_all_bind(user_id))
+        await weibo_sign_check(user=user, user_ids=user_ids)
         await weibo_code_check(user=user, user_ids=user_ids)
     logger.info(f"{plugin_config.preference.log_head}微博自动任务执行完成")
-
-
-manually_weibo_check = on_command(plugin_config.preference.command_start + 'wb兑换', priority=5, block=True)
-
-
-@manually_weibo_check.handle()
-async def weibo_schedule(event: Union[GeneralMessageEvent], matcher: Matcher):
-    if isinstance(event, GeneralGroupMessageEvent):
-        await matcher.send("⚠️为了保护您的隐私，请私聊进行查询。")
-    else:
-        user_id = event.get_user_id()
-        user = PluginDataManager.plugin_data.users.get(user_id)
-        await weibo_code_check(user=user, user_ids=[user_id], matcher=matcher)
```

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/setting.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/setting.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from nonebot import on_command
 from nonebot.internal.params import ArgStr
 from nonebot.matcher import Matcher
 from nonebot.params import T_State
 
 from ..api import BaseMission
+from ..api.weibo import Tool
 from ..command.common import CommandRegistry
 from ..model import PluginDataManager, plugin_config, UserAccount, CommandUsage, UserData
 from ..utils import COMMAND_BEGIN, GeneralMessageEvent
 
 __all__ = ["setting", "account_setting", "global_setting"]
 
 setting = on_command(plugin_config.preference.command_start + '设置', priority=4, block=True)
@@ -153,19 +154,25 @@
             "\n\n🚪发送“退出”即可退出"
         )
         state["setting_item"] = "setting_notice_value"
         return
     elif setting_id == "7":
         user: UserData = state["user"]
         msg = ""
-        msg += "请发送想要设置的微博参数："
+        msg += "请发送想要设置的微博功能开关或账号："
         msg += f"\n1. 微博签到与兑换：{'开' if user.enable_weibo else '关'}"
-        msg += "\n2. 微博cookie" \
-               "\n3. 微博params" \
-               "\n\n🚪发送“退出”即可退出"
+        count = 1
+        if len(user.weibo) > 0:
+            for users in user.weibo:
+                for k_u, v_u in users.items():
+                    if k_u == 'name':
+                        count += 1
+                        msg += f"\n{count}. {str(v_u)}"
+        msg += "\n发送“添加账号”或已有账号名称进行添加/修改"
+        msg += "\n\n🚪发送“退出”即可退出"
         await account_setting.send(msg)
         state["setting_item"] = "weibo_value"
         return
     elif setting_id == '8':
         state["prepare_to_delete"] = True
         await account_setting.reject(f"⚠️确认删除账号 {account.display_name} ？发送 \"确认删除\" 以确定。")
     elif setting_id == '确认删除' and state["prepare_to_delete"]:
@@ -202,29 +209,26 @@
 
     elif state["setting_item"] == "weibo_value":
         user: UserData = state["user"]
         if notice_game == "1":
             user.enable_weibo = not user.enable_weibo
             PluginDataManager.write_plugin_data()
             await account_setting.finish(f"微博签到与兑换功能已 {'✅开启' if user.enable_weibo else '❌关闭'}")
-        elif notice_game == "2":
-            await account_setting.send(
-                "请微博cookie："
-                "发送格式不带cookie="
-                "\n\n🚪发送“退出”即可退出"
-            )
-            state["setting_item"] = "setting_weibo_value_cookie"
-        elif notice_game == "3":
+        else:
             await account_setting.send(
-                "请微博params："
-                "发送格式不带params="
-                "params必要参数: s、gsid、aid、from"
-                "\n\n🚪发送“退出”即可退出"
+                "参数说明：\n"
+                "  cookie必填SUB,SUBP\n"
+                "  params必填s,gsid,aid,from\n"
+                "  参数以 ; 相连\n"
+                "  如 xxx: a=x;b=x;\n"
+                "发送以下格式进行添加：\n"
+                "name:名称|cookie:xxx|params:xxx\n\n"
+                "🚪发送“退出”即可退出"
             )
-            state["setting_item"] = "setting_weibo_value_params"
+            state["setting_item"] = "setting_weibo_value"
 
 
 @account_setting.got('setting_value')
 async def _(_: Union[GeneralMessageEvent], state: T_State, setting_value=ArgStr()):
     if setting_value == '退出':
         await account_setting.finish('🚪已成功退出')
     account: UserAccount = state['account']
@@ -274,23 +278,26 @@
         account.mission_games = mission_games
         PluginDataManager.write_plugin_data()
         setting_value = setting_value.replace(" ", "、")
         await account_setting.finish(f"💬执行米游币任务的频道已更改为『{setting_value}』")
 
     # 做区分，以下应用在用户数据中，而非米游社数据中
     user: UserData = state["user"]
-    print(user)
-    if state["setting_item"] == "setting_weibo_value_cookie":
-        user.weibo_cookie = str(setting_value)
-        PluginDataManager.write_plugin_data()
-        await account_setting.finish("设置微博cookie成功")
-    elif state["setting_item"] == "setting_weibo_value_params":
-        user.weibo_params = str(setting_value)
+    if state["setting_item"] == "setting_weibo_value":
+        userdata_dict = Tool.weibo_user_dict(setting_value)
+        if len(user.weibo) > 0:
+            for usr in user.weibo:
+                if usr['name'] == userdata_dict['name']:
+                    usr.update(userdata_dict)
+                else:
+                    user.weibo.append(userdata_dict)
+        elif len(user.weibo) == 0:
+            user.weibo.append(userdata_dict)
         PluginDataManager.write_plugin_data()
-        await account_setting.finish("设置微博params成功")
+        await account_setting.finish(f"{userdata_dict['name']}微博账号设置成功")
 
 
 global_setting = on_command(plugin_config.preference.command_start + '通知设置', priority=5, block=True)
 
 CommandRegistry.set_usage(
     global_setting,
     CommandUsage(
```

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/user_check.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/command/user_check.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/common.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/config.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from datetime import time, timedelta, datetime
 from pathlib import Path
 from typing import Union, Optional, Tuple, Any, Dict, TYPE_CHECKING
 
 import nonebot
 from nonebot.log import logger
 from pydantic import BaseModel, BaseSettings, validator
@@ -148,15 +149,15 @@
     开源字体 Source Han Sans 思源黑体
     https://github.com/adobe-fonts/source-han-sans
     '''
     FONT_SIZE: int = 50
     '''字体大小'''
     SAVE_PATH: Path = data_path
     '''商品列表图片缓存目录'''
-    MULTI_PROCESS: bool = True
+    MULTI_PROCESS: bool = sys.platform != "win32"
     '''是否使用多进程生成图片（如果生成图片时崩溃，可尝试关闭此选项）'''
 
 
 class SaltConfig(BaseModel):
     """
     生成Headers - DS所用salt值，非必要请勿修改
     """
```

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/data.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,19 +364,17 @@
 
     >>> userdata = UserData()
     >>> hash(userdata)
     """
     enable_notice: bool = True
     """是否开启通知"""
     enable_weibo: bool = False
-    '''是否开启微博兑换码功能'''
-    weibo_cookie: str = ""
-    '''微博查询活动签到用的 cookie'''
-    weibo_params: str = ""
-    '''微博查询活动签到用的 params'''
+    '''是否开启微博功能'''
+    weibo: list = []
+    '''微博超话签到及兑换用的参数,适配多账号'''
     geetest_url: Optional[str]
     '''极验Geetest人机验证打码接口URL'''
     geetest_params: Optional[Dict[str, Any]] = None
     '''极验Geetest人机验证打码API发送的参数（除gt，challenge外）'''
     uuid: Optional[str] = None
     """用户UUID密钥，用于不同NoneBot适配器平台之间的数据同步，因此不可泄露"""
     qq_guild: Optional[Dict[str, int]] = {}
```

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/common.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/upgrade/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/configV2.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/upgrade/configV2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/dataV2.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/model/upgrade/dataV2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/common.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/utils/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 
 try:
     from loguru import Logger
 except ImportError:
     Logger = None
     pass
 
-from nonebot import Adapter, Bot, require
+from nonebot import Adapter, Bot
 
-require("nonebot_plugin_saa")
 from nonebot_plugin_saa import MessageSegmentFactory, Text, AggregatedMessageFactory, TargetQQPrivate, \
     TargetQQGuildDirect, enable_auto_select_bot
 
 from nonebot.adapters.onebot.v11 import MessageEvent as OneBotV11MessageEvent, PrivateMessageEvent, GroupMessageEvent, \
     Adapter as OneBotV11Adapter, Bot as OneBotV11Bot
 from nonebot.adapters.qq import DirectMessageCreateEvent, MessageCreateEvent, \
     Adapter as QQGuildAdapter, Bot as QQGuildBot, MessageEvent
@@ -233,14 +232,15 @@
         return f"{t},{r},{c}"
 
 
 async def get_validate(user: UserData, gt: str = None, challenge: str = None, retry: bool = True):
     """
     使用打码平台获取人机验证validate
 
+    :param user: 用户数据对象
     :param gt: 验证码gt
     :param challenge: challenge
     :param retry: 是否允许重试
     :return: 如果配置了平台URL，且 gt, challenge 不为空，返回 GeetestResult
     """
     if not plugin_config.preference.global_geetest:
         if not (gt and challenge) or not user.geetest_url:
@@ -254,30 +254,32 @@
         geetest_url = plugin_config.preference.geetest_url
         params = {"gt": gt, "challenge": challenge}
         params.update(plugin_config.preference.geetest_params)
     content = deepcopy(plugin_config.preference.geetest_json or Preference().geetest_json)
     for key, value in content.items():
         if isinstance(value, str):
             content[key] = value.format(gt=gt, challenge=challenge)
+    debug_log = {"geetest_url": geetest_url, "params": params, "content": content}
+    logger.debug(f"{plugin_config.preference.log_head}get_validate: {debug_log}")
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
                 async with httpx.AsyncClient() as client:
                     res = await client.post(
                         geetest_url,
                         params=params,
                         json=content,
                         timeout=60
                     )
                 geetest_data = res.json()
+                logger.debug(f"{plugin_config.preference.log_head}人机验证结果：{geetest_data}")
                 validate = geetest_data['data']['validate']
                 seccode = geetest_data['data'].get('seccode') or f"{validate}|jordan"
-                logger.debug(f"{plugin_config.preference.log_head}人机验证结果：{geetest_data}")
                 return GeetestResult(validate=validate, seccode=seccode)
-    except tenacity.RetryError as e:
+    except tenacity.RetryError:
         logger.exception(f"{plugin_config.preference.log_head}获取人机验证validate失败")
 
 
 def generate_seed_id(length: int = 8) -> str:
     """
     生成随机的 seed_id（即长度为8的十六进制数）
```

### Comparing `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/good_image.py` & `nonebot_plugin_mystool-2.5.0/src/nonebot_plugin_mystool/utils/good_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.4.0/PKG-INFO` & `nonebot_plugin_mystool-2.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mystool
-Version: 2.4.0
+Version: 2.5.0
 Summary: QQ聊天、频道机器人插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神崩铁便笺提醒
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs,qq-guild,star-rail,genshin-impact
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.asia
 Requires-Python: >=3.9,<4.0
@@ -44,14 +44,18 @@
 
 [![CodeFactor](https://www.codefactor.io/repository/github/ljzd-pro/nonebot-plugin-mystool/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/ljzd-pro/nonebot-plugin-mystool)
 [![最新发行版](https://img.shields.io/github/v/release/Ljzd-PRO/nonebot-plugin-mysTool?logo=python&style=for-the-badge)](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/releases/latest)
 [![最后提交](https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-plugin-mysTool/dev?style=for-the-badge)](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/commits/dev)
 
 # mysTool - 米游社辅助工具插件
 
+> [!Note]
+> 目前本项目基本不再新增功能，问题修复可能也会比较迟，主要是由于当前项目代码可维护性较差（\
+> 以及个人时间安排等。未来可能考虑彻底重做一次
+
 ## ⚡ 功能和特性
 
 - 支持QQ聊天和QQ频道
 - 短信验证登录，免抓包获取 Cookie
 - 自动完成每日米游币任务
 - 自动进行游戏签到
 - 可制定米游币商品兑换计划，到点兑换（因加入了人机验证，成功率较低）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mystool Version: 2.4.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mystool Version: 2.5.0 Summary:
 QQèå¤©ãé¢éæºå¨äººæä»¶ | ç±³æ¸¸ç¤¾å·¥å·-
 æ¯æ¥ç±³æ¸¸å¸ä»»å¡ãæ¸¸æç­¾å°ãåååæ¢ãåæåç»å½ãåç¥å´©éä¾¿ç¬ºæé
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs,qq-
 guild,star-rail,genshin-impact Author: Ljzd-PRO Author-email: ljzd@office.ljzd-
 pro.asia Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,17 @@
 www.codefactor.io/repository/github/ljzd-pro/nonebot-plugin-mystool/
 badge?style=for-the-badge)](https://www.codefactor.io/repository/github/ljzd-
 pro/nonebot-plugin-mystool) [![ææ°åè¡ç](https://img.shields.io/github/
 v/release/Ljzd-PRO/nonebot-plugin-mysTool?logo=python&style=for-the-badge)]
 (https://github.com/Ljzd-PRO/nonebot-plugin-mystool/releases/latest) [!
 [æåæäº¤](https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-
 plugin-mysTool/dev?style=for-the-badge)](https://github.com/Ljzd-PRO/nonebot-
-plugin-mystool/commits/dev) # mysTool - ç±³æ¸¸ç¤¾è¾å©å·¥å·æä»¶ ## â¡
+plugin-mystool/commits/dev) # mysTool - ç±³æ¸¸ç¤¾è¾å©å·¥å·æä»¶ > [!Note] >
+ç®åæ¬é¡¹ç®åºæ¬ä¸åæ°å¢åè½ï¼é®é¢ä¿®å¤å¯è½ä¹ä¼æ¯è¾è¿ï¼ä¸»è¦æ¯ç±äºå½åé¡¹ç®ä»£ç å¯ç»´æ¤æ§è¾å·®ï¼\
+> ä»¥åä¸ªäººæ¶é´å®æç­ãæªæ¥å¯è½èèå½»åºéåä¸æ¬¡ ## â¡
 åè½åç¹æ§ - æ¯æQQèå¤©åQQé¢é -
 ç­ä¿¡éªè¯ç»å½ï¼åæåè·å Cookie - èªå¨å®ææ¯æ¥ç±³æ¸¸å¸ä»»å¡
 - èªå¨è¿è¡æ¸¸æç­¾å° -
 å¯å¶å®ç±³æ¸¸å¸åååæ¢è®¡åï¼å°ç¹åæ¢ï¼å å å¥äºäººæºéªè¯ï¼æåçè¾ä½ï¼
 - å¯æ¯æå¤ä¸ª QQ è´¦å·ï¼æ¯ä¸ª QQ è´¦å·å¯ç»å®å¤ä¸ªç±³åæ¸¸è´¦æ· -
 QQ æ¨éæ§è¡ç»æéç¥ - åç¥ãå´©åï¼æç©¹ééç¶æä¾¿ç¬ºéç¥
 -
```

