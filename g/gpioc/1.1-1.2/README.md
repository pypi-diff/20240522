# Comparing `tmp/gpioc-1.1.tar.gz` & `tmp/gpioc-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpioc-1.1.tar", last modified: Wed May 15 07:45:02 2024, max compression
+gzip compressed data, was "gpioc-1.2.tar", last modified: Wed May 22 01:56:18 2024, max compression
```

## Comparing `gpioc-1.1.tar` & `gpioc-1.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.608765 gpioc-1.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-15 07:44:58.000000 gpioc-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 07:44:58.000000 gpioc-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-15 07:45:02.608765 gpioc-1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2664 2024-05-15 07:44:58.000000 gpioc-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-15 07:44:58.000000 gpioc-1.1/README_PY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.604765 gpioc-1.1/examples-python/
--rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-05-15 07:44:58.000000 gpioc-1.1/examples-python/gpio.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-15 07:44:58.000000 gpioc-1.1/examples-python/pwm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.604765 gpioc-1.1/gpioc/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.604765 gpioc-1.1/gpioc/chips/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1103 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/chips/H616.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/chips/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2997 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/pin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1136 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/pwm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.608765 gpioc-1.1/gpioc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-15 07:45:02.000000 gpioc-1.1/gpioc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-15 07:45:02.000000 gpioc-1.1/gpioc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:45:02.000000 gpioc-1.1/gpioc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 07:45:02.000000 gpioc-1.1/gpioc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.608765 gpioc-1.1/libgpio/
--rwxr-xr-x   0 runner    (1001) docker     (127)      239 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/board.c
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/board.h
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/gpio.h
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl-sun50i-h616-r.c
--rw-r--r--   0 runner    (1001) docker     (127)    22484 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl-sun50i-h616.c
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl-sunxi.c
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl-sunxi.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     1848 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      607 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     2359 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl_py.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     4608 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/softpwm.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/softpwm.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/softpwm_py.c
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:45:02.608765 gpioc-1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1060 2024-05-15 07:44:58.000000 gpioc-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:18.090057 gpioc-1.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-22 01:56:14.000000 gpioc-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 01:56:14.000000 gpioc-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-22 01:56:18.090057 gpioc-1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2664 2024-05-22 01:56:14.000000 gpioc-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-22 01:56:14.000000 gpioc-1.2/README_PY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:18.086057 gpioc-1.2/examples-python/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-05-22 01:56:14.000000 gpioc-1.2/examples-python/gpio.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-22 01:56:14.000000 gpioc-1.2/examples-python/pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:18.086057 gpioc-1.2/gpioc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:14.000000 gpioc-1.2/gpioc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:18.086057 gpioc-1.2/gpioc/chips/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1103 2024-05-22 01:56:14.000000 gpioc-1.2/gpioc/chips/H616.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:14.000000 gpioc-1.2/gpioc/chips/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2997 2024-05-22 01:56:14.000000 gpioc-1.2/gpioc/pin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1136 2024-05-22 01:56:14.000000 gpioc-1.2/gpioc/pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:18.090057 gpioc-1.2/gpioc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-22 01:56:18.000000 gpioc-1.2/gpioc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 01:56:18.000000 gpioc-1.2/gpioc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:18.000000 gpioc-1.2/gpioc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 01:56:18.000000 gpioc-1.2/gpioc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:18.090057 gpioc-1.2/libgpio/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      239 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/board.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/board.h
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/gpio.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/pinctrl-sun50i-h616-r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22484 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/pinctrl-sun50i-h616.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/pinctrl-sunxi.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/pinctrl-sunxi.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1848 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/pinctrl.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      607 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/pinctrl.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2359 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/pinctrl_py.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4608 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/softpwm.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/softpwm.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-05-22 01:56:14.000000 gpioc-1.2/libgpio/softpwm_py.c
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:56:18.090057 gpioc-1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1060 2024-05-22 01:56:14.000000 gpioc-1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-22 01:56:14.000000 gpioc-1.2/version
```

### Comparing `gpioc-1.1/LICENSE` & `gpioc-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/PKG-INFO` & `gpioc-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpioc
-Version: 1.1
+Version: 1.2
 Summary: A module to control GPIO
 Home-page: https://github.com/sc-bin/gpioc
 Author: sc-bin
 Author-email: 3335447573@qq.com
 License: MIT
 Platform: manylinux
 Description-Content-Type: text/markdown
