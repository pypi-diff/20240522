# Comparing `tmp/tinyticker-0.6.1.tar.gz` & `tmp/tinyticker-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.6.1.tar", max compression
+gzip compressed data, was "tinyticker-0.6.2.tar", max compression
```

## Comparing `tinyticker-0.6.1.tar` & `tinyticker-0.6.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1068 2024-05-22 14:15:18.402828 tinyticker-0.6.1/LICENSE
--rw-r--r--   0        0        0     3858 2024-05-22 14:15:18.402828 tinyticker-0.6.1/README.md
--rw-r--r--   0        0        0      917 2024-05-22 14:15:18.406828 tinyticker-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      465 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/__init__.py
--rw-r--r--   0        0        0     5893 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/__main__.py
--rw-r--r--   0        0        0     2496 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/config.py
--rw-r--r--   0        0        0     9000 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/paths.py
--rw-r--r--   0        0        0     4235 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3618 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     2915 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-22 14:15:18.406828 tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     1283 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2583 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6750 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/app.py
--rw-r--r--   0        0        0     3021 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    15682 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1904 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2349 2024-05-22 14:15:18.410828 tinyticker-0.6.1/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 tinyticker-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-22 15:08:06.073083 tinyticker-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3953 2024-05-22 15:08:06.073083 tinyticker-0.6.2/README.md
+-rw-r--r--   0        0        0      917 2024-05-22 15:08:06.073083 tinyticker-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      465 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/__init__.py
+-rw-r--r--   0        0        0     5893 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2496 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/config.py
+-rw-r--r--   0        0        0     9000 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/paths.py
+-rw-r--r--   0        0        0     4235 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3618 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     2915 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    19697 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1423 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2583 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6750 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3021 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    15682 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1904 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2349 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 tinyticker-0.6.2/PKG-INFO
```

### Comparing `tinyticker-0.6.1/LICENSE` & `tinyticker-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/README.md` & `tinyticker-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 Shopping list:
 
 - [Raspberry Pi Zero WH](https://www.adafruit.com/product/3708)
 - One of these ePaper displays:
   - [Waveshare ePaper 2.13in Black & White](https://www.waveshare.com/wiki/2.13inch_e-Paper_HAT)
   - [Waveshare ePaper 2.13in Black, White & Red](<https://www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(B)>)
   - [Waveshare ePaper 2.13in Black, White & Yellow](<https://www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(C)>)
+  - [Waveshare ePaper 2.7in Black & White](https://www.waveshare.com/wiki/2.7inch_e-Paper_HAT)
 - A micro sd card
 
 ## 📦 Installation
 
 ### Recommended setup
 
 Flash the [tinyticker image](https://drive.google.com/drive/folders/1U-PGzkOtSynN6FGDq2MsXF9kXGdkzd0D) onto a SD card and you should be good to go.
```

#### html2text {}

```diff
@@ -13,20 +13,21 @@
 (https://github.com/ranaroussi/yfinance) package to get the stock financial
 data. ## ð Hardware Shopping list: - [Raspberry Pi Zero WH](https://
 www.adafruit.com/product/3708) - One of these ePaper displays: - [Waveshare
 ePaper 2.13in Black & White](https://www.waveshare.com/wiki/2.13inch_e-
 Paper_HAT) - [Waveshare ePaper 2.13in Black, White & Red](
 www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(B)>) - [Waveshare ePaper 2.13in
 Black, White & Yellow](
-www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(C)>) - A micro sd card ## ð¦
-Installation ### Recommended setup Flash the [tinyticker image](https://
-drive.google.com/drive/folders/1U-PGzkOtSynN6FGDq2MsXF9kXGdkzd0D) onto a SD
-card and you should be good to go. > [!NOTE] > To build your own image, see the
-[`pi-gen`](https://github.com/loiccoyle/pi-gen) repo. ### Manual setup >
-[!NOTE] > This is much more involved than the recommended setup and will most
+www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(C)>) - [Waveshare ePaper 2.7in
+Black & White](https://www.waveshare.com/wiki/2.7inch_e-Paper_HAT) - A micro sd
+card ## ð¦ Installation ### Recommended setup Flash the [tinyticker image]
+(https://drive.google.com/drive/folders/1U-PGzkOtSynN6FGDq2MsXF9kXGdkzd0D) onto
+a SD card and you should be good to go. > [!NOTE] > To build your own image,
+see the [`pi-gen`](https://github.com/loiccoyle/pi-gen) repo. ### Manual setup
+> [!NOTE] > This is much more involved than the recommended setup and will most
 likely require some debugging. Expand I highly recommend using [comitup](https:
 //github.com/davesteele/comitup) to setup the networking on your RPi. - Write
 the `comitup` [image](https://davesteele.github.io/comitup/latest/comitup-lite-
 img-latest.html) to your sd card - Boot up the RPi and setup the networking -
 ssh into your RPi, you'll probably want to change the password while you're at
 it - Enable the [SPI interface](https://www.raspberrypi-spy.co.uk/2014/08/
 enabling-the-spi-interface-on-the-raspberry-pi/) - (Optional) rename the
```

### Comparing `tinyticker-0.6.1/pyproject.toml` & `tinyticker-0.6.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.6.1"
+version = "0.6.2"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.6.1/tinyticker/__main__.py` & `tinyticker-0.6.2/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/config.py` & `tinyticker-0.6.2/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/display.py` & `tinyticker-0.6.2/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/sequence.py` & `tinyticker-0.6.2/tinyticker/sequence.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/tickers/__init__.py` & `tinyticker-0.6.2/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/tickers/_base.py` & `tinyticker-0.6.2/tinyticker/tickers/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/tickers/crypto.py` & `tinyticker-0.6.2/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/tickers/stock.py` & `tinyticker-0.6.2/tinyticker/tickers/stock.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/utils.py` & `tinyticker-0.6.2/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/device.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/waveshare_lib/models.py` & `tinyticker-0.6.2/tinyticker/waveshare_lib/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     epd2in13,
     epd2in13_V2,
     epd2in13_V3,
     epd2in13_V4,
     epd2in13b_V3,
     epd2in13b_V4,
     epd2in13bc,
+    epd2in7_V2,
 )
 from ._base import EPDHighlight, EPDMonochrome
 
 
 @dataclass
 class EPDModel:
     name: str
@@ -52,9 +53,14 @@
         desc="Black, White and Red 2.13 inch V4",
     ),
     EPDModel(
         name="EPDbc",
         class_=epd2in13bc.EPD,
         desc="Black, White and Yellow 2.13 inch",
     ),
+    EPDModel(
+        name="EPD_2in7_v2",
+        class_=epd2in7_V2.EPD,
+        desc="Black and White 2.7 inch V2",
+    ),
 ]
 MODELS = {model.name: model for model in MODELS}
```

### Comparing `tinyticker-0.6.1/tinyticker/web/__main__.py` & `tinyticker-0.6.2/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/app.py` & `tinyticker-0.6.2/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/command.py` & `tinyticker-0.6.2/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.6.2/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.6.2/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.6.2/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.6.2/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/templates/index.html` & `tinyticker-0.6.2/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/templates/js/index.js` & `tinyticker-0.6.2/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.6.2/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.6.2/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/tinyticker/web/templates/logfiles.html` & `tinyticker-0.6.2/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.1/PKG-INFO` & `tinyticker-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
@@ -54,14 +54,15 @@
 Shopping list:
 
 - [Raspberry Pi Zero WH](https://www.adafruit.com/product/3708)
 - One of these ePaper displays:
   - [Waveshare ePaper 2.13in Black & White](https://www.waveshare.com/wiki/2.13inch_e-Paper_HAT)
   - [Waveshare ePaper 2.13in Black, White & Red](<https://www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(B)>)
   - [Waveshare ePaper 2.13in Black, White & Yellow](<https://www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(C)>)
+  - [Waveshare ePaper 2.7in Black & White](https://www.waveshare.com/wiki/2.7inch_e-Paper_HAT)
 - A micro sd card
 
 ## 📦 Installation
 
 ### Recommended setup
 
 Flash the [tinyticker image](https://drive.google.com/drive/folders/1U-PGzkOtSynN6FGDq2MsXF9kXGdkzd0D) onto a SD card and you should be good to go.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.6.1 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.6.2 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -31,20 +31,21 @@
 (https://github.com/ranaroussi/yfinance) package to get the stock financial
 data. ## ð Hardware Shopping list: - [Raspberry Pi Zero WH](https://
 www.adafruit.com/product/3708) - One of these ePaper displays: - [Waveshare
 ePaper 2.13in Black & White](https://www.waveshare.com/wiki/2.13inch_e-
 Paper_HAT) - [Waveshare ePaper 2.13in Black, White & Red](
 www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(B)>) - [Waveshare ePaper 2.13in
 Black, White & Yellow](
-www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(C)>) - A micro sd card ## ð¦
-Installation ### Recommended setup Flash the [tinyticker image](https://
-drive.google.com/drive/folders/1U-PGzkOtSynN6FGDq2MsXF9kXGdkzd0D) onto a SD
-card and you should be good to go. > [!NOTE] > To build your own image, see the
-[`pi-gen`](https://github.com/loiccoyle/pi-gen) repo. ### Manual setup >
-[!NOTE] > This is much more involved than the recommended setup and will most
+www.waveshare.com/wiki/2.13inch_e-Paper_HAT_(C)>) - [Waveshare ePaper 2.7in
+Black & White](https://www.waveshare.com/wiki/2.7inch_e-Paper_HAT) - A micro sd
+card ## ð¦ Installation ### Recommended setup Flash the [tinyticker image]
+(https://drive.google.com/drive/folders/1U-PGzkOtSynN6FGDq2MsXF9kXGdkzd0D) onto
+a SD card and you should be good to go. > [!NOTE] > To build your own image,
+see the [`pi-gen`](https://github.com/loiccoyle/pi-gen) repo. ### Manual setup
+> [!NOTE] > This is much more involved than the recommended setup and will most
 likely require some debugging. Expand I highly recommend using [comitup](https:
 //github.com/davesteele/comitup) to setup the networking on your RPi. - Write
 the `comitup` [image](https://davesteele.github.io/comitup/latest/comitup-lite-
 img-latest.html) to your sd card - Boot up the RPi and setup the networking -
 ssh into your RPi, you'll probably want to change the password while you're at
 it - Enable the [SPI interface](https://www.raspberrypi-spy.co.uk/2014/08/
 enabling-the-spi-interface-on-the-raspberry-pi/) - (Optional) rename the
```

