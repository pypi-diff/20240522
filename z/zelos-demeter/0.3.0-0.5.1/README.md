# Comparing `tmp/zelos-demeter-0.3.0.tar.gz` & `tmp/zelos-demeter-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zelos-demeter-0.3.0.tar", last modified: Thu Nov  2 11:21:39 2023, max compression
+gzip compressed data, was "zelos-demeter-0.5.1.tar", last modified: Wed May 22 04:43:18 2024, max compression
```

## Comparing `zelos-demeter-0.3.0.tar` & `zelos-demeter-0.5.1.tar`

### file list

```diff
@@ -1,52 +1,62 @@
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.277221 zelos-demeter-0.3.0/
--rw-r--r--   0 florije    (501) staff       (20)     1063 2023-07-17 01:38:36.000000 zelos-demeter-0.3.0/LICENSE
--rw-r--r--   0 florije    (501) staff       (20)      648 2023-11-02 11:21:39.277387 zelos-demeter-0.3.0/PKG-INFO
--rw-r--r--   0 florije    (501) staff       (20)      349 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/README.md
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.247552 zelos-demeter-0.3.0/demeter/
--rw-r--r--   0 florije    (501) staff       (20)      620 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)     3502 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/_typing.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.253415 zelos-demeter-0.3.0/demeter/aave/
--rw-r--r--   0 florije    (501) staff       (20)      611 2023-11-02 11:07:08.000000 zelos-demeter-0.3.0/demeter/aave/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)    17937 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/aave/_typing.py
--rw-r--r--   0 florije    (501) staff       (20)     9311 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/aave/core.py
--rw-r--r--   0 florije    (501) staff       (20)     2065 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/aave/helper.py
--rw-r--r--   0 florije    (501) staff       (20)    50418 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/aave/market.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.255685 zelos-demeter-0.3.0/demeter/broker/
--rw-r--r--   0 florije    (501) staff       (20)      375 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/broker/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)    11119 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/broker/_typing.py
--rw-r--r--   0 florije    (501) staff       (20)     8022 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/broker/broker.py
--rw-r--r--   0 florije    (501) staff       (20)     4900 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/broker/market.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.259949 zelos-demeter-0.3.0/demeter/core/
--rw-r--r--   0 florije    (501) staff       (20)      107 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/core/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)    21292 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/core/actuator.py
--rw-r--r--   0 florije    (501) staff       (20)     6009 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/core/evaluating_indicator.py
--rw-r--r--   0 florije    (501) staff       (20)     3612 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/core/math_helper.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.263706 zelos-demeter-0.3.0/demeter/indicator/
--rw-r--r--   0 florije    (501) staff       (20)      200 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/indicator/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)     1180 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/indicator/common.py
--rw-r--r--   0 florije    (501) staff       (20)     2010 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/indicator/ma.py
--rw-r--r--   0 florije    (501) staff       (20)     1673 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/indicator/volatility.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.265557 zelos-demeter-0.3.0/demeter/strategy/
--rw-r--r--   0 florije    (501) staff       (20)      284 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/strategy/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)     2982 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/strategy/strategy.py
--rw-r--r--   0 florije    (501) staff       (20)     8319 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/strategy/trigger.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.269314 zelos-demeter-0.3.0/demeter/uniswap/
--rw-r--r--   0 florije    (501) staff       (20)      465 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/uniswap/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)    16442 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/uniswap/_typing.py
--rw-r--r--   0 florije    (501) staff       (20)     5095 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/uniswap/core.py
--rw-r--r--   0 florije    (501) staff       (20)     6510 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/uniswap/data.py
--rw-r--r--   0 florije    (501) staff       (20)     7854 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/uniswap/helper.py
--rw-r--r--   0 florije    (501) staff       (20)     7269 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/uniswap/liquitidy_math.py
--rw-r--r--   0 florije    (501) staff       (20)    34348 2023-11-02 11:07:08.000000 zelos-demeter-0.3.0/demeter/uniswap/market.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.271905 zelos-demeter-0.3.0/demeter/utils/
--rw-r--r--   0 florije    (501) staff       (20)      265 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/utils/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)     2154 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/utils/application.py
--rw-r--r--   0 florije    (501) staff       (20)     3461 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/demeter/utils/console_text.py
--rw-r--r--   0 florije    (501) staff       (20)       38 2023-11-02 11:21:39.278340 zelos-demeter-0.3.0/setup.cfg
--rw-r--r--   0 florije    (501) staff       (20)      899 2023-11-02 10:44:16.000000 zelos-demeter-0.3.0/setup.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2023-11-02 11:21:39.276158 zelos-demeter-0.3.0/zelos_demeter.egg-info/
--rw-r--r--   0 florije    (501) staff       (20)      648 2023-11-02 11:21:39.000000 zelos-demeter-0.3.0/zelos_demeter.egg-info/PKG-INFO
--rw-r--r--   0 florije    (501) staff       (20)     1067 2023-11-02 11:21:39.000000 zelos-demeter-0.3.0/zelos_demeter.egg-info/SOURCES.txt
--rw-r--r--   0 florije    (501) staff       (20)        1 2023-11-02 11:21:39.000000 zelos-demeter-0.3.0/zelos_demeter.egg-info/dependency_links.txt
--rw-r--r--   0 florije    (501) staff       (20)       57 2023-11-02 11:21:39.000000 zelos-demeter-0.3.0/zelos_demeter.egg-info/requires.txt
--rw-r--r--   0 florije    (501) staff       (20)        8 2023-11-02 11:21:39.000000 zelos-demeter-0.3.0/zelos_demeter.egg-info/top_level.txt
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.778192 zelos-demeter-0.5.1/
+-rw-r--r--   0 florije    (501) staff       (20)     1063 2022-11-03 09:30:12.000000 zelos-demeter-0.5.1/LICENSE
+-rw-r--r--   0 florije    (501) staff       (20)     4191 2024-05-22 04:43:18.778583 zelos-demeter-0.5.1/PKG-INFO
+-rw-r--r--   0 florije    (501) staff       (20)     3872 2023-12-28 05:10:47.000000 zelos-demeter-0.5.1/README.md
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.582463 zelos-demeter-0.5.1/demeter/
+-rw-r--r--   0 florije    (501) staff       (20)      732 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)     3332 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/_typing.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.590285 zelos-demeter-0.5.1/demeter/aave/
+-rw-r--r--   0 florije    (501) staff       (20)      611 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/aave/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)    18088 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/aave/_typing.py
+-rw-r--r--   0 florije    (501) staff       (20)     9311 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/aave/core.py
+-rw-r--r--   0 florije    (501) staff       (20)     2065 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/aave/helper.py
+-rw-r--r--   0 florije    (501) staff       (20)    51408 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/aave/market.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.596683 zelos-demeter-0.5.1/demeter/broker/
+-rw-r--r--   0 florije    (501) staff       (20)      402 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/broker/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)    11737 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/broker/_typing.py
+-rw-r--r--   0 florije    (501) staff       (20)     8090 2024-05-22 04:07:47.000000 zelos-demeter-0.5.1/demeter/broker/broker.py
+-rw-r--r--   0 florije    (501) staff       (20)     5599 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/broker/market.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.608929 zelos-demeter-0.5.1/demeter/core/
+-rw-r--r--   0 florije    (501) staff       (20)      107 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/core/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)    22045 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/core/actuator.py
+-rw-r--r--   0 florije    (501) staff       (20)     7611 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/core/evaluating_indicator.py
+-rw-r--r--   0 florije    (501) staff       (20)     3612 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/core/math_helper.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.620749 zelos-demeter-0.5.1/demeter/deribit/
+-rw-r--r--   0 florije    (501) staff       (20)      279 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/deribit/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)    10275 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/deribit/_typing.py
+-rw-r--r--   0 florije    (501) staff       (20)     2174 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/deribit/helper.py
+-rw-r--r--   0 florije    (501) staff       (20)    23578 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/deribit/market.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.674881 zelos-demeter-0.5.1/demeter/indicator/
+-rw-r--r--   0 florije    (501) staff       (20)      200 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/indicator/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)     1180 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/indicator/common.py
+-rw-r--r--   0 florije    (501) staff       (20)     1932 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/indicator/ma.py
+-rw-r--r--   0 florije    (501) staff       (20)     1673 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/indicator/volatility.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.680760 zelos-demeter-0.5.1/demeter/squeeth/
+-rw-r--r--   0 florije    (501) staff       (20)      299 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/squeeth/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)     7127 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/squeeth/_typing.py
+-rw-r--r--   0 florije    (501) staff       (20)     1224 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/squeeth/helper.py
+-rw-r--r--   0 florije    (501) staff       (20)    35381 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/squeeth/market.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.685509 zelos-demeter-0.5.1/demeter/strategy/
+-rw-r--r--   0 florije    (501) staff       (20)      284 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/strategy/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)     2947 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/strategy/strategy.py
+-rw-r--r--   0 florije    (501) staff       (20)     8319 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/strategy/trigger.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.732396 zelos-demeter-0.5.1/demeter/uniswap/
+-rw-r--r--   0 florije    (501) staff       (20)      465 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/uniswap/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)    17769 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/uniswap/_typing.py
+-rw-r--r--   0 florije    (501) staff       (20)     5248 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/uniswap/core.py
+-rw-r--r--   0 florije    (501) staff       (20)     6724 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/uniswap/data.py
+-rw-r--r--   0 florije    (501) staff       (20)     8649 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/uniswap/helper.py
+-rw-r--r--   0 florije    (501) staff       (20)     7269 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/uniswap/liquitidy_math.py
+-rw-r--r--   0 florije    (501) staff       (20)    37817 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/uniswap/market.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.743611 zelos-demeter-0.5.1/demeter/utils/
+-rw-r--r--   0 florije    (501) staff       (20)      265 2023-11-10 00:30:05.000000 zelos-demeter-0.5.1/demeter/utils/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)     2159 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/utils/application.py
+-rw-r--r--   0 florije    (501) staff       (20)     4285 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/demeter/utils/console_text.py
+-rw-r--r--   0 florije    (501) staff       (20)       38 2024-05-22 04:43:18.782610 zelos-demeter-0.5.1/setup.cfg
+-rw-r--r--   0 florije    (501) staff       (20)      986 2024-05-22 04:07:33.000000 zelos-demeter-0.5.1/setup.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2024-05-22 04:43:18.776376 zelos-demeter-0.5.1/zelos_demeter.egg-info/
+-rw-r--r--   0 florije    (501) staff       (20)     4191 2024-05-22 04:43:18.000000 zelos-demeter-0.5.1/zelos_demeter.egg-info/PKG-INFO
+-rw-r--r--   0 florije    (501) staff       (20)     1281 2024-05-22 04:43:18.000000 zelos-demeter-0.5.1/zelos_demeter.egg-info/SOURCES.txt
+-rw-r--r--   0 florije    (501) staff       (20)        1 2024-05-22 04:43:18.000000 zelos-demeter-0.5.1/zelos_demeter.egg-info/dependency_links.txt
+-rw-r--r--   0 florije    (501) staff       (20)      127 2024-05-22 04:43:18.000000 zelos-demeter-0.5.1/zelos_demeter.egg-info/requires.txt
+-rw-r--r--   0 florije    (501) staff       (20)        8 2024-05-22 04:43:18.000000 zelos-demeter-0.5.1/zelos_demeter.egg-info/top_level.txt
```

### Comparing `zelos-demeter-0.3.0/LICENSE` & `zelos-demeter-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.3.0/demeter/_typing.py` & `zelos-demeter-0.5.1/demeter/_typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from decimal import Decimal
 from enum import Enum
 
 
+class Formats:
+    # follow the document here: https://python-reference.readthedocs.io/en/latest/docs/functions/format.html
+    global_num_format: str = ".8g"
+
+
 # constant value for number 1
 DECIMAL_0 = Decimal(0)
 
 # constant value for number 0
 DECIMAL_1 = Decimal(1)
 
 
@@ -29,38 +34,33 @@
 
     It's inherit from Decimal, but considering performance issues, calculate function is not override,
     so if you do calculate on this object, return type will be Decimal
 
     :param number: number to keep
     :type number: Decimal
     :param unit: unit of the number, e.g. eth
-    :type _unit: str
-    :param output_format: output format, follow the document here: https://python-reference.readthedocs.io/en/latest/docs/functions/format.html
-    :type output_format: str
+    :type unit: str
     """
 
     __integral = Decimal(1)
 
-    default_output_format = ".8g"
-
-    def __new__(cls, value, unit: str = "", output_format=None):
+    def __new__(cls, value, unit: str = ""):
         obj = Decimal.__new__(cls, value)
         obj._unit = unit
-        obj.output_format = output_format if output_format is not None else UnitDecimal.default_output_format
         return obj
 
     def to_str(self):
         """
         Get formatted string like "12.34 eth". Decimal format is predefined by self.output_format attribute
 
         :return: formatted string
         :rtype: str
         """
         dec = self.quantize(DECIMAL_1) if (self == self.to_integral() and self < 1e29) else self.normalize()
-        return "{:{}} {}".format(dec, self.output_format, self._unit)
+        return "{:{}} {}".format(dec, Formats.global_num_format, self._unit)
 
     @property
     def unit(self):
         return self._unit
 
     @unit.setter
     def unit(self, value):
@@ -133,14 +133,15 @@
         self.message = message
 
 
 class ChainType(str, Enum):
     """
     Enum for chains
     """
+
     ethereum = "ethereum"
     polygon = "polygon"
     optimism = "optimism"
     arbitrum = "arbitrum"
     celo = "celo"
     bsc = "bsc"
     base = "base"
```

### Comparing `zelos-demeter-0.3.0/demeter/aave/__init__.py` & `zelos-demeter-0.5.1/demeter/aave/__init__.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.3.0/demeter/aave/_typing.py` & `zelos-demeter-0.5.1/demeter/aave/_typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Dict, NamedTuple, Union
 from typing import TypeVar
 
 import pandas as pd
 
 from .. import TokenInfo, UnitDecimal
 from ..broker import MarketBalance, MarketStatus, BaseAction, ActionTypeEnum
+from ..utils import console_text
 
 T = TypeVar("T")
 K = TypeVar("K")
 
 
 class InterestRateMode(Enum):
     """
@@ -151,19 +152,19 @@
         "collateral": [],
         "amount": [],
         "apy": [],
         "value": [],
     }
     for k, v in supplies.items():
         pos_dict["token"].append(v.token.name)
-        pos_dict["base_amount"].append(v.base_amount)
+        pos_dict["base_amount"].append(console_text.format_value(v.base_amount))
         pos_dict["collateral"].append(v.collateral)
-        pos_dict["amount"].append(v.amount)
-        pos_dict["apy"].append(v.apy)
-        pos_dict["value"].append(v.value)
+        pos_dict["amount"].append(console_text.format_value(v.amount))
+        pos_dict["apy"].append(console_text.format_value(v.apy))
+        pos_dict["value"].append((console_text.format_value(v.value)))
     return pd.DataFrame(pos_dict)
 
 
 @dataclass
 class BorrowInfo:
     """
     Basic info for borrow, designed to kept properties inside market
@@ -213,26 +214,26 @@
     """
     convert borrow dict to a dataframe
 
     """
     pos_dict = {
         "token": [],
         "base_amount": [],
-        "interest_rate_mode": [],
+        "mode": [],
         "amount": [],
         "apy": [],
         "value": [],
     }
     for k, v in supplies.items():
         pos_dict["token"].append(v.token.name)
-        pos_dict["base_amount"].append(v.base_amount)
-        pos_dict["interest_rate_mode"].append(v.interest_rate_mode.name)
-        pos_dict["amount"].append(v.amount)
-        pos_dict["apy"].append(v.apy)
-        pos_dict["value"].append(v.value)
+        pos_dict["base_amount"].append(console_text.format_value(v.base_amount))
+        pos_dict["mode"].append(v.interest_rate_mode.name)
+        pos_dict["amount"].append(console_text.format_value(v.amount))
+        pos_dict["apy"].append(console_text.format_value(v.apy))
+        pos_dict["value"].append(console_text.format_value(v.value))
     return pd.DataFrame(pos_dict)
 
 
 @dataclass
 class AaveBalance(MarketBalance):
     """
     Asset or position value in aave market.
@@ -355,24 +356,24 @@
 
 @dataclass
 class SupplyAction(BaseAction):
     """
     Describe parameters and results of supply transaction
 
     :param token: which token is supplied
-    :type token: TokenInfo
+    :type token: str
     :param amount: amount supplied
     :type amount: UnitDecimal
     :param collateral: collateral the supply or not.
     :type collateral: bool
     :param deposit_after: total supply amount of this token after supply
     :type deposit_after: UnitDecimal
     """
 
-    token: TokenInfo
+    token: str
     """which token is supplied"""
     amount: UnitDecimal
     """amount supplied"""
     collateral: bool
     """collateral the supply or not."""
     deposit_after: UnitDecimal
     """total supply amount of this token after supply"""
@@ -383,22 +384,22 @@
 
 @dataclass
 class WithdrawAction(BaseAction):
     """
     Describe parameters and results of withdraw transaction
 
     :param token: which token is supplied
-    :type token: TokenInfo
+    :type token: str
     :param amount: amount supplied
     :type amount: UnitDecimal
     :param deposit_after: total supply amount of this token after withdraw
     :type deposit_after: UnitDecimal
     """
 
-    token: TokenInfo
+    token: str
     """which token is supplied"""
     amount: UnitDecimal
     """amount supplied"""
     deposit_after: UnitDecimal
     """total supply amount of this token after withdraw"""
 
     def set_type(self):
@@ -407,24 +408,24 @@
 
 @dataclass
 class BorrowAction(BaseAction):
     """
     Describe parameters and results of borrow transaction
 
     :param token: which token is borrowed
-    :type token: TokenInfo
+    :type token: str
     :param interest_rate_mode: interest rate mode
     :type interest_rate_mode: InterestRateMode
     :param amount: amount borrowed
     :type amount: UnitDecimal
     :param debt_after: total borrow amount of this token after borrow transaction
     :type debt_after: UnitDecimal
     """
 
-    token: TokenInfo
+    token: str
     """which token is borrowed"""
     interest_rate_mode: InterestRateMode
     """interest rate mode"""
     amount: UnitDecimal
     """amount borrowed"""
     debt_after: UnitDecimal
     """total borrow amount of this token after borrow transaction"""