```

### Comparing `gpioc-1.1/README.md` & `gpioc-1.2/README.md`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/README_PY.md` & `gpioc-1.2/README_PY.md`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/gpioc/chips/H616.py` & `gpioc-1.2/gpioc/chips/H616.py`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/gpioc/pin.py` & `gpioc-1.2/gpioc/pin.py`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/gpioc/pwm.py` & `gpioc-1.2/gpioc/pwm.py`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/gpioc.egg-info/PKG-INFO` & `gpioc-1.2/gpioc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpioc
-Version: 1.1
+Version: 1.2
 Summary: A module to control GPIO
 Home-page: https://github.com/sc-bin/gpioc
 Author: sc-bin
 Author-email: 3335447573@qq.com
 License: MIT
 Platform: manylinux
 Description-Content-Type: text/markdown
```

### Comparing `gpioc-1.1/gpioc.egg-info/SOURCES.txt` & `gpioc-1.2/gpioc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 README_PY.md
 setup.py
+version
 examples-python/gpio.py
 examples-python/pwm.py
 gpioc/__init__.py
 gpioc/pin.py
 gpioc/pwm.py
 gpioc.egg-info/PKG-INFO
 gpioc.egg-info/SOURCES.txt
```

### Comparing `gpioc-1.1/libgpio/board.c` & `gpioc-1.2/libgpio/board.c`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/board.h` & `gpioc-1.2/libgpio/board.h`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/gpio.h` & `gpioc-1.2/libgpio/gpio.h`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/pinctrl-sun50i-h616-r.c` & `gpioc-1.2/libgpio/pinctrl-sun50i-h616-r.c`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/pinctrl-sun50i-h616.c` & `gpioc-1.2/libgpio/pinctrl-sun50i-h616.c`

 * *Files 6% similar despite different names*

```diff
@@ -34,489 +34,489 @@
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(A, 7),
 		  SUNXI_FUNCTION(0x2, "emac1_ETXEN")),		/* ETXEN */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(A, 8),
 		  SUNXI_FUNCTION(0x2, "emac1_EMDC")),		/* EMDC */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(A, 9),
 		  SUNXI_FUNCTION(0x2, "emac1_EMDIO")),		/* EMDIO */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(A, 10),
-		  SUNXI_FUNCTION(0x2, "i2c3_SCK")),		/* SCK */
+		  SUNXI_FUNCTION(0x2, "I2C3_SCK")),		/* SCK */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(A, 11),
-		  SUNXI_FUNCTION(0x2, "i2c3_SDA")),		/* SDA */
+		  SUNXI_FUNCTION(0x2, "I2C3_SDA")),		/* SDA */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(A, 12),
-		  SUNXI_FUNCTION(0x2, "pwm5")),
+		  SUNXI_FUNCTION(0x2, "PWM5")),
 	/* Hole */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 0),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_WE"),		/* WE */
