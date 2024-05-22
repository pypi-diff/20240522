# Comparing `tmp/vnpy_datarecorder-1.0.6.tar.gz` & `tmp/vnpy_datarecorder-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_datarecorder-1.0.6.tar", last modified: Fri Sep  8 08:48:44 2023, max compression
+gzip compressed data, was "vnpy_datarecorder-1.0.7.tar", last modified: Wed May 22 10:42:20 2024, max compression
```

## Comparing `vnpy_datarecorder-1.0.6.tar` & `vnpy_datarecorder-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-09-08 08:48:44.766643 vnpy_datarecorder-1.0.6/
--rw-rw-rw-   0        0        0     1107 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     2033 2023-09-08 08:48:44.766643 vnpy_datarecorder-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2023-09-08 08:47:39.000000 vnpy_datarecorder-1.0.6/README.md
--rw-rw-rw-   0        0        0      986 2023-09-08 08:48:44.770315 vnpy_datarecorder-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-08 08:48:44.711047 vnpy_datarecorder-1.0.6/vnpy_datarecorder/
--rw-rw-rw-   0        0        0     1801 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder/__init__.py
--rw-rw-rw-   0        0        0    10483 2023-09-08 08:47:07.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder/engine.py
-drwxrwxrwx   0        0        0        0 2023-09-08 08:48:44.764614 vnpy_datarecorder-1.0.6/vnpy_datarecorder/ui/
--rw-rw-rw-   0        0        0       37 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder/ui/__init__.py
--rw-rw-rw-   0        0        0    67646 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder/ui/recorder.ico
--rw-rw-rw-   0        0        0     7085 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder/ui/widget.py
-drwxrwxrwx   0        0        0        0 2023-09-08 08:48:44.739183 vnpy_datarecorder-1.0.6/vnpy_datarecorder.egg-info/
--rw-rw-rw-   0        0        0     2033 2023-09-08 08:48:44.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-09-08 08:48:44.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-08 08:48:44.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-09-08 08:48:44.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-09-08 08:48:44.000000 vnpy_datarecorder-1.0.6/vnpy_datarecorder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 10:42:20.892306 vnpy_datarecorder-1.0.7/
+-rw-rw-rw-   0        0        0     1107 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2035 2024-05-22 10:42:20.892306 vnpy_datarecorder-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1108 2024-05-22 10:40:07.000000 vnpy_datarecorder-1.0.7/README.md
+-rw-rw-rw-   0        0        0      986 2024-05-22 10:42:20.900121 vnpy_datarecorder-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:42:20.844458 vnpy_datarecorder-1.0.7/vnpy_datarecorder/
+-rw-rw-rw-   0        0        0     1801 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder/__init__.py
+-rw-rw-rw-   0        0        0    10528 2024-05-22 10:41:05.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder/engine.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:42:20.891260 vnpy_datarecorder-1.0.7/vnpy_datarecorder/ui/
+-rw-rw-rw-   0        0        0       37 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder/ui/__init__.py
+-rw-rw-rw-   0        0        0    67646 2023-09-04 01:00:56.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder/ui/recorder.ico
+-rw-rw-rw-   0        0        0     7058 2024-05-22 10:40:43.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder/ui/widget.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:42:20.884482 vnpy_datarecorder-1.0.7/vnpy_datarecorder.egg-info/
+-rw-rw-rw-   0        0        0     2035 2024-05-22 10:42:20.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-05-22 10:42:20.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 10:42:20.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-22 10:42:20.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2024-05-22 10:42:20.000000 vnpy_datarecorder-1.0.7/vnpy_datarecorder.egg-info/top_level.txt
```

### Comparing `vnpy_datarecorder-1.0.6/LICENSE` & `vnpy_datarecorder-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_datarecorder-1.0.6/PKG-INFO` & `vnpy_datarecorder-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_datarecorder
-Version: 1.0.6
+Version: 1.0.7
 Summary: Data recorder application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,29 +23,29 @@
 # VeighNa框架的行情录制模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.6-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.7-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 DataRecorder是用于实时行情记录的模块，用户可以利用该模块记录实时Tick数据和K线数据，并自动写入保存到数据库中。
 
 记录的数据可以通过DataManager模块查看，也可以用于CtaBacktester的历史回测，以及CtaStrategy、PortfolioStrategy等策略的实盘初始化。
 
 ## 安装
 
-安装环境推荐基于3.7.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
+安装环境推荐基于3.9.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
 
 直接使用pip命令：
 
 ```
 pip install vnpy_datarecorder
 ```