@@ -435,24 +436,24 @@
 
 @dataclass
 class RepayAction(BaseAction):
     """
     Describe parameters and results of RepayAction transaction
 
     :param token: which token is borrowed
-    :type token: TokenInfo
+    :type token: str
     :param interest_rate_mode: interest rate mode
     :type interest_rate_mode: InterestRateMode
     :param amount: amount repaid
     :type amount: UnitDecimal
     :param debt_after: total borrow amount of this token after repay transaction
     :type debt_after: UnitDecimal
     """
 
-    token: TokenInfo
+    token: str
     """which token is borrowed"""
     interest_rate_mode: InterestRateMode
     """interest rate mode"""
     amount: UnitDecimal
     """amount repaid"""
     debt_after: UnitDecimal
     """total borrow amount of this token after repay transaction"""
@@ -463,17 +464,17 @@
 
 @dataclass
 class LiquidationAction(BaseAction):
     """
     Describe parameters and results of a liquidation
 
     :param collateral_token: which collateral token is used in liquidation
-    :type collateral_token: TokenInfo
+    :type collateral_token: str
     :param debt_token:  which debt token is used in liquidation
-    :type debt_token: TokenInfo
+    :type debt_token: str
     :param delt_to_cover: Debt amount to be liquidated, should be equal to variable_delt_liquidated+stable_delt_liquidated
     :type delt_to_cover: UnitDecimal
     :param collateral_used: Collateral amount to subtract in liquidation
     :type collateral_used: UnitDecimal
     :param variable_delt_liquidated: liquidated debt token amount in variable delt
     :type variable_delt_liquidated: UnitDecimal
     :param stable_delt_liquidated: liquidated debt token amount in stable delt
@@ -486,17 +487,17 @@
     :type collateral_after: UnitDecimal
     :param variable_debt_after: variable debt token amount after liquidation
     :type variable_debt_after: UnitDecimal
     :param stable_delt_after: stable delt token amount after liquidation
     :type stable_delt_after: UnitDecimal
     """
 
-    collateral_token: TokenInfo
+    collateral_token: str
     """which collateral token is used in liquidation"""
-    debt_token: TokenInfo
+    debt_token: str
     """which debt token is used in liquidation"""
     delt_to_cover: UnitDecimal
     """Debt amount to be liquidated, should be equal to variable_delt_liquidated+stable_delt_liquidated"""
     collateral_used: UnitDecimal
     """Collateral amount to subtract in liquidation"""
     variable_delt_liquidated: UnitDecimal
     """liquidated debt token amount in variable delt"""
```

### Comparing `zelos-demeter-0.3.0/demeter/aave/core.py` & `zelos-demeter-0.5.1/demeter/aave/core.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.3.0/demeter/aave/helper.py` & `zelos-demeter-0.5.1/demeter/aave/helper.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.3.0/demeter/aave/market.py` & `zelos-demeter-0.5.1/demeter/aave/market.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     DictCache,
     AaveMarketDescription,
     AaveMarketStatus,
 )
 from .core import AaveV3CoreLib
 from .. import DemeterError, TokenInfo
 from .._typing import DECIMAL_0, UnitDecimal, ChainType
-from ..broker import Market, MarketInfo
-from ..utils import get_formatted_predefined, STYLE, get_formatted_from_dict
+from ..broker import Market, MarketInfo, write_func
+from ..utils import get_formatted_predefined, STYLE, get_formatted_from_dict, console_text
 from ..utils.application import require, float_param_formatter, to_decimal
 
 DEFAULT_DATA_PATH = "./data"
 
 
 class AaveV3Market(Market):
     """
@@ -65,15 +65,17 @@
         data_path: str = DEFAULT_DATA_PATH,
     ):
         super().__init__(market_info=market_info, data_path=data_path, data=data)
         tokens = tokens if token is not None else []  # just to set an initial value
         self._supplies: Dict[SupplyKey, SupplyInfo] = {}
         self._borrows: Dict[BorrowKey, BorrowInfo] = {}
 
-        self._risk_parameters: pd.DataFrame | Dict[str, RiskParameter] = helper.load_risk_parameter(risk_parameters_path)
+        self._risk_parameters: pd.DataFrame | Dict[str, RiskParameter] = helper.load_risk_parameter(
+            risk_parameters_path
+        )
 
         # caches, since amounts and values are calculated by base_amount, and they are commonly used, cache is introduced to speed up back test.
         # when base amount or price has changed, they must be reset.
         # Maybe I'm just bring trouble on oneself
         self._collaterals_amount_cache = DictCache()
         self._supplies_amount_cache = DictCache()
         self._supplies_cache = DictCache()
@@ -95,15 +97,17 @@
     def __str__(self):
         return json.dumps(self.description()._asdict())
 
     def description(self):
         """
         Get a brief description of this market
         """
-        return AaveMarketDescription(type(self).__name__, self._market_info.name, len(self._supplies), len(self._borrows))
+        return AaveMarketDescription(
+            type(self).__name__, self._market_info.name, len(self._supplies), len(self._borrows)
+        )
 
     @property
     def data(self) -> pd.DataFrame:
         """
         | Get data attribute. data have multiple column index.
         | Columns are organized by token, like this:
 
@@ -166,15 +170,15 @@
         :type token_info: TokenInfo
         :param token_data: data
         :type token_data: DataFrame
         """
         if self._data is not None and token_info.name in self._data:
             raise DemeterError(f"{token_info.name} has already set to data")
         if isinstance(token_data, pd.DataFrame):
-            token_data = token_data.applymap(to_decimal)
+            token_data = token_data.map(to_decimal)
             token_data.columns = pd.MultiIndex.from_tuples([(token_info.name, c) for c in token_data.columns])
             self._data = pd.concat([self._data, token_data], axis="columns")
         else:
             raise ValueError()
 
     def load_data(self, chain: ChainType, token_info_list: List[TokenInfo], start_date: date, end_date: date):
         """
@@ -197,15 +201,17 @@
                 raise DemeterError(f"address of {token_info.name} not set")
             while day <= end_date:
                 path = os.path.join(
                     self.data_path,
                     f"{chain.name.lower()}-aave_v3-{token_info.address}-{day.strftime('%Y-%m-%d')}.minute.csv",
                 )
                 if not os.path.exists(path):
-                    raise IOError(f"resource file {path} not found, please download with demeter-fetch: https://github.com/zelos-alpha/demeter-fetch")
+                    raise IOError(
+                        f"resource file {path} not found, please download with demeter-fetch: https://github.com/zelos-alpha/demeter-fetch"
+                    )
                 csv_converters = {n: to_decimal for n in AaveV3Market.REQUIRED_DATA_COLUMN}
                 day_df = pd.read_csv(
                     path,
                     converters=csv_converters,
                     index_col=0,
                     parse_dates=True,
                 )
@@ -275,15 +281,17 @@
         :return: value of all borrows
         :rtype: Dict[BorrowKey, Decimal]
         """
         if self._borrows_amount_cache.empty:
             for k, v in self._borrows.items():
                 self._borrows_amount_cache.set(
                     k,
-                    AaveV3CoreLib.get_amount(v.base_amount, self._market_status.data[k.token.name].variable_borrow_index)
+                    AaveV3CoreLib.get_amount(
+                        v.base_amount, self._market_status.data[k.token.name].variable_borrow_index
+                    )
                     * self._price_status[k.token.name],
                 )
         return self._borrows_amount_cache.value
 
     @property
     def total_borrows_value(self) -> Decimal:
         """
@@ -348,28 +356,25 @@
         Set up pool status of this moment, such as liquidity index, supply/borrow rate, and price
 
         :param data: market status
         :type data: AaveMarketStatus
         :param price: current price of tokens involved
         :type price: Series
         """
+        super().set_market_status(data, price)
         if data.data is None:
             data.data = self.data.loc[data.timestamp]
         self._market_status = data
 
-        self._price_status: pd.Series = price
-
         self._borrows_amount_cache.reset()
         self._supplies_amount_cache.reset()
         self._collaterals_amount_cache.reset()
         self._borrows_cache.reset()
         self._supplies_cache.reset()
 
-        self.has_update = False
-
     @property
     def liquidation_threshold(self) -> Decimal:
         """
         Get liquidation threshold
         """
         return AaveV3CoreLib.total_liquidation_threshold(self.collateral_value, self._risk_parameters)
 
@@ -417,15 +422,17 @@
         """
         Calculate total apy based on borrow/supply apy and amount
         """
         total_supplies = self.total_supply_value
         total_borrows = self.total_borrows_value
         supply_apy = self.supply_apy
         borrow_apy = self.borrow_apy
-        return AaveV3CoreLib.safe_div_zero(supply_apy * total_supplies - borrow_apy * total_borrows, total_supplies - total_borrows)
+        return AaveV3CoreLib.safe_div_zero(
+            supply_apy * total_supplies - borrow_apy * total_borrows, total_supplies - total_borrows
+        )
 
     def get_supply(self, supply_key: SupplyKey = None, token_info: TokenInfo = None) -> Supply:
         """
         Get details of supply position, include value, amount, apy etc.
 
         :params supply_key: supply key, you can query by supply_key or token_info
         :type supply_key: SupplyKey
@@ -495,15 +502,17 @@
         rounding = Decimal("0.0001")
         total_supplies = self.total_supply_value.quantize(rounding)
         total_borrows = self.total_borrows_value.quantize(rounding)
         net_worth = total_supplies - total_borrows
 
         supply_apy = self.supply_apy.quantize(rounding)
         borrow_apy = self.borrow_apy.quantize(rounding)