-		  SUNXI_FUNCTION(0x3, "mmc2_DS"),		/* DS */
-		  SUNXI_FUNCTION(0x4, "spi0_CLK"),		/* CLK */
+		  SUNXI_FUNCTION(0x3, "MMC2_DS"),		/* DS */
+		  SUNXI_FUNCTION(0x4, "SPI0_CLK"),		/* CLK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 0)),	/* PC_EINT0 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 1),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_ALE"),		/* ALE */
-		  SUNXI_FUNCTION(0x3, "mmc2_RST"),		/* RST */
+		  SUNXI_FUNCTION(0x3, "MMC2_RST"),		/* RST */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 1)),	/* PC_EINT1 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 2),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_CLE"),		/* CLE */
-		  SUNXI_FUNCTION(0x4, "spi0_MOSI"),		/* MOSI */
+		  SUNXI_FUNCTION(0x4, "SPI0_MOSI"),		/* MOSI */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 2)),	/* PC_EINT2 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 3),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_CE1"),		/* CE1 */
-		  SUNXI_FUNCTION(0x4, "spi0_CS0"),		/* CS0 */
+		  SUNXI_FUNCTION(0x4, "SPI0_CS0"),		/* CS0 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 3)),	/* PC_EINT3 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 4),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_CE0"),		/* CE0 */
-		  SUNXI_FUNCTION(0x4, "spi0_MISO"),		/* MISO */
+		  SUNXI_FUNCTION(0x4, "SPI0_MISO"),		/* MISO */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 4)),	/* PC_EINT4 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 5),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_RE"),		/* RE */
-		  SUNXI_FUNCTION(0x3, "mmc2_CLK"),		/* CLK */
+		  SUNXI_FUNCTION(0x3, "MMC2_CLK"),		/* CLK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 5)),	/* PC_EINT5 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 6),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_RB0"),		/* RB0 */
-		  SUNXI_FUNCTION(0x3, "mmc2_CMD"),		/* CMD */
+		  SUNXI_FUNCTION(0x3, "MMC2_CMD"),		/* CMD */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 6)),	/* PC_EINT6 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 7),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_RB1"),		/* RB1 */
-		  SUNXI_FUNCTION(0x4, "spi0_CS1"),		/* CS1 */
+		  SUNXI_FUNCTION(0x4, "SPI0_CS1"),		/* CS1 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 7)),	/* PC_EINT7 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 8),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_DQ7"),		/* DQ7 */
-		  SUNXI_FUNCTION(0x3, "mmc2_D3"),		/* D3 */
+		  SUNXI_FUNCTION(0x3, "MMC2_D3"),		/* D3 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 8)),	/* PC_EINT8 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 9),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_DQ6"),		/* DQ6 */
-		  SUNXI_FUNCTION(0x3, "mmc2_D4"),		/* D4 */
+		  SUNXI_FUNCTION(0x3, "MMC2_D4"),		/* D4 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 9)),	/* PC_EINT9 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 10),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_DQ5"),		/* DQ5 */
-		  SUNXI_FUNCTION(0x3, "mmc2_D0"),		/* D0 */
+		  SUNXI_FUNCTION(0x3, "MMC2_D0"),		/* D0 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 10)),	/* PC_EINT10 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 11),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_DQ4"),		/* DQ4 */
-		  SUNXI_FUNCTION(0x3, "mmc2_D5"),		/* D5 */
+		  SUNXI_FUNCTION(0x3, "MMC2_D5"),		/* D5 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 11)),	/* PC_EINT11 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 12),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_DQS"),		/* DQS */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 12)),	/* PC_EINT12 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 13),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_DQ3"),		/* DQ3 */
-		  SUNXI_FUNCTION(0x3, "mmc2_D1"),		/* D1 */
+		  SUNXI_FUNCTION(0x3, "MMC2_D1"),		/* D1 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 13)),	/* PC_EINT13 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 14),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_DQ2"),		/* DQ2 */
-		  SUNXI_FUNCTION(0x3, "mmc2_D6"),		/* D6 */
+		  SUNXI_FUNCTION(0x3, "MMC2_D6"),		/* D6 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 14)),	/* PC_EINT14 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 15),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_DQ1"),		/* DQ1 */
-		  SUNXI_FUNCTION(0x3, "mmc2_D2"),		/* D2 */
-		  SUNXI_FUNCTION(0x4, "spi0_WP"),		/* WP */
+		  SUNXI_FUNCTION(0x3, "MMC2_D2"),		/* D2 */
+		  SUNXI_FUNCTION(0x4, "SPI0_WP"),		/* WP */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 15)),	/* PC_EINT15 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(C, 16),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "nand0_DQ0"),		/* DQ0 */
-		  SUNXI_FUNCTION(0x3, "mmc2_D7"),		/* D7 */
-		  SUNXI_FUNCTION(0x4, "spi0_HOLD"),		/* HOLD */
+		  SUNXI_FUNCTION(0x3, "MMC2_D7"),		/* D7 */
+		  SUNXI_FUNCTION(0x4, "SPI0_HOLD"),		/* HOLD */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 1, 16)),	/* PC_EINT16 */
 	/* Hole */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(F, 0),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc0_D1"),		/* D1 */
+		  SUNXI_FUNCTION(0x2, "MMC0_D1"),		/* D1 */
 		  SUNXI_FUNCTION(0x3, "jtag_MS"),		/* MS */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 4, 0)),	/* PF_EINT0 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(F, 1),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc0_D0"),		/* D0 */
+		  SUNXI_FUNCTION(0x2, "MMC0_D0"),		/* D0 */
 		  SUNXI_FUNCTION(0x3, "jtag_DI"),		/* DI */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 4, 1)),	/* PF_EINT1 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(F, 2),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc0_CLK"),		/* CLK */
-		  SUNXI_FUNCTION(0x3, "uart0_TX"),		/* TX */
+		  SUNXI_FUNCTION(0x2, "MMC0_CLK"),		/* CLK */
+		  SUNXI_FUNCTION(0x3, "UART0_TX"),		/* TX */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 4, 2)),	/* PF_EINT2 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(F, 3),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc0_CMD"),		/* CMD */
+		  SUNXI_FUNCTION(0x2, "MMC0_CMD"),		/* CMD */
 		  SUNXI_FUNCTION(0x3, "jtag_DO"),		/* DO */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 4, 3)),	/* PF_EINT3 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(F, 4),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc0_D3"),		/* D3 */