```

### Comparing `vnpy_datarecorder-1.0.6/README.md` & `vnpy_datarecorder-1.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # VeighNa框架的行情录制模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.6-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.7-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 DataRecorder是用于实时行情记录的模块，用户可以利用该模块记录实时Tick数据和K线数据，并自动写入保存到数据库中。
 
 记录的数据可以通过DataManager模块查看，也可以用于CtaBacktester的历史回测，以及CtaStrategy、PortfolioStrategy等策略的实盘初始化。
 
 ## 安装
 
-安装环境推荐基于3.7.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
+安装环境推荐基于3.9.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
 
 直接使用pip命令：
 
 ```
 pip install vnpy_datarecorder
 ```
```

### Comparing `vnpy_datarecorder-1.0.6/setup.cfg` & `vnpy_datarecorder-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 6461 7461 7265 636f   = vnpy_datareco
 00000020: 7264 6572 0d0a 7665 7273 696f 6e20 3d20  rder..version = 
-00000030: 312e 302e 360d 0a75 726c 203d 2068 7474  1.0.6..url = htt
+00000030: 312e 302e 370d 0a75 726c 203d 2068 7474  1.0.7..url = htt
 00000040: 7073 3a2f 2f77 7777 2e76 6e70 792e 636f  ps://www.vnpy.co
 00000050: 6d0d 0a6c 6963 656e 7365 203d 204d 4954  m..license = MIT
 00000060: 0d0a 6175 7468 6f72 203d 2058 6961 6f79  ..author = Xiaoy
 00000070: 6f75 2043 6865 6e0d 0a61 7574 686f 725f  ou Chen..author_
 00000080: 656d 6169 6c20 3d20 7869 616f 796f 752e  email = xiaoyou.
 00000090: 6368 656e 406d 6169 6c2e 766e 7079 2e63  chen@mail.vnpy.c
 000000a0: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description
```

### Comparing `vnpy_datarecorder-1.0.6/vnpy_datarecorder/__init__.py` & `vnpy_datarecorder-1.0.7/vnpy_datarecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_datarecorder-1.0.6/vnpy_datarecorder/engine.py` & `vnpy_datarecorder-1.0.7/vnpy_datarecorder/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import sys
+import traceback
 from threading import Thread
 from queue import Queue, Empty
 from copy import copy
 from collections import defaultdict
-from typing import Any, Dict, List, Optional
+from typing import Optional
 from datetime import datetime, timedelta
 
 from vnpy.event import Event, EventEngine
 from vnpy.trader.engine import BaseEngine, MainEngine
 from vnpy.trader.constant import Exchange
 from vnpy.trader.object import (
     SubscribeRequest,
@@ -39,23 +39,23 @@
         """"""
         super().__init__(main_engine, event_engine, APP_NAME)
 
         self.queue: Queue = Queue()
         self.thread: Thread = Thread(target=self.run)
         self.active: bool = False
 
-        self.tick_recordings: Dict[str, Dict] = {}
-        self.bar_recordings: Dict[str, Dict] = {}
-        self.bar_generators: Dict[str, BarGenerator] = {}
+        self.tick_recordings: dict[str, dict] = {}
+        self.bar_recordings: dict[str, dict] = {}
+        self.bar_generators: dict[str, BarGenerator] = {}
 
         self.timer_count: int = 0
         self.timer_interval: int = 10
 
-        self.ticks: Dict[str, List[TickData]] = defaultdict(list)
-        self.bars: Dict[str, List[BarData]] = defaultdict(list)
+        self.ticks: dict[str, list[TickData]] = defaultdict(list)
+        self.bars: dict[str, list[BarData]] = defaultdict(list)
 
         self.filter_dt: datetime = datetime.now(DB_TZ)      # Tick数据过滤的时间戳
         self.filter_window: int = 60                        # Tick数据过滤的时间窗口，默认60秒
         self.filter_delta: timedelta = None                 # Tick数据过滤的时间偏差对象
 
         self.database: BaseDatabase = get_database()
 
@@ -81,29 +81,29 @@
         }
         save_json(self.setting_filename, setting)
 
     def run(self) -> None:
         """"""
         while self.active:
             try:
-                task: Any = self.queue.get(timeout=1)
+                task: object = self.queue.get(timeout=1)
                 task_type, data = task
 
                 if task_type == "tick":
                     self.database.save_tick_data(data, stream=True)
                 elif task_type == "bar":
                     self.database.save_bar_data(data, stream=True)
 
             except Empty:
                 continue
 
             except Exception:
                 self.active = False
 