-        net_apy = AaveV3CoreLib.safe_div_zero(supply_apy * total_supplies - borrow_apy * total_borrows, total_supplies - total_borrows)
+        net_apy = AaveV3CoreLib.safe_div_zero(
+            supply_apy * total_supplies - borrow_apy * total_borrows, total_supplies - total_borrows
+        )
 
         return AaveBalance(
             net_value=net_worth,
             supplies_count=len(self._supplies),
             borrows_count=len(self._borrows),
             liquidation_threshold=AaveV3CoreLib.safe_rounding(self.liquidation_threshold, rounding),
             health_factor=AaveV3CoreLib.safe_rounding(self.health_factor, rounding),
@@ -520,15 +529,18 @@
     def check_market(self):
         """
         Check market tokens before back test
         """
         super().check_market()
         require(len(self.tokens) > 0, "should set tokens")
         for t in self.tokens:
-            require(t.name in self.risk_parameters.index, f"According to risk_parameter, {t.name} is not supported in this chain. ")
+            require(
+                t.name in self.risk_parameters.index,
+                f"According to risk_parameter, {t.name} is not supported in this chain. ",
+            )
             for col in AaveV3Market.REQUIRED_DATA_COLUMN:
                 require((t.name, col) in self.data.columns, f"{t.name}.{col} not found in data")
 
     def update(self):
         """
         Trigger update of this market
         """
@@ -541,36 +553,38 @@
         value = get_formatted_predefined(f"{self.market_info.name}({type(self).__name__})", STYLE["header3"]) + "\n"
         token_dict = {"tokens": ",".join([t.name for t in self._tokens])}
         value += get_formatted_from_dict(token_dict) + "\n"
         balance = self.get_market_balance()
         value += (
             get_formatted_from_dict(
                 {
-                    "net_value": "{:.2f}".format(balance.net_value),
-                    "health_factor": "{:.2f}".format(balance.health_factor),
-                    "borrow_balance": "{:.2f}".format(balance.borrows_value),
-                    "supply_balance": "{:.2f}".format(balance.supplies_value),
-                    "collateral_balance": "{:.2f}".format(balance.collaterals_value),
-                    "supply_apy": "{:.2f}".format(balance.supply_apy),
-                    "borrow_apy": "{:.2f}".format(balance.borrow_apy),
-                    "net_apy": "{:.2f}".format(balance.net_apy),
+                    "net_value": console_text.format_value(balance.net_value),
+                    "health_factor": console_text.format_value(balance.health_factor),
+                    "borrow_balance": console_text.format_value(balance.borrows_value),
+                    "supply_balance": console_text.format_value(balance.supplies_value),
+                    "collateral_balance": console_text.format_value(balance.collaterals_value),
+                    "supply_apy": console_text.format_value(balance.supply_apy),
+                    "borrow_apy": console_text.format_value(balance.borrow_apy),
+                    "net_apy": console_text.format_value(balance.net_apy),
                 }
             )
             + "\n"
         )
         value += get_formatted_predefined("Supplies", STYLE["key"]) + "\n"
         supply_df = supply_to_dataframe(self.supplies)
         value += supply_df.to_string() + "\n" if len(supply_df.index) > 0 else "Empty DataFrame\n"
         value += get_formatted_predefined("Borrows", STYLE["key"]) + "\n"
         borrow_df = borrow_to_dataframe(self.borrows)
         value += borrow_df.to_string() + "\n" if len(borrow_df.index) > 0 else "Empty DataFrame\n"
 
         return value
 
     # endregion
+
+    @write_func
     @float_param_formatter
     def supply(self, token_info: TokenInfo, amount: Decimal | float, collateral: bool = True) -> SupplyKey:
         """
         | Supply asset to aave pool
         | Note:
         | 1. some token are not allow to collateral, it's decided by risk parameter
         | 2. if append amount to existing supply, collateral can not change.
@@ -602,36 +616,41 @@
         self._supplies_amount_cache.reset()
         self._supplies_cache.reset()
         self._collaterals_amount_cache.reset()
 
         self._record_action(
             SupplyAction(
                 market=self.market_info,
-                token=token_info,
+                token=token_info.name,
                 amount=UnitDecimal(amount, token_info.name),
                 collateral=collateral,
-                deposit_after=UnitDecimal(AaveV3CoreLib.get_amount(self._supplies[key].base_amount, token_status.liquidity_index), token_info.name),
+                deposit_after=UnitDecimal(
+                    AaveV3CoreLib.get_amount(self._supplies[key].base_amount, token_status.liquidity_index),
+                    token_info.name,
+                ),
             )
         )
-        self.has_update = True
 
         return key
 
     @staticmethod
     def __get_supply_key(supply_key: SupplyKey = None, token_info: TokenInfo = None):
         if supply_key is not None:
             key = supply_key
             token_info = key.token
         elif token_info is not None:
             key = SupplyKey(token_info)
         else:
             raise DemeterError("supply_key or token should be specified")
         return key, token_info
 
-    def change_collateral(self, collateral: bool, supply_key: SupplyKey = None, token_info: TokenInfo = None) -> SupplyKey:
+    @write_func
+    def change_collateral(
+        self, collateral: bool, supply_key: SupplyKey = None, token_info: TokenInfo = None
+    ) -> SupplyKey:
         """
         Change collateral type of supply position. Health factor will be checked to prevent liquidation
 
         :param collateral: new value
         :type collateral: bool
         :param supply_key: key of supply, you can set by supply_key or token_info
         :type supply_key: SupplyKey
@@ -649,18 +668,18 @@
         self._collaterals_amount_cache.reset()
 
         if (not collateral) and self.health_factor < AaveV3CoreLib.HEALTH_FACTOR_LIQUIDATION_THRESHOLD:
             # revert
             self._supplies[SupplyKey(token_info)].collateral = old_collateral
             self._collaterals_amount_cache.reset()
             raise AssertionError("health factor lower than liquidation threshold")
-        self.has_update = True
 
         return key
 
+    @write_func
     @float_param_formatter
     def withdraw(
         self,
         supply_key: SupplyKey = None,
         amount: Decimal | float = None,
         token_info: TokenInfo = None,
     ):
@@ -681,32 +700,35 @@
             amount = supply.amount
         require(amount != 0, "invalid amount")
         require(amount <= supply.amount, "not enough available user balance")
 
         # try calc new health factor after withdraw. if health factor is low, raise a error
         if self._supplies[key].collateral:
             old_base_amount = self._supplies[key].base_amount
-            self._supplies[key].base_amount -= AaveV3CoreLib.get_base_amount(amount, self._market_status.data[key.token.name].liquidity_index)
+            self._supplies[key].base_amount -= AaveV3CoreLib.get_base_amount(
+                amount, self._market_status.data[key.token.name].liquidity_index
+            )
             self._supplies_amount_cache.reset()
             self._collaterals_amount_cache.reset()
             if self.health_factor < AaveV3CoreLib.HEALTH_FACTOR_LIQUIDATION_THRESHOLD:
                 raise AssertionError("health factor lower than liquidation threshold")
             self._supplies[key].base_amount = old_base_amount
 
         final_base_amount = self.__sub_supply_amount(key, amount)
         self.broker.add_to_balance(token_info, amount)
         self._record_action(
             WithdrawAction(
                 market=self.market_info,
-                token=token_info,
+                token=token_info.name,
                 amount=UnitDecimal(amount, token_info.name),
-                deposit_after=UnitDecimal(AaveV3CoreLib.get_amount(final_base_amount, token_status.liquidity_index), token_info.name),
+                deposit_after=UnitDecimal(
+                    AaveV3CoreLib.get_amount(final_base_amount, token_status.liquidity_index), token_info.name
+                ),
             )
         )
-        self.has_update = True
 
         pass
 
     def get_max_withdraw_amount(self, supply_key: SupplyKey = None, token_info: TokenInfo = None) -> Decimal:
         """
         Get max available withdraw amount
 
@@ -715,29 +737,34 @@
         :param token_info: which token to query. you can set by supply_key or token_info
         :type token_info: TokenInfo
         :return: max withdraw amount
         :rtype: Decimal
         """
         key, token_info = AaveV3Market.__get_supply_key(supply_key, token_info)
         return self.supplies[key].amount - AaveV3CoreLib.get_min_withdraw_kept_amount(
-            token_info, self.collateral_value, self.borrows_value, self._risk_parameters, self._price_status[token_info.name]
+            token_info,
+            self.collateral_value,
+            self.borrows_value,
+            self._risk_parameters,
+            self._price_status[token_info.name],
         )
 
     def get_max_borrow_amount(self, token_info: TokenInfo) -> Decimal:
         """
         Get max token amount to borrow.
 
         :param token_info: token to query
         :param token_info: TokenInfo
         :return: max borrow amount
         :rtype: Decimal
         """
         value = AaveV3CoreLib.get_max_borrow_value(self.collateral_value, self.borrows_value, self.risk_parameters)
         return value / self._price_status[token_info.name]
 
+    @write_func
     @float_param_formatter
     def borrow(
         self,
         token_info: TokenInfo,
         amount: Decimal | float = None,
         interest_rate_mode: InterestRateMode = InterestRateMode.variable,
     ) -> BorrowKey:
@@ -765,24 +792,29 @@
 
         require(self._risk_parameters.loc[token_info.name, "canBorrow"], f"borrow is not enabled for {token_info.name}")
         collateral_balance = sum(self.collateral_value.values())
         require(collateral_balance != 0, "collateral balance is zero")
         current_ltv = self.current_ltv
         require(current_ltv != 0, "ltv validation failed")
 
-        require(self.health_factor > AaveV3CoreLib.HEALTH_FACTOR_LIQUIDATION_THRESHOLD, "health factor lower than liquidation threshold")
+        require(
+            self.health_factor > AaveV3CoreLib.HEALTH_FACTOR_LIQUIDATION_THRESHOLD,
+            "health factor lower than liquidation threshold",
+        )
 
         value = amount * self._price_status.loc[token_info.name]
         collateral_needed = sum(self.borrows.values()) + value / current_ltv
         require(collateral_needed <= collateral_balance, "collateral cannot cover new borrow")
 
         if interest_rate_mode == InterestRateMode.stable:
             require(self._risk_parameters.loc[token_info.name, "canBorrowStable"], "stable borrowing not enabled")
 
-            is_using_as_collateral = (token_info in self._supplies) and (self._supplies[SupplyKey(token_info)].collateral is True)
+            is_using_as_collateral = (token_info in self._supplies) and (
+                self._supplies[SupplyKey(token_info)].collateral is True
+            )
 
             require(
                 (not is_using_as_collateral)
                 or self._risk_parameters.loc[token_info.name, "LTV"] == 0
                 or amount > self.broker.get_token_balance(token_info),
                 "collateral same as borrowing currency",
             )
@@ -799,53 +831,62 @@
 
         self._borrows_amount_cache.reset()
         self._borrows_cache.reset()
 
         self._record_action(
             BorrowAction(
                 market=self.market_info,
-                token=token_info,
+                token=token_info.name,
                 amount=UnitDecimal(amount, token_info.name),
                 interest_rate_mode=interest_rate_mode,
-                debt_after=UnitDecimal(AaveV3CoreLib.get_amount(self._borrows[key].base_amount, token_status.variable_borrow_index), token_info.name),
+                debt_after=UnitDecimal(
+                    AaveV3CoreLib.get_amount(self._borrows[key].base_amount, token_status.variable_borrow_index),
+                    token_info.name,
+                ),
             )
         )
-        self.has_update = True
 
         return key
 
-    def get_max_repay_amount(self, key: BorrowKey = None, token_info: TokenInfo = None, interest_rate_mode: InterestRateMode = None) -> Decimal:
+    def get_max_repay_amount(
+        self, key: BorrowKey = None, token_info: TokenInfo = None, interest_rate_mode: InterestRateMode = None
+    ) -> Decimal:
         """
         Get max token amount to repay.
 
         :param key: key for borrow. Either fill key parameter or token_info+interest_rate_mode parameter.
         :type key: BorrowKey
         :param token_info: token to borrow, Either fill key parameter or token_info+interest_rate_mode parameter.
         :type token_info: TokenInfo
         :param interest_rate_mode: interest rate mode, Either fill key parameter or token_info+interest_rate_mode parameter.
         :type interest_rate_mode: InterestRateMode
         :return: max amount to repay
         :rtype: Decimal
         """
         (key, _, _) = AaveV3Market.__get_borrow_key(key, token_info, interest_rate_mode)
-        return AaveV3CoreLib.get_amount(self._borrows[key].base_amount, self.market_status.data[key.token.name].variable_borrow_index)
+        return AaveV3CoreLib.get_amount(
+            self._borrows[key].base_amount, self.market_status.data[key.token.name].variable_borrow_index
+        )
 
     @staticmethod
-    def __get_borrow_key(key: BorrowKey = None, token_info: TokenInfo = None, interest_rate_mode: InterestRateMode = None):
+    def __get_borrow_key(
+        key: BorrowKey = None, token_info: TokenInfo = None, interest_rate_mode: InterestRateMode = None
+    ):
         if key is None:
             if token_info is None:
                 raise DemeterError("either key or token should be filled")
             key = BorrowKey(token_info, interest_rate_mode)
         token_info = key.token
         interest_rate_mode = key.interest_rate_mode
         return key, token_info, interest_rate_mode
 
     def _get_swap_amount(self, from_token: TokenInfo, to_token: TokenInfo, amount: Decimal, swap_fee=0):
         return amount * (1 - swap_fee) * self._price_status.loc[from_token.name] / self._price_status.loc[to_token.name]
 
+    @write_func
     @float_param_formatter
     def repay(
         self,
         key: BorrowKey = None,
         payback_amount: Decimal | float = None,
         borrow_token: TokenInfo = None,
         interest_rate_mode: InterestRateMode = None,
@@ -878,17 +919,21 @@
             payback_amount = borrow.amount
 
         if repay_with_collateral:
             if repay_collateral_token is None:
                 repay_collateral_token = borrow_token
             repay_collateral_key = SupplyKey(repay_collateral_token)
             require(repay_collateral_key in self.supplies.keys(), f"token {repay_collateral_token} is not in supply")
-            require(self.supplies[repay_collateral_key].collateral, f"token {repay_collateral_token} is not in collateral")
+            require(
+                self.supplies[repay_collateral_key].collateral, f"token {repay_collateral_token} is not in collateral"
+            )
 
-            required_amount_in_collateral_token = self._get_swap_amount(borrow_token, repay_collateral_token, payback_amount)
+            required_amount_in_collateral_token = self._get_swap_amount(
+                borrow_token, repay_collateral_token, payback_amount
+            )
             supply = self.get_supply(supply_key=repay_collateral_key)
             if required_amount_in_collateral_token > supply.amount:
                 # contract will change payback amount instead of raise a error
                 payback_amount = self._get_swap_amount(repay_collateral_token, borrow_token, supply.amount)
 
         payback_base_amount = AaveV3CoreLib.get_base_amount(payback_amount, token_status.variable_borrow_index)
 
@@ -900,32 +945,34 @@
             self.__sub_supply_amount(SupplyKey(repay_collateral_token), payback_amount_in_collateral)
         else:
             self.broker.subtract_from_balance(borrow_token, payback_amount)
         debt = self.__sub_borrow_amount(key, payback_amount)
         self._record_action(
             RepayAction(
                 market=self.market_info,
-                token=borrow_token,
+                token=borrow_token.name,
                 amount=UnitDecimal(payback_amount, borrow_token.name),
                 interest_rate_mode=interest_rate_mode,
-                debt_after=UnitDecimal(AaveV3CoreLib.get_amount(debt, token_status.variable_borrow_index), borrow_token.name),
+                debt_after=UnitDecimal(
+                    AaveV3CoreLib.get_amount(debt, token_status.variable_borrow_index), borrow_token.name
+                ),
             )
         )
-        self.has_update = True
 
         pass
 
     def __sub_supply_amount(self, key: SupplyKey, amount: Decimal) -> Decimal:
         if key not in self._supplies:
             if amount == Decimal(0):
                 return Decimal(0)
             else:
                 raise DemeterError(f"{key} not exist in supplies")
         self._supplies[key].base_amount = helper.sub_base_amount(
-            self._supplies[key].base_amount, AaveV3CoreLib.get_base_amount(amount, self._market_status.data[key.token.name].liquidity_index)
+            self._supplies[key].base_amount,
+            AaveV3CoreLib.get_base_amount(amount, self._market_status.data[key.token.name].liquidity_index),
         )
         if self._supplies[key].collateral:
             self._collaterals_amount_cache.reset()
         self._supplies_amount_cache.reset()
         self._supplies_cache.reset()
         if self._supplies[key].base_amount == DECIMAL_0:
             if self._supplies[key].collateral:
@@ -938,24 +985,26 @@
     def __sub_borrow_amount(self, key: BorrowKey, amount: Decimal) -> Decimal:
         if key not in self._borrows:
             if amount == Decimal(0):
                 return Decimal(0)
             else:
                 raise DemeterError(f"{key} not exist in borrows")
         self._borrows[key].base_amount = helper.sub_base_amount(
-            self._borrows[key].base_amount, AaveV3CoreLib.get_base_amount(amount, self._market_status.data[key.token.name].variable_borrow_index)
+            self._borrows[key].base_amount,
+            AaveV3CoreLib.get_base_amount(amount, self._market_status.data[key.token.name].variable_borrow_index),
         )
         self._borrows_amount_cache.reset()
         self._borrows_cache.reset()
         if self._borrows[key].base_amount == DECIMAL_0:
             del self._borrows[key]
             return DECIMAL_0
         else:
             return self._borrows[key].base_amount
 
+    @write_func
     def _liquidate(self):
         """
         | Do passive liquidate. If health factor is below 1, liquidate will be triggered. And user can not make a liquidation transaction. Because currently demeter doesn't support that.
         | First is to decide when to liquidate, if in current loop, health factor is below 1, liquidation will happen immediately. Triggered by update function.
         | Second step to choose the assets. Here we will pick the most valuable collateral asset and least valuable debt.
         | After liquidation, if health factor is still below 1. Will choose a pair of collateral and debt to liquidate again.
         | But if a debt asset has liquidated, It will not be liquidated again.
@@ -992,15 +1041,14 @@
 
             try:
                 self._do_liquidate(max_supply_key.token, min_borrow_key.token, min_borrow_value)
             except AssertionError:
                 # if a liquidated is rejected, choose another delt token to liquidate
                 pass
             health_factor = self.health_factor
-        self.has_update = True
 
     def _do_liquidate(self, collateral_token: TokenInfo, delt_token: TokenInfo, delt_value_to_cover: Decimal):
         """
         Make a liquidation transaction;
 
         :param collateral_token: Which collateral token will be used
         :type collateral_token: TokenInfo
@@ -1025,47 +1073,60 @@
         total_debt = stable_delt + variable_delt
         close_factor = (
             AaveV3CoreLib.DEFAULT_LIQUIDATION_CLOSE_FACTOR
             if old_health_factor > AaveV3CoreLib.CLOSE_FACTOR_HF_THRESHOLD
             else AaveV3CoreLib.MAX_LIQUIDATION_CLOSE_FACTOR
         )
         max_liquidatable_debt = total_debt * close_factor
-        actual_debt_to_liquidate = max_liquidatable_debt if delt_value_to_cover > max_liquidatable_debt else delt_value_to_cover
+        actual_debt_to_liquidate = (
+            max_liquidatable_debt if delt_value_to_cover > max_liquidatable_debt else delt_value_to_cover
+        )
 
         # validate delt
-        is_collateral_enabled = self._risk_parameters.loc[collateral_token.name].liqThereshold != 0 and self._supplies[collateral_key].collateral
+        is_collateral_enabled = (
+            self._risk_parameters.loc[collateral_token.name].liqThereshold != 0
+            and self._supplies[collateral_key].collateral
+        )
 
         require(is_collateral_enabled, "collateral cannot be liquidated")
         require(total_debt != DECIMAL_0, "specified currency not borrowed by user")
 
         user_collateral_balance = (
-            self._supplies[SupplyKey(collateral_token)].base_amount * self._market_status.data[collateral_token.name].liquidity_index
+            self._supplies[SupplyKey(collateral_token)].base_amount
+            * self._market_status.data[collateral_token.name].liquidity_index
         )
 
         # calculate actual amount
-        should_collateral = self._price_status.loc[delt_token.name] * actual_debt_to_liquidate / self._price_status.loc[collateral_token.name]
+        should_collateral = (
+            self._price_status.loc[delt_token.name]
+            * actual_debt_to_liquidate
+            / self._price_status.loc[collateral_token.name]
+        )
         max_collateral_to_liquidate = should_collateral * (1 + liquidation_bonus)
 
         if max_collateral_to_liquidate > user_collateral_balance:
             actual_collateral_to_liquidate = user_collateral_balance
-            actual_debt_to_liquidate = (self._price_status.loc[collateral_token.name] * actual_collateral_to_liquidate) / (
-                self._price_status.loc[delt_token.name] * (1 + liquidation_bonus)
-            )
+            actual_debt_to_liquidate = (
+                self._price_status.loc[collateral_token.name] * actual_collateral_to_liquidate
+            ) / (self._price_status.loc[delt_token.name] * (1 + liquidation_bonus))
         else:
             actual_collateral_to_liquidate = max_collateral_to_liquidate
             actual_debt_to_liquidate = actual_debt_to_liquidate
         self._supplies[collateral_key].base_amount = helper.sub_base_amount(
-            self._supplies[collateral_key].base_amount, AaveV3CoreLib.get_base_amount(actual_collateral_to_liquidate, supply_index)
+            self._supplies[collateral_key].base_amount,
+            AaveV3CoreLib.get_base_amount(actual_collateral_to_liquidate, supply_index),
         )
 
         if self._supplies[collateral_key].base_amount == 0:
             del self._supplies[collateral_key]
         if variable_delt > actual_debt_to_liquidate:
             vari_debt_remaining_base = self.__sub_borrow_amount(variable_key, actual_debt_to_liquidate)
-            stable_debt_remaining_base = self._borrows[stable_key].base_amount if stable_key in self._borrows else DECIMAL_0
+            stable_debt_remaining_base = (
+                self._borrows[stable_key].base_amount if stable_key in self._borrows else DECIMAL_0
+            )
             vari_debt_liquidated = actual_debt_to_liquidate
             stable_debt_liquidated = DECIMAL_0
 
         else:
             vari_debt_liquidated = variable_delt
             stable_debt_liquidated = actual_debt_to_liquidate - variable_delt
             vari_debt_remaining_base = self.__sub_borrow_amount(variable_key, variable_delt)
@@ -1076,25 +1137,30 @@
         self._supplies_amount_cache.reset()
         self._supplies_cache.reset()
         self._collaterals_amount_cache.reset()
 
         self._record_action(
             LiquidationAction(
                 market=self.market_info,
-                collateral_token=collateral_token,
-                debt_token=delt_token,
+                collateral_token=collateral_token.name,
+                debt_token=delt_token.name,
                 delt_to_cover=UnitDecimal(delt_value_to_cover, delt_token.name),
                 collateral_used=UnitDecimal(actual_collateral_to_liquidate, collateral_token.name),
                 variable_delt_liquidated=UnitDecimal(vari_debt_liquidated, delt_token.name),
                 stable_delt_liquidated=UnitDecimal(stable_debt_liquidated, delt_token.name),
                 health_factor_before=old_health_factor,
                 health_factor_after=self.health_factor,
                 collateral_after=UnitDecimal(
                     AaveV3CoreLib.get_amount(
-                        self._supplies[collateral_key].base_amount if collateral_key in self._supplies else DECIMAL_0, supply_index
+                        self._supplies[collateral_key].base_amount if collateral_key in self._supplies else DECIMAL_0,
+                        supply_index,
                     ),
                     collateral_token.name,
                 ),
-                variable_debt_after=UnitDecimal(AaveV3CoreLib.get_amount(vari_debt_remaining_base, borrow_index), delt_token.name),
-                stable_delt_after=UnitDecimal(AaveV3CoreLib.get_amount(stable_debt_remaining_base, borrow_index), delt_token.name),
+                variable_debt_after=UnitDecimal(
+                    AaveV3CoreLib.get_amount(vari_debt_remaining_base, borrow_index), delt_token.name
+                ),
+                stable_delt_after=UnitDecimal(
+                    AaveV3CoreLib.get_amount(stable_debt_remaining_base, borrow_index), delt_token.name
+                ),
             )
         )
```

### Comparing `zelos-demeter-0.3.0/demeter/broker/_typing.py` & `zelos-demeter-0.5.1/demeter/broker/_typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from dataclasses import dataclass, field
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum
-from typing import Generic, NamedTuple, List, Dict, TypeVar
+from typing import Generic, NamedTuple, List, Dict, TypeVar, Union
 
 import pandas as pd
 
 from .._typing import DemeterError, TokenInfo
 
 T = TypeVar("T")
 
@@ -29,25 +29,27 @@
 #     """
 #
 #     timestamp: datetime = None
 #     row_id: int = None
 
 
 class MarketTypeEnum(Enum):
-    uniswap = 1
+    uniswap_v3 = 1
     aave_v3 = 2
+    deribit_option = 3
+    squeeth = 4
 
 
 class MarketInfo(NamedTuple):
     """
     MarketInfo properties
     """
 
     name: str  # uni_market
-    type: MarketTypeEnum = MarketTypeEnum.uniswap
+    type: MarketTypeEnum = MarketTypeEnum.uniswap_v3
 
     def __str__(self):
         return f"{self.name}({self.type.name})"
 
     def __repr__(self):
         return f"{self.name}({self.type.name})"
 
@@ -118,15 +120,18 @@
             self.balance -= amount
         else:
             # if difference between amount and balance is below 0.01%, will deduct all the balance
             # That's because, the amount calculated by v3_core, has some acceptable error.
             if abs((self.balance - amount) / base) < 0.00001:
                 self.balance = Decimal(0)
             elif self.balance - amount < Decimal(0):
-                raise AssertionError(f"insufficient balance, balance is {self.balance}{self.name}, " f"but sub amount is {amount}{self.name}")
+                raise AssertionError(
+                    f"insufficient balance, balance is {self.balance}{self.name}, "
+                    f"but sub amount is {amount}{self.name}"
+                )
             else:
                 self.balance -= amount
 
         return self
 
     def amount_in_wei(self):
         """
@@ -151,20 +156,31 @@
     * collect_fee
     """
 
     uni_lp_add_liquidity = "add_liquidity"
     uni_lp_remove_liquidity = "remove_liquidity"
     uni_lp_buy = "buy"
     uni_lp_sell = "sell"
+    uni_lp_swap = "swap"
     uni_lp_collect = "collect"
     aave_supply = "supply"
     aave_withdraw = "withdraw"
     aave_borrow = "borrow"
     aave_repay = "repay"
     aave_liquidation = "liquidation"
+    option_buy = "option_buy"
+    option_sell = "option_sell"
+    option_exercise = "option_exercise"
+    squeeth_open_vault = "open_vault"
+    squeeth_update_collateral = "update_collateral"
+    squeeth_update_short = "update_short"
+    squeeth_deposit_lp = "deposit_uni_lp"
+    squeeth_withdraw_lp = "withdraw_uni_lp"
+    squeeth_reduce_debt = "reduce_debt"
+    squeeth_liquidation = "liquidation"
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return self.name
 
@@ -224,15 +240,15 @@
     """
     MarketStatus properties
 
     :type timestamp: datetime
     """
 
     timestamp: datetime | None
-    data: pd.Series = None
+    data: pd.Series | None = None
 
 
 T = TypeVar("T")
 
 
 class MarketDict(Generic[T]):
     """
@@ -417,15 +433,17 @@
         """
         status list convert to dataframe
         :param status_list:
         :return:
         """
         index = [i.timestamp for i in status_list]
         if len(index) > 0:
-            return pd.DataFrame(columns=status_list[0].get_names(), index=index, data=map(lambda d: d.to_array(), status_list))
+            return pd.DataFrame(
+                columns=status_list[0].get_names(), index=index, data=map(lambda d: d.to_array(), status_list)
+            )
         else:
             return pd.DataFrame()
 
 
 class PositionManager:
     def __init__(self):
         self.positions: Dict[str, Decimal] = {}
@@ -457,11 +475,14 @@
     def has(self, stock: T) -> bool:
         key = str(stock)
         return key in self.positions
 
 
 @dataclass
 class RowData:
-    timestamp: datetime # Time of this iteration
-    row_id: int # index of this iteration, start from 0
-    prices: pd.Series # price of tokens at this time
-    market_status: MarketDict[pd.Series] = MarketDict() # status of markets at this time
+    timestamp: datetime  # Time of this iteration
+    row_id: int  # index of this iteration, start from 0
+    prices: pd.Series  # price of tokens at this time
+    market_status: MarketDict[Union[pd.Series, pd.DataFrame]] = MarketDict()  # status of markets at this time
+
+
+BASE_FREQ = "1min"
```

### Comparing `zelos-demeter-0.3.0/demeter/broker/broker.py` & `zelos-demeter-0.5.1/demeter/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from .market import Market
 from .._typing import DemeterError, UnitDecimal
 from ..utils import get_formatted_from_dict, get_formatted_predefined, STYLE, float_param_formatter
 
 
 class Broker:
     """
-    Broker supports different order types, checking a submitted order cash requirements against current cash, keeping track of cash and value for each iteration of actuator and keeping the current position on different datas.
+    Broker supports different order types, checking a submitted order cash requirements against current cash,
+    keeping track of cash and value for each iteration of actuator and keeping the current position on different datas.
 
     :param allow_negative_balance: allow cash balance can be negative value or not. Default is False
     :type allow_negative_balance: bool
     :param record_action_callback: A callback function used to notify actions(buy/sell). When new actions is taken, this function will be called, and action instance will be passed as parameter. function should be like: def callback(action:BaseAction)
     :type record_action_callback: Callable[[BaseAction], None]
     """
 
@@ -185,14 +186,15 @@
         for k, v in self.markets.items():
             account_status.market_status[k] = v.get_market_balance(prices)
         account_status.market_status.set_default_key(self.markets.get_default_key())
         for k, v in self.assets.items():
             account_status.asset_balances[k] = v.balance
         asset_sum = sum([v * prices[k.name] for k, v in account_status.asset_balances.items()])
         market_sum = sum([v.net_value for v in account_status.market_status.values()])
+        print('asset_sum', asset_sum, 'market_sum', market_sum)
         account_status.net_value = asset_sum + market_sum
         return account_status
 
     def formatted_str(self):
         """
         Get formatted broker description string to print in console
```

### Comparing `zelos-demeter-0.3.0/demeter/broker/market.py` & `zelos-demeter-0.5.1/demeter/broker/market.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 import logging
 from decimal import Decimal
+from functools import wraps
 from typing import Dict, Callable
 
 import pandas as pd
 
-from ._typing import BaseAction, MarketBalance, MarketStatus, MarketInfo
+from ._typing import BaseAction, MarketBalance, MarketStatus, MarketInfo, RowData
 from .._typing import DECIMAL_0, DemeterError
 
 DEFAULT_DATA_PATH = "./data"
 
 
+def write_func(func):
+    @wraps(func)
+    def wrapper_func(*args, **kwargs):
+        instance = args[0]
+        if not instance.is_open:
+            raise DemeterError(f"{instance.market_info.name} is not open.")
+        ret = func(*args, **kwargs)
+        instance.has_update = True
+        return ret
+
+    return wrapper_func
+
+
 class Market:
     """
 
     | Market is the place to invest your assets.
     | This is an abstract class, you should use subclass instead this one
 
     :param market_info: Key of this market.
@@ -33,19 +47,24 @@
         self._market_info: MarketInfo = market_info
         self.broker = None
         self._record_action_callback: Callable[[BaseAction], None] = None
         self.data_path: str = data_path
         self.logger = logging.getLogger(__name__)
         self._market_status: MarketStatus = MarketStatus(None, pd.Series())
         self._price_status: pd.Series | None = None
-        # if some var that related to market status has changed, should set this to True, then the second set_market_status in every minute will be triggerd
+        # if some var that related to market status has changed, should set this to True,
+        # then the second set_market_status in every minute will be triggerd
         # e.g. At uniswap market, when add liquidity in the head of the minute, this flag will be set to True,
         # so user liquidity will be added to total liquidity in this minute, and get more fee
         # remember set this flag to False after set_market_status
         self.has_update = False
+        self.open: Callable[[RowData], None] = None
+        # if market interval is minutely, is_open will always true,
+        # or it will be false until timestamp is on it's interval
+        self.is_open: bool = True
 
     def __str__(self):
         return f"{self._market_info.name}:{type(self).__name__}"
 
     @property
     def market_info(self) -> MarketInfo:
         """
@@ -114,16 +133,17 @@
 
         :param data: market status
         :type data: Series | MarketStatus
         :param price: current price
         :type price: Series
 
         """
-        self._market_status = data
+        # self._market_status = data
         self._price_status = price
+        self.is_open = True if self._data is None or data.timestamp in self._data.index else False
         self.has_update = False
 
     def get_market_balance(self, prices: pd.Series | Dict[str, Decimal]) -> MarketBalance:
         """
         Get market asset balance, such as current positions, net values
 
         :param prices: current price of each token
```

### Comparing `zelos-demeter-0.3.0/demeter/core/actuator.py` & `zelos-demeter-0.5.1/demeter/core/actuator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import logging
 import os
 import pickle
 import time
+from dataclasses import dataclass, field
 from datetime import datetime
+from decimal import Decimal
 from typing import List, Dict, Union
-from dataclasses import dataclass, field
+
 import orjson
 import pandas as pd
 from pandas import Timestamp
 from tqdm import tqdm  # process bar
 
 from .evaluating_indicator import Evaluator
 from .. import Broker, Asset
 from .._typing import DemeterError, EvaluatorEnum, UnitDecimal
 from ..broker import BaseAction, AccountStatus, MarketInfo, MarketDict, MarketStatus, RowData
-from ..uniswap import UniLpMarket, PositionInfo
 from ..strategy import Strategy
+from ..uniswap import UniLpMarket, PositionInfo
 from ..utils import get_formatted_predefined, STYLE, to_decimal
+from ..utils import console_text
 
 
 class Actuator(object):
     """
     Core component of a back test. Manage the resources in a test, including broker/strategy/data/indicator,
 
     :param allow_negative_balance: Allow cash balance of broker can be negative value or not. Default is False
@@ -46,15 +49,14 @@
         # path of source data, which is saved by downloader
         # evaluating indicator calculator
         self._evaluator: Evaluator | None = None
         self._enabled_evaluator: [] = []
         # logging
         logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s")
         self.logger = logging.getLogger(__name__)
-
         # internal var
         self.__backtest_finished = False
 
     def _record_action_list(self, action: BaseAction):
         """
         record action list
 
@@ -170,35 +172,14 @@
         :type value: Strategy
         """
         if isinstance(value, Strategy):
             self._strategy = value
         else:
             raise ValueError()
 
-    @property
-    def number_format(self) -> str:
-        """
-        number format for console output, e.g. ".8g", ".5f"
-
-        :return: number format
-        :rtype: str
-        """
-        return self._number_format
-
-    @number_format.setter
-    def number_format(self, value: str):
-        """
-        | number format for console output, e.g. ".8g", ".5f",
-        | follow the document here: https://python-reference.readthedocs.io/en/latest/docs/functions/format.html
-
-        :param value: number format,
-        :type value:str
-        """
-        self._number_format = value
-
     # endregion
 
     def get_account_status_dataframe(self) -> pd.DataFrame:
         """
         | Get account status in dataframe. it contains account balance/position change of every minute.
         | Row(datetimeindex) is per minute.
         | Column is net value/positions.
@@ -231,15 +212,15 @@
         +-------------------+---------+-------+
         |2023-08-13 00:01:00| 1848.12 | 1     |
         +-------------------+---------+-------+
 
         :param prices: dataframe or series contains prices
         :type prices: Union[pd.DataFrame, pd.Series]
         """
-        prices = prices.applymap(lambda y: to_decimal(y))
+        prices = prices.map(lambda y: to_decimal(y))
         if isinstance(prices, pd.DataFrame):
             if self._token_prices is None:
                 self._token_prices = prices
             else:
                 self._token_prices = pd.concat([self._token_prices, prices])
         else:
             if self._token_prices is None:
@@ -277,64 +258,76 @@
         if self._token_prices is None:
             # if price is not set and market is uni_lp_market, get price from market automatically
             for market in self.broker.markets.values():
                 if isinstance(market, UniLpMarket):
                     self.set_price(market.get_price_from_data())
             if self._token_prices is None:
                 raise DemeterError("token prices is not set")
-        for token in self._broker.assets.keys():  # dict_keys([TokenInfo(name='usdc', decimal=6), TokenInfo(name='eth', decimal=18)])
-            if token.name not in self._token_prices:
-                raise DemeterError(f"Price of {token.name} has not set yet")
+        # for token in self._broker.assets.keys():  # dict_keys([TokenInfo(name='usdc', decimal=6), TokenInfo(name='eth', decimal=18)])
+        #     if token.name not in self._token_prices:
+        #         raise DemeterError(f"Price of {token.name} has not set yet")
 
         data_length = []  # [1440]
         for market in self._broker.markets.values():
             data_length.append(len(market.data.index))
             market.check_market()  # check each market, including assets
         # ensure data length same
-        if List.count(data_length, data_length[0]) != len(data_length):
-            raise DemeterError("data length among markets are not same")
+        # if List.count(data_length, data_length[0]) != len(data_length):
+        #     raise DemeterError("data length among markets are not same")
         default_market_data = self._broker.markets.default.data
         if (
-            self._token_prices.head(1).index[0] > default_market_data.head(1).index[0]
-            or self._token_prices.tail(1).index[0] < default_market_data.tail(1).index[0]
+            self._token_prices.head(1).index[0] > default_market_data.head(1).index.get_level_values(0).unique()[0]
+            or self._token_prices.tail(1).index[0] < default_market_data.tail(1).index.get_level_values(0).unique()[0]
         ):
             raise DemeterError("Time range of price doesn't cover market data")
-        length = data_length[0]
+
         # ensure data interval same
-        data_interval = []
-        if length > 1:
-            for market in self._broker.markets.values():
-                data_interval.append(market.data.index[1] - market.data.index[0])
-            if List.count(data_interval, data_interval[0]) != len(data_interval):
-                raise DemeterError("data interval among markets are not same")
-            price_interval = self._token_prices.index[1] - self._token_prices.index[0]
-            if price_interval != data_interval[0]:
-                raise DemeterError("price list interval and data interval are not same")
+        # length = data_length[0]
+        # data_interval = []
+        # if length > 1:
+        #     for market in self._broker.markets.values():
+        #         data_interval.append(market.data.index[1] - market.data.index[0])
+        #     if List.count(data_interval, data_interval[0]) != len(data_interval):
+        #         raise DemeterError("data interval among markets are not same")
+        #     price_interval = self._token_prices.index[1] - self._token_prices.index[0]
+        #     if price_interval != data_interval[0]:
+        #         raise DemeterError("price list interval and data interval are not same")
 
     def __get_row_data(self, timestamp, row_id, current_price) -> RowData:
         row_data = RowData(timestamp.to_pydatetime(), row_id, current_price)
         for market_info, market in self.broker.markets.items():
             row_data.market_status[market_info] = market.market_status.data
         row_data.market_status.set_default_key(self.broker.markets.get_default_key())
         return row_data
 
-    def __set_row_to_markets(self, timestamp: Timestamp, update: bool = False):
+    def __set_market_timestamp(self, timestamp: Timestamp, update: bool = False):
         """
         set markets row data
         :param timestamp:
-        :param market_row_dict:
         :param update: enable or disable has_update flag in markets, if set to false, will always update, if set to true, just update when necessary
         :return:
         """
 
         for market_key in self.broker.markets.keys():
             if (not update) or (update and self._broker.markets[market_key].has_update):
                 ms = MarketStatus(timestamp, None)
                 self._broker.markets[market_key].set_market_status(ms, self._token_prices.loc[timestamp])
 
+    def get_test_range(self):
+        longest_data = max(map(lambda m: len(m.data.index.get_level_values(0).unique()), self._broker.markets.values()))
+        largest_market = list(
+            filter(
+                lambda m: len(m.data.index.get_level_values(0).unique()) == longest_data, self._broker.markets.values()
+            )
+        )[0]
+        # start = largest_market.data.head(1).index.get_level_values(0).unique()
+        # end = largest_market.data.tail(1).index.get_level_values(0).unique()
+
+        return largest_market.data.index.get_level_values(0).unique()
+
     def run(self, evaluator: List[EvaluatorEnum] | None = None, output: bool = True):
         """
         Start back test, the whole process including:
 
         * reset actuator
         * initialize strategy (set object to strategy, then run strategy.initialize())
         * process each row in data
@@ -356,66 +349,80 @@
         """
         evaluator = evaluator if evaluator is not None else []
         run_begin_time = time.time()  # 1681718968.267463
         self.reset()
 
         self._enabled_evaluator = evaluator
         self._check_backtest()
-        index_array: pd.DatetimeIndex = list(self._broker.markets.values())[0].data.index
+        index_array: pd.DatetimeIndex = (
+            self.get_test_range()
+        )  # list(self._broker.markets.values())[0].data.index.get_level_values(0).unique()
         self.logger.info("init strategy...")
 
         # set initial status for strategy, so user can run some calculation in initial function.
-        self.__set_row_to_markets(index_array[0], False)
+        self.__set_market_timestamp(index_array[0], False)
+        self._currents.timestamp = index_array[0].to_pydatetime()
         # keep initial balance for evaluating
-        init_account_status = self._broker.get_account_status(self._token_prices.head(1).iloc[0])
+        init_account_status = self._broker.get_account_status(
+            self._token_prices.head(1).iloc[0], index_array[0].to_pydatetime()
+        )
         self.init_strategy()
         row_id = 0
         data_length = len(index_array)
         self.logger.info("start main loop...")
         with tqdm(total=data_length, ncols=150) as pbar:
             for timestamp_index in index_array:
                 current_price = self._token_prices.loc[timestamp_index]
                 # prepare data of a row
 
-                self.__set_row_to_markets(timestamp_index, False)
+                self.__set_market_timestamp(timestamp_index, False)
                 # execute strategy, and some calculate
                 self._currents.timestamp = timestamp_index.to_pydatetime()
                 row_data = self.__get_row_data(timestamp_index, row_id, current_price)
                 if self._strategy.triggers:
                     for trigger in self._strategy.triggers:
                         if trigger.when(row_data):
                             trigger.do(row_data)
+
+                for market in self.broker.markets.values():
+                    if market.is_open and market.open is not None:
+                        market.open(row_data)
+
                 self._strategy.on_bar(row_data)
 
                 # important, take uniswap market for example,
                 # if liquidity has changed in the head of this minute, this will add the new liquidity to total_liquidity in current minute.
-                self.__set_row_to_markets(timestamp_index, True)
+                self.__set_market_timestamp(timestamp_index, True)
 
                 # update broker status, e.g. re-calculate fee
                 # and read the latest status from broker
                 for market in self._broker.markets.values():
                     market.update()
 
                 row_data = self.__get_row_data(timestamp_index, row_id, current_price)
                 self._strategy.after_bar(row_data)
 
-                self._account_status_list.append(self._broker.get_account_status(current_price, timestamp_index))
+                self._account_status_list.append(
+                    self._broker.get_account_status(current_price, timestamp_index.to_pydatetime())
+                )
                 # notify actions in current loop
                 self.notify(self.strategy, self._currents.actions)
                 self._currents.actions = []
                 # move forward for process bar and index
                 pbar.update()
                 row_id += 1
 
         self.logger.info("main loop finished")
         self._account_status_df: pd.DataFrame = self.get_account_status_dataframe()
 
         if len(self._enabled_evaluator) > 0:
             self.logger.info("Start calculate evaluating indicator...")
-            self._evaluator = Evaluator(init_account_status, self._account_status_df, self._token_prices, self.actions)
+            self._evaluator = Evaluator(
+                init_account_status, self._account_status_df, self._token_prices, self._broker.markets
+            )
             self._evaluator.run(self._enabled_evaluator)
             self.logger.info("Evaluating indicator has finished it's job.")
         self._strategy.finalize()
         self.__backtest_finished = True
         if output:
             self.output()
 
@@ -431,15 +438,15 @@
         """
         if not self.__backtest_finished:
             raise DemeterError("Please run strategy first")
         self.logger.info(f"Print actuator summary")
         print(get_formatted_predefined("Final account status", STYLE["header1"]))
         print(self.broker.formatted_str())
         print(get_formatted_predefined("Account balance history", STYLE["header1"]))
-        print(self._account_status_df)
+        console_text.print_dataframe_with_precision(self._account_status_df)
         if len(self._enabled_evaluator) > 0:
             print("Evaluating indicator")
             print(self._evaluator)
 
     def save_result(self, path: str, account=True, actions=True) -> List[str]:
         """
         Save backtesting result
@@ -507,24 +514,29 @@
     def __str__(self):
         return '{{"Account status":{}, "action_count":{}, "timestamp":"{}", "strategy":"{}", "price_df_rows":{}, "price_assets":{} }}'.format(
             str(self.broker),
             len(self._action_list),
             self._currents.timestamp,
             type(self._strategy).__name__,
             len(self._token_prices.index) if self._token_prices is not None else 0,
-            "[" + ",".join(f'"{x}"' for x in self._token_prices.columns) + "]" if self._token_prices is not None else str([]),
+            (
+                "[" + ",".join(f'"{x}"' for x in self._token_prices.columns) + "]"
+                if self._token_prices is not None
+                else str([])
+            ),
         )
 
 
 @dataclass
 class Currents:
     """
     Values in current timestamp.
 
     """
+
     actions: List[BaseAction] = field(default_factory=list)
     """Actions in this iteration"""
     timestamp: datetime = None
     """Current timestamp"""
 
 
 def _json_default(obj):
@@ -532,13 +544,15 @@
     format json data
 
     :param obj:
     :return:
     """
     if isinstance(obj, UnitDecimal):
         return obj.to_str()
+    elif isinstance(obj, Decimal):
+        return str(obj)
     elif isinstance(obj, MarketInfo):
-        return {"name": obj.name}
+        return f"{obj.name}({obj.type.name})"
     elif isinstance(obj, PositionInfo):
         return {"lower_tick": obj.lower_tick, "upper_tick": obj.upper_tick}
     else:
         raise TypeError
```

### Comparing `zelos-demeter-0.3.0/demeter/core/evaluating_indicator.py` & `zelos-demeter-0.5.1/demeter/core/evaluating_indicator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Dict, List
 
 import pandas as pd
 
 from .._typing import UnitDecimal, DemeterError, EvaluatorEnum
 from ..broker import AccountStatus, AccountStatusCommon
+from ..broker._typing import MarketDict
 from .math_helper import max_draw_down_fast, annualized_returns, get_benchmark_returns
 
 
 class Evaluator(object):
     """
     Calculate evaluator indicator for strategy.
 
@@ -17,24 +18,24 @@
     :type data: DataFrame
     :param prices: dataframe of AccountStatusCommon
     :type prices: DataFrame
     :param actions: all actions during backtest
     :type actions: List
     """
 
-    def __init__(self, init_status: AccountStatus, data: pd.DataFrame, prices: pd.DataFrame, actions: List):
+    def __init__(self, init_status: AccountStatus, data: pd.DataFrame, prices: pd.DataFrame, markets: MarketDict):
         """
         init Evaluator
 
         """
         self.init_status: AccountStatus = init_status
         self.end_status: AccountStatusCommon = data.iloc[-1]
         self.prices: pd.DataFrame = prices
         self.data: pd.DataFrame = data
-        self.actions = actions
+        self.markets = markets
         if len(data) < 2:
             raise DemeterError("not enough data")
         self.time_span_in_day = len(data.index) * (data.index[1] - data.index[0]).seconds / (60 * 60 * 24)
         self._result = None
 
     def run(self, enables: List[EvaluatorEnum]) -> Dict[EvaluatorEnum, UnitDecimal]:
         """
@@ -73,36 +74,60 @@
                 case EvaluatorEnum.max_draw_down:
                     result = UnitDecimal(max_draw_down_fast(self.data.net_value), "")
                 case EvaluatorEnum.net_value:
                     result = UnitDecimal(self.end_status.net_value / self.init_status.net_value)
                 case EvaluatorEnum.profit:
                     result = UnitDecimal(self.end_status.net_value - self.init_status.net_value)
                 case EvaluatorEnum.net_value_up_down_rate:
-                    result = UnitDecimal((self.end_status.net_value - self.init_status.net_value) / self.init_status.net_value)
+                    result = UnitDecimal((self.end_status.net_value - self.init_status.net_value) /
+                                         self.init_status.net_value)
                 case EvaluatorEnum.eth_up_down_rate:
-                    result = UnitDecimal((self.prices.iloc[-1]["ETH"] - self.prices.iloc[0]["ETH"]) / self.prices.iloc[0]["ETH"])
+                    result = UnitDecimal((self.prices.iloc[-1]["ETH"] - self.prices.iloc[0]["ETH"]) /
+                                         self.prices.iloc[0]["ETH"])
                 case EvaluatorEnum.position_fee_profit:
-                    fee_df = self.data[["market1_base_uncollected", "market1_quote_uncollected"]]
-                    fee_df.sort_values(by=["market1_base_uncollected", "market1_quote_uncollected"], ascending=[False, False], inplace=True)
-                    fee_price_df = pd.merge(fee_df, self.prices, how="left", left_index=True, right_index=True)
-                    latest_fee = fee_price_df.iloc[0]
-                    fee_value = latest_fee["market1_base_uncollected"] * latest_fee["ETH"] + latest_fee["market1_quote_uncollected"]
+                    fee_value = UnitDecimal(0)
+                    for _, market in self.markets.items():
+                        fee_df = self.data[[f"{market.market_info.name}_base_uncollected",
+                                            f"{market.market_info.name}_quote_uncollected"]]
+                        fee_df = fee_df.sort_values(by=[f"{market.market_info.name}_base_uncollected",
+                                                    f"{market.market_info.name}_quote_uncollected"],
+                                                    ascending=[False, False])
+                        fee_price_df = pd.merge(fee_df, self.prices, how="left", left_index=True, right_index=True)
+                        latest_fee = fee_price_df.iloc[0]
+                        fee_value += (latest_fee[f"{market.market_info.name}_base_uncollected"] +
+                                      latest_fee[f"{market.market_info.name}_quote_uncollected"] * latest_fee["ETH"])
                     result = UnitDecimal(fee_value)
                 case EvaluatorEnum.position_fee_annualized_returns:
-                    fee_df = self.data[(self.data["market1_base_uncollected"] > 0) | (self.data["market1_quote_uncollected"] > 0)]
-                    fee_df = fee_df[["market1_base_uncollected", "market1_quote_uncollected"]]
-                    fee_df.sort_values(by=["market1_base_uncollected", "market1_quote_uncollected"], ascending=[False, False], inplace=True)
-                    fee_price_df = pd.merge(fee_df, self.prices, how="left", left_index=True, right_index=True)
-                    latest_fee = fee_price_df.iloc[0]
-                    fee_value = latest_fee["market1_base_uncollected"] * latest_fee["ETH"] + latest_fee["market1_quote_uncollected"]
-                    fee_annualized_returns = (fee_value / self.init_status.net_value) * UnitDecimal(len(fee_df) / len(self.data) * 365)
-                    result = UnitDecimal(fee_annualized_returns)
+                    fee_value = UnitDecimal(0)
+                    for _, market in self.markets.items():
+                        fee_df = self.data[(self.data[f"{market.market_info.name}_base_uncollected"] > 0) |
+                                           (self.data[f"{market.market_info.name}_quote_uncollected"] > 0)]
+                        fee_df = fee_df[[f"{market.market_info.name}_base_uncollected",
+                                         f"{market.market_info.name}_quote_uncollected"]]
+                        if not fee_df.empty:
+                            fee_df = fee_df.sort_values(by=[f"{market.market_info.name}_base_uncollected",
+                                                            f"{market.market_info.name}_quote_uncollected"],
+                                                        ascending=[False, False])
+                            fee_price_df = pd.merge(fee_df, self.prices, how="left", left_index=True, right_index=True)
+                            latest_fee = fee_price_df.iloc[0]
+                            fee_value = (latest_fee[f"{market.market_info.name}_base_uncollected"] +
+                                         latest_fee[f"{market.market_info.name}_quote_uncollected"] * latest_fee["ETH"])
+                            fee_annualized_returns = ((fee_value / self.init_status.net_value) *
+                                                      UnitDecimal(len(fee_df) / len(self.data) * 365))
+                            fee_value += UnitDecimal(fee_annualized_returns)
+                        else:
+                            fee_value += UnitDecimal(0)
+                    result = fee_value
                 case EvaluatorEnum.position_market_time_rate:
-                    fee_df = self.data[(self.data["market1_base_uncollected"] > 0) | (self.data["market1_quote_uncollected"] > 0)]
-                    result = UnitDecimal(len(fee_df) / len(self.data))
+                    market_time_rate = UnitDecimal(0)
+                    for _, market in self.markets.items():
+                        fee_df = self.data[(self.data[f"{market.market_info.name}_base_uncollected"] > 0) |
+                                           (self.data[f"{market.market_info.name}_quote_uncollected"] > 0)]
+                        market_time_rate += UnitDecimal(len(fee_df) / len(self.data))
+                    result = market_time_rate
                 case _:
                     raise DemeterError(f"{request} has not implied")
             result_dict[request] = result
         self._result = result_dict
         return result_dict
 
     @property
@@ -117,9 +142,9 @@
 
     def __str__(self):
         """
         Evaluator print function
         """
         str_array = []
         for k, v in self._result.items():
-            str_array.append(f"{k.name}:{v}")
-        return "; ".join(str_array)
+            str_array.append(f"{k.name:<35}:{v:.15}")
+        return ";\n".join(str_array)
```

### Comparing `zelos-demeter-0.3.0/demeter/core/math_helper.py` & `zelos-demeter-0.5.1/demeter/core/math_helper.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.3.0/demeter/indicator/common.py` & `zelos-demeter-0.5.1/demeter/indicator/common.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.3.0/demeter/indicator/ma.py` & `zelos-demeter-0.5.1/demeter/indicator/ma.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 def simple_moving_average(
     data: pd.Series | pd.DataFrame,
     window: timedelta = timedelta(hours=5),
     min_periods: int | None = None,
     center: bool = False,
     win_type: str | None = None,
     on: str | None = None,
-    axis: Axis = 0,
     closed: str | None = None,
     method: str = "single",
 ) -> pd.Series:
     """
     calculate simple moving average, Note: window is based on time span
 
     docs for other params, see https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.rolling.html
@@ -34,30 +33,28 @@
 
     return data.rolling(
         window=get_real_n(data, window),
         min_periods=min_periods,
         center=center,
         win_type=win_type,
         on=on,
-        axis=axis,
         closed=closed,
         method=method,
     ).mean()
 
 
 def exponential_moving_average(
     data: pd.Series | pd.DataFrame,
     com: float | None = None,
     span: float | None = None,
     halflife: float | TimedeltaConvertibleTypes | None = None,
     alpha: float | None = None,
     min_periods: int | None = 0,
     adjust: bool = True,
     ignore_na: bool = False,
-    axis: Axis = 0,
     times: str | np.ndarray | pd.DataFrame | pd.Series | None = None,
     method: str = "single",
 ):
     """
     calculate exponential moving average, just a shortcut for pandas.evm().mean()
 
     docs for params, see: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.ewm.html
@@ -66,11 +63,10 @@
         com=com,
         span=span,
         halflife=halflife,
         alpha=alpha,
         min_periods=min_periods,
         adjust=adjust,
         ignore_na=ignore_na,
-        axis=axis,
         times=times,
         method=method,
     ).mean()
```

### Comparing `zelos-demeter-0.3.0/demeter/indicator/volatility.py` & `zelos-demeter-0.5.1/demeter/indicator/volatility.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.3.0/demeter/strategy/strategy.py` & `zelos-demeter-0.5.1/demeter/strategy/strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     Parent class of strategy, all user's strategy should inherit this class
     """
 
     def __init__(self):
         self.broker: Broker | None = None
         self.data: MarketDict[pd.DataFrame] = MarketDict()
         self.markets: MarketDict[Market] = MarketDict()
-        self.number_format = ".8g"
         self.prices: pd.DataFrame | None = None
         self.triggers: [Trigger] = []
         self.account_status: List[AccountStatus] = []
         self.assets: AssetDict[Asset] = AssetDict()
         self.actions: List[BaseAction] = []
 
     def initialize(self):
```

### Comparing `zelos-demeter-0.3.0/demeter/strategy/trigger.py` & `zelos-demeter-0.5.1/demeter/strategy/trigger.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.3.0/demeter/uniswap/_typing.py` & `zelos-demeter-0.5.1/demeter/uniswap/_typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Dict, NamedTuple, Union
 
 import pandas as pd
 
 from .._typing import TokenInfo, UnitDecimal
 from ..broker import BaseAction, ActionTypeEnum, MarketBalance, MarketStatus
 from ..utils import get_formatted_from_dict
+from ..utils import console_text
 
 
 class PositionInfo(NamedTuple):
     """
     get_position information, including tick range and liquidity. It contains immutable properties of a get_position, and used as a key for get_position dict
 
     :param lower_tick: lower tick
@@ -51,34 +52,34 @@
 
     :param token0: First token in  pool contract.
     :type token0:  TokenInfo
     :param token1: Second token in  pool contract.
     :type token1: TokenInfo
     :param fee: fee rate of this pool, should be among [0.05, 0.3, 1]
     :type fee: float, 0.05
-    :param base_token: which token will be considered as base token. e.g. to a token pair of USDT/BTC, if you want price unit to be like 10000 usdt/btc, you should set usdt as base token, otherwise if price unit is 0.00001 btc/usdt, you should set btc as base token
-    :type base_token: TokenInfo
+    :param quote_token: which token will be considered as base token. e.g. to a token pair of USDT/BTC, if you want price unit to be like 10000 usdt/btc, you should set usdt as base token, otherwise if price unit is 0.00001 btc/usdt, you should set btc as base token
+    :type quote_token: TokenInfo
     """
 
-    def __init__(self, token0: TokenInfo, token1: TokenInfo, fee: float, base_token: TokenInfo):
+    def __init__(self, token0: TokenInfo, token1: TokenInfo, fee: float, quote_token: TokenInfo):
         fee = Decimal(str(fee))
         self.token0 = token0
         self.token1 = token1
-        self.is_token0_base = base_token == token0
-        self.base_token = base_token
+        self.is_token0_quote = quote_token == token0
+        self.quote_token = quote_token
         self.tickSpacing = int(fee * 200)
         self.fee: Decimal = fee * Decimal(10000)
         self.fee_rate: Decimal = Decimal(fee) / Decimal(100)
 
     def __str__(self):
         return (
             "PoolBaseInfo(Token0: {},".format(self.token0)
             + "Token1: {},".format(self.token1)
-            + "fee: {},".format(self.fee_rate * Decimal(100))
-            + "base token: {})".format(self.token0.name if self.is_token0_base else self.token1.name)
+            + "fee: {}%,".format(self.fee_rate * Decimal(100))
+            + "base token: {})".format(self.token0.name if self.is_token0_quote else self.token1.name)
         )
 
     def __repr__(self):
         return self.__str__()
 
 
 @dataclass
@@ -205,29 +206,30 @@
     """
     keeps variables for get_position
     """
 
     pending_amount0: Decimal
     pending_amount1: Decimal
     liquidity: int
+    transferred: bool = False  # this position(nft) has been transferred, so owner is not current user.
 
 
 def position_dict_to_dataframe(positions: Dict[PositionInfo, Position]) -> pd.DataFrame:
     pos_dict = {
         "lower_tick": [],
         "upper_tick": [],
         "pending0": [],
         "pending1": [],
         "liquidity": [],
     }
     for k, v in positions.items():
         pos_dict["lower_tick"].append(k.lower_tick)
         pos_dict["upper_tick"].append(k.upper_tick)
-        pos_dict["pending0"].append(v.pending_amount0)
-        pos_dict["pending1"].append(v.pending_amount1)
+        pos_dict["pending0"].append(console_text.format_value(v.pending_amount0))
+        pos_dict["pending1"].append(console_text.format_value(v.pending_amount1))
         pos_dict["liquidity"].append(v.liquidity)
     return pd.DataFrame(pos_dict)
 
 
 @dataclass
 class UniV3PoolStatus:
     """
@@ -430,14 +432,56 @@
                 "removed liquidity": self.removed_liquidity,
                 "remain liquidity": self.remain_liquidity,
             }
         )
 
 
 @dataclass
+class SwapAction(BaseAction):
+    """
+    buy token, swap from base token to quote token.
+
+    :param amount: amount to buy(in quote token)
+    :type amount: UnitDecimal
+    :param price: price,
+    :type price: UnitDecimal
+    :param fee: fee paid (in base token)
+    :type fee: UnitDecimal
+    :param base_change: base token amount changed
+    :type base_change: PositionInfo
+    :param quote_change: quote token amount changed
+    :type quote_change: UnitDecimal
+
+    """
+
+    amount: UnitDecimal
+    price: UnitDecimal
+    fee: UnitDecimal
+    to_amount: UnitDecimal
+
+    def set_type(self):
+        self.action_type = ActionTypeEnum.uni_lp_swap
+
+    def get_output_str(self) -> str:
+        """
+        get colored and formatted string to output in console
+
+        :return: formatted string
+        :rtype: str
+        """
+        return f"""\033[1;36m{"Swap":<20}\033[0m""" + get_formatted_from_dict(
+            {
+                "price": self.price.to_str(),
+                "fee": self.fee.to_str(),
+                "amount": f"{self.amount.to_str()}->{self.to_amount.to_str()}",
+            }
+        )
+
+
+@dataclass
 class BuyAction(UniLpBaseAction):
     """
     buy token, swap from base token to quote token.
 
     :param amount: amount to buy(in quote token)
     :type amount: UnitDecimal
     :param price: price,
```

### Comparing `zelos-demeter-0.3.0/demeter/uniswap/core.py` & `zelos-demeter-0.5.1/demeter/uniswap/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from decimal import Decimal
 
 from ._typing import UniV3Pool, Position, UniV3PoolStatus, PositionInfo
-from .helper import quote_price_to_tick, from_wei
+from .helper import base_unit_price_to_tick, from_atomic_unit
 from .liquitidy_math import get_amounts, get_liquidity
 
 
 class V3CoreLib(object):
     @staticmethod
     def new_position(
         pool: UniV3Pool,
@@ -93,26 +93,27 @@
         quote price pair to tick
 
         :param pool: operation on which pool
         :param lower_quote_price: lower quote price
         :param upper_quote_price: upper quote price
         :return: lower_tick, upper_tick
         """
-        lower_tick = quote_price_to_tick(
+        lower_tick = base_unit_price_to_tick(
             lower_quote_price,
             pool.token0.decimal,
             pool.token1.decimal,
-            pool.is_token0_base,
+            pool.is_token0_quote,
         )
-        upper_tick = quote_price_to_tick(
+        upper_tick = base_unit_price_to_tick(
             upper_quote_price,
             pool.token0.decimal,
             pool.token1.decimal,
-            pool.is_token0_base,
+            pool.is_token0_quote,
         )
+        lower_tick, upper_tick = (lower_tick, upper_tick) if not pool.is_token0_quote else (upper_tick,lower_tick)
         return lower_tick, upper_tick
 
     @staticmethod
     def update_fee(last_tick:int,pool: UniV3Pool, pos: PositionInfo, position: Position, state: UniV3PoolStatus):
         """
         update fee
 
@@ -123,16 +124,16 @@
         :param last_tick:
         :return: None
         """
 
         # in most cases, tick will not cross to on_bar one, which means L will not change.
         def calc_amounts():
             share = Decimal(position.liquidity) / Decimal(state.currentLiquidity)
-            position.pending_amount0 += from_wei(state.inAmount0, pool.token0.decimal) * share * pool.fee_rate
-            position.pending_amount1 += from_wei(state.inAmount1, pool.token1.decimal) * share * pool.fee_rate
+            position.pending_amount0 += from_atomic_unit(state.inAmount0, pool.token0.decimal) * share * pool.fee_rate
+            position.pending_amount1 += from_atomic_unit(state.inAmount1, pool.token1.decimal) * share * pool.fee_rate
 
         condition_in_position = pos.upper_tick >= state.closeTick >= pos.lower_tick
         if last_tick:
             condition_over_position = (last_tick > pos.upper_tick and state.closeTick < pos.lower_tick) or (
                     state.closeTick > pos.upper_tick and last_tick < pos.lower_tick
             )
             condition_in_to_out_position = pos.upper_tick >= last_tick >= pos.lower_tick and (
```

### Comparing `zelos-demeter-0.3.0/demeter/uniswap/data.py` & `zelos-demeter-0.5.1/demeter/uniswap/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,52 +95,43 @@
     else:
         return EMPTY_RULE
 
 
 def resample(
     df: pd.DataFrame,
     rule,
-    axis=0,
     closed: str | None = None,
     label: str | None = None,
-    convention: str = "start",
-    kind: str | None = None,
     on=None,
     level=None,
     origin: str | pd_typing.TimestampConvertibleTypes = "start_day",
     offset: pd_typing.TimedeltaConvertibleTypes | None = None,
     agg: Dict[str, str] = None,
     group_keys: bool = False,
 ) -> pd.DataFrame:
     """
     resample data
 
     :param df: data in dataframe
     :param rule: resample rule, see Dataframe.resample doc
-    :param axis: resample axis, see Dataframe.resample doc
     :param closed: resample closed, see Dataframe.resample doc
     :param label: resample label, see Dataframe.resample doc
-    :param convention: resample convention, see Dataframe.resample doc
-    :param kind: resample kind, see Dataframe.resample doc
     :param on: resample on, see Dataframe.resample doc
     :param level: resample level, see Dataframe.resample doc
     :param origin: resample origin, see Dataframe.resample doc
     :param offset: resample offset, see Dataframe.resample doc
     :param group_keys: resample group_keys, see Dataframe.resample doc
     :param agg: aggregate method
     :return: aggregated dataframe
     """
     agg = agg if agg else {}
     resampler = df.resample(
         rule=rule,
-        axis=axis,
         closed=closed,
         label=label,
-        convention=convention,
-        kind=kind,
         on=on,
         level=level,
         origin=origin,
         offset=offset,
         group_keys=group_keys,
     )
     agg_dict = {}
@@ -160,40 +151,40 @@
 def fillna(
     df: pd.DataFrame,
     value: object | pd_typing.ArrayLike | None = None,
     method: pd_typing.FillnaOptions | None = None,
     axis: pd_typing.Axis | None = None,
     inplace: bool = False,
     limit=None,
-    downcast=None,
 ) -> pd.DataFrame | None:
     """
     fill empty item. param is the same to pandas.Series.fillna
 
     if column name is predefined, method and value will be omitted, and data will be filled as predefined
 
     """
     new_df = df.copy(False)
 
     # fill close tick first, it will be used later.
     if LineTypeEnum.closeTick.name in new_df.columns:
-        new_df[LineTypeEnum.closeTick.name] = new_df[LineTypeEnum.closeTick.name].fillna(
-            value=None,
+        new_df[LineTypeEnum.closeTick.name] = df_fill_na(
+            new_df[LineTypeEnum.closeTick.name],
             method=get_line_rules_safe(LineTypeEnum.closeTick.name).fillna_method,
             axis=axis,
             inplace=inplace,
             limit=limit,
-            downcast=downcast,
         )
     for column_name in new_df.columns:
         if column_name == LineTypeEnum.closeTick.name:
             continue
         rule = get_line_rules_safe(column_name)
         if rule.fillna_method is None and rule.fillna_value is None:
-            new_df[column_name] = new_df[column_name].fillna(value=value, method=method, axis=axis, inplace=inplace, limit=limit, downcast=downcast)
+            new_df[column_name] = df_fill_na(
+                new_df[column_name], value=value, method=method, axis=axis, inplace=inplace, limit=limit
+            )
         else:
             current_method = rule.fillna_method if rule.fillna_method else method
             current_value = rule.fillna_value if rule.fillna_value is not None else value
             # all tick related field will be filled with close_tick.
             if (
                 column_name
                 in [
@@ -201,16 +192,34 @@
                     LineTypeEnum.highestTick.name,
                     LineTypeEnum.lowestTick.name,
                 ]
                 and LineTypeEnum.closeTick.name in new_df.columns
             ):
                 current_method = None
                 current_value = new_df[LineTypeEnum.closeTick.name]
-            new_df[column_name] = new_df[column_name].fillna(
+            new_df[column_name] = df_fill_na(
+                new_df[column_name],
                 value=current_value,
                 method=current_method,
                 axis=axis,
                 inplace=inplace,
                 limit=limit,
-                downcast=downcast,
             )
     return new_df
+
+
+def df_fill_na(
+    df: pd.DataFrame,
+    value=None,
+    method: pd_typing.FillnaOptions | None = None,
+    axis: pd_typing.Axis | None = None,
+    inplace: bool = False,
+    limit: int | None = None,
+) -> pd.DataFrame:
+    if value is not None:
+        return df.fillna(value=value, axis=axis, inplace=inplace, limit=limit)
+    elif method == "ffill":
+        return df.ffill(axis=axis, inplace=inplace, limit=limit)
+    elif method == "bfill":
+        return df.bfill(axis=axis, inplace=inplace, limit=limit)
+    else:
+        raise ValueError(f"{method} is not supported, use bfill or ffill")
```

### Comparing `zelos-demeter-0.3.0/demeter/uniswap/helper.py` & `zelos-demeter-0.5.1/demeter/uniswap/helper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,224 +1,240 @@
 import math
-from decimal import Decimal
+from decimal import Decimal, getcontext
 from typing import Tuple
 
 from .liquitidy_math import get_sqrt_ratio_at_tick
 
+Q96 = Decimal(2**96)
+SQRT_1p0001 = math.sqrt(Decimal(1.0001))
+getcontext().prec = 35  # default is 28, 33 is good enough for 3000
 
-def _x96_to_decimal(number: int):
+
+def _from_x96(number: int) -> Decimal:
     """
     decimal divide 2 ** 96
 
-    :param number: sqrt x96 price
-    :return: result
+    :param number: sqrted x96 price
+    :return: sqrted price
     """
-    return Decimal(number) / 2**96
+    return Decimal(number) / Q96
 
 
-def decimal_to_x96(number: Decimal):
+def _to_x96(sqrt_price: Decimal) -> int:
     """
     decimal multiple 2 ** 96
 
-    :param number: decimal price
+    :param sqrt_price: price in base unit
     :return: result
     """
-    return int(Decimal(number) * 2**96)
+    if not isinstance(sqrt_price, Decimal):
+        sqrt_price = Decimal(sqrt_price)
+    return int(sqrt_price * Q96)
 
 
-def _x96_sqrt_to_decimal(sqrt_priceX96, token_decimal_diff=12):
+def sqrt_price_x96_to_base_unit_price(
+    sqrt_price_x96, token_0_decimal: int, token_1_decimal: int, is_token0_quote: bool
+) -> Decimal:
     """
     convert sqrt x96 price to decimal
 
-    :param sqrt_priceX96: sqrt x96 price
-    :param token_decimal_diff: decimal different between two tokens
-    :return: decimal price
+    :param sqrt_price_x96: sqrt x96 price
+    :param token_0_decimal: decimal of token 0
+    :param token_1_decimal: decimal of token 1
+    :param is_token0_quote: is token 0 the quote token
+    :return: price in base unit, e.g. 1234.56 eth/usdc
     """
-    price = _x96_to_decimal(sqrt_priceX96)
-    return (price**2) / 10**token_decimal_diff
+    sqrt_price = _from_x96(sqrt_price_x96)
+    pool_price = sqrt_price**2 * Decimal(10 ** (token_0_decimal - token_1_decimal))
+
+    return Decimal(1 / pool_price) if is_token0_quote else pool_price
 
 
-## can round by spacing?
-def sqrt_price_to_tick(sqrt_priceX96: int) -> int:
+def base_unit_price_to_sqrt_price_x96(
+    price: Decimal, token_0_decimal: int, token_1_decimal: int, is_token0_quote: bool
+) -> int:
     """
-    convert sqrt_priceX96 to tick data
+    convert quote price to sqrt
+
+    :param price: price in base/quote
+    :param token_0_decimal: token0 decimal
+    :param token_1_decimal: token1 decimal
+    :param is_token0_quote: token 0 is quote token
+    :return: sqrt price x96
+    """
+    # quote price->add decimal pool price->sqrt_price ->ticker
+
+    price = 1 / price if is_token0_quote else price
+    atomic_unit_price = price / Decimal(10 ** (token_0_decimal - token_1_decimal))
+    sqrt_price = Decimal.sqrt(atomic_unit_price)
+    return _to_x96(sqrt_price)
+
 
-    :param sqrt_priceX96: sqrt x96 price
+# can round by spacing?
+def sqrt_price_x96_to_tick(sqrt_price_x96: int) -> int:
+    """
+    convert sqrt_priceX96 to tick
+
+    :param sqrt_price_x96: sqrt x96 price
     :return: tick price
     """
-    decimal_price = _x96_to_decimal(sqrt_priceX96)
-    return pool_price_to_tick(decimal_price)
+    sqrt_price = _from_x96(sqrt_price_x96)
+    return _sqrt_price_to_tick(sqrt_price)
 
 
-def pool_price_to_tick(price_decimal: Decimal):
+def _sqrt_price_to_tick(sqrt_price: Decimal) -> int:
     """
     pool price to tick price
 
-    :param price_decimal: decimal price to tick price
+    :param sqrt_price: sqrt price
     :return: tick price
     """
-    return int(math.log(price_decimal, math.sqrt(1.0001)))
+    return int(math.log(sqrt_price, SQRT_1p0001))
 
 
-def tick_to_sqrtPriceX96(tick: int):
+def tick_to_sqrt_price_x96(tick: int) -> int:
     """
     convert tick data to sqrt X96 price
 
     :param tick: tick price
     :return: sqrt x96 price
     """
     return get_sqrt_ratio_at_tick(tick)
 
 
-def tick_to_quote_price(tick: int, token_0_decimal, token_1_decimal, is_token0_base: bool):
+def tick_to_base_unit_price(tick: int, token_0_decimal: int, token_1_decimal: int, is_token0_quote: bool):
     """
     get quote price from tick price
 
     :param tick: tick data
     :param token_0_decimal: token0 decimal
     :param token_1_decimal: token1 decimal
-    :param is_token0_base: base on token0
+    :param is_token0_quote: quote on token0
     :return: quote price
     """
-    sqrt_price = get_sqrt_ratio_at_tick(tick)
-    decimal_price = _x96_to_decimal(sqrt_price) ** 2
-    pool_price = decimal_price * Decimal(10 ** (token_0_decimal - token_1_decimal))
-    return Decimal(1 / pool_price) if is_token0_base else pool_price
+    sqrt_price_x96 = get_sqrt_ratio_at_tick(tick)
+    atomic_unit_price = _from_x96(sqrt_price_x96) ** 2
+    pool_price = atomic_unit_price * Decimal(10 ** (token_0_decimal - token_1_decimal))
+    return Decimal(1 / pool_price) if is_token0_quote else pool_price
 
 
-def quote_price_to_tick(based_price: Decimal, token_0_decimal: int, token_1_decimal: int, is_token_base) -> int:
+def base_unit_price_to_tick(price: Decimal, token_0_decimal: int, token_1_decimal: int, is_token0_quote: bool) -> int:
     """
     quote price to tick price
 
-    :param based_price: base price
+    :param price: price in base unit, e.g. 1234.56 eth/usdc
     :param token_0_decimal: token0 decimal
     :param token_1_decimal: token1 decimal
-    :param is_token_base: base on token
+    :param is_token0_quote: token 0 is quote token
     :return: tick price
     """
-    # quote price->add decimal pool price->sqrt_price ->ticker
-    sqrt_price = quote_price_to_sqrt(based_price, token_0_decimal, token_1_decimal, is_token_base)
-    tick = sqrt_price_to_tick(sqrt_price)
-    return tick
-
-
-def quote_price_to_sqrt(based_price: Decimal, token_0_decimal: int, token_1_decimal: int, is_token_base) -> int:
-    """
-    convert quote price to sqrt
-
-    :param based_price: price of base token
-    :param token_0_decimal: token 0 decimal
-    :param token_1_decimal: token 1 decimal
-    :param is_token_base: if is base token
-    :return: sqrt price
-    """
-    # quote price->add decimal pool price->sqrt_price ->ticker
 
-    price = 1 / based_price if is_token_base else based_price
-    pool_price = price / Decimal(10 ** (token_0_decimal - token_1_decimal))
-    decimal_price = Decimal.sqrt(pool_price)
-    return decimal_to_x96(decimal_price)
+    # quote price->add decimal pool price->sqrt_price ->tick
+    price = 1 / price if is_token0_quote else price
+    atomic_unit_price = price / Decimal(10 ** (token_0_decimal - token_1_decimal))
+    sqrt_price = Decimal.sqrt(atomic_unit_price)
+    return _sqrt_price_to_tick(sqrt_price)
 
 
-def from_wei(token_amt: int, decimal: int) -> Decimal:
+def from_atomic_unit(atomic_unit_amount: int, decimal: int) -> Decimal:
     """
     Convert token amount to wei
 
-    :param token_amt: token amount
+    :param atomic_unit_amount: token amount
     :param decimal: decimal of token
-    :return: token amount in wei
+    :return: token amount in base unit
     """
-    return Decimal(int(token_amt)) / Decimal(10**decimal)
+    return Decimal(int(atomic_unit_amount)) / Decimal(10**decimal)
 
 
 def get_delta_gamma(
     lower_price: float,
     upper_price: float,
     price: float,
     liquidity: int,
     decimal0: int,
     decimal1: int,
-    is_0_base: bool,
+    is_token0_quote: bool,
 ) -> Tuple[Decimal, Decimal]:
     """
     get delta gamma
 
     :param lower_price: lower price
     :param upper_price: upper price
     :param price: price
     :param liquidity: liquidity
     :param decimal0: decimal 0
     :param decimal1: decimal 1
-    :param is_0_base: check if token 0 is base
+    :param is_token0_quote: check if token 0 is quote
     :return: delta and gamma
     """
-    lower_price_sqrtX96 = quote_price_to_sqrt(Decimal(lower_price), decimal0, decimal1, is_0_base)
-    upper_price_sqrtX96 = quote_price_to_sqrt(Decimal(upper_price), decimal0, decimal1, is_0_base)
-    if lower_price_sqrtX96 > upper_price_sqrtX96:
-        (lower_price_sqrtX96, upper_price_sqrtX96) = (
-            upper_price_sqrtX96,
-            lower_price_sqrtX96,
+    lower_price_sqrt_x96 = base_unit_price_to_sqrt_price_x96(Decimal(lower_price), decimal0, decimal1, is_token0_quote)
+    upper_price_sqrt_x96 = base_unit_price_to_sqrt_price_x96(Decimal(upper_price), decimal0, decimal1, is_token0_quote)
+    if lower_price_sqrt_x96 > upper_price_sqrt_x96:
+        (lower_price_sqrt_x96, upper_price_sqrt_x96) = (
+            upper_price_sqrt_x96,
+            lower_price_sqrt_x96,
         )
-    return get_delta_gamma_sqrtX96(
+    return get_delta_gamma_sqrt_x96(
         lower_price,
-        lower_price_sqrtX96,
+        lower_price_sqrt_x96,
         upper_price,
-        upper_price_sqrtX96,
+        upper_price_sqrt_x96,
         price,
         liquidity,
         decimal0,
         decimal1,
-        is_0_base,
+        is_token0_quote,
     )
 
 
-def get_delta_gamma_sqrtX96(
+def get_delta_gamma_sqrt_x96(
     lower_price,
     sqrtA: int,
     upper_price,
     sqrtB: int,
     price,
     liquidity: int,
     d0: int,
     d1: int,
-    is_0_base: bool,
+    is_token0_quote: bool,
 ) -> Tuple[Decimal, Decimal]:
     """
     Get delta gamma in sqrtX96 price
 
     """
     """
     Delta is calculated by integrating net worth, and gamma is calculated by integrating delta,
     Therefore, the most important thing is to find the calculation formula of the net value (with tick range, price, and liquidity as parameters),
     and then derive the formula after integration
 
     The following comment indicates how to calculate net value.
 
     * a: amount
-    * p: decimal price in base token
+    * p: decimal price of base token
 
 
     k = 2 ** 96
     a0 = k * (10**(-d)) * Liquidity * (1/SqrtPrice - 1/upper_price_sqrtX96)
     a1= Liquidity / k / 10**d * (SqrtPrice - lower_price_sqrtX96)
 
 
-    if 0 base:
+    if 0 quote:
     SqrtPrice=k / (10 ** (d/2)) / (p**0.5)
     net_value = a1 * p                    price <= lower, a1 is constant
                 a0 + a1 * p               lower < price < upper
                 a0                        price >= upper, a0 is constant
 
     a0 + a1 * p = liquidity * 10 ** (0.5 * d) / 10 ** d0 * price_float ** 0.5 - \
               k / upper_sqrt * liquidity / 10 ** d0 + \
               liquidity*  price_float ** 0.5 / 10 ** d1 / 10 ** (0.5 * d) - \
               lower_sqrt / k * price_float * liquidity / 10 ** d1
 
 
-    if 1 base
+    if 1 quote
     SqrtPrice = k * p**0.5 / (10 ** (d/2))
 
     net_value = a0 * p                         price <= lower, a0 is constant
                 a0 * p + a1                    lower < price < upper
                 a1                             price >= upper, a1 is constant
 
     a0 * p + a1 = liquidity * price_float ** 0.5 * 10 ** (0.5 * d) / 10 ** d0 - \
@@ -229,15 +245,15 @@
 
 
     a0 + p * a1 =  Liquidity / 10**(d/2) / p**(1/2) + Liquidity * p**(1.5) / 10 ** (1.5*d) -
                    Liquidity * lower_price_sqrtX96 * p / 2**96 / 10**d
     """
     k = 2**96
     d = d0 - d1
-    if is_0_base:
+    if is_token0_quote:
         if price <= lower_price:
             delta = liquidity / 2**96 / 10**d1 * (sqrtB - sqrtA)
             gamma = 0
         elif lower_price < price < upper_price:
             m = 10 ** (0.5 * d)
             delta = liquidity * (0.5 * m / price**0.5 / 10**d0 + 0.5 / 10**d1 / m / price**0.5 - sqrtA / k / 10**d1)
             gamma = -0.25 * liquidity / price**1.5 * (m / 10**d0 + 1 / 10**d1 / m)
```

### Comparing `zelos-demeter-0.3.0/demeter/uniswap/liquitidy_math.py` & `zelos-demeter-0.5.1/demeter/uniswap/liquitidy_math.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.3.0/demeter/uniswap/market.py` & `zelos-demeter-0.5.1/demeter/uniswap/market.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import os
-from datetime import date, timedelta
+from datetime import date, timedelta, datetime, time
 from decimal import Decimal
-from typing import Dict
+from typing import Dict, Tuple
 
 import numpy as np
 import pandas as pd
 
 from ._typing import (
     UniV3Pool,
     TokenInfo,
@@ -17,26 +17,27 @@
     CollectFeeAction,
     BuyAction,
     SellAction,
     position_dict_to_dataframe,
     PositionInfo,
     UniDescription,
     UniswapMarketStatus,
+    SwapAction,
 )
 from .core import V3CoreLib
 from .data import fillna
 from .helper import (
-    tick_to_quote_price,
-    quote_price_to_tick,
-    quote_price_to_sqrt,
-    tick_to_sqrtPriceX96,
+    tick_to_base_unit_price,
+    base_unit_price_to_tick,
+    base_unit_price_to_sqrt_price_x96,
+    tick_to_sqrt_price_x96,
 )
 from .liquitidy_math import get_sqrt_ratio_at_tick
 from .._typing import DemeterError, DECIMAL_0, UnitDecimal
-from ..broker import MarketBalance, Market, MarketInfo, MarketStatus
+from ..broker import MarketBalance, Market, MarketInfo, MarketStatus, write_func
 from ..utils import (
     get_formatted_from_dict,
     get_formatted_predefined,
     STYLE,
     float_param_formatter,
     to_decimal,
 )
@@ -53,19 +54,21 @@
     :type pool_info: UniV3Pool
     :param data: pool data for back test. downloaded by demeter-fetch
     :type data: pd.DataFrame
     :param data_path: path to load pool data
     :type data_path: str
     """
 
-    def __init__(self, market_info: MarketInfo, pool_info: UniV3Pool, data: pd.DataFrame = None, data_path: str = "./data"):
+    def __init__(
+        self, market_info: MarketInfo, pool_info: UniV3Pool, data: pd.DataFrame = None, data_path: str = "./data"
+    ):
         super().__init__(market_info=market_info, data=data, data_path=data_path)
         self._pool: UniV3Pool = pool_info
         # init balance
-        self._is_token0_base = pool_info.is_token0_base
+        self._is_token0_quote = pool_info.is_token0_quote
         # reference for super().assets dict.
         self.base_token, self.quote_token = self._convert_pair(self.pool_info.token0, self.pool_info.token1)
         # status
         self._positions: Dict[PositionInfo, Position] = {}
         # In order to distinguish price in pool and to u, we call former one "pool price"
         self._pool_price_unit = f"{self.base_token.name}/{self.quote_token.name}"
         # internal temporary variable
@@ -76,15 +79,20 @@
     # region properties
 
     def __str__(self):
         return json.dumps(self.description._asdict())
 
     @property
     def description(self) -> UniDescription:
-        return UniDescription(type(self).__name__, self._market_info.name, len(self._positions), sum([p.liquidity for p in self._positions.values()]))
+        return UniDescription(
+            type(self).__name__,
+            self._market_info.name,
+            len(self._positions),
+            sum([p.liquidity for p in self._positions.values()]),
+        )
 
     @property
     def positions(self) -> Dict[PositionInfo, Position]:
         """
         current positions in broker
 
         :return: all positions
@@ -154,51 +162,50 @@
 
         :param market_status: market data
         :type market_status: UniswapMarketStatus
         :param price: price of token at this moment
         :type price: pd.Series
         """
         # update price tick
+        super().set_market_status(market_status, price)
+
         total_virtual_liq = sum([p.liquidity for p in self._positions.values()])
         self.last_tick = self._market_status.data.closeTick if "closeTick" in self._market_status.data.index else np.nan
 
         if market_status.data is None:
             market_status.data = self.data.loc[market_status.timestamp].copy()
         market_status.data.currentLiquidity = market_status.data.currentLiquidity + total_virtual_liq
         self._market_status = market_status
 
-        self._price_status = price
-        self.has_update = False
-
     def get_price_from_data(self) -> pd.DataFrame:
         """
         Extract token pair price from pool data.
 
         :return: a dataframe includes quote token price, and base token price will be set to 1
         :rtype: DataFrame
 
         """
         if self.data is None:
             raise DemeterError("data has not set")
         price_series: pd.Series = self.data.price
-        df = pd.DataFrame(index=price_series.index, data={self.quote_token.name: price_series})
-        df[self.base_token.name] = 1
+        df = pd.DataFrame(index=price_series.index, data={self.base_token.name: price_series})
+        df[self.quote_token.name] = 1
         return df
 
     def _convert_pair(self, any0, any1):
         """
-        convert order of token0/token1 to base_token/quote_token, according to self.is_token0_base.
+        convert order of token0/token1 to base_token/quote_token, according to self.is_token0_quote.
 
         Or convert order of base_token/quote_token to token0/token1
 
         :param any0: token0 or any property of token0, e.g. balance...
         :param any1: token1 or any property of token1, e.g. balance...
         :return: (base,qoute) or (token0,token1)
         """
-        return (any0, any1) if self._is_token0_base else (any1, any0)
+        return (any1, any0) if self._is_token0_quote else (any0, any1)
 
     def check_market(self):
         """
         Verify settings before backtest
         """
         super().check_market()
         required_columns = [
@@ -210,17 +217,17 @@
         ]
         for col in required_columns:
             assert col in self.data.columns
 
         if not self._pool:
             raise DemeterError("set up pool info first")
         if self.base_token not in self.broker.assets:
-            raise DemeterError(f"base token {self.base_token.name} not exist in asset dict")
+            self.broker.set_balance(self.base_token, DECIMAL_0)
         if self.quote_token not in self.broker.assets:
-            raise DemeterError(f"quote token {self.quote_token.name} not exist in asset dict")
+            self.broker.set_balance(self.quote_token, DECIMAL_0)
 
     def update(self):
         """
         re-calculate status.
         """
         self.__update_fee()
 
@@ -229,97 +236,126 @@
         update fee in all positions according to current status
 
         fee will be calculated by liquidity
         """
         for position_info, position in self._positions.items():
             V3CoreLib.update_fee(self.last_tick, self.pool_info, position_info, position, self.market_status.data)
 
+    def get_position_amount(self, position_info: PositionInfo) -> Tuple[Decimal, Decimal]:
+        if position_info not in self.positions:
+            return DECIMAL_0, DECIMAL_0
+        pool_price = self._market_status.data.price
+        sqrt_price = base_unit_price_to_sqrt_price_x96(
+            pool_price,
+            self._pool.token0.decimal,
+            self._pool.token1.decimal,
+            self._is_token0_quote,
+        )
+        position = self.positions[position_info]
+        amount0, amount1 = V3CoreLib.get_token_amounts(self._pool, position_info, sqrt_price, position.liquidity)
+        return amount0, amount1
+
     def get_market_balance(self, external_prices: pd.Series | Dict[str, Decimal] = None) -> MarketBalance:
         """
         get current status, including positions, balances
 
         :param external_prices: current price, used for calculate get_position value and net value, if set to None, will use token pair price of this pool
         :type external_prices: pd.Series | Dict[str, Decimal]
 
         :return: MarketBalance
         """
         pool_price = self._market_status.data.price
         if external_prices is None:
             if self._price_status is None:
-                external_prices = {self.base_token.name: Decimal(1), self.quote_token.name: pool_price}
+                external_prices = {self.quote_token.name: Decimal(1), self.base_token.name: pool_price}
             else:
                 external_prices = self._price_status
 
-        sqrt_price = quote_price_to_sqrt(
+        sqrt_price = base_unit_price_to_sqrt_price_x96(
             pool_price,
             self._pool.token0.decimal,
             self._pool.token1.decimal,
-            self._is_token0_base,
+            self._is_token0_quote,
         )
         base_fee_sum = Decimal(0)
         quote_fee_sum = Decimal(0)
         deposit_amount0 = Decimal(0)
         deposit_amount1 = Decimal(0)
         for position_info, position in self._positions.items():
+            if position.transferred:
+                continue
             base_fee, quote_fee = self._convert_pair(position.pending_amount0, position.pending_amount1)
             base_fee_sum += base_fee
             quote_fee_sum += quote_fee
             amount0, amount1 = V3CoreLib.get_token_amounts(self._pool, position_info, sqrt_price, position.liquidity)
             deposit_amount0 += amount0
             deposit_amount1 += amount1
 
         base_deposit_amount, quote_deposit_amount = self._convert_pair(deposit_amount0, deposit_amount1)
-        # net value here is calculated by external price, because we usually want a net value with usd base,
+        # net value here is calculated by external price, If you want a net value with usd base,
         net_value = (base_fee_sum + base_deposit_amount) * external_prices[self.base_token.name] + (
             quote_fee_sum + quote_deposit_amount
         ) * external_prices[self.quote_token.name]
 
         val = UniLpBalance(
             net_value=net_value,
             base_uncollected=UnitDecimal(base_fee_sum, self.base_token.name),
             quote_uncollected=UnitDecimal(quote_fee_sum, self.quote_token.name),
             base_in_position=UnitDecimal(base_deposit_amount, self.base_token.name),
             quote_in_position=UnitDecimal(quote_deposit_amount, self.quote_token.name),
-            position_count=len(self._positions),
+            position_count=len(list(filter(lambda p: not p.transferred, self._positions.values()))),
         )
         return val
 
+    def transfer_position_out(self, position_info: PositionInfo):
+        if position_info in self.positions and not self.positions[position_info].transferred:
+            self.positions[position_info].transferred = True
+        else:
+            raise DemeterError("position not exist or has transferred out ")
+
+    def transfer_position_in(self, position_info: PositionInfo):
+        if position_info in self.positions and self.positions[position_info].transferred:
+            self.positions[position_info].transferred = False
+        else:
+            raise DemeterError("position not exist or has not transferred yet ")
+
     def tick_to_price(self, tick: int) -> Decimal:
         """
         convert tick to price
 
         :param tick: tick
         :type tick: int
         :return: price
         :rtype: Decimal
         """
-        return tick_to_quote_price(
+        return tick_to_base_unit_price(
             int(tick),
             self._pool.token0.decimal,
             self._pool.token1.decimal,
-            self._is_token0_base,
+            self._is_token0_quote,
         )
 
     @float_param_formatter
     def price_to_tick(self, price: Decimal | float) -> int:
         """
         convert price to tick
 
         :param price: price
         :type price:  Decimal | float
         :return: tick
         :rtype: int
         """
-        return quote_price_to_tick(
+        return base_unit_price_to_tick(
             price,
             self._pool.token0.decimal,
             self._pool.token1.decimal,
-            self._is_token0_base,
+            self._is_token0_quote,
         )
 
+    @write_func
     def _add_liquidity_by_tick(
         self,
         token0_amount: Decimal,
         token1_amount: Decimal,
         lower_tick: int,
         upper_tick: int,
         sqrt_price_x96: int = -1,
@@ -344,69 +380,79 @@
         )
         if position_info in self._positions:
             self._positions[position_info].liquidity += liquidity
         else:
             self._positions[position_info] = Position(DECIMAL_0, DECIMAL_0, liquidity)
         self.broker.subtract_from_balance(self.token0, token0_used)
         self.broker.subtract_from_balance(self.token1, token1_used)
-        self.has_update = True
         return position_info, token0_used, token1_used, liquidity
 
+    @write_func
     def __remove_liquidity(self, position: PositionInfo, liquidity: int = None, sqrt_price_x96: int = -1):
-        sqrt_price_x96 = int(sqrt_price_x96) if sqrt_price_x96 != -1 else get_sqrt_ratio_at_tick(self.market_status.data.closeTick)
+        sqrt_price_x96 = (
+            int(sqrt_price_x96) if sqrt_price_x96 != -1 else get_sqrt_ratio_at_tick(self.market_status.data.closeTick)
+        )
         delta_liquidity = (
-            liquidity if (liquidity is not None) and liquidity < self.positions[position].liquidity else self.positions[position].liquidity
+            liquidity
+            if (liquidity is not None) and liquidity < self.positions[position].liquidity
+            else self.positions[position].liquidity
         )
         token0_get, token1_get = V3CoreLib.close_position(self._pool, position, delta_liquidity, sqrt_price_x96)
 
         self._positions[position].liquidity = self.positions[position].liquidity - delta_liquidity
         self._positions[position].pending_amount0 += token0_get
         self._positions[position].pending_amount1 += token1_get
-        self.has_update = True
 
         return token0_get, token1_get, delta_liquidity
 
+    @write_func
     def __collect_fee(
         self,
         position: Position,
         max_collect_amount0: Decimal = None,
         max_collect_amount1: Decimal = None,
+        collect_to_user: bool = True,
     ):
         """
         Collect fee
 
         :param position: get_position
         :param max_collect_amount0: max collect amount0
         :param max_collect_amount1: max collect amount1
+        :param collect_to_user: Transfer collected token to user balance, default is true
         :return:
         """
         token0_fee = (
-            max_collect_amount0 if max_collect_amount0 is not None and max_collect_amount0 < position.pending_amount0 else position.pending_amount0
+            max_collect_amount0
+            if max_collect_amount0 is not None and max_collect_amount0 < position.pending_amount0
+            else position.pending_amount0
         )
         token1_fee = (
-            max_collect_amount1 if max_collect_amount1 is not None and max_collect_amount1 < position.pending_amount1 else position.pending_amount1
+            max_collect_amount1
+            if max_collect_amount1 is not None and max_collect_amount1 < position.pending_amount1
+            else position.pending_amount1
         )
 
         position.pending_amount0 -= token0_fee
         position.pending_amount1 -= token1_fee
         # add un_collect fee to current balance
-        self.broker.add_to_balance(self.token0, token0_fee)
-        self.broker.add_to_balance(self.token1, token1_fee)
-        self.has_update = True
+        if collect_to_user:
+            self.broker.add_to_balance(self.token0, token0_fee)
+            self.broker.add_to_balance(self.token1, token1_fee)
         return token0_fee, token1_fee
 
     # action for strategy
 
     @float_param_formatter
     def add_liquidity(
         self,
         lower_quote_price: Decimal | float,
         upper_quote_price: Decimal | float,
-        base_max_amount: Decimal | float = None,
         quote_max_amount: Decimal | float = None,
+        base_max_amount: Decimal | float = None,
     ) -> (PositionInfo, Decimal, Decimal, int):
         """
 
         add liquidity, then get a new get_position
 
         :param lower_quote_price: lower price base on quote token.
         :type lower_quote_price: Decimal | float
@@ -416,19 +462,21 @@
         :type base_max_amount: Decimal | float
         :param quote_max_amount: inputted base token amount, also the max amount to deposit, if is None, will use all the balance of base token
         :type quote_max_amount: Decimal | float
         :return: added get_position, base token used, quote token used
         :rtype: (PositionInfo, Decimal, Decimal)
         """
         base_max_amount = self.broker.get_token_balance(self.base_token) if base_max_amount is None else base_max_amount
-        quote_max_amount = self.broker.get_token_balance(self.quote_token) if quote_max_amount is None else quote_max_amount
+        quote_max_amount = (
+            self.broker.get_token_balance(self.quote_token) if quote_max_amount is None else quote_max_amount
+        )
 
         token0_amt, token1_amt = self._convert_pair(base_max_amount, quote_max_amount)
         lower_tick, upper_tick = V3CoreLib.quote_price_pair_to_tick(self._pool, lower_quote_price, upper_quote_price)
-        lower_tick, upper_tick = self._convert_pair(upper_tick, lower_tick)
+        # lower_tick, upper_tick = self._convert_pair(upper_tick, lower_tick)
         (
             created_position,
             token0_used,
             token1_used,
             liquidity,
         ) = self._add_liquidity_by_tick(token0_amt, token1_amt, lower_tick, upper_tick)
         base_used, quote_used = self._convert_pair(token0_used, token1_used)
@@ -453,15 +501,15 @@
         self,
         lower_tick: int,
         upper_tick: int,
         base_max_amount: Decimal | float = None,
         quote_max_amount: Decimal | float = None,
         sqrt_price_x96: int = -1,
         tick: int = -1,
-    ):
+    ) -> (PositionInfo, Decimal, Decimal, int):
         """
 
         add liquidity, you need to set tick instead of price.
 
         :param lower_tick: lower tick
         :type lower_tick: int
         :param upper_tick: upper tick
@@ -477,18 +525,20 @@
         :return: added get_position, base token used, quote token used
         :rtype: (PositionInfo, Decimal, Decimal)
         """
         if lower_tick > upper_tick:
             lower_tick, upper_tick = upper_tick, lower_tick
 
         if sqrt_price_x96 == -1 and tick != -1:
-            sqrt_price_x96 = tick_to_sqrtPriceX96(tick)
+            sqrt_price_x96 = tick_to_sqrt_price_x96(tick)
 
         base_max_amount = self.broker.get_token_balance(self.base_token) if base_max_amount is None else base_max_amount
-        quote_max_amount = self.broker.get_token_balance(self.quote_token) if quote_max_amount is None else quote_max_amount
+        quote_max_amount = (
+            self.broker.get_token_balance(self.quote_token) if quote_max_amount is None else quote_max_amount
+        )
 
         token0_amt, token1_amt = self._convert_pair(base_max_amount, quote_max_amount)
         (
             created_position,
             token0_used,
             token1_used,
             liquidity,
@@ -563,33 +613,38 @@
     @float_param_formatter
     def collect_fee(
         self,
         position: PositionInfo,
         max_collect_amount0: Decimal = None,
         max_collect_amount1: Decimal = None,
         remove_dry_pool: bool = True,
+        collect_to_user: bool = True,
     ) -> (Decimal, Decimal):
         """
         | collect fee and token from positions,
         | if the amount and liquidity is zero, this get_position will be deleted.
 
         :param position: get_position to collect
         :type position: PositionInfo
         :param max_collect_amount0: max token0 amount to collect, e.g. 1.2345 usdc, if set to None, all the amount will be collect
         :type max_collect_amount0: Decimal
         :param max_collect_amount1: max token0 amount to collect, if set to None, all the amount will be collect
         :type max_collect_amount1: Decimal
         :param remove_dry_pool: remove pool which liquidity==0, effect when collect==True
         :type remove_dry_pool: bool
+        :param collect_to_user: Transfer collected token to user balance, default is true
+        :type collect_to_user: bool
         :return: (base_got,quote_get), base and quote token amounts collected from get_position
         :rtype:  (Decimal,Decimal)
         """
         if (max_collect_amount0 and max_collect_amount0 < 0) or (max_collect_amount1 and max_collect_amount1 < 0):
             raise DemeterError("collect amount should large than 0")
-        token0_get, token1_get = self.__collect_fee(self._positions[position], max_collect_amount0, max_collect_amount1)
+        token0_get, token1_get = self.__collect_fee(
+            self._positions[position], max_collect_amount0, max_collect_amount1, collect_to_user
+        )
 
         base_get, quote_get = self._convert_pair(token0_get, token1_get)
         if self._positions[position]:
             self._record_action(
                 CollectFeeAction(
                     market=self.market_info,
                     base_balance_after=self.broker.get_token_balance_with_unit(self.base_token),
@@ -605,102 +660,138 @@
             and self._positions[position].liquidity == 0
             and remove_dry_pool
         ):
             del self.positions[position]
         return base_get, quote_get
 
     @float_param_formatter
-    def buy(self, amount: Decimal | float, price: Decimal | float = None) -> (Decimal, Decimal, Decimal):
+    def swap(
+        self,
+        from_amount: Decimal | float,
+        from_token: TokenInfo,
+        to_token: TokenInfo,
+        price: Decimal | float = None,
+        throw_action=True,
+    ):
+        if from_token == to_token:
+            raise DemeterError("from and to token can not same")
+        if from_token not in [self.quote_token, self.base_token] or to_token not in [self.quote_token, self.base_token]:
+            raise DemeterError("from or to token not in pool")
+
+        if from_token == self.base_token:
+            # e.g. swap 1 eth for 3000 usdc
+            price = price if price else self.market_status.data.price
+        else:
+            # e.g. swap 3000 usdc for 1 eth
+            price = price if price else 1 / self.market_status.data.price
+        fee_in_from = from_amount * self.pool_info.fee_rate
+        to_amount = (from_amount - fee_in_from) * price
+        self.broker.subtract_from_balance(from_token, from_amount)
+        self.broker.add_to_balance(to_token, to_amount)
+        if throw_action:
+            self._record_action(
+                SwapAction(
+                    market=self.market_info,
+                    amount=UnitDecimal(from_amount, from_token.name),
+                    price=UnitDecimal(price, f"{from_token.name}/{to_token.name}"),
+                    fee=UnitDecimal(fee_in_from, from_token.name),
+                    to_amount=UnitDecimal(to_amount, to_token.name),
+                )
+            )
+        return fee_in_from, to_amount
+
+    @float_param_formatter
+    def buy(self, base_token_amount: Decimal | float, price: Decimal | float = None) -> (Decimal, Decimal, Decimal):
         """
-        buy token, swap from base token to quote token.
+        buy base token, swap from quote token to base token.
 
-        :param amount: amount to buy(in quote token)
-        :type amount:  Decimal | float
-        :param price: price, e.g. 1234 eth/usdc, if leave to None, will use pool price
+        :param base_token_amount: amount to buy(in base token)
+        :type base_token_amount:  Decimal | float
+        :param price: price in base/quote, e.g. 1234 eth/usdc, if leave to None, will use pool price
         :type price: Decimal | float
-        :return: fee, base token amount spend, quote token amount got
+        :return: fee in base token, quote token amount spend, base token amount got
         :rtype: (Decimal, Decimal, Decimal)
         """
+        if base_token_amount == 0:
+            return DECIMAL_0, DECIMAL_0, DECIMAL_0
         price = price if price else self.market_status.data.price
-        from_amount = price * amount
-        from_amount_with_fee = from_amount * (1 + self._pool.fee_rate)
-        fee = from_amount_with_fee - from_amount
-        from_token, to_token = self._convert_pair(self.token0, self.token1)
-        self.broker.subtract_from_balance(from_token, from_amount_with_fee)
-        self.broker.add_to_balance(to_token, amount)
-        base_amount, quote_amount = self._convert_pair(from_amount, amount)
+        quote_amount_with_fee = base_token_amount * price / (1 - self._pool.fee_rate)
+        fee_in_quote, base_amount_got = self.swap(
+            quote_amount_with_fee, self.quote_token, self.base_token, 1 / price, False
+        )
         self._record_action(
             BuyAction(
                 market=self.market_info,
                 base_balance_after=self.broker.get_token_balance_with_unit(self.base_token),
                 quote_balance_after=self.broker.get_token_balance_with_unit(self.quote_token),
-                amount=UnitDecimal(amount, self.quote_token.name),
+                amount=UnitDecimal(base_token_amount, self.base_token.name),
                 price=UnitDecimal(price, self._pool_price_unit),
-                fee=UnitDecimal(fee, self.base_token.name),
-                base_change=UnitDecimal(base_amount, self.base_token.name),
-                quote_change=UnitDecimal(quote_amount, self.quote_token.name),
+                fee=UnitDecimal(fee_in_quote, self.quote_token.name),
+                base_change=UnitDecimal(base_amount_got, self.base_token.name),
+                quote_change=UnitDecimal(quote_amount_with_fee, self.quote_token.name),
             )
         )
-        return fee, base_amount, quote_amount
+        return fee_in_quote, quote_amount_with_fee, base_amount_got
 
     @float_param_formatter
-    def sell(self, amount: Decimal | float, price: Decimal | float = None) -> (Decimal, Decimal, Decimal):
+    def sell(self, base_token_amount: Decimal | float, price: Decimal | float = None) -> (Decimal, Decimal, Decimal):
         """
-        sell token, swap from quote token to base token.
+        Sell base token, swap from base token to quote token.
 
-        :param amount: amount to sell(in quote token)
-        :type amount:  Decimal | float
+        :param base_token_amount: amount to sell(in base token)
+        :type base_token_amount:  Decimal | float
         :param price: price, e.g. 1234 eth/usdc, if leave to None, will use pool price
         :type price: Decimal | float
-        :return: fee, base token amount got, quote token amount spend
+        :return: fee in quote token, base token amount spend, quote token amount got
         :rtype: (Decimal, Decimal, Decimal)
         """
+        if base_token_amount == 0:
+            return DECIMAL_0, DECIMAL_0, DECIMAL_0
         price = price if price else self.market_status.data.price
-        from_amount_with_fee = amount
-        from_amount = from_amount_with_fee * (1 - self._pool.fee_rate)
-        to_amount = from_amount * price
-        fee = from_amount_with_fee - from_amount
-        to_token, from_token = self._convert_pair(self.token0, self.token1)
-        self.broker.subtract_from_balance(from_token, from_amount_with_fee)
-        self.broker.add_to_balance(to_token, to_amount)
-        base_amount, quote_amount = self._convert_pair(to_amount, from_amount)
+
+        fee_in_base, quote_amount_got = self.swap(base_token_amount, self.base_token, self.quote_token, price, False)
+
         self._record_action(
             SellAction(
                 market=self.market_info,
                 base_balance_after=self.broker.get_token_balance_with_unit(self.base_token),
                 quote_balance_after=self.broker.get_token_balance_with_unit(self.quote_token),
-                amount=UnitDecimal(amount, self.base_token.name),
+                amount=UnitDecimal(base_token_amount, self.base_token.name),
                 price=UnitDecimal(price, self._pool_price_unit),
-                fee=UnitDecimal(fee, self.quote_token.name),
-                base_change=UnitDecimal(base_amount, self.base_token.name),
-                quote_change=UnitDecimal(quote_amount, self.quote_token.name),
+                fee=UnitDecimal(fee_in_base, self.base_token.name),
+                base_change=UnitDecimal(base_token_amount, self.base_token.name),
+                quote_change=UnitDecimal(quote_amount_got, self.quote_token.name),
             )
         )
 
-        return fee, base_amount, quote_amount
+        return fee_in_base, base_token_amount, quote_amount_got
 
-    def even_rebalance(self, price: Decimal = None) -> (Decimal, Decimal, Decimal):
+    def even_rebalance(self, price: Decimal | None = None):
         """
         Divide assets equally between two tokens.
 
         :param price: price of quote token. e.g. 1234 eth/usdc, if leave to None, will use pool price
         :type price: Decimal
-        :return: fee, base token amount spend, quote token amount got
-        :rtype: (Decimal, Decimal, Decimal)
         """
         if price is None:
             price = self._market_status.data.price
 
-        total_capital = self.broker.get_token_balance(self.base_token) + self.broker.get_token_balance(self.quote_token) * price
-        target_base_amount = total_capital / 2
-        quote_amount_diff = target_base_amount / price - self.broker.get_token_balance(self.quote_token)
-        if quote_amount_diff > 0:
-            return self.buy(quote_amount_diff)
-        elif quote_amount_diff < 0:
-            return self.sell(0 - quote_amount_diff)
+        amount_quote = self.broker.get_token_balance(self.quote_token)
+        amount_base = self.broker.get_token_balance(self.base_token)
+
+        delta_base = (amount_quote / price - amount_base) / (Decimal(2) + self.pool_info.fee_rate)
+        if delta_base >= 0:
+            self.buy(delta_base)
+            return
+
+        delta_quote = (amount_base - amount_quote / price) / (Decimal(2) - self.pool_info.fee_rate)
+        if delta_quote >= 0:
+            self.sell(delta_quote)
+            return
+        pass
 
     def remove_all_liquidity(self):
         """
         remove all the positions kept in broker.
         """
         if len(self.positions) < 1:
             return
@@ -722,15 +813,17 @@
         :param df: original data
         :type df: pd.DataFrame
 
         """
         # add statistic column
         df["open"] = df["openTick"].map(lambda x: self.tick_to_price(x))
         df["price"] = df["closeTick"].map(lambda x: self.tick_to_price(x))
-        high_name, low_name = ("lowestTick", "highestTick") if self.pool_info.is_token0_base else ("highestTick", "lowestTick")
+        high_name, low_name = (
+            ("lowestTick", "highestTick") if self.pool_info.is_token0_quote else ("highestTick", "lowestTick")
+        )
         df["low"] = df[high_name].map(lambda x: self.tick_to_price(x))
         df["high"] = df[low_name].map(lambda x: self.tick_to_price(x))
         df["volume0"] = df["inAmount0"].map(lambda x: Decimal(x) / 10**self.pool_info.token0.decimal)
         df["volume1"] = df["inAmount1"].map(lambda x: Decimal(x) / 10**self.pool_info.token1.decimal)
 
     def load_data(self, chain: str, contract_addr: str, start_date: date, end_date: date):
         """
@@ -750,15 +843,15 @@
         :param end_date: end test date
         :type end_date: date
         """
         self.logger.info(f"start load files from {start_date} to {end_date}...")
         df = pd.DataFrame()
         day = start_date
         if start_date > end_date:
-            raise DemeterError(f"start date {start_date} should eariler than end date {end_date}")
+            raise DemeterError(f"start date {start_date} should earlier than end date {end_date}")
         while day <= end_date:
             new_type_path = os.path.join(
                 self.data_path,
                 f"{chain.lower()}-{contract_addr}-{day.strftime('%Y-%m-%d')}.minute.csv",
             )
             path = (
                 new_type_path
@@ -786,35 +879,42 @@
             day = day + timedelta(days=1)
         self.logger.info("load file complete, preparing...")
 
         df["timestamp"] = pd.to_datetime(df["timestamp"])
         df.set_index("timestamp", inplace=True)
 
         # fill empty row (first minutes in a day, might be blank)
-        full_indexes = pd.date_range(start=df.index[0], end=df.index[df.index.size - 1], freq="1min")
+        full_indexes = pd.date_range(
+            start=start_date,
+            end=datetime.combine(end_date, time(0, 0, 0)) + timedelta(days=1) - timedelta(minutes=1),
+            freq="1min",
+        )
         df = df.reindex(full_indexes)
         # df = Lines.from_dataframe(df)
         # df = df.fillna()
-        df = fillna(df)
+        df: pd.DataFrame = fillna(df)
+        if pd.isna(df.iloc[0]["closeTick"]):
+            df = df.bfill()
+
         self.add_statistic_column(df)
         self.data = df
         self.logger.info("data has been prepared")
 
     def formatted_str(self) -> str:
         """
         Return a brief description of this market in pretty format. Used for print in console.
         """
         value = get_formatted_predefined(f"{self.market_info.name}({type(self).__name__})", STYLE["header3"]) + "\n"
         value += (
             get_formatted_from_dict(
                 {
                     "token0": self.pool_info.token0.name,
                     "token1": self.pool_info.token1.name,
-                    "fee": self.pool_info.fee_rate * 100,
-                    "is 0 base": self.pool_info.is_token0_base,
+                    "fee(%)": self.pool_info.fee_rate * 100,
+                    "quote token": self.quote_token.name,
                 }
             )
             + "\n"
         )
         value += get_formatted_predefined("positions", STYLE["key"]) + "\n"
         df = position_dict_to_dataframe(self.positions)
         if len(df.index) > 0:
```

### Comparing `zelos-demeter-0.3.0/demeter/utils/application.py` & `zelos-demeter-0.5.1/demeter/utils/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     :param value: any value
     :type value: Any
     :return: Decimal value
     :rtype: Decimal
 
     """
-    return Decimal(value)
+    return Decimal(str(value))
 
 
 def object_to_decimal(num: Any) -> Any:
     """
     If number is float or int, return Decimal, else return original value
 
     :param value: any value
```

### Comparing `zelos-demeter-0.3.0/setup.py` & `zelos-demeter-0.5.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
-    name='zelos-demeter',
-    version='0.3.0',
+    name="zelos-demeter",
+    version="0.5.1",
     packages=find_packages(exclude=["tests", "tests.*", "samples", "samples.*"]),
-    url='https://zelos-demeter.readthedocs.io',
-    license='MIT',
-    author='zelos research',
-    author_email='zelos@antalpha.com',
-    description='better DEFI backtesting tool',
+    url="https://zelos-demeter.readthedocs.io",
+    license="MIT",
+    author="zelos research",
+    author_email="zelos@antalpha.com",
+    description="better DEFI backtesting tool",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    python_requires='>=3.10',
-    install_requires=["pandas>=1.4.4",
-                      "tqdm>=4.64.1",
-                      "db-dtypes>=1.0.4",
-                      "toml>=0.10.2"],
+    long_description_content_type="text/markdown",
+    python_requires=">=3.10",
+    install_requires=[
+        "numpy==1.26.4",
+        "pandas==2.2.0",
+        "python-dateutil==2.9.0.post0",
+        "pytz==2024.1",
+        "six==1.16.0",
+        "db-dtypes==1.2.0",
+        "tqdm==4.66.2",
+        "orjson==3.9.15",
+    ],
 )
 
 # rm -rf ./demeter.egg-info/ && python setup.py sdist upload -r private
 # python setup.py sdist
 # twine upload -r pypi dist/*
```

### Comparing `zelos-demeter-0.3.0/zelos_demeter.egg-info/SOURCES.txt` & `zelos-demeter-0.5.1/zelos_demeter.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,26 @@
 demeter/broker/_typing.py
 demeter/broker/broker.py
 demeter/broker/market.py
 demeter/core/__init__.py
 demeter/core/actuator.py
 demeter/core/evaluating_indicator.py
 demeter/core/math_helper.py
+demeter/deribit/__init__.py
+demeter/deribit/_typing.py
+demeter/deribit/helper.py
+demeter/deribit/market.py
 demeter/indicator/__init__.py
 demeter/indicator/common.py
 demeter/indicator/ma.py
 demeter/indicator/volatility.py
+demeter/squeeth/__init__.py
+demeter/squeeth/_typing.py
+demeter/squeeth/helper.py
+demeter/squeeth/market.py
 demeter/strategy/__init__.py
 demeter/strategy/strategy.py
 demeter/strategy/trigger.py
 demeter/uniswap/__init__.py
 demeter/uniswap/_typing.py
 demeter/uniswap/core.py
 demeter/uniswap/data.py
```