-		  SUNXI_FUNCTION(0x3, "uart0_RX"),		/* RX */
+		  SUNXI_FUNCTION(0x2, "MMC0_D3"),		/* D3 */
+		  SUNXI_FUNCTION(0x3, "UART0_RX"),		/* RX */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 4, 4)),	/* PF_EINT4 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(F, 5),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc0_D2"),		/* D2 */
+		  SUNXI_FUNCTION(0x2, "MMC0_D2"),		/* D2 */
 		  SUNXI_FUNCTION(0x3, "jtag_CK"),		/* CK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 4, 5)),	/* PF_EINT5 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(F, 6),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 4, 6)),	/* PF_EINT6 */
 	/* Hole */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 0),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc1_CLK"),		/* CLK */
+		  SUNXI_FUNCTION(0x2, "MMC1_CLK"),		/* CLK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 0)),	/* PG_EINT0 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 1),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc1_CMD"),		/* CMD */
+		  SUNXI_FUNCTION(0x2, "MMC1_CMD"),		/* CMD */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 1)),	/* PG_EINT1 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 2),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc1_D0"),		/* D0 */
+		  SUNXI_FUNCTION(0x2, "MMC1_D0"),		/* D0 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 2)),	/* PG_EINT2 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 3),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc1_D1"),		/* D1 */
+		  SUNXI_FUNCTION(0x2, "MMC1_D1"),		/* D1 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 3)),	/* PG_EINT3 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 4),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc1_D2"),		/* D2 */
+		  SUNXI_FUNCTION(0x2, "MMC1_D2"),		/* D2 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 4)),	/* PG_EINT4 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 5),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "mmc1_D3"),		/* D3 */
+		  SUNXI_FUNCTION(0x2, "MMC1_D3"),		/* D3 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 5)),	/* PG_EINT5 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 6),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart1_TX"),		/* TX */
+		  SUNXI_FUNCTION(0x2, "UART1_TX"),		/* TX */
 		  SUNXI_FUNCTION(0x4, "jtag_MS"),		/* MS */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 6)),	/* PG_EINT6 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 7),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart1_RX"),		/* RX */
+		  SUNXI_FUNCTION(0x2, "UART1_RX"),		/* RX */
 		  SUNXI_FUNCTION(0x4, "jtag_CK"),		/* CK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 7)),	/* PG_EINT7 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 8),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart1_RTS"),		/* RTS */
+		  SUNXI_FUNCTION(0x2, "UART1_RTS"),		/* RTS */
 		  SUNXI_FUNCTION(0x3, "clock_PLL_LOCK_DEBUG"),		/* PLL_LOCK_DEBUG */
 		  SUNXI_FUNCTION(0x4, "jtag_DO"),		/* DO */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 8)),	/* PG_EINT8 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 9),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart1_CTS"),		/* CTS */
+		  SUNXI_FUNCTION(0x2, "UART1_CTS"),		/* CTS */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 9)),	/* PG_EINT9 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 10),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "i2s2_MCLK"),		/* MCLK */
+		  SUNXI_FUNCTION(0x2, "I2S2_MCLK"),		/* MCLK */
 		  SUNXI_FUNCTION(0x3, "clock_X32KFOUT"),		/* X32KFOUT */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 10)),	/* PG_EINT10 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 11),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "i2s2_BCLK"),		/* BCLK */
+		  SUNXI_FUNCTION(0x2, "I2S2_BCLK"),		/* BCLK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 11)),	/* PG_EINT11 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 12),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "i2s2_SYNC"),		/* SYNC */
+		  SUNXI_FUNCTION(0x2, "I2S2_SYNC"),		/* SYNC */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 12)),	/* PG_EINT12 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 13),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "i2s2_DOUT"),		/* DOUT */
+		  SUNXI_FUNCTION(0x2, "I2S2_DOUT"),		/* DOUT */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 13)),	/* PG_EINT13 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 14),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "i2s2_DIN"),		/* DIN */
+		  SUNXI_FUNCTION(0x2, "I2S2_DIN"),		/* DIN */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 14)),	/* PG_EINT14 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 15),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart2_TX"),		/* TX */
-		  SUNXI_FUNCTION(0x5, "i2c4_SCK"),		/* SCK */
+		  SUNXI_FUNCTION(0x2, "UART2_TX"),		/* TX */
+		  SUNXI_FUNCTION(0x5, "I2C4_SCK"),		/* SCK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 15)),	/* PG_EINT15 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 16),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart2_RX"),		/* RX */
-		  SUNXI_FUNCTION(0x5, "i2c4_SDA"),		/* SDA */
+		  SUNXI_FUNCTION(0x2, "UART2_RX"),		/* RX */
+		  SUNXI_FUNCTION(0x5, "I2C4_SDA"),		/* SDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 16)),	/* PG_EINT16 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 17),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart2_RTS"),		/* RTS */
-		  SUNXI_FUNCTION(0x5, "i2c3_SCK"),		/* SCK */
+		  SUNXI_FUNCTION(0x2, "UART2_RTS"),		/* RTS */
+		  SUNXI_FUNCTION(0x5, "I2C3_SCK"),		/* SCK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 17)),	/* PG_EINT17 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 18),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart2_CTS"),		/* CTS */
-		  SUNXI_FUNCTION(0x5, "i2c3_SDA"),		/* SDA */
+		  SUNXI_FUNCTION(0x2, "UART2_CTS"),		/* CTS */
+		  SUNXI_FUNCTION(0x5, "I2C3_SDA"),		/* SDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 18)),	/* PG_EINT18 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(G, 19),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x4, "pwm1"),
+		  SUNXI_FUNCTION(0x4, "PWM1"),
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 5, 19)),	/* PG_EINT19 */
 	/* Hole */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 0),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart0_TX"),		/* TX */