-                info = sys.exc_info()
+                info = traceback.format_exc()
                 event: Event = Event(EVENT_RECORDER_EXCEPTION, info)
                 self.event_engine.put(event)
 
     def close(self) -> None:
         """"""
         self.active = False
 
@@ -255,14 +255,15 @@
             datetime=spread_item.datetime,
             name=spread_item.name,
             last_price=(spread_item.bid_price + spread_item.ask_price) / 2,
             bid_price_1=spread_item.bid_price,
             ask_price_1=spread_item.ask_price,
             bid_volume_1=spread_item.bid_volume,
             ask_volume_1=spread_item.ask_volume,
+            localtime=spread_item.datetime,
             gateway_name="SPREAD"
         )
 
         # Filter not inited spread data
         if tick.datetime:
             self.update_tick(tick)
 
@@ -272,18 +273,18 @@
             EVENT_RECORDER_LOG,
             msg
         )
         self.event_engine.put(event)
 
     def put_event(self) -> None:
         """"""
-        tick_symbols: List[str] = list(self.tick_recordings.keys())
+        tick_symbols: list[str] = list(self.tick_recordings.keys())
         tick_symbols.sort()
 
-        bar_symbols: List[str] = list(self.bar_recordings.keys())
+        bar_symbols: list[str] = list(self.bar_recordings.keys())
         bar_symbols.sort()
 
         data: dict = {
             "tick": tick_symbols,
             "bar": bar_symbols
         }
```

### Comparing `vnpy_datarecorder-1.0.6/vnpy_datarecorder/ui/recorder.ico` & `vnpy_datarecorder-1.0.7/vnpy_datarecorder/ui/recorder.ico`

 * *Files identical despite different names*

### Comparing `vnpy_datarecorder-1.0.6/vnpy_datarecorder/ui/widget.py` & `vnpy_datarecorder-1.0.7/vnpy_datarecorder/ui/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from datetime import datetime
-from typing import Any, List
 
 from vnpy.event import Event, EventEngine
 from vnpy.trader.engine import MainEngine
 from vnpy.trader.ui import QtCore, QtWidgets
 from vnpy.trader.event import EVENT_CONTRACT
 from vnpy.trader.object import ContractData
 
@@ -46,15 +45,15 @@
         self.interval_spin: QtWidgets.QSpinBox = QtWidgets.QSpinBox()
         self.interval_spin.setMinimum(1)
         self.interval_spin.setMaximum(60)
         self.interval_spin.setValue(self.recorder_engine.timer_interval)
         self.interval_spin.setSuffix("秒")
         self.interval_spin.valueChanged.connect(self.set_interval)
 
-        contracts: List[ContractData] = self.main_engine.get_all_contracts()
+        contracts: list[ContractData] = self.main_engine.get_all_contracts()
         self.vt_symbols: list = [contract.vt_symbol for contract in contracts]
 
         self.symbol_completer: QtWidgets.QCompleter = QtWidgets.QCompleter(self.vt_symbols)
         self.symbol_completer.setFilterMode(QtCore.Qt.MatchContains)
         self.symbol_completer.setCompletionMode(
             self.symbol_completer.PopupCompletion)
         self.symbol_line.setCompleter(self.symbol_completer)
@@ -129,15 +128,15 @@
         """"""
         timestamp: str = datetime.now().strftime("%H:%M:%S")
         msg: str = f"{timestamp}\t{event.data}"
         self.log_edit.append(msg)
 
     def process_update_event(self, event: Event) -> None:
         """"""
-        data: Any = event.data
+        data: object = event.data
 
         self.bar_recording_edit.clear()
         bar_text: str = "\n".join(data["bar"])
         self.bar_recording_edit.setText(bar_text)
 
         self.tick_recording_edit.clear()
         tick_text: str = "\n".join(data["tick"])
```

### Comparing `vnpy_datarecorder-1.0.6/vnpy_datarecorder.egg-info/PKG-INFO` & `vnpy_datarecorder-1.0.7/vnpy_datarecorder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-datarecorder
-Version: 1.0.6
+Version: 1.0.7
 Summary: Data recorder application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,29 +23,29 @@
 # VeighNa框架的行情录制模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.6-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.7-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 DataRecorder是用于实时行情记录的模块，用户可以利用该模块记录实时Tick数据和K线数据，并自动写入保存到数据库中。
 
 记录的数据可以通过DataManager模块查看，也可以用于CtaBacktester的历史回测，以及CtaStrategy、PortfolioStrategy等策略的实盘初始化。
 
 ## 安装
 
-安装环境推荐基于3.7.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
+安装环境推荐基于3.9.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
 
 直接使用pip命令：
 
 ```
 pip install vnpy_datarecorder
 ```
```