-		  SUNXI_FUNCTION(0x4, "pwm3"),
-		  SUNXI_FUNCTION(0x5, "i2c1_SCK"),		/* SCK */
+		  SUNXI_FUNCTION(0x2, "UART0_TX"),		/* TX */
+		  SUNXI_FUNCTION(0x4, "PWM3"),
+		  SUNXI_FUNCTION(0x5, "I2C1_SCK"),		/* SCK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 0)),	/* PH_EINT0 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 1),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart0_RX"),		/* RX */
-		  SUNXI_FUNCTION(0x4, "pwm4"),
-		  SUNXI_FUNCTION(0x5, "i2c1_SDA"),		/* SDA */
+		  SUNXI_FUNCTION(0x2, "UART0_RX"),		/* RX */
+		  SUNXI_FUNCTION(0x4, "PWM4"),
+		  SUNXI_FUNCTION(0x5, "I2C1_SDA"),		/* SDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 1)),	/* PH_EINT1 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 2),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart5_TX"),		/* TX */
+		  SUNXI_FUNCTION(0x2, "UART5_TX"),		/* TX */
 		  SUNXI_FUNCTION(0x3, "spdif_MCLK"),		/* MCLK */
-		  SUNXI_FUNCTION(0x4, "pwm2"),
-		  SUNXI_FUNCTION(0x5, "i2c2_SCK"),		/* SCK */
+		  SUNXI_FUNCTION(0x4, "PWM2"),
+		  SUNXI_FUNCTION(0x5, "I2C2_SCK"),		/* SCK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 2)),	/* PH_EINT2 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 3),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart5_RX"),		/* RX */
-		  SUNXI_FUNCTION(0x4, "pwm1"),
-		  SUNXI_FUNCTION(0x5, "i2c2_SDA"),		/* SDA */
+		  SUNXI_FUNCTION(0x2, "UART5_RX"),		/* RX */
+		  SUNXI_FUNCTION(0x4, "PWM1"),
+		  SUNXI_FUNCTION(0x5, "I2C2_SDA"),		/* SDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 3)),	/* PH_EINT3 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 4),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x3, "spdif_OUT"),		/* OUT */
-		  SUNXI_FUNCTION(0x5, "i2c3_SCK"),		/* SCK */
+		  SUNXI_FUNCTION(0x5, "I2C3_SCK"),		/* SCK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 4)),	/* PH_EINT4 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 5),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart2_TX"),		/* TX */
-		  SUNXI_FUNCTION(0x3, "i2s3_MCLK"),		/* MCLK */
-		  SUNXI_FUNCTION(0x4, "spi1_CS0"),		/* CS0 */
-		  SUNXI_FUNCTION(0x5, "i2c3_SDA"),		/* SDA */
+		  SUNXI_FUNCTION(0x2, "UART2_TX"),		/* TX */
+		  SUNXI_FUNCTION(0x3, "I2S3_MCLK"),		/* MCLK */
+		  SUNXI_FUNCTION(0x4, "SPI1_CS0"),		/* CS0 */
+		  SUNXI_FUNCTION(0x5, "I2C3_SDA"),		/* SDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 5)),	/* PH_EINT5 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 6),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart2_RX"),		/* RX */
-		  SUNXI_FUNCTION(0x3, "i2s3_BCLK"),		/* BCLK */
-		  SUNXI_FUNCTION(0x4, "spi1_CLK"),		/* CLK */
-		  SUNXI_FUNCTION(0x5, "i2c4_SCK"),		/* SCK */
+		  SUNXI_FUNCTION(0x2, "UART2_RX"),		/* RX */
+		  SUNXI_FUNCTION(0x3, "I2S3_BCLK"),		/* BCLK */
+		  SUNXI_FUNCTION(0x4, "SPI1_CLK"),		/* CLK */
+		  SUNXI_FUNCTION(0x5, "I2C4_SCK"),		/* SCK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 6)),	/* PH_EINT6 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 7),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart2_RTS"),		/* RTS */
-		  SUNXI_FUNCTION(0x3, "i2s3_SYNC"),		/* SYNC */
-		  SUNXI_FUNCTION(0x4, "spi1_MOSI"),		/* MOSI */
-		  SUNXI_FUNCTION(0x5, "i2c4_SDA"),		/* SDA */
+		  SUNXI_FUNCTION(0x2, "UART2_RTS"),		/* RTS */
+		  SUNXI_FUNCTION(0x3, "I2S3_SYNC"),		/* SYNC */
+		  SUNXI_FUNCTION(0x4, "SPI1_MOSI"),		/* MOSI */
+		  SUNXI_FUNCTION(0x5, "I2C4_SDA"),		/* SDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 7)),	/* PH_EINT7 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 8),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x2, "uart2_CTS"),		/* CTS */
-		  SUNXI_FUNCTION(0x3, "i2s3_dout0_DO0"),		/* DO0 */
-		  SUNXI_FUNCTION(0x4, "spi1_MISO"),		/* MISO */
-		  SUNXI_FUNCTION(0x5, "i2s3_din1_DI1"),		/* DI1 */
+		  SUNXI_FUNCTION(0x2, "UART2_CTS"),		/* CTS */
+		  SUNXI_FUNCTION(0x3, "I2S3_dout0_DO0"),		/* DO0 */
+		  SUNXI_FUNCTION(0x4, "SPI1_MISO"),		/* MISO */
+		  SUNXI_FUNCTION(0x5, "I2S3_din1_DI1"),		/* DI1 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 8)),	/* PH_EINT8 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 9),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
-		  SUNXI_FUNCTION(0x3, "i2s3_din0_DI0"),		/* DI0 */
-		  SUNXI_FUNCTION(0x4, "spi1_CS1"),		/* CS1 */
-		  SUNXI_FUNCTION(0x5, "i2s3_dout1_DO1"),		/* DO1 */
+		  SUNXI_FUNCTION(0x3, "I2S3_din0_DI0"),		/* DI0 */
+		  SUNXI_FUNCTION(0x4, "SPI1_CS1"),		/* CS1 */
+		  SUNXI_FUNCTION(0x5, "I2S3_dout1_DO1"),		/* DO1 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 9)),	/* PH_EINT9 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(H, 10),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x3, "ir_rx"),
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 6, 10)),	/* PH_EINT10 */
 	/* Hole */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 0),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ERXD3"),		/* ERXD3 */
 		  SUNXI_FUNCTION(0x3, "dmic_CLK"),		/* CLK */
-		  SUNXI_FUNCTION(0x4, "i2s0_MCLK"),		/* MCLK */
+		  SUNXI_FUNCTION(0x4, "I2S0_MCLK"),		/* MCLK */
 		  SUNXI_FUNCTION(0x5, "hdmi_HSCL"),		/* HSCL */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 0)),	/* PI_EINT0 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 1),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ERXD2"),		/* ERXD2 */
 		  SUNXI_FUNCTION(0x3, "dmic_DATA0"),		/* DATA0 */
-		  SUNXI_FUNCTION(0x4, "i2s0_BCLK"),		/* BCLK */
+		  SUNXI_FUNCTION(0x4, "I2S0_BCLK"),		/* BCLK */
 		  SUNXI_FUNCTION(0x5, "hdmi_HSDA"),		/* HSDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 1)),	/* PI_EINT1 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 2),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ERXD1"),		/* ERXD1 */
 		  SUNXI_FUNCTION(0x3, "dmic_DATA1"),		/* DATA1 */
-		  SUNXI_FUNCTION(0x4, "i2s0_SYNC"),		/* SYNC */
+		  SUNXI_FUNCTION(0x4, "I2S0_SYNC"),		/* SYNC */
 		  SUNXI_FUNCTION(0x5, "hdmi_HCEC"),		/* HCEC */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 2)),	/* PI_EINT2 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 3),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ERXD0"),		/* ERXD0 */
 		  SUNXI_FUNCTION(0x3, "dmic_DATA2"),		/* DATA2 */
-		  SUNXI_FUNCTION(0x4, "i2s0_dout0_DO0"),		/* DO0 */
-		  SUNXI_FUNCTION(0x5, "i2s0_din1_DI1"),		/* DI1 */
+		  SUNXI_FUNCTION(0x4, "I2S0_dout0_DO0"),		/* DO0 */
+		  SUNXI_FUNCTION(0x5, "I2S0_din1_DI1"),		/* DI1 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 3)),	/* PI_EINT3 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 4),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ERXCK"),		/* ERXCK */
 		  SUNXI_FUNCTION(0x3, "dmic_DATA3"),		/* DATA3 */
-		  SUNXI_FUNCTION(0x4, "i2s0_din0_DI0"),		/* DI0 */
-		  SUNXI_FUNCTION(0x5, "i2s0_dout1_DO1"),		/* DO1 */
+		  SUNXI_FUNCTION(0x4, "I2S0_din0_DI0"),		/* DI0 */
+		  SUNXI_FUNCTION(0x5, "I2S0_dout1_DO1"),		/* DO1 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 4)),	/* PI_EINT4 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 5),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ERXCTL"),		/* ERXCTL */
-		  SUNXI_FUNCTION(0x3, "uart2_TX"),		/* TX */
+		  SUNXI_FUNCTION(0x3, "UART2_TX"),		/* TX */
 		  SUNXI_FUNCTION(0x4, "ts0_CLK"),		/* CLK */
-		  SUNXI_FUNCTION(0x5, "i2c0_SCK"),		/* SCK */
+		  SUNXI_FUNCTION(0x5, "I2C0_SCK"),		/* SCK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 5)),	/* PI_EINT5 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 6),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ENULL"),		/* ENULL */
-		  SUNXI_FUNCTION(0x3, "uart2_RX"),		/* RX */
+		  SUNXI_FUNCTION(0x3, "UART2_RX"),		/* RX */
 		  SUNXI_FUNCTION(0x4, "ts0_ERR"),		/* ERR */
-		  SUNXI_FUNCTION(0x5, "i2c0_SDA"),		/* SDA */
+		  SUNXI_FUNCTION(0x5, "I2C0_SDA"),		/* SDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 6)),	/* PI_EINT6 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 7),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ETXD3"),		/* ETXD3 */
-		  SUNXI_FUNCTION(0x3, "uart2_RTS"),		/* RTS */
+		  SUNXI_FUNCTION(0x3, "UART2_RTS"),		/* RTS */
 		  SUNXI_FUNCTION(0x4, "ts0_SYNC"),		/* SYNC */
-		  SUNXI_FUNCTION(0x5, "i2c1_SCK"),		/* SCK */
+		  SUNXI_FUNCTION(0x5, "I2C1_SCK"),		/* SCK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 7)),	/* PI_EINT7 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 8),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ETXD2"),		/* ETXD2 */
-		  SUNXI_FUNCTION(0x3, "uart2_CTS"),		/* CTS */
+		  SUNXI_FUNCTION(0x3, "UART2_CTS"),		/* CTS */
 		  SUNXI_FUNCTION(0x4, "ts0_DVLD"),		/* DVLD */
-		  SUNXI_FUNCTION(0x5, "i2c1_SDA"),		/* SDA */
+		  SUNXI_FUNCTION(0x5, "I2C1_SDA"),		/* SDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 8)),	/* PI_EINT8 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 9),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ETXD1"),		/* ETXD1 */
-		  SUNXI_FUNCTION(0x3, "uart3_TX"),		/* TX */
+		  SUNXI_FUNCTION(0x3, "UART3_TX"),		/* TX */
 		  SUNXI_FUNCTION(0x4, "ts0_D0"),		/* D0 */
-		  SUNXI_FUNCTION(0x5, "i2c2_SCK"),		/* SCK */
+		  SUNXI_FUNCTION(0x5, "I2C2_SCK"),		/* SCK */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 9)),	/* PI_EINT9 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 10),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ETXD0"),		/* ETXD0 */
-		  SUNXI_FUNCTION(0x3, "uart3_RX"),		/* RX */
+		  SUNXI_FUNCTION(0x3, "UART3_RX"),		/* RX */
 		  SUNXI_FUNCTION(0x4, "ts0_D1"),		/* D1 */
-		  SUNXI_FUNCTION(0x5, "i2c2_SDA"),		/* SDA */
+		  SUNXI_FUNCTION(0x5, "I2C2_SDA"),		/* SDA */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 10)),	/* PI_EINT10 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 11),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ETXCK"),		/* ETXCK */
-		  SUNXI_FUNCTION(0x3, "uart3_RTS"),		/* RTS */
+		  SUNXI_FUNCTION(0x3, "UART3_RTS"),		/* RTS */
 		  SUNXI_FUNCTION(0x4, "ts0_D2"),		/* D2 */
-		  SUNXI_FUNCTION(0x5, "pwm1"),
+		  SUNXI_FUNCTION(0x5, "PWM1"),
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 11)),	/* PI_EINT11 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 12),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ETXCTL"),		/* ETXCTL */
-		  SUNXI_FUNCTION(0x3, "uart3_CTS"),		/* CTS */
+		  SUNXI_FUNCTION(0x3, "UART3_CTS"),		/* CTS */
 		  SUNXI_FUNCTION(0x4, "ts0_D3"),		/* D3 */
-		  SUNXI_FUNCTION(0x5, "pwm2"),
+		  SUNXI_FUNCTION(0x5, "PWM2"),
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 12)),	/* PI_EINT12 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 13),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_ECLKIN"),		/* ECLKIN */
-		  SUNXI_FUNCTION(0x3, "uart4_TX"),		/* TX */
+		  SUNXI_FUNCTION(0x3, "UART4_TX"),		/* TX */
 		  SUNXI_FUNCTION(0x4, "ts0_D4"),		/* D4 */
-		  SUNXI_FUNCTION(0x5, "pwm3"),
+		  SUNXI_FUNCTION(0x5, "PWM3"),
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 13)),	/* PI_EINT13 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 14),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_MDC"),		/* MDC */
-		  SUNXI_FUNCTION(0x3, "uart4_RX"),		/* RX */
+		  SUNXI_FUNCTION(0x3, "UART4_RX"),		/* RX */
 		  SUNXI_FUNCTION(0x4, "ts0_D5"),		/* D5 */
-		  SUNXI_FUNCTION(0x5, "pwm4"),
+		  SUNXI_FUNCTION(0x5, "PWM4"),
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 14)),	/* PI_EINT14 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 15),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_MDIO"),		/* MDIO */
-		  SUNXI_FUNCTION(0x3, "uart4_RTS"),		/* RTS */
+		  SUNXI_FUNCTION(0x3, "UART4_RTS"),		/* RTS */
 		  SUNXI_FUNCTION(0x4, "ts0_D6"),		/* D6 */
 		  SUNXI_FUNCTION(0x5, "clock_CLK_FANOUT0"),		/* CLK_FANOUT0 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 15)),	/* PI_EINT15 */
 	SUNXI_PIN(SUNXI_PINCTRL_PIN(I, 16),
 		  SUNXI_FUNCTION(0x0, "IN"),
 		  SUNXI_FUNCTION(0x1, "OUT"),
 		  SUNXI_FUNCTION(0x2, "emac0_EPHY_CLK"),		/* EPHY_CLK */
-		  SUNXI_FUNCTION(0x3, "uart4_CTS"),		/* CTS */
+		  SUNXI_FUNCTION(0x3, "UART4_CTS"),		/* CTS */
 		  SUNXI_FUNCTION(0x4, "ts0_D7"),		/* D7 */
 		  SUNXI_FUNCTION(0x5, "clock_CLK_FANOUT1"),		/* CLK_FANOUT1 */
 		  SUNXI_FUNCTION_IRQ_BANK(0x6, 7, 16)),	/* PI_EINT16 */
 };
 static const unsigned int h616_irq_bank_map[] = { 0, 2, 3, 4, 5, 6, 7, 8 };
 
 const struct sunxi_pinctrl_desc h616_pinctrl_data = {
```

### Comparing `gpioc-1.1/libgpio/pinctrl-sunxi.c` & `gpioc-1.2/libgpio/pinctrl-sunxi.c`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/pinctrl-sunxi.h` & `gpioc-1.2/libgpio/pinctrl-sunxi.h`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/pinctrl.c` & `gpioc-1.2/libgpio/pinctrl.c`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/pinctrl.h` & `gpioc-1.2/libgpio/pinctrl.h`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/pinctrl_py.c` & `gpioc-1.2/libgpio/pinctrl_py.c`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/softpwm.c` & `gpioc-1.2/libgpio/softpwm.c`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/libgpio/softpwm_py.c` & `gpioc-1.2/libgpio/softpwm_py.c`

 * *Files identical despite different names*

### Comparing `gpioc-1.1/setup.py` & `gpioc-1.2/setup.py`

 * *Files identical despite different names*

