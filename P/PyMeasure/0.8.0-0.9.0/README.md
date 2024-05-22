# Comparing `tmp/PyMeasure-0.8.0.tar.gz` & `tmp/PyMeasure-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyMeasure-0.8.0.tar", last modified: Sun Mar 29 18:05:50 2020, max compression
+gzip compressed data, was "dist/PyMeasure-0.9.0.tar", last modified: Sun Feb  7 20:25:01 2021, max compression
```

## Comparing `PyMeasure-0.8.0.tar` & `PyMeasure-0.9.0.tar`

### file list

```diff
@@ -1,316 +1,355 @@
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/
--rw-rw-r--   0 colin     (1000) colin     (1000)      348 2020-03-29 15:29:21.000000 PyMeasure-0.8.0/AUTHORS.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)     7922 2020-03-29 18:04:47.000000 PyMeasure-0.8.0/CHANGES.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)     1069 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/LICENSE.txt
--rw-r--r--   0 colin     (1000) colin     (1000)      252 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/MANIFEST.in
--rw-rw-r--   0 colin     (1000) colin     (1000)    13045 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/PKG-INFO
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/PyMeasure.egg-info/
--rw-r--r--   0 colin     (1000) colin     (1000)    13045 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/PyMeasure.egg-info/PKG-INFO
--rw-r--r--   0 colin     (1000) colin     (1000)     9125 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/PyMeasure.egg-info/SOURCES.txt
--rw-r--r--   0 colin     (1000) colin     (1000)        1 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/PyMeasure.egg-info/dependency_links.txt
--rw-r--r--   0 colin     (1000) colin     (1000)      174 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/PyMeasure.egg-info/requires.txt
--rw-r--r--   0 colin     (1000) colin     (1000)       10 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/PyMeasure.egg-info/top_level.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)     2254 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/README.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/
--rw-r--r--   0 colin     (1000) colin     (1000)     6774 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/Makefile
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/about/
--rw-rw-r--   0 colin     (1000) colin     (1000)      756 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/about/authors.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)     1086 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/docs/about/license.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1573 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/adapters.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/display/
--rw-r--r--   0 colin     (1000) colin     (1000)      208 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/Qt.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      128 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/browser.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      124 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/curves.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      284 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      124 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/inputs.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      136 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/listeners.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      112 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/log.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      128 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/manager.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      122 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/plotter.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      124 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/thread.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      125 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/widgets.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      128 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/display/windows.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/experiment/
--rw-r--r--   0 colin     (1000) colin     (1000)      260 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/experiment/experiment.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      258 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/experiment/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      150 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/experiment/listeners.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      260 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/experiment/parameters.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      110 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/experiment/procedure.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      101 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/experiment/results.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      142 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/experiment/workers.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/advantest/
--rw-rw-r--   0 colin     (1000) colin     (1000)      229 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/advantest/advantestR3767CG.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      348 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/advantest/index.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/
--rw-rw-r--   0 colin     (1000) colin     (1000)      229 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/agilent33220A.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      273 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/agilent33500.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      256 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/agilent33521A.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      188 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/agilent34410A.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      249 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/agilent4156.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      188 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/agilent8257D.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      213 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/agilent8722ES.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      195 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/agilentE4408B.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      181 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/agilentE4980.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      466 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/agilent/index.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/ametek/
--rwxrwxr-x   0 colin     (1000) colin     (1000)      199 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/ametek/ametek7270.rst
--rwxrwxr-x   0 colin     (1000) colin     (1000)      327 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/ametek/index.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/ami/
--rw-r--r--   0 colin     (1000) colin     (1000)      148 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/ami/ami430.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      307 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/ami/index.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/anritsu/
--rw-r--r--   0 colin     (1000) colin     (1000)      196 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/anritsu/anritsuMG3692C.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      226 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/anritsu/anritsuMS9710C.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      354 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/anritsu/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      284 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/comedi.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/danfysik/
--rw-r--r--   0 colin     (1000) colin     (1000)      171 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/danfysik/adapters.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      177 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/danfysik/danfysik8500.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      350 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/danfysik/index.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/deltaelektronica/
--rw-rw-r--   0 colin     (1000) colin     (1000)      378 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/deltaelektronica/index.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      217 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/deltaelektronica/sm7045d.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/fwbell/
--rw-r--r--   0 colin     (1000) colin     (1000)      197 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/fwbell/fwbell5080.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      338 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/fwbell/index.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/hp/
--rw-r--r--   0 colin     (1000) colin     (1000)      203 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/hp/hp33120A.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      150 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/hp/hp34401A.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      369 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/hp/index.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      681 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      200 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/instruments.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/keithley/
--rw-rw-r--   0 colin     (1000) colin     (1000)      419 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/keithley/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      280 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/keithley/keithley2000.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      283 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/keithley/keithley2400.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      283 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/keithley/keithley2450.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      322 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/keithley/keithley2700.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      323 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/keithley/keithley2750.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      322 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/keithley/keithley6221.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/keysight/
--rw-rw-r--   0 colin     (1000) colin     (1000)      340 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/keysight/index.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      295 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/keysight/keysightN5767A.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/lakeshore/
--rw-r--r--   0 colin     (1000) colin     (1000)      209 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/lakeshore/adapters.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      419 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/lakeshore/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      211 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/lakeshore/lakeshore331.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      175 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/lakeshore/lakeshore425.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/newport/
--rw-r--r--   0 colin     (1000) colin     (1000)      465 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/newport/esp300.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      327 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/newport/index.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/ni/
--rw-rw-r--   0 colin     (1000) colin     (1000)      380 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/ni/index.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      801 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/ni/virtualbench.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/oxfordinstruments/
--rw-rw-r--   0 colin     (1000) colin     (1000)      271 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/oxfordinstruments/ITC503.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      388 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/oxfordinstruments/index.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/parker/
--rw-r--r--   0 colin     (1000) colin     (1000)      325 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/parker/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      193 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/parker/parkerGV6.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      218 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/resources.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/signalrecovery/
--rw-r--r--   0 colin     (1000) colin     (1000)      178 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/signalrecovery/dsp7265.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      367 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/signalrecovery/index.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/srs/
--rw-r--r--   0 colin     (1000) colin     (1000)      400 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/srs/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      156 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/srs/sr830.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/tektronix/
--rw-rw-r--   0 colin     (1000) colin     (1000)      208 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/tektronix/afg3152c.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      350 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/tektronix/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      155 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/tektronix/tds2000.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/thorlabs/
--rw-r--r--   0 colin     (1000) colin     (1000)      342 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/thorlabs/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      187 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/thorlabs/thorlabspm100usb.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      471 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/validators.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/api/instruments/yokogawa/
--rw-r--r--   0 colin     (1000) colin     (1000)      338 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/yokogawa/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      198 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/api/instruments/yokogawa/yokogawa7651.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)     8763 2020-03-29 18:04:47.000000 PyMeasure-0.8.0/docs/conf.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/dev/
--rw-rw-r--   0 colin     (1000) colin     (1000)    14336 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/docs/dev/adding_instruments.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)     1517 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/dev/coding_standards.rst
--rw-r--r--   0 colin     (1000) colin     (1000)     5040 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/dev/contribute.rst
--rw-r--r--   0 colin     (1000) colin     (1000)      310 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/dev/reporting_errors.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/images/
--rw-r--r--   0 colin     (1000) colin     (1000)    11879 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/images/PyMeasure logo.png
--rw-r--r--   0 colin     (1000) colin     (1000)    10682 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/images/PyMeasure logo.svg
--rw-rw-r--   0 colin     (1000) colin     (1000)    53215 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/images/PyMeasure preview.png
--rw-rw-r--   0 colin     (1000) colin     (1000)    12529 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/images/PyMeasure preview.svg
--rw-r--r--   0 colin     (1000) colin     (1000)     8627 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/images/PyMeasure.png
--rw-r--r--   0 colin     (1000) colin     (1000)    12669 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/images/PyMeasure.svg
--rw-r--r--   0 colin     (1000) colin     (1000)     2387 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)     2167 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/introduction.rst
--rw-r--r--   0 colin     (1000) colin     (1000)     6707 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/make.bat
--rw-r--r--   0 colin     (1000) colin     (1000)     1973 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/quick_start.rst
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/docs/tutorial/
--rw-rw-r--   0 colin     (1000) colin     (1000)     4121 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/connecting.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)    16789 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/graphical.rst
--rw-rw-r--   0 colin     (1000) colin     (1000)      158 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/gui_sequencer_example_sequence.txt
--rw-r--r--   0 colin     (1000) colin     (1000)      182 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/index.rst
--rw-r--r--   0 colin     (1000) colin     (1000)    16597 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/procedure.rst
--rw-r--r--   0 colin     (1000) colin     (1000)    88072 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/pymeasure-managedwindow-queued.png
--rw-r--r--   0 colin     (1000) colin     (1000)    78696 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/pymeasure-managedwindow-resume.png
--rw-r--r--   0 colin     (1000) colin     (1000)    79458 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/pymeasure-managedwindow-running.png
--rw-r--r--   0 colin     (1000) colin     (1000)    54424 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/pymeasure-managedwindow.png
--rw-r--r--   0 colin     (1000) colin     (1000)    28013 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/pymeasure-plotter.png
--rw-rw-r--   0 colin     (1000) colin     (1000)    11413 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/docs/tutorial/pymeasure-sequencer.png
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1179 2020-03-29 18:04:47.000000 PyMeasure-0.8.0/pymeasure/__init__.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/adapters/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1751 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/adapters/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4674 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/adapters/adapter.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     5238 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/adapters/prologix.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3063 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/adapters/serial.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     6536 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/adapters/visa.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3914 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/adapters/vxi11.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2131 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/console.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/display/
--rw-rw-r--   0 colin     (1000) colin     (1000)     2191 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/Qt.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1813 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     5317 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/browser.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     9549 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/curves.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     9635 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/inputs.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4453 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/listeners.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1569 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/log.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    12209 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/manager.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2586 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/plotter.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2180 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/thread.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    34935 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/widgets.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    34694 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/display/windows.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1293 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/errors.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/experiment/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1590 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/experiment/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1847 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/experiment/config.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     9657 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/experiment/experiment.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3991 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/experiment/listeners.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    15438 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/experiment/parameters.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     9505 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/experiment/procedure.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    13474 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/experiment/results.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     6330 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/experiment/workers.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1709 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/__init__.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/advantest/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1204 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/advantest/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2762 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/advantest/advantestR3767CG.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1516 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    12216 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent33220A.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    19408 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent33500.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2417 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent33521A.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2244 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent34410A.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    34297 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent4156.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    12507 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent8257D.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     7368 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent8722ES.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4314 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/agilentE4408B.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     7110 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/agilent/agilentE4980.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/ametek/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1192 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/ametek/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     8117 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/ametek/ametek7270.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/ami/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1184 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/ami/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     7503 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/ami/ami430.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/anritsu/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1243 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/anritsu/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2718 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/anritsu/anritsuMG3692C.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    10650 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/anritsu/anritsuMS9710C.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     6940 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/comedi.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/danfysik/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1234 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/danfysik/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2899 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/danfysik/adapters.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    12155 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/danfysik/danfysik8500.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/deltaelektronika/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1186 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/deltaelektronika/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4897 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/deltaelektronika/sm7045d.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/fwbell/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1192 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/fwbell/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     5785 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/fwbell/fwbell5080.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/hp/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1219 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/hp/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4833 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/hp/hp33120A.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2036 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/hp/hp34401A.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    14722 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/instrument.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/keithley/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1391 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/keithley/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4712 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/keithley/buffer.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    24815 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2000.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    27031 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2400.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    19237 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2450.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    13016 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2700.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3507 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2750.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    19204 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley6221.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/keysight/
--rw-rw-r--   0 colin     (1000) colin     (1000)       42 2020-03-29 15:29:24.000000 PyMeasure-0.8.0/pymeasure/instruments/keysight/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3846 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/keysight/keysightN5767A.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/lakeshore/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1277 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/lakeshore/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2114 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/lakeshore/adapters.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     5077 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/lakeshore/lakeshore331.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4398 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/lakeshore/lakeshore425.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3124 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/mock.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/newport/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1184 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/newport/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    10943 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/newport/esp300.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/ni/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1502 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/ni/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     6773 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/ni/daqmx.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2493 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/ni/nidaq.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    74100 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/ni/virtualbench.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/oxfordinstruments/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1184 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/oxfordinstruments/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    11320 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/oxfordinstruments/itc503.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/parker/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1190 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/parker/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     7657 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/parker/parkerGV6.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2273 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/resources.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/signalrecovery/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1186 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/signalrecovery/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     9898 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/signalrecovery/dsp7265.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/srs/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1207 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/srs/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3826 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/srs/sg380.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    16407 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/srs/sr830.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/tektronix/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1217 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/tektronix/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     7664 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/tektronix/afg3152c.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3438 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/tektronix/tds2000.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/thorlabs/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1204 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/thorlabs/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4089 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/thorlabs/thorlabspm100usb.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     5673 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/validators.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/pymeasure/instruments/yokogawa/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1196 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/yokogawa/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     9096 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/instruments/yokogawa/yokogawa7651.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3894 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/log.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2251 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/process.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2121 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/pymeasure/thread.py
--rw-r--r--   0 colin     (1000) colin     (1000)       63 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/setup.cfg
--rw-rw-r--   0 colin     (1000) colin     (1000)     2884 2020-03-29 18:04:47.000000 PyMeasure-0.8.0/setup.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/tests/
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/tests/adapters/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1609 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/adapters/test_adapter.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1271 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/adapters/test_visa.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1171 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/conftest.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/tests/display/
--rw-rw-r--   0 colin     (1000) colin     (1000)     7926 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/display/test_inputs.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2014 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/display/test_plotter.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2377 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/display/test_windows.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/tests/experiment/
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/tests/experiment/data/
--rw-r--r--   0 colin     (1000) colin     (1000)        0 2020-03-29 15:29:21.000000 PyMeasure-0.8.0/tests/experiment/data/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1989 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/experiment/data/procedure_for_testing.py
--rw-r--r--   0 colin     (1000) colin     (1000)        0 2020-03-29 15:29:21.000000 PyMeasure-0.8.0/tests/experiment/data/results_for_testing.csv
--rw-rw-r--   0 colin     (1000) colin     (1000)     1510 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/experiment/test_listeners.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     3217 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/experiment/test_parameters.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2096 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/experiment/test_procedure.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4523 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/experiment/test_results.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     2558 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/experiment/test_workers.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/tests/instruments/
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2020-03-29 18:05:50.000000 PyMeasure-0.8.0/tests/instruments/keithley/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1982 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/instruments/keithley/test_keithley2750.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4710 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/instruments/test_instrument.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     4352 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/instruments/test_validators.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1660 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/test_log.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1510 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/test_process.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     1449 2020-03-29 15:33:43.000000 PyMeasure-0.8.0/tests/test_thread.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/tests/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1510 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/test_process.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/tests/instruments/
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/tests/instruments/keithley/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1982 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/instruments/keithley/test_keithley2750.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/tests/instruments/keysight/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    14075 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/instruments/keysight/test_keysightDSOX1102G.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4352 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/instruments/test_validators.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/tests/instruments/agilent/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    19972 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/instruments/agilent/test_agilent34450A.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5873 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/instruments/test_instrument.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/tests/adapters/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2028 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/adapters/test_adapter.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2631 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/adapters/test_visa.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1171 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/conftest.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1449 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/test_thread.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/tests/display/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9581 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/display/test_inputs.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2014 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/display/test_plotter.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2377 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/display/test_windows.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2083 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/test_log.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/tests/experiment/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2932 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/experiment/test_workers.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/tests/experiment/data/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4776 2021-02-07 19:53:45.000000 PyMeasure-0.9.0/tests/experiment/data/results_for_testing_parameters.csv
+-rw-r--r--   0 colin     (1000) colin     (1000)        0 2020-03-29 15:29:21.000000 PyMeasure-0.9.0/tests/experiment/data/results_for_testing.csv
+-rw-r--r--   0 colin     (1000) colin     (1000)        0 2021-02-07 18:42:22.000000 PyMeasure-0.9.0/tests/experiment/data/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1989 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/experiment/data/procedure_for_testing.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2096 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/experiment/test_procedure.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5356 2021-02-07 19:53:45.000000 PyMeasure-0.9.0/tests/experiment/test_parameters.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1510 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/tests/experiment/test_listeners.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5518 2021-02-07 19:53:45.000000 PyMeasure-0.9.0/tests/experiment/test_results.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2912 2021-02-07 20:24:25.000000 PyMeasure-0.9.0/setup.py
+-rw-r--r--   0 colin     (1000) colin     (1000)       63 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/setup.cfg
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9346 2021-02-07 20:24:25.000000 PyMeasure-0.9.0/CHANGES.txt
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/PyMeasure.egg-info/
+-rw-r--r--   0 colin     (1000) colin     (1000)        1 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/PyMeasure.egg-info/dependency_links.txt
+-rw-r--r--   0 colin     (1000) colin     (1000)       10 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/PyMeasure.egg-info/top_level.txt
+-rw-r--r--   0 colin     (1000) colin     (1000)    10512 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/PyMeasure.egg-info/SOURCES.txt
+-rw-r--r--   0 colin     (1000) colin     (1000)      174 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/PyMeasure.egg-info/requires.txt
+-rw-r--r--   0 colin     (1000) colin     (1000)    14473 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/PyMeasure.egg-info/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)      536 2021-02-07 18:42:52.000000 PyMeasure-0.9.0/AUTHORS.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2078 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/README.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      252 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/MANIFEST.in
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1069 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/LICENSE.txt
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/
+-rw-r--r--   0 colin     (1000) colin     (1000)     6707 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/make.bat
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2658 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)     2167 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/introduction.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/dev/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      309 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/dev/reporting_errors.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5036 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/dev/contribute.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)    20463 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/docs/dev/adding_instruments.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1611 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/dev/coding_standards.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)     6774 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/Makefile
+-rw-rw-r--   0 colin     (1000) colin     (1000)     8781 2021-02-07 20:24:25.000000 PyMeasure-0.9.0/docs/conf.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/danfysik/
+-rw-r--r--   0 colin     (1000) colin     (1000)      350 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/danfysik/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      177 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/danfysik/danfysik8500.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      171 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/danfysik/adapters.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      736 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/index.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/keithley/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      435 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keithley/index.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      323 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keithley/keithley2750.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      322 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keithley/keithley2700.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      280 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keithley/keithley2000.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      322 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keithley/keithley6221.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      306 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keithley/keithley6517b.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      283 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keithley/keithley2400.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      283 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keithley/keithley2450.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/keysight/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      361 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keysight/index.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      244 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keysight/keysightDSOX1102G.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      295 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/keysight/keysightN5767A.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/signalrecovery/
+-rw-r--r--   0 colin     (1000) colin     (1000)      367 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/signalrecovery/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      178 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/signalrecovery/dsp7265.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      471 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/validators.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/advantest/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      348 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/advantest/index.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      229 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/advantest/advantestR3767CG.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/attocube/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      345 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/attocube/index.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      306 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/attocube/anc300.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      170 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/attocube/adapters.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/
+-rw-r--r--   0 colin     (1000) colin     (1000)      181 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilentE4980.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      213 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilent8722ES.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      499 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      195 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilentE4408B.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      273 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilent33500.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      188 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilent8257D.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      235 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilent34450A.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      188 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilent34410A.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)    11151 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilentB1500.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      249 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilent4156.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      256 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilent33521A.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      229 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/agilent/agilent33220A.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/yokogawa/
+-rw-r--r--   0 colin     (1000) colin     (1000)      338 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/yokogawa/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      198 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/yokogawa/yokogawa7651.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/deltaelektronica/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      378 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/deltaelektronica/index.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      217 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/deltaelektronica/sm7045d.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/lakeshore/
+-rw-r--r--   0 colin     (1000) colin     (1000)      175 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/lakeshore/lakeshore425.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      419 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/lakeshore/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      211 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/lakeshore/lakeshore331.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      209 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/lakeshore/adapters.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      284 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/comedi.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/oxfordinstruments/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      388 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/oxfordinstruments/index.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      271 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/oxfordinstruments/ITC503.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/fwbell/
+-rw-r--r--   0 colin     (1000) colin     (1000)      338 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/fwbell/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      197 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/fwbell/fwbell5080.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/tektronix/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      350 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/tektronix/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      155 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/tektronix/tds2000.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      208 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/tektronix/afg3152c.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/anapico/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      193 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/anapico/apsin12G.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      329 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/anapico/index.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/ni/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      380 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/ni/index.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1255 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/ni/virtualbench.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/srs/
+-rw-r--r--   0 colin     (1000) colin     (1000)      156 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/srs/sr830.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      409 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/srs/index.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      156 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/srs/sr860.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/anritsu/
+-rw-r--r--   0 colin     (1000) colin     (1000)      196 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/anritsu/anritsuMG3692C.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      354 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/anritsu/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      226 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/anritsu/anritsuMS9710C.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/parker/
+-rw-r--r--   0 colin     (1000) colin     (1000)      325 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/parker/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      193 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/parker/parkerGV6.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/newport/
+-rw-r--r--   0 colin     (1000) colin     (1000)      327 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/newport/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      465 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/newport/esp300.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/hp/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      369 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/hp/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      203 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/hp/hp33120A.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      150 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/hp/hp34401A.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      200 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/instruments.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/razorbill/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      346 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/razorbill/index.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      346 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/razorbill/razorbillRP100.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/thorlabs/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      362 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/thorlabs/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      187 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/thorlabs/thorlabspm100usb.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)      217 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/thorlabs/thorlabspro8000.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/ami/
+-rw-r--r--   0 colin     (1000) colin     (1000)      307 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/ami/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      148 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/ami/ami430.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/instruments/ametek/
+-rwxrwxr-x   0 colin     (1000) colin     (1000)      199 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/ametek/ametek7270.rst
+-rwxrwxr-x   0 colin     (1000) colin     (1000)      327 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/ametek/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      218 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/instruments/resources.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/display/
+-rw-r--r--   0 colin     (1000) colin     (1000)      122 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/plotter.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      124 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/curves.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      284 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      208 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/Qt.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      128 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/browser.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      128 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/windows.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      112 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/log.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      125 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/widgets.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      124 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/inputs.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      136 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/listeners.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      124 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/thread.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      128 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/display/manager.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/api/experiment/
+-rw-r--r--   0 colin     (1000) colin     (1000)      258 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/experiment/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      110 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/experiment/procedure.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      101 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/experiment/results.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      260 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/experiment/parameters.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      142 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/experiment/workers.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      150 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/experiment/listeners.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)      260 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/experiment/experiment.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1749 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/api/adapters.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/tutorial/
+-rw-r--r--   0 colin     (1000) colin     (1000)      182 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/tutorial/index.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)    54424 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/tutorial/pymeasure-managedwindow.png
+-rw-rw-r--   0 colin     (1000) colin     (1000)    16599 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/tutorial/procedure.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4121 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/tutorial/connecting.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)    11413 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/tutorial/pymeasure-sequencer.png
+-rw-r--r--   0 colin     (1000) colin     (1000)    88072 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/tutorial/pymeasure-managedwindow-queued.png
+-rw-rw-r--   0 colin     (1000) colin     (1000)    18428 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/tutorial/graphical.rst
+-rw-r--r--   0 colin     (1000) colin     (1000)    78696 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/tutorial/pymeasure-managedwindow-resume.png
+-rw-rw-r--   0 colin     (1000) colin     (1000)      158 2021-02-07 18:42:52.000000 PyMeasure-0.9.0/docs/tutorial/gui_sequencer_example_sequence.txt
+-rw-r--r--   0 colin     (1000) colin     (1000)    79458 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/tutorial/pymeasure-managedwindow-running.png
+-rw-r--r--   0 colin     (1000) colin     (1000)    28013 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/tutorial/pymeasure-plotter.png
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4681 2021-01-17 19:45:57.000000 PyMeasure-0.9.0/docs/tutorial/pymeasure-directoryinput.png
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1968 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/quick_start.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/about/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      902 2021-02-07 18:42:44.000000 PyMeasure-0.9.0/docs/about/authors.rst
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1086 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/docs/about/license.rst
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/docs/images/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    12529 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/images/PyMeasure preview.svg
+-rw-r--r--   0 colin     (1000) colin     (1000)     8627 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/images/PyMeasure.png
+-rw-rw-r--   0 colin     (1000) colin     (1000)    53215 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/images/PyMeasure preview.png
+-rw-r--r--   0 colin     (1000) colin     (1000)    10682 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/images/PyMeasure logo.svg
+-rw-r--r--   0 colin     (1000) colin     (1000)    11879 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/images/PyMeasure logo.png
+-rw-r--r--   0 colin     (1000) colin     (1000)    12669 2020-03-29 15:29:24.000000 PyMeasure-0.9.0/docs/images/PyMeasure.svg
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2655 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/thread.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/danfysik/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2899 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/danfysik/adapters.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1234 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/danfysik/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    12155 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/danfysik/danfysik8500.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4712 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/buffer.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    28819 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2400.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    24815 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2000.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    19204 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley6221.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    12629 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley6517b.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1432 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    13041 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2700.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3507 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2750.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    23927 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2450.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/keysight/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3846 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keysight/keysightN5767A.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    23150 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/keysight/keysightDSOX1102G.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)       92 2021-02-07 18:42:22.000000 PyMeasure-0.9.0/pymeasure/instruments/keysight/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/signalrecovery/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9898 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/signalrecovery/dsp7265.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1186 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/signalrecovery/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/advantest/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2762 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/advantest/advantestR3767CG.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1204 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/advantest/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/attocube/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9497 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/attocube/anc300.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5397 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/attocube/adapters.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1239 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/attocube/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    12494 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent8257D.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2417 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent33521A.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    78530 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilentB1500.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    12216 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent33220A.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    34299 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent4156.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9883 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent8722ES.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2232 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent34410A.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1596 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    25278 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent34450A.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4314 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilentE4408B.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    19408 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent33500.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     7110 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/agilent/agilentE4980.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/yokogawa/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9091 2021-02-07 20:24:25.000000 PyMeasure-0.9.0/pymeasure/instruments/yokogawa/yokogawa7651.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1196 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/yokogawa/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/lakeshore/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2114 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/lakeshore/adapters.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1277 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/lakeshore/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4398 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/lakeshore/lakeshore425.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5077 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/lakeshore/lakeshore331.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/oxfordinstruments/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    13198 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/oxfordinstruments/itc503.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1184 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/oxfordinstruments/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/fwbell/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5785 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/fwbell/fwbell5080.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1192 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/fwbell/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/tektronix/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3438 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/tektronix/tds2000.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1217 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/tektronix/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     7664 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/tektronix/afg3152c.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/anapico/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3078 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/anapico/apsin12G.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1188 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/anapico/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/ni/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     6773 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/ni/daqmx.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2493 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/ni/nidaq.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    63203 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/ni/virtualbench.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1502 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/ni/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    14730 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/instrument.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/srs/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    23058 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/srs/sr860.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    16597 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/srs/sr830.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3826 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/srs/sg380.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1232 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/srs/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5673 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/validators.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2281 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/resources.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3124 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/mock.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/anritsu/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2718 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/anritsu/anritsuMG3692C.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    10650 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/anritsu/anritsuMS9710C.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1243 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/anritsu/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/deltaelektronika/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4897 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/deltaelektronika/sm7045d.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1186 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/deltaelektronika/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/parker/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     7657 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/parker/parkerGV6.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1190 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/parker/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/newport/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    10943 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/newport/esp300.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1184 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/newport/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1890 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/hp/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4833 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/hp/hp33120A.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1219 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/hp/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2036 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/hp/hp34401A.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     6940 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/comedi.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/razorbill/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4601 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/razorbill/razorbillRP100.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1200 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/razorbill/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/thorlabs/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4089 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/thorlabs/thorlabspm100usb.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3667 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/thorlabs/thorlabspro8000.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1249 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/thorlabs/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/ami/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1184 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/ami/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     7503 2021-02-07 20:24:25.000000 PyMeasure-0.9.0/pymeasure/instruments/ami/ami430.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/instruments/ametek/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     8117 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/ametek/ametek7270.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1192 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/instruments/ametek/__init__.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/adapters/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5489 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/adapters/prologix.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4150 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/adapters/vxi11.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     6310 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/adapters/visa.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5687 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/adapters/adapter.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1804 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/adapters/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3174 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/adapters/serial.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3344 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/adapters/telnet.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2131 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/console.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2251 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/process.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3890 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/log.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1179 2021-02-07 20:24:25.000000 PyMeasure-0.9.0/pymeasure/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1293 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/errors.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/display/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    36004 2021-02-07 20:24:25.000000 PyMeasure-0.9.0/pymeasure/display/widgets.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2191 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/Qt.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2180 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/thread.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     5317 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/browser.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    12238 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/manager.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9771 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/inputs.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1569 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/log.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2586 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/plotter.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9549 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/curves.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1813 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    37068 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/windows.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4453 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/display/listeners.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/pymeasure/experiment/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9800 2021-02-07 20:24:25.000000 PyMeasure-0.9.0/pymeasure/experiment/experiment.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    12930 2021-02-07 19:53:45.000000 PyMeasure-0.9.0/pymeasure/experiment/results.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    17172 2021-02-07 19:53:45.000000 PyMeasure-0.9.0/pymeasure/experiment/parameters.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1881 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/experiment/config.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     6330 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/experiment/workers.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1590 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/experiment/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9505 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/experiment/procedure.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     4102 2021-02-07 19:29:19.000000 PyMeasure-0.9.0/pymeasure/experiment/listeners.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    14473 2021-02-07 20:25:01.000000 PyMeasure-0.9.0/PKG-INFO
```

### Comparing `PyMeasure-0.8.0/CHANGES.txt` & `PyMeasure-0.9.0/CHANGES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Version 0.9 -- released 2/7/21
+==============================
+- PyMeasure is now officially at github.com/pymeasure/pymeasure
+- Python 3.9 is now supported, Python 3.5 removed due to EOL
+- Move to GitHub Actions from TravisCI and Appveyor for CI (@bilderbuchi)
+- New additions to Oxford Instruments ITC 503 (@CasperSchippers)
+- New Agilent 34450A and Keysight DSOX1102G instruments (@theMashUp, @jlarochelle)
+- Improvements to NI VirtualBench (@moritzj29)
+- New Agilent B1500 instrument (@moritzj29)
+- New Keithley 6517B instrument (@wehlgrundspitze)
+- Major improvements to PyVISA compatbility (@bilderbuchi, @msmttchr, @CasperSchippers, @cjermain)
+- New Anapico APSIN12G instrument (@StePhanino)
+- Improvements to Thorelabs Pro 8000 and SR830 (@Mike-HubGit)
+- New SR860 instrument (@StevenSiegl, @bklebel)
+- Fix to escape sequences (@tirkarthi)
+- New directory input for ManagedWindow (@paulgoulain)
+- New TelnetAdapter and Attocube ANC300 Piezo controller (@dkriegner)
+- New Agilent 34450A (@theMashUp)
+- New Razorbill RP100 strain cell controller (@pheowl)
+- Fixes to precision and default value of ScientificInput and FloatParameter (@moritzj29)
+- Fixes for Keithly 2400 and 2450 controls (@pyMatJ)
+- Improvments to Inputs and open_file_externally (@msmttchr)
+- Fixes to Agilent 8722ES (@alexmcnabb)
+- Fixes to QThread cleanup (@neal-kepler, @msmttchr)
+- Fixes to Keyboard interrupt, and parameters (@CasperSchippers)
+
 Version 0.8 -- released 3/29/19
 ===============================
 - Python 3.8 is now supported
 - New Measurement Sequencer allows for running over a large parameter space (@CasperSchippers)
 - New image plotting feature for live image measurements (@jmittelstaedt)
 - Improvements to VISA adapter (@moritzj29)
 - Added Tektronix AFG 3000, Keithley 2750 (@StePhanino, @dennisfeng2)
```

### Comparing `PyMeasure-0.8.0/LICENSE.txt` & `PyMeasure-0.9.0/docs/about/license.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-Copyright (c) 2013-2020 PyMeasure Developers
+License
+=======
+
+Copyright (c) 2013-2021 PyMeasure Developers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/PKG-INFO` & `PyMeasure-0.9.0/PyMeasure.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 Metadata-Version: 2.1
 Name: PyMeasure
-Version: 0.8.0
+Version: 0.9.0
 Summary: Scientific measurement library for instruments, experiments, and live-plotting
-Home-page: https://github.com/ralph-group/pymeasure
+Home-page: https://github.com/pymeasure/pymeasure
 Author: PyMeasure Developers
 License: MIT License
-Download-URL: https://github.com/ralph-group/pymeasure/tarball/v0.8.0
-Description: .. image:: https://raw.githubusercontent.com/ralph-group/pymeasure/master/docs/images/PyMeasure.png
+Download-URL: https://github.com/pymeasure/pymeasure/tarball/v0.9.0
+Description: .. image:: https://raw.githubusercontent.com/pymeasure/pymeasure/master/docs/images/PyMeasure.png
             :alt: PyMeasure Scientific package
         
         PyMeasure scientific package
         ############################
         
         PyMeasure makes scientific measurements easy to set up and run. The package contains a repository of instrument classes and a system for running experiment procedures, which provides graphical interfaces for graphing live data and managing queues of experiments. Both parts of the package are independent, and when combined provide all the necessary requirements for advanced measurements with only limited coding.
         
         PyMeasure is currently under active development, so please report any issues you experience to our `Issues page`_.
         
-        .. _Issues page: https://github.com/ralph-group/pymeasure/issues
+        .. _Issues page: https://github.com/pymeasure/pymeasure/issues
         
-        PyMeasure runs on Python 3.5, 3.6, 3.7 and 3.8, and is tested with continous-integration on Linux, macOS, and Windows.
+        PyMeasure runs on Python 3.6, 3.7, 3.8 and 3.9, and is tested with continous-integration on Linux, macOS, and Windows.
         
-        .. image:: https://ci.appveyor.com/api/projects/status/hcj2n2a7l97wfbb8/branch/master?svg=true
-            :target: https://ci.appveyor.com/project/cjermain/pymeasure
-        
-        .. image:: https://travis-ci.org/ralph-group/pymeasure.svg?branch=master
-            :target: https://travis-ci.org/ralph-group/pymeasure
+        .. image:: https://github.com/pymeasure/pymeasure/workflows/Pymeasure%20CI/badge.svg
+            :target: https://github.com/pymeasure/pymeasure/actions
         
         .. image:: http://readthedocs.org/projects/pymeasure/badge/?version=latest
             :target: http://pymeasure.readthedocs.io/en/latest/?badge=latest
             :alt: Documentation Status
         
-        .. image:: https://zenodo.org/badge/23569/ralph-group/pymeasure.svg
-           :target: https://zenodo.org/badge/latestdoi/23569/ralph-group/pymeasure
+        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3732545.svg
+           :target: https://doi.org/10.5281/zenodo.3732545
         
         .. image:: https://anaconda.org/conda-forge/pymeasure/badges/version.svg
            :target: https://anaconda.org/conda-forge/pymeasure
         
         .. image:: https://anaconda.org/conda-forge/pymeasure/badges/downloads.svg
            :target: https://anaconda.org/conda-forge/pymeasure
         
@@ -45,16 +42,42 @@
         
         Check out `the documentation`_ for the `quick start guide`_, that covers the installation of Python and PyMeasure.
         
         There are a number of examples in the `examples`_ directory that can help you get up and running.
         
         .. _the documentation: http://pymeasure.readthedocs.org/en/latest/
         .. _quick start guide: http://pymeasure.readthedocs.io/en/latest/quick_start.html
-        .. _examples: https://github.com/ralph-group/pymeasure/tree/master/examples
+        .. _examples: https://github.com/pymeasure/pymeasure/tree/master/examples
+        
         
+        Version 0.9 -- released 2/7/21
+        ==============================
+        - PyMeasure is now officially at github.com/pymeasure/pymeasure
+        - Python 3.9 is now supported, Python 3.5 removed due to EOL
+        - Move to GitHub Actions from TravisCI and Appveyor for CI (@bilderbuchi)
+        - New additions to Oxford Instruments ITC 503 (@CasperSchippers)
+        - New Agilent 34450A and Keysight DSOX1102G instruments (@theMashUp, @jlarochelle)
+        - Improvements to NI VirtualBench (@moritzj29)
+        - New Agilent B1500 instrument (@moritzj29)
+        - New Keithley 6517B instrument (@wehlgrundspitze)
+        - Major improvements to PyVISA compatbility (@bilderbuchi, @msmttchr, @CasperSchippers, @cjermain)
+        - New Anapico APSIN12G instrument (@StePhanino)
+        - Improvements to Thorelabs Pro 8000 and SR830 (@Mike-HubGit)
+        - New SR860 instrument (@StevenSiegl, @bklebel)
+        - Fix to escape sequences (@tirkarthi)
+        - New directory input for ManagedWindow (@paulgoulain)
+        - New TelnetAdapter and Attocube ANC300 Piezo controller (@dkriegner)
+        - New Agilent 34450A (@theMashUp)
+        - New Razorbill RP100 strain cell controller (@pheowl)
+        - Fixes to precision and default value of ScientificInput and FloatParameter (@moritzj29)
+        - Fixes for Keithly 2400 and 2450 controls (@pyMatJ)
+        - Improvments to Inputs and open_file_externally (@msmttchr)
+        - Fixes to Agilent 8722ES (@alexmcnabb)
+        - Fixes to QThread cleanup (@neal-kepler, @msmttchr)
+        - Fixes to Keyboard interrupt, and parameters (@CasperSchippers)
         
         Version 0.8 -- released 3/29/19
         ===============================
         - Python 3.8 is now supported
         - New Measurement Sequencer allows for running over a large parameter space (@CasperSchippers)
         - New image plotting feature for live image measurements (@jmittelstaedt)
         - Improvements to VISA adapter (@moritzj29)
@@ -234,15 +257,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Provides-Extra: python-vxi11
 Provides-Extra: matplotlib
 Provides-Extra: tcp
+Provides-Extra: python-vxi11
```

### Comparing `PyMeasure-0.8.0/PyMeasure.egg-info/PKG-INFO` & `PyMeasure-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 Metadata-Version: 2.1
 Name: PyMeasure
-Version: 0.8.0
+Version: 0.9.0
 Summary: Scientific measurement library for instruments, experiments, and live-plotting
-Home-page: https://github.com/ralph-group/pymeasure
+Home-page: https://github.com/pymeasure/pymeasure
 Author: PyMeasure Developers
 License: MIT License
-Download-URL: https://github.com/ralph-group/pymeasure/tarball/v0.8.0
-Description: .. image:: https://raw.githubusercontent.com/ralph-group/pymeasure/master/docs/images/PyMeasure.png
+Download-URL: https://github.com/pymeasure/pymeasure/tarball/v0.9.0
+Description: .. image:: https://raw.githubusercontent.com/pymeasure/pymeasure/master/docs/images/PyMeasure.png
             :alt: PyMeasure Scientific package
         
         PyMeasure scientific package
         ############################
         
         PyMeasure makes scientific measurements easy to set up and run. The package contains a repository of instrument classes and a system for running experiment procedures, which provides graphical interfaces for graphing live data and managing queues of experiments. Both parts of the package are independent, and when combined provide all the necessary requirements for advanced measurements with only limited coding.
         
         PyMeasure is currently under active development, so please report any issues you experience to our `Issues page`_.
         
-        .. _Issues page: https://github.com/ralph-group/pymeasure/issues
+        .. _Issues page: https://github.com/pymeasure/pymeasure/issues
         
-        PyMeasure runs on Python 3.5, 3.6, 3.7 and 3.8, and is tested with continous-integration on Linux, macOS, and Windows.
+        PyMeasure runs on Python 3.6, 3.7, 3.8 and 3.9, and is tested with continous-integration on Linux, macOS, and Windows.
         
-        .. image:: https://ci.appveyor.com/api/projects/status/hcj2n2a7l97wfbb8/branch/master?svg=true
-            :target: https://ci.appveyor.com/project/cjermain/pymeasure
-        
-        .. image:: https://travis-ci.org/ralph-group/pymeasure.svg?branch=master
-            :target: https://travis-ci.org/ralph-group/pymeasure
+        .. image:: https://github.com/pymeasure/pymeasure/workflows/Pymeasure%20CI/badge.svg
+            :target: https://github.com/pymeasure/pymeasure/actions
         
         .. image:: http://readthedocs.org/projects/pymeasure/badge/?version=latest
             :target: http://pymeasure.readthedocs.io/en/latest/?badge=latest
             :alt: Documentation Status
         
-        .. image:: https://zenodo.org/badge/23569/ralph-group/pymeasure.svg
-           :target: https://zenodo.org/badge/latestdoi/23569/ralph-group/pymeasure
+        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3732545.svg
+           :target: https://doi.org/10.5281/zenodo.3732545
         
         .. image:: https://anaconda.org/conda-forge/pymeasure/badges/version.svg
            :target: https://anaconda.org/conda-forge/pymeasure
         
         .. image:: https://anaconda.org/conda-forge/pymeasure/badges/downloads.svg
            :target: https://anaconda.org/conda-forge/pymeasure
         
@@ -45,16 +42,42 @@
         
         Check out `the documentation`_ for the `quick start guide`_, that covers the installation of Python and PyMeasure.
         
         There are a number of examples in the `examples`_ directory that can help you get up and running.
         
         .. _the documentation: http://pymeasure.readthedocs.org/en/latest/
         .. _quick start guide: http://pymeasure.readthedocs.io/en/latest/quick_start.html
-        .. _examples: https://github.com/ralph-group/pymeasure/tree/master/examples
+        .. _examples: https://github.com/pymeasure/pymeasure/tree/master/examples
+        
         
+        Version 0.9 -- released 2/7/21
+        ==============================
+        - PyMeasure is now officially at github.com/pymeasure/pymeasure
+        - Python 3.9 is now supported, Python 3.5 removed due to EOL
+        - Move to GitHub Actions from TravisCI and Appveyor for CI (@bilderbuchi)
+        - New additions to Oxford Instruments ITC 503 (@CasperSchippers)
+        - New Agilent 34450A and Keysight DSOX1102G instruments (@theMashUp, @jlarochelle)
+        - Improvements to NI VirtualBench (@moritzj29)
+        - New Agilent B1500 instrument (@moritzj29)
+        - New Keithley 6517B instrument (@wehlgrundspitze)
+        - Major improvements to PyVISA compatbility (@bilderbuchi, @msmttchr, @CasperSchippers, @cjermain)
+        - New Anapico APSIN12G instrument (@StePhanino)
+        - Improvements to Thorelabs Pro 8000 and SR830 (@Mike-HubGit)
+        - New SR860 instrument (@StevenSiegl, @bklebel)
+        - Fix to escape sequences (@tirkarthi)
+        - New directory input for ManagedWindow (@paulgoulain)
+        - New TelnetAdapter and Attocube ANC300 Piezo controller (@dkriegner)
+        - New Agilent 34450A (@theMashUp)
+        - New Razorbill RP100 strain cell controller (@pheowl)
+        - Fixes to precision and default value of ScientificInput and FloatParameter (@moritzj29)
+        - Fixes for Keithly 2400 and 2450 controls (@pyMatJ)
+        - Improvments to Inputs and open_file_externally (@msmttchr)
+        - Fixes to Agilent 8722ES (@alexmcnabb)
+        - Fixes to QThread cleanup (@neal-kepler, @msmttchr)
+        - Fixes to Keyboard interrupt, and parameters (@CasperSchippers)
         
         Version 0.8 -- released 3/29/19
         ===============================
         - Python 3.8 is now supported
         - New Measurement Sequencer allows for running over a large parameter space (@CasperSchippers)
         - New image plotting feature for live image measurements (@jmittelstaedt)
         - Improvements to VISA adapter (@moritzj29)
@@ -234,15 +257,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Provides-Extra: python-vxi11
 Provides-Extra: matplotlib
 Provides-Extra: tcp
+Provides-Extra: python-vxi11
```

### Comparing `PyMeasure-0.8.0/PyMeasure.egg-info/SOURCES.txt` & `PyMeasure-0.9.0/PyMeasure.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,34 @@
 docs/api/instruments/validators.rst
 docs/api/instruments/advantest/advantestR3767CG.rst
 docs/api/instruments/advantest/index.rst
 docs/api/instruments/agilent/agilent33220A.rst
 docs/api/instruments/agilent/agilent33500.rst
 docs/api/instruments/agilent/agilent33521A.rst
 docs/api/instruments/agilent/agilent34410A.rst
+docs/api/instruments/agilent/agilent34450A.rst
 docs/api/instruments/agilent/agilent4156.rst
 docs/api/instruments/agilent/agilent8257D.rst
 docs/api/instruments/agilent/agilent8722ES.rst
+docs/api/instruments/agilent/agilentB1500.rst
 docs/api/instruments/agilent/agilentE4408B.rst
 docs/api/instruments/agilent/agilentE4980.rst
 docs/api/instruments/agilent/index.rst
 docs/api/instruments/ametek/ametek7270.rst
 docs/api/instruments/ametek/index.rst
 docs/api/instruments/ami/ami430.rst
 docs/api/instruments/ami/index.rst
+docs/api/instruments/anapico/apsin12G.rst
+docs/api/instruments/anapico/index.rst
 docs/api/instruments/anritsu/anritsuMG3692C.rst
 docs/api/instruments/anritsu/anritsuMS9710C.rst
 docs/api/instruments/anritsu/index.rst
+docs/api/instruments/attocube/adapters.rst
+docs/api/instruments/attocube/anc300.rst
+docs/api/instruments/attocube/index.rst
 docs/api/instruments/danfysik/adapters.rst
 docs/api/instruments/danfysik/danfysik8500.rst
 docs/api/instruments/danfysik/index.rst
 docs/api/instruments/deltaelektronica/index.rst
 docs/api/instruments/deltaelektronica/sm7045d.rst
 docs/api/instruments/fwbell/fwbell5080.rst
 docs/api/instruments/fwbell/index.rst
@@ -75,37 +82,43 @@
 docs/api/instruments/keithley/index.rst
 docs/api/instruments/keithley/keithley2000.rst
 docs/api/instruments/keithley/keithley2400.rst
 docs/api/instruments/keithley/keithley2450.rst
 docs/api/instruments/keithley/keithley2700.rst
 docs/api/instruments/keithley/keithley2750.rst
 docs/api/instruments/keithley/keithley6221.rst
+docs/api/instruments/keithley/keithley6517b.rst
 docs/api/instruments/keysight/index.rst
+docs/api/instruments/keysight/keysightDSOX1102G.rst
 docs/api/instruments/keysight/keysightN5767A.rst
 docs/api/instruments/lakeshore/adapters.rst
 docs/api/instruments/lakeshore/index.rst
 docs/api/instruments/lakeshore/lakeshore331.rst
 docs/api/instruments/lakeshore/lakeshore425.rst
 docs/api/instruments/newport/esp300.rst
 docs/api/instruments/newport/index.rst
 docs/api/instruments/ni/index.rst
 docs/api/instruments/ni/virtualbench.rst
 docs/api/instruments/oxfordinstruments/ITC503.rst
 docs/api/instruments/oxfordinstruments/index.rst
 docs/api/instruments/parker/index.rst
 docs/api/instruments/parker/parkerGV6.rst
+docs/api/instruments/razorbill/index.rst
+docs/api/instruments/razorbill/razorbillRP100.rst
 docs/api/instruments/signalrecovery/dsp7265.rst
 docs/api/instruments/signalrecovery/index.rst
 docs/api/instruments/srs/index.rst
 docs/api/instruments/srs/sr830.rst
+docs/api/instruments/srs/sr860.rst
 docs/api/instruments/tektronix/afg3152c.rst
 docs/api/instruments/tektronix/index.rst
 docs/api/instruments/tektronix/tds2000.rst
 docs/api/instruments/thorlabs/index.rst
 docs/api/instruments/thorlabs/thorlabspm100usb.rst
+docs/api/instruments/thorlabs/thorlabspro8000.rst
 docs/api/instruments/yokogawa/index.rst
 docs/api/instruments/yokogawa/yokogawa7651.rst
 docs/dev/adding_instruments.rst
 docs/dev/coding_standards.rst
 docs/dev/contribute.rst
 docs/dev/reporting_errors.rst
 docs/images/PyMeasure logo.png
@@ -115,14 +128,15 @@
 docs/images/PyMeasure.png
 docs/images/PyMeasure.svg
 docs/tutorial/connecting.rst
 docs/tutorial/graphical.rst
 docs/tutorial/gui_sequencer_example_sequence.txt
 docs/tutorial/index.rst
 docs/tutorial/procedure.rst
+docs/tutorial/pymeasure-directoryinput.png
 docs/tutorial/pymeasure-managedwindow-queued.png
 docs/tutorial/pymeasure-managedwindow-resume.png
 docs/tutorial/pymeasure-managedwindow-running.png
 docs/tutorial/pymeasure-managedwindow.png
 docs/tutorial/pymeasure-plotter.png
 docs/tutorial/pymeasure-sequencer.png
 pymeasure/__init__.py
@@ -131,14 +145,15 @@
 pymeasure/log.py
 pymeasure/process.py
 pymeasure/thread.py
 pymeasure/adapters/__init__.py
 pymeasure/adapters/adapter.py
 pymeasure/adapters/prologix.py
 pymeasure/adapters/serial.py
+pymeasure/adapters/telnet.py
 pymeasure/adapters/visa.py
 pymeasure/adapters/vxi11.py
 pymeasure/display/Qt.py
 pymeasure/display/__init__.py
 pymeasure/display/browser.py
 pymeasure/display/curves.py
 pymeasure/display/inputs.py
@@ -166,26 +181,33 @@
 pymeasure/instruments/advantest/__init__.py
 pymeasure/instruments/advantest/advantestR3767CG.py
 pymeasure/instruments/agilent/__init__.py
 pymeasure/instruments/agilent/agilent33220A.py
 pymeasure/instruments/agilent/agilent33500.py
 pymeasure/instruments/agilent/agilent33521A.py
 pymeasure/instruments/agilent/agilent34410A.py
+pymeasure/instruments/agilent/agilent34450A.py
 pymeasure/instruments/agilent/agilent4156.py
 pymeasure/instruments/agilent/agilent8257D.py
 pymeasure/instruments/agilent/agilent8722ES.py
+pymeasure/instruments/agilent/agilentB1500.py
 pymeasure/instruments/agilent/agilentE4408B.py
 pymeasure/instruments/agilent/agilentE4980.py
 pymeasure/instruments/ametek/__init__.py
 pymeasure/instruments/ametek/ametek7270.py
 pymeasure/instruments/ami/__init__.py
 pymeasure/instruments/ami/ami430.py
+pymeasure/instruments/anapico/__init__.py
+pymeasure/instruments/anapico/apsin12G.py
 pymeasure/instruments/anritsu/__init__.py
 pymeasure/instruments/anritsu/anritsuMG3692C.py
 pymeasure/instruments/anritsu/anritsuMS9710C.py
+pymeasure/instruments/attocube/__init__.py
+pymeasure/instruments/attocube/adapters.py
+pymeasure/instruments/attocube/anc300.py
 pymeasure/instruments/danfysik/__init__.py
 pymeasure/instruments/danfysik/adapters.py
 pymeasure/instruments/danfysik/danfysik8500.py
 pymeasure/instruments/deltaelektronika/__init__.py
 pymeasure/instruments/deltaelektronika/sm7045d.py
 pymeasure/instruments/fwbell/__init__.py
 pymeasure/instruments/fwbell/fwbell5080.py
@@ -196,15 +218,17 @@
 pymeasure/instruments/keithley/buffer.py
 pymeasure/instruments/keithley/keithley2000.py
 pymeasure/instruments/keithley/keithley2400.py
 pymeasure/instruments/keithley/keithley2450.py
 pymeasure/instruments/keithley/keithley2700.py
 pymeasure/instruments/keithley/keithley2750.py
 pymeasure/instruments/keithley/keithley6221.py
+pymeasure/instruments/keithley/keithley6517b.py
 pymeasure/instruments/keysight/__init__.py
+pymeasure/instruments/keysight/keysightDSOX1102G.py
 pymeasure/instruments/keysight/keysightN5767A.py
 pymeasure/instruments/lakeshore/__init__.py
 pymeasure/instruments/lakeshore/adapters.py
 pymeasure/instruments/lakeshore/lakeshore331.py
 pymeasure/instruments/lakeshore/lakeshore425.py
 pymeasure/instruments/newport/__init__.py
 pymeasure/instruments/newport/esp300.py
@@ -212,24 +236,28 @@
 pymeasure/instruments/ni/daqmx.py
 pymeasure/instruments/ni/nidaq.py
 pymeasure/instruments/ni/virtualbench.py
 pymeasure/instruments/oxfordinstruments/__init__.py
 pymeasure/instruments/oxfordinstruments/itc503.py
 pymeasure/instruments/parker/__init__.py
 pymeasure/instruments/parker/parkerGV6.py
+pymeasure/instruments/razorbill/__init__.py
+pymeasure/instruments/razorbill/razorbillRP100.py
 pymeasure/instruments/signalrecovery/__init__.py
 pymeasure/instruments/signalrecovery/dsp7265.py
 pymeasure/instruments/srs/__init__.py
 pymeasure/instruments/srs/sg380.py
 pymeasure/instruments/srs/sr830.py
+pymeasure/instruments/srs/sr860.py
 pymeasure/instruments/tektronix/__init__.py
 pymeasure/instruments/tektronix/afg3152c.py
 pymeasure/instruments/tektronix/tds2000.py
 pymeasure/instruments/thorlabs/__init__.py
 pymeasure/instruments/thorlabs/thorlabspm100usb.py
+pymeasure/instruments/thorlabs/thorlabspro8000.py
 pymeasure/instruments/yokogawa/__init__.py
 pymeasure/instruments/yokogawa/yokogawa7651.py
 tests/conftest.py
 tests/test_log.py
 tests/test_process.py
 tests/test_thread.py
 tests/adapters/test_adapter.py
@@ -241,10 +269,13 @@
 tests/experiment/test_parameters.py
 tests/experiment/test_procedure.py
 tests/experiment/test_results.py
 tests/experiment/test_workers.py
 tests/experiment/data/__init__.py
 tests/experiment/data/procedure_for_testing.py
 tests/experiment/data/results_for_testing.csv
+tests/experiment/data/results_for_testing_parameters.csv
 tests/instruments/test_instrument.py
 tests/instruments/test_validators.py
-tests/instruments/keithley/test_keithley2750.py
+tests/instruments/agilent/test_agilent34450A.py
+tests/instruments/keithley/test_keithley2750.py
+tests/instruments/keysight/test_keysightDSOX1102G.py
```

### Comparing `PyMeasure-0.8.0/README.rst` & `PyMeasure-0.9.0/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,90 @@
-.. image:: https://raw.githubusercontent.com/ralph-group/pymeasure/master/docs/images/PyMeasure.png
-    :alt: PyMeasure Scientific package
+.. PyMeasure documentation master file, created by
+   sphinx-quickstart on Mon Apr  6 13:06:00 2015.
+   You can adapt this file completely to your liking, but it should at least
+   contain the root `toctree` directive.
 
+############################
 PyMeasure scientific package
 ############################
 
-PyMeasure makes scientific measurements easy to set up and run. The package contains a repository of instrument classes and a system for running experiment procedures, which provides graphical interfaces for graphing live data and managing queues of experiments. Both parts of the package are independent, and when combined provide all the necessary requirements for advanced measurements with only limited coding.
-
-PyMeasure is currently under active development, so please report any issues you experience to our `Issues page`_.
+.. image:: images/PyMeasure.png
+    :alt: PyMeasure Scientific package
 
-.. _Issues page: https://github.com/ralph-group/pymeasure/issues
+PyMeasure makes scientific measurements easy to set up and run. The package contains a repository of instrument classes and a system for running experiment procedures, which provides graphical interfaces for graphing live data and managing queues of experiments. Both parts of the package are independent, and when combined provide all the necessary requirements for advanced measurements with only limited coding.
 
-PyMeasure runs on Python 3.5, 3.6, 3.7 and 3.8, and is tested with continous-integration on Linux, macOS, and Windows.
+Installing Python and PyMeasure are demonstrated in the :doc:`Quick Start guide <quick_start>`. From there, checkout the existing :doc:`instruments that are available for use <api/instruments/index>`.
 
-.. image:: https://ci.appveyor.com/api/projects/status/hcj2n2a7l97wfbb8/branch/master?svg=true
-    :target: https://ci.appveyor.com/project/cjermain/pymeasure
+PyMeasure is currently under active development, so please report any issues you experience on our `Issues page`_.
 
-.. image:: https://travis-ci.org/ralph-group/pymeasure.svg?branch=master
-    :target: https://travis-ci.org/ralph-group/pymeasure
+.. image:: https://github.com/pymeasure/pymeasure/workflows/Pymeasure%20CI/badge.svg
+    :target: https://github.com/pymeasure/pymeasure/actions
 
 .. image:: http://readthedocs.org/projects/pymeasure/badge/?version=latest
     :target: http://pymeasure.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://zenodo.org/badge/23569/ralph-group/pymeasure.svg
-   :target: https://zenodo.org/badge/latestdoi/23569/ralph-group/pymeasure
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3732545.svg
+   :target: https://doi.org/10.5281/zenodo.3732545
 
 .. image:: https://anaconda.org/conda-forge/pymeasure/badges/version.svg
    :target: https://anaconda.org/conda-forge/pymeasure
 
 .. image:: https://anaconda.org/conda-forge/pymeasure/badges/downloads.svg
    :target: https://anaconda.org/conda-forge/pymeasure
 
+.. _Issues page: https://github.com/pymeasure/pymeasure/issues
+
+
+The main documentation for the site is organized into a couple sections:
+
+* :ref:`learning-docs`
+* :ref:`api-docs`
+* :ref:`about-docs`
+
+Information about development is also available:
+
+* :ref:`dev-docs`
+
+
+.. _learning-docs:
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Learning PyMeasure
+
+   introduction
+   quick_start
+   tutorial/index
+
+
+.. _api-docs:
+
+.. toctree::
+   :maxdepth: 1
+   :caption: API References
+
+   api/adapters
+   api/experiment/index
+   api/display/index
+   api/instruments/index
+
+.. _dev-docs:
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Getting involved
+
+   dev/contribute
+   dev/reporting_errors
+   dev/adding_instruments
+   dev/coding_standards
 
-Quick start
-===========
+.. _about-docs:
 
-Check out `the documentation`_ for the `quick start guide`_, that covers the installation of Python and PyMeasure.
+.. toctree::
+   :maxdepth: 2
+   :caption: About PyMeasure
 
-There are a number of examples in the `examples`_ directory that can help you get up and running.
+   about/authors
+   about/license
 
-.. _the documentation: http://pymeasure.readthedocs.org/en/latest/
-.. _quick start guide: http://pymeasure.readthedocs.io/en/latest/quick_start.html
-.. _examples: https://github.com/ralph-group/pymeasure/tree/master/examples
```

### Comparing `PyMeasure-0.8.0/docs/Makefile` & `PyMeasure-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/about/authors.rst` & `PyMeasure-0.9.0/docs/about/authors.rst`

 * *Files 27% similar despite different names*

```diff
@@ -19,7 +19,15 @@
 | Julian Dlugosch
 | Vikram Sekar
 | Casper Schippers
 | Sumatran Tiger
 | Dennis Feng
 | Stefano Pirotta
 | Moritz Jung
+| Manuel Zahn
+| Dominik Kriegner
+| Jonathan Larochelle
+| Dominic Caron
+| Mathieu Plante
+| Michele Sardo
+| Steven Siegl
+| Benjamin Klebel-Knobloch
```

### Comparing `PyMeasure-0.8.0/docs/about/license.rst` & `PyMeasure-0.9.0/pymeasure/instruments/parker/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-License
-=======
+#
+# This file is part of the PyMeasure package.
+#
+# Copyright (c) 2013-2021 PyMeasure Developers
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+# THE SOFTWARE.
+#
 
-Copyright (c) 2013-2020 PyMeasure Developers
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+from .parkerGV6 import ParkerGV6
```

### Comparing `PyMeasure-0.8.0/docs/api/adapters.rst` & `PyMeasure-0.9.0/docs/api/adapters.rst`

 * *Files 6% similar despite different names*

```diff
@@ -59,7 +59,17 @@
 ==============
 
 .. autoclass:: pymeasure.adapters.VXI11Adapter
     :members:
     :undoc-members:
     :inherited-members:
     :show-inheritance: 
+
+==============
+Telnet adapter
+==============
+
+.. autoclass:: pymeasure.adapters.TelnetAdapter
+    :members:
+    :undoc-members:
+    :inherited-members:
+    :show-inheritance:
```

### Comparing `PyMeasure-0.8.0/docs/conf.py` & `PyMeasure-0.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,24 +52,24 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'PyMeasure'
-copyright = u'2013-2020, PyMeasure Developers'
+copyright = u'2013-2021, PyMeasure Developers'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.8.0'
+version = '0.9.0'
 # The full version, including alpha/beta/rc tags.
-release = '0.8.0'
+release = '0.9.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -266,8 +266,8 @@
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
 
 # Automatically mock optional packages
-autodoc_mock_imports = ['pyqtgraph', 'zmq', 'cloudpickle', 'vxi11']
+autodoc_mock_imports = ['pyqtgraph', 'zmq', 'cloudpickle', 'vxi11', 'pyvirtualbench']
```

### Comparing `PyMeasure-0.8.0/docs/dev/adding_instruments.rst` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent33220A.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,329 +1,327 @@
-##################
-Adding instruments
-##################
-
-You can make a significant contribution to PyMeasure by adding a new instrument to the :code:`pymeasure.instruments` package. Even adding an instrument with a few features can help get the ball rolling, since its likely that others are interested in the same instrument.
-
-Before getting started, become familiar with the :doc:`contributing work-flow <contribute>` for PyMeasure, which steps through the process of adding a new feature (like an instrument) to the development version of the source code. This section will describe how to lay out your instrument code.
-
-File structure
-==============
-
-Your new instrument should be placed in the directory corresponding to the manufacturer of the instrument. For example, if you are going to add an "Extreme 5000" instrument you should add the following files assuming "Extreme" is the manufacturer. Use lowercase for all filenames to distinguish packages from CamelCase Python classes.
-
-.. code-block:: none
-
-    pymeasure/pymeasure/instruments/extreme/
-        |--> __init__.py
-        |--> extreme5000.py
-
-Updating the init file
-**********************
-
-The :code:`__init__.py` file in the manufacturer directory should import all of the instruments that correspond to the manufacturer, to allow the files to be easily imported. For a new manufacturer, the manufacturer should also be added to :code:`pymeasure/pymeasure/instruments/__init__.py`. In this case, you also need to add the new package to the :code:`pymeasure/setup.py` file in the :code:`packages` argument.
-
-Adding documentation
-********************
-
-Documentation for each instrument is required, and helps others understand the features you have implemented. Add a new reStructuredText file to the documentation.
-
-.. code-block:: none
-
-    pymeasure/docs/api/instruments/extreme/
-        |--> index.rst
-        |--> extreme5000.rst
-
-Copy an existing instrument documentation file, which will automatically generate the documentation for the instrument. The :code:`index.rst` file should link to the :code:`extreme5000` file. For a new manufacturer, the manufacturer should be also linked in :code:`pymeasure/docs/api/instruments/index.rst`.
-
-Instrument file
-===============
-
-All standard instruments should be child class of :class:`Instrument <pymeasure.instruments.Instrument>`. This provides the basic functionality for working with :class:`Adapters <pymeasure.adapters.Adapter>`, which perform the actual communication. 
-
-The most basic instrument, for our "Extreme 5000" example starts like this:
-
-.. testcode::
-
-    #
-    # This file is part of the PyMeasure package.
-    #
-    # Copyright (c) 2013-2020 PyMeasure Developers
-    #
-    # Permission is hereby granted, free of charge, to any person obtaining a copy
-    # of this software and associated documentation files (the "Software"), to deal
-    # in the Software without restriction, including without limitation the rights
-    # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-    # copies of the Software, and to permit persons to whom the Software is
-    # furnished to do so, subject to the following conditions:
-    #
-    # The above copyright notice and this permission notice shall be included in
-    # all copies or substantial portions of the Software.
-    #
-    # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-    # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-    # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-    # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-    # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-    # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-    # THE SOFTWARE.
-    #
-
-    # from pymeasure.instruments import Instrument
-    
-.. testcode::
-    :hide:
-
-    # Behind the scene, replace Instrument with FakeInstrument to enable
-    # doctesting all this
-    from pymeasure.instruments.instrument import FakeInstrument as Instrument
-
-This is a minimal instrument definition:
-
-.. testcode::
-    
-    class Extreme5000(Instrument):
-        """ Represents the imaginary Extreme 5000 instrument.
-        """
-
-        def __init__(self, resourceName, **kwargs):
-            super(Extreme5000, self).__init__(
-                resourceName,
-                "Extreme 5000",
-                **kwargs
-            )
-
-Make sure to include the PyMeasure license to each file, and add yourself as an author to the :code:`AUTHORS.txt` file.
-
-In principle you are free to write any functions that are necessary for interacting with the instrument. When doing so, make sure to use the :code:`self.ask(command)`, :code:`self.write(command)`, and :code:`self.read()` methods to issue command instead of calling the adapter directly.
-
-In practice, we have developed a number of convenience functions for making instruments easy to write and maintain. The following sections detail these conveniences and are highly encouraged.
-
-Writing properties
-==================
-
-In PyMeasure, `Python properties`_ are the preferred method for dealing with variables that are read or set. 
-PyMeasure comes with two convenience functions for making properties for classes. 
-The :func:`Instrument.measurement <pymeasure.instruments.Instrument.measurement>` function returns a property that issues a GPIB/SCPI requests when the value is used. 
-For example, if our "Extreme 5000" has the :code:`*IDN?` command we can write the following property to be added above the :code:`def __init__` line in our above example class, or added to the class after the fact as in the code here:
-
-.. _Python properties: https://docs.python.org/3/howto/descriptor.html#properties
-
-.. testcode::
-
-     Extreme5000.id = Instrument.measurement(
-        "*IDN?", """ Reads the instrument identification """
-     )
-
-.. testcode::
-    :hide:
-    
-    # We are not mocking this in FakeInstrument, let's override silently
-    Extreme5000.id = 'Extreme 5000 identification from instrument'
-    
-You will notice that a documentation string is required, and should be descriptive and specific.
-
-When we use this property we will get the identification information.
-
-.. doctest::
-
-    >>> extreme = Extreme5000("GPIB::1")
-    >>> extreme.id           # Reads "*IDN?"
-    'Extreme 5000 identification from instrument'
-
-The :func:`Instrument.control <pymeasure.instruments.Instrument.control>` function extends this behavior by creating a property that you can read and set. For example, if our "Extreme 5000" has the :code:`:VOLT?` and :code:`:VOLT <float>` commands that are in Volts, we can write the following property.
-
-.. testcode::
-
-    Extreme5000.voltage = Instrument.control(
-        ":VOLT?", ":VOLT %g",
-        """ A floating point property that controls the voltage
-        in Volts. This property can be set.
-        """
+#
+# This file is part of the PyMeasure package.
+#
+# Copyright (c) 2013-2021 PyMeasure Developers
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+# THE SOFTWARE.
+#
+
+import logging
+log = logging.getLogger(__name__)
+log.addHandler(logging.NullHandler())
+
+from pymeasure.instruments import Instrument
+from pymeasure.instruments.validators import strict_discrete_set,\
+    strict_range, joined_validators
+from time import time
+from pyvisa.errors import VisaIOError
+
+
+# Capitalize string arguments to allow for better conformity with other WFG's
+def capitalize_string(string: str, *args, **kwargs):
+    return string.upper()
+
+
+# Combine the capitalize function and validator
+string_validator = joined_validators(capitalize_string, strict_discrete_set)
+
+
+class Agilent33220A(Instrument):
+    """Represents the Agilent 33220A Arbitrary Waveform Generator.
+
+    .. code-block:: python
+
+        # Default channel for the Agilent 33220A
+        wfg = Agilent33220A("GPIB::10")
+
+        wfg.shape = "SINUSOID"          # Sets a sine waveform
+        wfg.frequency = 4.7e3           # Sets the frequency to 4.7 kHz
+        wfg.amplitude = 1               # Set amplitude of 1 V
+        wfg.offset = 0                  # Set the amplitude to 0 V
+
+        wfg.burst = True                # Enable burst mode
+        wfg.burst_ncycles = 10e3        # A burst will consist of 10 cycles
+        wfg.burst_mode = "TRIGGERED"    # A burst will be applied on a trigger
+        wfg.trigger_source = "BUS"      # A burst will be triggered on TRG*
+
+        wfg.output = True               # Enable output of waveform generator
+        wfg.trigger()                   # Trigger a burst
+        wfg.wait_for_trigger()          # Wait until the triggering is finished
+        wfg.beep()                      # "beep"
+
+        wfg.check_errors()              # Get the error queue
+
+    """
+
+    def __init__(self, adapter, **kwargs):
+        super(Agilent33220A, self).__init__(
+            adapter,
+            "Agilent 33220A Arbitrary Waveform generator",
+            **kwargs
+        )
+
+    shape = Instrument.control(
+        "FUNC?", "FUNC %s",
+        """ A string property that controls the output waveform. Can be set to:
+        SIN<USOID>, SQU<ARE>, RAMP, PULS<E>, NOIS<E>, DC, USER. """,
+        validator=string_validator,
+        values=["SINUSOID", "SIN", "SQUARE", "SQU", "RAMP",
+                "PULSE", "PULS", "NOISE", "NOIS", "DC", "USER"],
     )
 
-You will notice that we use the `Python string format`_ :code:`%g` to pass through the floating point.
-
-.. _Python string format: https://docs.python.org/3/library/string.html#format-specification-mini-language
-
-We can use this property to set the voltage to 100 mV, which will execute the command and then request the current voltage.
-
-.. doctest::
-
-    >>> extreme = Extreme5000("GPIB::1")
-    >>> extreme.voltage = 0.1        # Executes ":VOLT 0.1"
-    >>> extreme.voltage              # Reads ":VOLT?"
-    0.1
-
-Using both of these functions, you can create a number of properties for basic measurements and controls. The next section details additional features of :func:`Instrument.control <pymeasure.instruments.Instrument.control>` that allow you to write properties that cover specific ranges, or have to map between a real value to one used in the command.
-
-.. _advanced-properties:
-
-Advanced properties
-===================
-
-Many GPIB/SCIP commands are more restrictive than our basic examples above. The :func:`Instrument.control <pymeasure.instruments.Instrument.control>` function has the ability to encode these restrictions using :mod:`validators <pymeasure.instruments.validators>`. A validator is a function that takes a value and a set of values, and returns a valid value or raises an exception. There are a number of pre-defined validators in :mod:`pymeasure.instruments.validators` that should cover most situations. We will cover the four basic types here.
-
-In the examples below we assume you have imported the validators.
-
-.. testcode::
-    :hide:
-
-    from pymeasure.instruments.validators import strict_discrete_set, strict_range, truncated_range, truncated_discrete_set
-
-In a restricted range
-*********************
-
-If you have a property with a restricted range, you can use the :func:`strict_range <pymeasure.instruments.validators.strict_range>` and :func:`truncated_range <pymeasure.instruments.validators.strict_range>` functions.
-
-For example, if our "Extreme 5000" can only support voltages from -1 V to 1 V, we can modify our previous example to use a strict validator over this range.
-
-.. testcode::
-  
-    Extreme5000.voltage = Instrument.control(
-        ":VOLT?", ":VOLT %g",
-        """ A floating point property that controls the voltage
-        in Volts, from -1 to 1 V. This property can be set. """,
+    frequency = Instrument.control(
+        "FREQ?", "FREQ %s",
+        """ A floating point property that controls the frequency of the output
+        waveform in Hz, from 1e-6 (1 uHz) to 20e+6 (20 MHz), depending on the
+        specified function. Can be set. """,
         validator=strict_range,
-        values=[-1, 1]
+        values=[1e-6, 5e+6],
     )
 
-Now our voltage will raise a ValueError if the value is out of the range.
-
-.. doctest::
-
-    >>> extreme = Extreme5000("GPIB::1")
-    >>> extreme.voltage = 100
-    Traceback (most recent call last):
-    ...
-    ValueError: Value of 100 is not in range [-1,1]
-
-This is useful if you want to alert the programmer that they are using an invalid value. However, sometimes it can be nicer to truncate the value to be within the range.
-
-.. testcode::
-
-    Extreme5000.voltage = Instrument.control(
-        ":VOLT?", ":VOLT %g",
-        """ A floating point property that controls the voltage
-        in Volts, from -1 to 1 V. Invalid voltages are truncated.
-        This property can be set. """,
-        validator=truncated_range,
-        values=[-1, 1]
+    amplitude = Instrument.control(
+        "VOLT?", "VOLT %f",
+        """ A floating point property that controls the voltage amplitude of the
+        output waveform in V, from 10e-3 V to 10 V. Can be set. """,
+        validator=strict_range,
+        values=[10e-3, 10],
     )
 
-Now our voltage will not raise an error, and will truncate the value to the range bounds.
-
-.. doctest::
-
-    >>> extreme = Extreme5000("GPIB::1")
-    >>> extreme.voltage = 100        # Executes ":VOLT 1"  
-    >>> extreme.voltage
-    1.0
-
-In a discrete set
-*****************
-
-Often a control property should only take a few discrete values. You can use the :func:`strict_discrete_set <pymeasure.instruments.validators.strict_discrete_set>` and :func:`truncated_discrete_set <pymeasure.instruments.validators.truncated_discrete_set>` functions to handle these situations. The strict version raises an error if the value is not in the set, as in the range examples above.
-
-For example, if our "Extreme 5000" has a :code:`:RANG <float>` command that sets the voltage range that can take values of 10 mV, 100 mV, and 1 V in Volts, then we can write a control as follows.
-
-.. testcode::
+    amplitude_unit = Instrument.control(
+        "VOLT:UNIT?", "VOLT:UNIT %s",
+        """ A string property that controls the units of the amplitude. Valid
+        values are Vpp (default), Vrms, and dBm. Can be set. """,
+        validator=string_validator,
+        values=["VPP", "VRMS", "DBM"],
+    )
 
-    Extreme5000.voltage = Instrument.control(
-        ":RANG?", ":RANG %g",
-        """ A floating point property that controls the voltage
-        range in Volts. This property can be set.
+    offset = Instrument.control(
+        "VOLT:OFFS?", "VOLT:OFFS %f",
+        """ A floating point property that controls the voltage offset of the
+        output waveform in V, from 0 V to 4.995 V, depending on the set
+        voltage amplitude (maximum offset = (10 - voltage) / 2). Can be set.
         """,
-        validator=truncated_discrete_set,
-        values=[10e-3, 100e-3, 1]
+        validator=strict_range,
+        values=[-4.995, +4.995],
     )
 
-Now we can set the voltage range, which will automatically truncate to an appropriate value.
-
-.. doctest::
-
-    >>> extreme = Extreme5000("GPIB::1")
-    >>> extreme.voltage = 0.08
-    >>> extreme.voltage
-    0.1
+    voltage_high = Instrument.control(
+        "VOLT:HIGH?", "VOLT:HIGH %f",
+        """ A floating point property that controls the upper voltage of the
+        output waveform in V, from -4.990 V to 5 V (must be higher than low
+        voltage). Can be set. """,
+        validator=strict_range,
+        values=[-4.99, 5],
+    )
 
+    voltage_low = Instrument.control(
+        "VOLT:LOW?", "VOLT:LOW %f",
+        """ A floating point property that controls the lower voltage of the
+        output waveform in V, from -5 V to 4.990 V (must be lower than high
+        voltage). Can be set. """,
+        validator=strict_range,
+        values=[-5, 4.99],
+    )
 
-Using maps
-**********
+    square_dutycycle = Instrument.control(
+        "FUNC:SQU:DCYC?", "FUNC:SQU:DCYC %f",
+        """ A floating point property that controls the duty cycle of a square
+        waveform function in percent. Can be set. """,
+        validator=strict_range,
+        values=[20, 80],
+    )
 
-Now that you are familiar with the validators, you can additionally use maps to satisfy instruments which require non-physical values. The :code:`map_values` argument of :func:`Instrument.control <pymeasure.instruments.Instrument.control>` enables this feature.
+    ramp_symmetry = Instrument.control(
+        "FUNC:RAMP:SYMM?", "FUNC:RAMP:SYMM %f",
+        """ A floating point property that controls the symmetry percentage
+        for the ramp waveform. Can be set. """,
+        validator=strict_range,
+        values=[0, 100],
+    )
 
-If your set of values is a list, then the command will use the index of the list. For example, if our "Extreme 5000" instead has a :code:`:RANG <integer>`, where 0, 1, and 2 correspond to 10 mV, 100 mV, and 1 V, then we can use the following control.
+    pulse_period = Instrument.control(
+        "PULS:PER?", "PULS:PER %f",
+        """ A floating point property that controls the period of a pulse
+        waveform function in seconds, ranging from 200 ns to 2000 s. Can be set
+        and overwrites the frequency for *all* waveforms. If the period is
+        shorter than the pulse width + the edge time, the edge time and pulse
+        width will be adjusted accordingly. """,
+        validator=strict_range,
+        values=[200e-9, 2e3],
+    )
 
-.. testcode::
+    pulse_hold = Instrument.control(
+        "FUNC:PULS:HOLD?", "FUNC:PULS:HOLD %s",
+        """ A string property that controls if either the pulse width or the
+        duty cycle is retained when changing the period or frequency of the
+        waveform. Can be set to: WIDT<H> or DCYC<LE>. """,
+        validator=string_validator,
+        values=["WIDT", "WIDTH", "DCYC", "DCYCLE"],
+    )
 
-    Extreme5000.voltage = Instrument.control(
-        ":RANG?", ":RANG %d",
-        """ A floating point property that controls the voltage
-        range in Volts, which takes values of 10 mV, 100 mV and 1 V.
-        This property can be set. """,
-        validator=truncated_discrete_set,
-        values=[10e-3, 100e-3, 1],
-        map_values=True
+    pulse_width = Instrument.control(
+        "FUNC:PULS:WIDT?", "FUNC:PULS:WIDT %f",
+        """ A floating point property that controls the width of a pulse
+        waveform function in seconds, ranging from 20 ns to 2000 s, within a
+        set of restrictions depending on the period. Can be set. """,
+        validator=strict_range,
+        values=[20e-9, 2e3],
     )
 
-Now the actual GPIB/SCIP command is ":RANG 1" for a value of 100 mV, since the index of 100 mV in the values list is 1.
+    pulse_dutycycle = Instrument.control(
+        "FUNC:PULS:DCYC?", "FUNC:PULS:DCYC %f",
+        """ A floating point property that controls the duty cycle of a pulse
+        waveform function in percent. Can be set. """,
+        validator=strict_range,
+        values=[0, 100],
+    )
 
-.. doctest::
+    pulse_transition = Instrument.control(
+        "FUNC:PULS:TRAN?", "FUNC:PULS:TRAN %f",
+        """ A floating point property that controls the the edge time in
+        seconds for both the rising and falling edges. It is defined as the
+        time between 0.1 and 0.9 of the threshold. Valid values are between
+        5 ns to 100 ns. Can be set. """,
+        validator=strict_range,
+        values=[5e-9, 100e-9],
+    )
 
-    >>> extreme = Extreme5000("GPIB::1")
-    >>> extreme.voltage = 100e-3
-    >>> extreme.read()
-    '1'
-    >>> extreme.voltage = 1
-    >>> extreme.voltage
-    1
+    output = Instrument.control(
+        "OUTP?", "OUTP %d",
+        """ A boolean property that turns on (True) or off (False) the output
+        of the function generator. Can be set. """,
+        validator=strict_discrete_set,
+        map_values=True,
+        values={True: 1, False: 0},
+    )
 
-Dictionaries provide a more flexible method for mapping between real-values and those required by the instrument. If instead the :code:`:RANG <integer>` took 1, 2, and 3 to correspond to 10 mV, 100 mV, and 1 V, then we can replace our previous control with the following.
+    burst_state = Instrument.control(
+        "BURS:STAT?", "BURS:STAT %d",
+        """ A boolean property that controls whether the burst mode is on
+        (True) or off (False). Can be set. """,
+        validator=strict_discrete_set,
+        map_values=True,
+        values={True: 1, False: 0},
+    )
 
-.. testcode::
+    burst_mode = Instrument.control(
+        "BURS:MODE?", "BURS:MODE %s",
+        """ A string property that controls the burst mode. Valid values
+        are: TRIG<GERED>, GAT<ED>. This setting can be set. """,
+        validator=string_validator,
+        values=["TRIG", "TRIGGERED", "GAT", "GATED"],
+    )
 
-    Extreme5000.voltage = Instrument.control(
-        ":RANG?", ":RANG %d",
-        """ A floating point property that controls the voltage
-        range in Volts, which takes values of 10 mV, 100 mV and 1 V.
-        This property can be set. """,
-        validator=truncated_discrete_set,
-        values={10e-3:1, 100e-3:2, 1:3},
-        map_values=True
+    burst_ncycles = Instrument.control(
+        "BURS:NCYC?", "BURS:NCYC %d",
+        """ An integer property that sets the number of cycles to be output
+        when a burst is triggered. Valid values are 1 to 50000. This can be
+        set. """,
+        validator=strict_discrete_set,
+        values=range(1, 50001),
     )
 
-.. doctest::
+    def trigger(self):
+        """ Send a trigger signal to the function generator. """
+        self.write("*TRG;*WAI")
+
+    def wait_for_trigger(self, timeout=3600, should_stop=lambda: False):
+        """ Wait until the triggering has finished or timeout is reached.
+
+        :param timeout: The maximum time the waiting is allowed to take. If
+                        timeout is exceeded, a TimeoutError is raised. If
+                        timeout is set to zero, no timeout will be used.
+        :param should_stop: Optional function (returning a bool) to allow the
+                            waiting to be stopped before its end.
 
-    >>> extreme = Extreme5000("GPIB::1")
-    >>> extreme.voltage = 10e-3
-    >>> extreme.read()
-    '1'
-    >>> extreme.voltage = 100e-3
-    >>> extreme.voltage
-    0.1
+        """
+        self.write("*OPC?")
 
-The dictionary now maps the keys to specific values. The values and keys can be any type, so this can support properties that use strings:
+        t0 = time()
+        while True:
+            try:
+                ready = bool(self.read())
+            except VisaIOError:
+                ready = False
+
+            if ready:
+                return
+
+            if timeout != 0 and time() - t0 > timeout:
+                raise TimeoutError(
+                    "Timeout expired while waiting for the Agilent 33220A" +
+                    " to finish the triggering."
+                )
+
+            if should_stop:
+                return
+
+    trigger_source = Instrument.control(
+        "TRIG:SOUR?", "TRIG:SOUR %s",
+        """ A string property that controls the trigger source. Valid values
+        are: IMM<EDIATE> (internal), EXT<ERNAL> (rear input), BUS (via trigger
+        command). This setting can be set. """,
+        validator=string_validator,
+        values=["IMM", "IMMEDIATE", "EXT", "EXTERNAL", "BUS"],
+    )
 
-.. testcode::
-  
-    Extreme5000.channel = Instrument.control(
-        ":CHAN?", ":CHAN %d",
-        """ A string property that controls the measurement channel,
-        which can take the values X, Y, or Z.
-        """,
+    trigger_state = Instrument.control(
+        "OUTP:TRIG?", "OUTP:TRIG %d",
+        """ A boolean property that controls whether the output is triggered
+        (True) or not (False). Can be set. """,
         validator=strict_discrete_set,
-        values={'X':1, 'Y':2, 'Z':3},
-        map_values=True
+        map_values=True,
+        values={True: 1, False: 0},
+    )
+
+    remote_local_state = Instrument.setting(
+        "SYST:COMM:RLST %s",
+        """ A string property that controls the remote/local state of the
+        function generator. Valid values are: LOC<AL>, REM<OTE>, RWL<OCK>.
+        This setting can only be set. """,
+        validator=string_validator,
+        values=["LOC", "LOCAL", "REM", "REMOTE", "RWL", "RWLOCK"],
     )
 
-.. doctest::
+    def check_errors(self):
+        """ Read all errors from the instrument. """
 
-    >>> extreme = Extreme5000("GPIB::1")
-    >>> extreme.channel = 'X'
-    >>> extreme.read()
-    '1'
-    >>> extreme.channel = 'Y'
-    >>> extreme.channel
-    'Y'
+        errors = []
+        while True:
+            err = self.values("SYST:ERR?")
+            if int(err[0]) != 0:
+                errmsg = "Agilent 33220A: %s: %s" % (err[0], err[1])
+                log.error(errmsg + '\n')
+                errors.append(errmsg)
+            else:
+                break
+
+        return errors
+
+    beeper_state = Instrument.control(
+        "SYST:BEEP:STAT?", "SYST:BEEP:STAT %d",
+        """ A boolean property that controls the state of the beeper. Can
+        be set. """,
+        validator=strict_discrete_set,
+        map_values=True,
+        values={True: 1, False: 0},
+    )
 
-As you have seen, the :func:`Instrument.control <pymeasure.instruments.Instrument.control>` function can be significantly extended by using validators and maps.
+    def beep(self):
+        """ Causes a system beep. """
+        self.write("SYST:BEEP")
```

### Comparing `PyMeasure-0.8.0/docs/dev/coding_standards.rst` & `PyMeasure-0.9.0/docs/dev/coding_standards.rst`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 ################
 
 In order to maintain consistency across the different instruments in the PyMeasure repository, we enforce the following standards.
 
 Python style guides
 ===================
 
-Only Python 3 is used in PyMeasure. This prevents the maintaininace overhead of supporting Python 2.7,  which will lose official support in the future.
-
 The `PEP8 style guide`_ and `PEP257 docstring conventions`_ should be followed.
 
 .. _PEP8 style guide: https://www.python.org/dev/peps/pep-0008/
 .. _PEP257 docstring conventions: https://www.python.org/dev/peps/pep-0257/
 
 Function and variable names should be lower case with underscores as needed to seperate words. CamelCase should only be used for class names, unless working with Qt, where its use is common.
 
+There are no plans to support type hinting in PyMeasure code. This adds a lot of additional code to manage, without a clear advantage for this project. 
+Type documentation should be placed in the docstring where not clear from the variable name.
+
 Documentation
 =============
 
 PyMeasure documents code using reStructuredText and the `Sphinx documentation generator`_. All functions, classes, and methods should be documented in the code using a `docstring`_.
 
 .. _Sphinx documentation generator: http://www.sphinx-doc.org/en/stable/
 .. _docstring: http://www.sphinx-doc.org/en/stable/ext/example_numpy.html?highlight=docstring
```

### Comparing `PyMeasure-0.8.0/docs/dev/contribute.rst` & `PyMeasure-0.9.0/docs/dev/contribute.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,20 @@
     git add file-that-changed.py
     git commit -m "A short description about what changed"
     git push
 
 Making a pull-request
 =====================
 
-While you are working, its helpful to start a pull-request (PR) on the :code:`master` branch of :code:`ralph-group/pymeasure`. This will allow you to discuss your feature with other contributors. We encourage you to start this pull-request after your first commit.
+While you are working, its helpful to start a pull-request (PR) on the :code:`master` branch of :code:`pymeasure/pymeasure`. This will allow you to discuss your feature with other contributors. We encourage you to start this pull-request after your first commit.
 
 `Start a pull-request`_ on the `PyMeasure GitHub page`_.
 
 .. _`Start a pull-request`: https://help.github.com/articles/using-pull-requests/
-.. _PyMeasure GitHub page: https://github.com/ralph-group/pymeasure
+.. _PyMeasure GitHub page: https://github.com/pymeasure/pymeasure
 
 Your pull-request will be merged by the PyMeasure maintainers once it meets the coding standards and passes unit tests. You will notice that your pull-request is automatically checked with the unit tests.
 
 Unit testing
 ============
 
 Unit tests are run each time a new commit is made to a branch. The purpose is to catch changes that break the current functionality, by testing each feature unit. PyMeasure relies on `pytest`_ to preform these tests, which are run on TravisCI and Appveyor for Linux/macOS and Windows respectively.
```

### Comparing `PyMeasure-0.8.0/docs/images/PyMeasure logo.png` & `PyMeasure-0.9.0/docs/images/PyMeasure logo.png`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/images/PyMeasure logo.svg` & `PyMeasure-0.9.0/docs/images/PyMeasure logo.svg`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/images/PyMeasure preview.png` & `PyMeasure-0.9.0/docs/images/PyMeasure preview.png`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/images/PyMeasure preview.svg` & `PyMeasure-0.9.0/docs/images/PyMeasure preview.svg`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/images/PyMeasure.png` & `PyMeasure-0.9.0/docs/images/PyMeasure.png`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/images/PyMeasure.svg` & `PyMeasure-0.9.0/docs/images/PyMeasure.svg`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/introduction.rst` & `PyMeasure-0.9.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/make.bat` & `PyMeasure-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/quick_start.rst` & `PyMeasure-0.9.0/docs/quick_start.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This section provides instructions for getting up and running quickly with PyMeasure.
 
 Setting up Python
 =================
 
 The easiest way to install the necessary Python environment for PyMeasure is through the `Anaconda distribution`_, which includes 720 scientific packages. The advantage of using this approach over just relying on the :code:`pip` installer is that it Anaconda correctly installs the required Qt libraries. 
 
-Download and install the appropriate Python 3.5 version of `Anaconda`_ for your operating system. 
+Download and install the appropriate Python version of `Anaconda`_ for your operating system.
 
 .. _Anaconda distribution: https://www.continuum.io/why-anaconda
 .. _Anaconda: https://www.continuum.io/downloads
 
 Installing PyMeasure
 ====================
```

### Comparing `PyMeasure-0.8.0/docs/tutorial/connecting.rst` & `PyMeasure-0.9.0/docs/tutorial/connecting.rst`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/tutorial/graphical.rst` & `PyMeasure-0.9.0/docs/tutorial/graphical.rst`

 * *Files 4% similar despite different names*

```diff
@@ -295,10 +295,48 @@
 In the sequence file each line adds one item to the sequence tree, starting with a number of dashes (:code:`-`) to indicate the level of the item (starting with 1 dash for top level), followed by the name of the parameter and the sequence string, both as a python string between parentheses.
 An example of such a sequence file is given below, resulting in the sequence shown in the figure above.
 
 .. literalinclude:: gui_sequencer_example_sequence.txt
 
 This file can also be automatically loaded at the start of the program by adding the key-word argument :code:`sequence_file="filename.txt"` to the :code:`super(MainWindow, self).__init__` call, as was done in the example.
 
+Using the directory input
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+It is possible to add a directory input in order to choose where the experiment's result will be saved. This option is activated by passing a boolean key-word argument :code:`directory_input` during the :class:`~pymeasure.display.windows.ManagedWindow` init. The value of the directory can be retrieved using the property :code:`directory`.
+
+Only the MainWindow needs to be modified in order to use this option (modified lines are marked).
+
+.. code-block:: python
+   :emphasize-lines: 10,15,16
+
+    class MainWindow(ManagedWindow):
+
+        def __init__(self):
+            super(MainWindow, self).__init__(
+                procedure_class=TestProcedure,
+                inputs=['iterations', 'delay', 'seed'],
+                displays=['iterations', 'delay', 'seed'],
+                x_axis='Iteration',
+                y_axis='Random Number',
+                directory_input=True,                                # Added line
+            )
+            self.setWindowTitle('GUI Example')
+
+        def queue(self):
+            directory = self.directory
+            filename = unique_filename(directory)                    # Modified line
+
+            results = Results(procedure, filename)
+            experiment = self.new_experiment(results)
+
+            self.manager.queue(experiment)
+
+This adds the input line above the Queue and Abort buttons.
+
+.. image:: pymeasure-directoryinput.png
+    :alt: Example of the directory input widget
+
+A completer is implemented allowing to quickly select an existing folder, and a button on the right side of the input widget opens a browse dialog.
 
 .. _pyqtgraph: http://www.pyqtgraph.org/
 .. _PlotItem: http://www.pyqtgraph.org/documentation/graphicsItems/plotitem.html
```

### Comparing `PyMeasure-0.8.0/docs/tutorial/procedure.rst` & `PyMeasure-0.9.0/docs/tutorial/procedure.rst`

 * *Files 1% similar despite different names*

```diff
@@ -260,16 +260,16 @@
     from pymeasure.experiment import IntegerParameter, FloatParameter
     from time import sleep
 
     class IVProcedure(Procedure):
 
         data_points = IntegerParameter('Data points', default=50)
         averages = IntegerParameter('Averages', default=50)
-        max_current = FloatParameter('Maximum Current', unit='A', default=0.01)
-        min_current = FloatParameter('Minimum Current', unit='A', default=-0.01)
+        max_current = FloatParameter('Maximum Current', units='A', default=0.01)
+        min_current = FloatParameter('Minimum Current', units='A', default=-0.01)
 
         DATA_COLUMNS = ['Current (A)', 'Voltage (V)', 'Voltage Std (V)']
 
         def startup(self):
             log.info("Connecting and configuring the instrument")
             self.sourcemeter = Keithley2400("GPIB::4")
             self.sourcemeter.reset()
```

### Comparing `PyMeasure-0.8.0/docs/tutorial/pymeasure-managedwindow-queued.png` & `PyMeasure-0.9.0/docs/tutorial/pymeasure-managedwindow-queued.png`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/tutorial/pymeasure-managedwindow-resume.png` & `PyMeasure-0.9.0/docs/tutorial/pymeasure-managedwindow-resume.png`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/tutorial/pymeasure-managedwindow-running.png` & `PyMeasure-0.9.0/docs/tutorial/pymeasure-managedwindow-running.png`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/tutorial/pymeasure-managedwindow.png` & `PyMeasure-0.9.0/docs/tutorial/pymeasure-managedwindow.png`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/tutorial/pymeasure-plotter.png` & `PyMeasure-0.9.0/docs/tutorial/pymeasure-plotter.png`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/docs/tutorial/pymeasure-sequencer.png` & `PyMeasure-0.9.0/docs/tutorial/pymeasure-sequencer.png`

 * *Files identical despite different names*

### Comparing `PyMeasure-0.8.0/pymeasure/__init__.py` & `PyMeasure-0.9.0/pymeasure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,8 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
```

### Comparing `PyMeasure-0.8.0/pymeasure/adapters/__init__.py` & `PyMeasure-0.9.0/pymeasure/adapters/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -39,7 +39,9 @@
 except ImportError:
     log.warning("PySerial library could not be loaded")
 
 try:
     from pymeasure.adapters.vxi11 import VXI11Adapter
 except ImportError:
     log.warning("VXI-11 library could not be loaded")
+
+from pymeasure.adapters.telnet import TelnetAdapter
```

### Comparing `PyMeasure-0.8.0/pymeasure/adapters/adapter.py` & `PyMeasure-0.9.0/pymeasure/instruments/attocube/adapters.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,115 +18,112 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-import numpy as np
-from copy import copy
+import re
+import time
 
+from pymeasure.adapters import TelnetAdapter
 
-class Adapter(object):
-    """ Base class for Adapter child classes, which adapt between the Instrument 
-    object and the connection, to allow flexible use of different connection 
-    techniques.
 
-    This class should only be inhereted from.
-    """
-
-    def write(self, command):
-        """ Writes a command to the instrument
+class AttocubeConsoleAdapter(TelnetAdapter):
+    """ Adapter class for connecting to the Attocube Standard Console. This
+    console is a Telnet prompt with password authentication.
 
-        :param command: SCPI command string to be sent to the instrument
-        """
-        raise NameError("Adapter (sub)class has not implemented writing")
-
-    def ask(self, command):
-        """ Writes the command to the instrument and returns the resulting 
-        ASCII response
+    :param host: host address of the instrument
+    :param port: TCPIP port
+    :param passwd: password required to open the connection
+    :param kwargs: Any valid key-word argument for TelnetAdapter
+    """
+    # compiled regular expression for finding numerical values in reply strings
+    _reg_value = re.compile(r"\w+\s+=\s+(\w+)")
 
-        :param command: SCPI command string to be sent to the instrument
-        :returns: String ASCII response of the instrument
-        """
-        self.write(command)
-        return self.read()
+    def __init__(self, host, port, passwd, **kwargs):
+        self.read_termination = '\r\n'
+        self.write_termination = self.read_termination
+        kwargs.setdefault('preprocess_reply', self.extract_value)
+        super().__init__(host, port, **kwargs)
+        time.sleep(self.query_delay)
+        super().read()  # clear messages sent upon opening the connection
+        # send password and check authorization
+        self.write(passwd, check_ack=False)
+        time.sleep(self.query_delay)
+        ret = super().read()
+        authmsg = ret.split(self.read_termination)[1]
+        if authmsg != 'Authorization success':
+            raise Exception(f"Attocube authorization failed '{authmsg}'")
+        # switch console echo off
+        _ = self.ask('echo off')
+
+    def extract_value(self, reply):
+        """ preprocess_reply function for the Attocube console. This function
+        tries to extract <value> from 'name = <value> [unit]'. If <value> can
+        not be identified the original string is returned.
+
+        :param reply: reply string
+        :returns: string with only the numerical value, or the original string
+        """
+        r = self._reg_value.search(reply)
+        if r:
+            return r.groups()[0]
+        else:
+            return reply
+
+    def check_acknowledgement(self, reply, msg=""):
+        """ checks the last reply of the instrument to be 'OK', otherwise a
+        ValueError is raised.
+
+        :param reply: last reply string of the instrument
+        :param msg: optional message for the eventual error
+        """
+        if reply != 'OK':
+            if msg == "":  # clear buffer
+                msg = reply
+                super().read()
+            raise ValueError("AttocubeConsoleAdapter: Error after command "
+                             f"{self.lastcommand} with message {msg}")
 
     def read(self):
-        """ Reads until the buffer is empty and returns the resulting
-        ASCII respone
+        """ Reads a reply of the instrument which consists of two or more
+        lines. The first ones are the reply to the command while the last one
+        is 'OK' or 'ERROR' to indicate any problem. In case the reply is not OK
+        a ValueError is raised.
 
         :returns: String ASCII response of the instrument.
         """
-        raise NameError("Adapter (sub)class has not implemented reading")
-
-    def values(self, command, separator=',', cast=float):
-        """ Writes a command to the instrument and returns a list of formatted
-        values from the result 
-
-        :param command: SCPI command to be sent to the instrument
-        :param separator: A separator character to split the string into a list
-        :param cast: A type to cast the result
-        :returns: A list of the desired type, or strings where the casting fails
-        """
-        results = str(self.ask(command)).strip()
-        results = results.split(separator)
-        for i, result in enumerate(results):
-            try:
-                if cast == bool:
-                    # Need to cast to float first since results are usually
-                    # strings and bool of a non-empty string is always True
-                    results[i] = bool(float(result))
-                else:
-                    results[i] = cast(result)
-            except Exception:
-                pass  # Keep as string
-        return results
-
-    def binary_values(self, command, header_bytes=0, dtype=np.float32):
-        """ Returns a numpy array from a query for binary data 
-
-        :param command: SCPI command to be sent to the instrument
-        :param header_bytes: Integer number of bytes to ignore in header
-        :param dtype: The NumPy data type to format the values with
-        :returns: NumPy array of values
-        """
-        raise NameError("Adapter (sub)class has not implemented the "
-                        "binary_values method")
-
+        raw = super().read().strip(self.read_termination)
+        # one would want to use self.read_termination as 'sep' below, but this
+        # is not possible because of a firmware bug resulting in inconsistent
+        # line endings
+        ret, ack = raw.rsplit(sep='\n', maxsplit=1)
+        ret = ret.strip('\r')  # strip possible CR char
+        self.check_acknowledgement(ack, ret)
+        return ret
 
-class FakeAdapter(Adapter):
-    """Provides a fake adapter for debugging purposes,
-    which bounces back the command so that arbitrary values 
-    testing is possible.
-
-    .. code-block:: python
-
-        a = FakeAdapter()
-        assert a.read() == ""
-        a.write("5")
-        assert a.read() == "5"
-        assert a.read() == ""
-        assert a.ask("10") == "10"
-        assert a.values("10") == [10]
+    def write(self, command, check_ack=True):
+        """ Writes a command to the instrument
 
-    """
+        :param command: command string to be sent to the instrument
+        :param check_ack: boolean flag to decide if the acknowledgement is read
+            back from the instrument. This should be True for set pure commands
+            and False otherwise.
+        """
+        self.lastcommand = command
+        super().write(command + self.write_termination)
+        if check_ack:
+            reply = self.connection.read_until(self.read_termination.encode())
+            msg = reply.decode().strip(self.read_termination)
+            self.check_acknowledgement(msg)
 
-    _buffer = ""
+    def ask(self, command):
+        """ Writes a command to the instrument and returns the resulting ASCII
+        response
 
-    def read(self):
-        """ Returns the last commands given after the
-        last read call.
-        """
-        result = copy(self._buffer)
-        # Reset the buffer
-        self._buffer = ""
-        return result
-
-    def write(self, command):
-        """ Writes the command to a buffer, so that it can
-        be read back.
+        :param command: command string to be sent to the instrument
+        :returns: String ASCII response of the instrument
         """
-        self._buffer += command
-
-    def __repr__(self):
-        return "<FakeAdapter>"
+        self.write(command, check_ack=False)
+        time.sleep(self.query_delay)
+        return self.read()
```

### Comparing `PyMeasure-0.8.0/pymeasure/adapters/prologix.py` & `PyMeasure-0.9.0/pymeasure/adapters/prologix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -37,14 +37,16 @@
     connection and the GPIB address to be communicated to.
     Serial connection sharing is achieved by using the :meth:`.gpib`
     method to spawn new PrologixAdapters for different GPIB addresses.
 
     :param port: The Serial port name or a serial.Serial object
     :param address: Integer GPIB address of the desired instrument
     :param rw_delay: An optional delay to set between a write and read call for slow to respond instruments.
+    :param preprocess_reply: optional callable used to preprocess strings
+        received from the instrument. The callable returns the processed string.
     :param kwargs: Key-word arguments if constructing a new serial object
 
     :ivar address: Integer GPIB address of the desired instrument
 
     To allow user access to the Prologix adapter in Linux, create the file:
     :code:`/etc/udev/rules.d/51-prologix.rules`, with contents:
 
@@ -57,16 +59,18 @@
     .. code-block:: bash
 
         sudo udevadm control --reload-rules
         sudo udevadm trigger
 
     """
 
-    def __init__(self, port, address=None, rw_delay=None, serial_timeout = 0.5, **kwargs):
-        super().__init__(port, timeout = serial_timeout, **kwargs)
+    def __init__(self, port, address=None, rw_delay=None, serial_timeout=0.5,
+                 preprocess_reply=None, **kwargs):
+        super().__init__(port, timeout=serial_timeout,
+                         preprocess_reply=preprocess_reply, **kwargs)
         self.address = address
         self.rw_delay = rw_delay
         if not isinstance(port, serial.Serial):
             self.set_defaults()
 
     def set_defaults(self):
         """ Sets up the default behavior of the Prologix-GPIB
```

### Comparing `PyMeasure-0.8.0/pymeasure/adapters/serial.py` & `PyMeasure-0.9.0/pymeasure/adapters/telnet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,67 +18,68 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-import logging
-
-import serial
-import numpy as np
+import telnetlib
+import time
 
 from .adapter import Adapter
 
-log = logging.getLogger(__name__)
-log.addHandler(logging.NullHandler())
-
 
-class SerialAdapter(Adapter):
-    """ Adapter class for using the Python Serial package to allow
-    serial communication to instrument
-
-    :param port: Serial port
-    :param kwargs: Any valid key-word argument for serial.Serial
+class TelnetAdapter(Adapter):
+    """ Adapter class for using the Python telnetlib package to allow
+    communication to instruments
+
+    :param host: host address of the instrument
+    :param port: TCPIP port
+    :param query_delay: delay in seconds between write and read in the ask
+        method
+    :param preprocess_reply: optional callable used to preprocess strings
+        received from the instrument. The callable returns the processed string.
+    :param kwargs: Valid keyword arguments for telnetlib.Telnet, currently
+        this is only 'timeout'
     """
 
-    def __init__(self, port, **kwargs):
-        if isinstance(port, serial.Serial):
-            self.connection = port
-        else:
-            self.connection = serial.Serial(port, **kwargs)
-
-    def __del__(self):
-        """ Ensures the connection is closed upon deletion
-        """
-        self.connection.close()
+    def __init__(self, host, port=0, query_delay=0, preprocess_reply=None,
+                 **kwargs):
+        super().__init__(preprocess_reply=preprocess_reply)
+        self.query_delay = query_delay
+        safe_keywords = ['timeout']
+        for kw in kwargs:
+            if kw not in safe_keywords:
+                raise TypeError(
+                    f"TelnetAdapter: unexpected keyword argument '{kw}', "
+                    f"allowed are: {str(safe_keywords)}")
+        self.connection = telnetlib.Telnet(host, port, **kwargs)
 
     def write(self, command):
         """ Writes a command to the instrument
 
-        :param command: SCPI command string to be sent to the instrument
+        :param command: command string to be sent to the instrument
         """
-        self.connection.write(command.encode())  # encode added for Python 3
+        self.connection.write(command.encode())
 
     def read(self):
-        """ Reads until the buffer is empty and returns the resulting
-        ASCII respone
+        """ Read something even with blocking the I/O. After something is
+        received check again to obtain a full reply.
 
         :returns: String ASCII response of the instrument.
         """
-        return b"\n".join(self.connection.readlines()).decode()
+        return self.connection.read_some().decode() + \
+                self.connection.read_very_eager().decode()
 
-    def binary_values(self, command, header_bytes=0, dtype=np.float32):
-        """ Returns a numpy array from a query for binary data 
+    def ask(self, command):
+        """ Writes a command to the instrument and returns the resulting ASCII
+        response
 
-        :param command: SCPI command to be sent to the instrument
-        :param header_bytes: Integer number of bytes to ignore in header
-        :param dtype: The NumPy data type to format the values with
-        :returns: NumPy array of values
+        :param command: command string to be sent to the instrument
+        :returns: String ASCII response of the instrument
         """
-        self.connection.write(command.encode())
-        binary = self.connection.read().decode()
-        header, data = binary[:header_bytes], binary[header_bytes:]
-        return np.fromstring(data, dtype=dtype)
+        self.write(command)
+        time.sleep(self.query_delay)
+        return self.read()
 
     def __repr__(self):
-        return "<SerialAdapter(port='%s')>" % self.connection.port
+        return "<TelnetAdapter(host=%s, port=%d)>" % (self.connection.host, self.connection.port)
```

### Comparing `PyMeasure-0.8.0/pymeasure/adapters/visa.py` & `PyMeasure-0.9.0/pymeasure/adapters/visa.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,15 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 import logging
 
 import copy
-import visa
+import pyvisa
 import numpy as np
 from pkg_resources import parse_version
 
 from .adapter import Adapter
 
 log = logging.getLogger(__name__)
 log.addHandler(logging.NullHandler())
@@ -39,49 +39,49 @@
 class VISAAdapter(Adapter):
     """ Adapter class for the VISA library using PyVISA to communicate
     with instruments.
 
     :param resource: VISA resource name that identifies the address
     :param visa_library: VisaLibrary Instance, path of the VISA library or VisaLibrary spec string (@py or @ni).
                          if not given, the default for the platform will be used.
+    :param preprocess_reply: optional callable used to preprocess strings
+        received from the instrument. The callable returns the processed string.
     :param kwargs: Any valid key-word arguments for constructing a PyVISA instrument
     """
 
-    def __init__(self, resourceName, visa_library='', **kwargs):
+    def __init__(self, resource_name, visa_library='', preprocess_reply=None, **kwargs):
+        super().__init__(preprocess_reply=preprocess_reply)
         if not VISAAdapter.has_supported_version():
             raise NotImplementedError("Please upgrade PyVISA to version 1.8 or later.")
 
-        if isinstance(resourceName, int):
-            resourceName = "GPIB0::%d::INSTR" % resourceName
-        super(VISAAdapter, self).__init__()
-        self.resource_name = resourceName
-        self.manager = visa.ResourceManager(visa_library)
-        safeKeywords = ['resource_name', 'timeout',
-                        'chunk_size', 'lock', 'delay', 'send_end',
-                        'values_format', 'read_termination', 'write_termination']
+        if isinstance(resource_name, int):
+            resource_name = "GPIB0::%d::INSTR" % resource_name
+        self.resource_name = resource_name
+        self.manager = pyvisa.ResourceManager(visa_library)
+        safeKeywords = [
+            'resource_name', 'timeout', 'chunk_size', 'lock', 'query_delay', 'send_end',
+            'read_termination', 'write_termination'
+        ]
         kwargsCopy = copy.deepcopy(kwargs)
         for key in kwargsCopy:
             if key not in safeKeywords:
                 kwargs.pop(key)
-        self.connection = self.manager.get_instrument(
-            resourceName,
+        self.connection = self.manager.open_resource(
+            resource_name,
             **kwargs
         )
 
     @staticmethod
     def has_supported_version():
         """ Returns True if the PyVISA version is greater than 1.8 """
-        if hasattr(visa, '__version__'):
-            return parse_version(visa.__version__) >= parse_version('1.8')
+        if hasattr(pyvisa, '__version__'):
+            return parse_version(pyvisa.__version__) >= parse_version('1.8')
         else:
             return False
 
-    def __repr__(self):
-        return "<VISAAdapter(resource='%s')>" % self.connection.resourceName
-
     def write(self, command):
         """ Writes a command to the instrument
 
         :param command: SCPI command string to be sent to the instrument
         """
         self.connection.write(command)
 
@@ -107,56 +107,52 @@
         ASCII response
 
         :param command: SCPI command string to be sent to the instrument
         :returns: String ASCII response of the instrument
         """
         return self.connection.query(command)
 
-    def ask_values(self, command):
+    def ask_values(self, command, **kwargs):
         """ Writes a command to the instrument and returns a list of formatted
-        values from the result. The format of the return is configurated by
-        self.config().
+        values from the result. This leverages the `query_ascii_values` method
+        in PyVISA.
 
         :param command: SCPI command to be sent to the instrument
+        :param kwargs: Key-word arguments to pass onto `query_ascii_values`
         :returns: Formatted response of the instrument.
         """
-        return self.connection.query_values(command)
+        return self.connection.query_ascii_values(command, **kwargs)
 
     def binary_values(self, command, header_bytes=0, dtype=np.float32):
         """ Returns a numpy array from a query for binary data
 
         :param command: SCPI command to be sent to the instrument
         :param header_bytes: Integer number of bytes to ignore in header
         :param dtype: The NumPy data type to format the values with
         :returns: NumPy array of values
         """
         self.connection.write(command)
         binary = self.connection.read_raw()
         header, data = binary[:header_bytes], binary[header_bytes:]
         return np.fromstring(data, dtype=dtype)
 
-    def config(self, is_binary=False, datatype='str',
-               container=np.array, converter='s',
-               separator=',', is_big_endian=False):
-        """ Configurate the format of data transfer to and from the instrument.
-
-        :param is_binary: If True, data is in binary format, otherwise ASCII.
-        :param datatype: Data type.
-        :param container: Return format. Any callable/type that takes an iterable.
-        :param converter: String converter, used in dealing with ASCII data.
-        :param separator: Delimiter of a series of data in ASCII.
-        :param is_big_endian: Endianness.
-        """
-        self.connection.values_format.is_binary = is_binary
-        self.connection.values_format.datatype = datatype
-        self.connection.values_format.container = container
-        self.connection.values_format.converter = converter
-        self.connection.values_format.separator = separator
-        self.connection.values_format.is_big_endian = is_big_endian
+    def write_binary_values(self, command, values, **kwargs):
+        """ Write binary data to the instrument, e.g. waveform for signal generators
+
+        :param command: SCPI command to be sent to the instrument
+        :param values: iterable representing the binary values
+        :param kwargs: Key-word arguments to pass onto `write_binary_values`
+        :returns: number of bytes written
+        """
+
+        return self.connection.write_binary_values(command, values, **kwargs)
 
     def wait_for_srq(self, timeout=25, delay=0.1):
         """ Blocks until a SRQ, and leaves the bit high
 
         :param timeout: Timeout duration in seconds
         :param delay: Time delay between checking SRQ in seconds
         """
         self.connection.wait_for_srq(timeout * 1000)
+
+    def __repr__(self):
+        return "<VISAAdapter(resource='%s')>" % self.connection.resource_name
```

### Comparing `PyMeasure-0.8.0/pymeasure/adapters/vxi11.py` & `PyMeasure-0.9.0/pymeasure/adapters/vxi11.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -37,31 +37,29 @@
 
 class VXI11Adapter(Adapter):
     """ VXI11 Adapter class. Provides a adapter object that
         wraps around the read, write and ask functionality
         of the vxi11 library.
 
     :param host: string containing the visa connection information.
-
+    :param preprocess_reply: optional callable used to preprocess strings
+        received from the instrument. The callable returns the processed string.
     """
 
-    def __init__(self, host, **kwargs):
-
+    def __init__(self, host, preprocess_reply=None, **kwargs):
+        super().__init__(preprocess_reply=preprocess_reply)
         # Filter valid arguments that can be passed to vxi instrument
         valid_args = ["name", "client_id", "term_char"]
         self.conn_kwargs = {}
         for key in kwargs:
             if key in valid_args:
                 self.conn_kwargs[key] = kwargs[key]
 
         self.connection = vxi11.Instrument(host, **self.conn_kwargs)
 
-    def __repr__(self):
-        return '<VXI11Adapter(host={})>'.format(self.connection.host)
-
     def write(self, command):
         """ Wrapper function for the write command using the
         vxi11 interface.
 
         :param command: string with command the that will be transmitted
                          to the instrument.
         """
@@ -109,7 +107,10 @@
 
         :param command: binary string with the command that will be
                         transmitted to the instrument
 
         :returns binary string containing the response from the device.
         """
         return self.connection.ask_raw(command)
+
+    def __repr__(self):
+        return '<VXI11Adapter(host={})>'.format(self.connection.host)
```

### Comparing `PyMeasure-0.8.0/pymeasure/console.py` & `PyMeasure-0.9.0/pymeasure/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/Qt.py` & `PyMeasure-0.9.0/pymeasure/display/Qt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/__init__.py` & `PyMeasure-0.9.0/pymeasure/display/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/browser.py` & `PyMeasure-0.9.0/pymeasure/display/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/curves.py` & `PyMeasure-0.9.0/pymeasure/display/curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/inputs.py` & `PyMeasure-0.9.0/pymeasure/display/inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -51,16 +51,16 @@
         Connects a new parameter to the input box, and initializes the box
         value.
 
         :param parameter: parameter to connect.
         """
         self._parameter = parameter
 
-        if parameter.default is not None:
-            self.setValue(parameter.default)
+        if parameter.is_set():
+            self.setValue(parameter.value)
 
         if hasattr(parameter, 'units') and parameter.units:
             self.setSuffix(" %s" % parameter.units)
 
     def update_parameter(self):
         """
         Update the parameter value with the Input GUI element's current value.
@@ -186,36 +186,38 @@
             Input.__init__(self, parameter)
         self._stringChoices = None
         self.setEditable(False)
 
     def set_parameter(self, parameter):
         # Override from :class:`Input`
         try:
-            self._stringChoices = tuple(str(choice) for choice in parameter.choices)
+            if hasattr(parameter, 'units') and parameter.units:
+                suffix = " %s"%parameter.units
+            else:
+                suffix = ""
+
+            self._stringChoices = tuple((str(choice) + suffix) for choice in parameter.choices)
         except TypeError: # choices is None
             self._stringChoices = tuple()
-        super().set_parameter(parameter)
         self.clear()
         self.addItems(self._stringChoices)
 
-        # can't be set in super().set_parameter: addItems not yet called there
-        if parameter.default is not None:
-            self.setValue(parameter.default)
+        super().set_parameter(parameter)
 
 
     def setValue(self, value):
         try:
             index = self._parameter.choices.index(value)
             self.setCurrentIndex(index)
         except (TypeError, ValueError) as e: # no choices or choice invalid
             raise ValueError("Invalid choice for parameter. "
                              "Must be one of %s" % str(self._parameter.choices)) from e
 
     def setSuffix(self, value):
-        self._stringChoices = tuple(choice + str(value) for choice in self._stringChoices)
+        pass
 
     def value(self):
         return self._parameter.choices[self.currentIndex()]
 
 
 class ScientificInput(QtGui.QDoubleSpinBox, Input):
     """
@@ -233,22 +235,26 @@
         else:
             QtGui.QDoubleSpinBox.__init__(self, parent, **kwargs)
             Input.__init__(self, parameter)
         self.setButtonSymbols(QtGui.QAbstractSpinBox.NoButtons)
 
     def set_parameter(self, parameter):
         # Override from :class:`Input`
-        self.setMinimum(parameter.minimum)
-        self.setMaximum(parameter.maximum)
+        self._parameter = parameter  # required before super().set_parameter
+        # for self.validate which is called when setting self.decimals()
         self.validator = QtGui.QDoubleValidator(
             parameter.minimum,
             parameter.maximum,
-            10, self)
+            parameter.decimals,
+            self)
+        self.setDecimals(parameter.decimals)
+        self.setMinimum(parameter.minimum)
+        self.setMaximum(parameter.maximum)
         self.validator.setNotation(QtGui.QDoubleValidator.ScientificNotation)
-        super().set_parameter(parameter) # default gets set here, after min/max
+        super().set_parameter(parameter)  # default gets set here, after min/max
 
     def validate(self, text, pos):
         if self._parameter.units:
             text = text[:-(len(self._parameter.units) + 1)]
             result = self.validator.validate(text, pos)
             return result[0], result[1] + " %s" % self._parameter.units, result[2]
         else:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/listeners.py` & `PyMeasure-0.9.0/pymeasure/display/listeners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/log.py` & `PyMeasure-0.9.0/pymeasure/display/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/manager.py` & `PyMeasure-0.9.0/pymeasure/display/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -226,14 +226,15 @@
     def _running(self):
         if self.is_running():
             self.running.emit(self._running_experiment)
 
     def _clean_up(self):
         self._worker.join()
         del self._worker
+        self._monitor.wait()
         del self._monitor
         self._worker = None
         self._running_experiment = None
         log.debug("Manager has cleaned up after the Worker")
 
     def _failed(self):
         log.debug("Manager's running experiment has failed")
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/plotter.py` & `PyMeasure-0.9.0/pymeasure/display/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/thread.py` & `PyMeasure-0.9.0/pymeasure/display/thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/widgets.py` & `PyMeasure-0.9.0/pymeasure/display/widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -311,15 +311,15 @@
                         item.update_img()
                 else:
                     item.update()
 
     def parse_axis(self, axis):
         """ Returns the units of an axis by searching the string
         """
-        units_pattern = "\((?P<units>\w+)\)"
+        units_pattern = r"\((?P<units>\w+)\)"
         try:
             match = re.search(units_pattern, axis)
         except TypeError:
             match = None
             
         if match:
             if 'units' in match.groupdict():
@@ -1002,7 +1002,37 @@
         else:
             log.error("No sequence entered for " +
                       "for parameter '{}', depth {}".format(name, depth))
             raise SequenceEvaluationException()
 
         evaluated_string = numpy.array(evaluated_string)
         return evaluated_string
+
+class DirectoryLineEdit(QtGui.QLineEdit):
+    """
+    Widget that allows to choose a directory path.
+    A completer is implemented for quick completion.
+    A browse button is available.
+    """
+
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+
+        completer = QtGui.QCompleter(self)
+        completer.setCompletionMode(QtGui.QCompleter.PopupCompletion)
+
+        model = QtGui.QDirModel(completer)
+        model.setFilter(QtCore.QDir.Dirs | QtCore.QDir.Drives | QtCore.QDir.NoDotAndDotDot | QtCore.QDir.AllDirs)
+        completer.setModel(model)
+
+        self.setCompleter(completer)
+
+        browse_action = QtGui.QAction(self)
+        browse_action.setIcon(self.style().standardIcon(getattr(QtGui.QStyle, 'SP_DialogOpenButton')))
+        browse_action.triggered.connect(self.browse_triggered)
+
+        self.addAction(browse_action, QtGui.QLineEdit.TrailingPosition)
+
+    def browse_triggered(self):
+        path = QtGui.QFileDialog.getExistingDirectory(self, 'Directory', '/')
+        if path != '':
+            self.setText(path)
```

### Comparing `PyMeasure-0.8.0/pymeasure/display/windows.py` & `PyMeasure-0.9.0/pymeasure/display/windows.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,28 +21,32 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 import logging
 
 import os
+import subprocess, platform
+
+
 import pyqtgraph as pg
 
 from .browser import BrowserItem
 from .curves import ResultsCurve
 from .manager import Manager, Experiment, ImageExperiment, ImageManager
 from .Qt import QtCore, QtGui
 from .widgets import (
     PlotWidget,
     BrowserWidget,
     InputsWidget,
     LogWidget,
     ResultsDialog,
     SequencerWidget,
     ImageWidget,
+    DirectoryLineEdit,
 )
 from ..experiment.results import Results
 
 log = logging.getLogger(__name__)
 log.addHandler(logging.NullHandler())
 
 
@@ -144,43 +148,48 @@
         accessed to further customise the plot view programmatically, e.g.,
         display log-log or semi-log axes by default, change axis range, etc.
 
     .. _pyqtgraph.PlotItem: http://www.pyqtgraph.org/documentation/graphicsItems/plotitem.html
 
 
     """
-    EDITOR = 'gedit'
 
     def __init__(self, procedure_class, inputs=(), displays=(), x_axis=None, y_axis=None,
                  log_channel='', log_level=logging.INFO, parent=None, sequencer=False,
-                 sequencer_inputs=None, sequence_file=None, inputs_in_scrollarea=False):
+                 sequencer_inputs=None, sequence_file=None, inputs_in_scrollarea=False, directory_input=False):
         super().__init__(parent)
         app = QtCore.QCoreApplication.instance()
         app.aboutToQuit.connect(self.quit)
         self.procedure_class = procedure_class
         self.inputs = inputs
         self.displays = displays
         self.use_sequencer = sequencer
         self.sequencer_inputs = sequencer_inputs
         self.sequence_file = sequence_file
         self.inputs_in_scrollarea = inputs_in_scrollarea
+        self.directory_input = directory_input
         self.log = logging.getLogger(log_channel)
         self.log_level = log_level
         log.setLevel(log_level)
         self.log.setLevel(log_level)
         self.x_axis, self.y_axis = x_axis, y_axis
         self._setup_ui()
         self._layout()
         self.setup_plot(self.plot)
 
     def _setup_ui(self):
         self.log_widget = LogWidget()
         self.log.addHandler(self.log_widget.handler)  # needs to be in Qt context?
         log.info("ManagedWindow connected to logging")
 
+        if self.directory_input:
+            self.directory_label = QtGui.QLabel(self)
+            self.directory_label.setText('Directory')
+            self.directory_line = DirectoryLineEdit(parent=self)
+
         self.queue_button = QtGui.QPushButton('Queue', self)
         self.queue_button.clicked.connect(self.queue)
 
         self.abort_button = QtGui.QPushButton('Abort', self)
         self.abort_button.setEnabled(False)
         self.abort_button.clicked.connect(self.abort)
 
@@ -232,27 +241,37 @@
         hbox = QtGui.QHBoxLayout()
         hbox.setSpacing(10)
         hbox.setContentsMargins(-1, 6, -1, 6)
         hbox.addWidget(self.queue_button)
         hbox.addWidget(self.abort_button)
         hbox.addStretch()
 
+        if self.directory_input:
+            vbox = QtGui.QVBoxLayout()
+            vbox.addWidget(self.directory_label)
+            vbox.addWidget(self.directory_line)
+            vbox.addLayout(hbox)
+
         if self.inputs_in_scrollarea:
             inputs_scroll = QtGui.QScrollArea()
             inputs_scroll.setWidgetResizable(True)
             inputs_scroll.setFrameStyle(QtGui.QScrollArea.NoFrame)
 
             self.inputs.setSizePolicy(1, 0)
             inputs_scroll.setWidget(self.inputs)
             inputs_vbox.addWidget(inputs_scroll, 1)
 
         else:
             inputs_vbox.addWidget(self.inputs)
 
-        inputs_vbox.addLayout(hbox)
+        if self.directory_input:
+            inputs_vbox.addLayout(vbox)
+        else:
+            inputs_vbox.addLayout(hbox)
+
         inputs_vbox.addStretch(0)
         inputs_dock.setLayout(inputs_vbox)
 
         dock = QtGui.QDockWidget('Input Parameters')
         dock.setWidget(inputs_dock)
         dock.setFeatures(QtGui.QDockWidget.NoDockWidgetFeatures)
         self.addDockWidget(QtCore.Qt.LeftDockWidgetArea, dock)
@@ -278,14 +297,17 @@
 
         self.main.setLayout(vbox)
         self.setCentralWidget(self.main)
         self.main.show()
         self.resize(1000, 800)
 
     def quit(self, evt=None):
+        if self.manager.is_running():
+            self.abort()
+
         self.close()
 
     def browser_item_changed(self, item, column):
         if column == 0:
             state = item.checkState(0)
             experiment = self.manager.experiments.with_browser_item(item)
             if state == 0:
@@ -383,17 +405,28 @@
         if color.isValid():
             pixelmap = QtGui.QPixmap(24, 24)
             pixelmap.fill(color)
             experiment.browser_item.setIcon(0, QtGui.QIcon(pixelmap))
             experiment.curve.setPen(pg.mkPen(color=color, width=2))
 
     def open_file_externally(self, filename):
-        # TODO: Make this function OS-agnostic
-        import subprocess
-        proc = subprocess.Popen([self.EDITOR, filename])
+        """ Method to open the datafile using an external editor or viewer. Uses the default
+        application to open a datafile of this filetype, but can be overridden by the child
+        class in order to open the file in another application of choice.
+        """
+        system = platform.system()
+        if (system == 'Windows'):
+            # The empty argument after the start is needed to be able to cope correctly with filenames with spaces
+            proc = subprocess.Popen(['start', '', filename], shell=True)
+        elif (system == 'Linux'):
+            proc = subprocess.Popen(['xdg-open', filename])
+        elif (system == 'Darwin'):
+            proc = subprocess.Popen(['open', filename])
+        else:
+            raise Exception("{cls} method open_file_externally does not support {system} OS".format(cls=type(self).__name__,system=system))
 
     def make_procedure(self):
         if not isinstance(self.inputs, InputsWidget):
             raise Exception("ManagedWindow can not make a Procedure"
                             " without a InputsWidget type")
         return self.inputs.get_procedure()
 
@@ -501,14 +534,19 @@
             self.browser_widget.clear_button.setEnabled(True)
 
     def finished(self, experiment):
         if not self.manager.experiments.has_next():
             self.abort_button.setEnabled(False)
             self.browser_widget.clear_button.setEnabled(True)
 
+    @property
+    def directory(self):
+        if not self.directory_input:
+            raise ValueError("No directory input in the ManagedWindow")
+        return self.directory_line.text()
 
 # TODO: Inheret from ManagedWindow to share code and features
 class ManagedImageWindow(QtGui.QMainWindow):
     """
     Abstract base class.
 
     The MangedImageWindow provides an interface for inputting experiment
@@ -532,16 +570,14 @@
         display log-log or semi-log axes by default, change axis range, etc.
 
     .. _pyqtgraph.PlotItem: http://www.pyqtgraph.org/documentation/graphicsItems/plotitem.html
 
 
     """
 
-    EDITOR = 'gedit'
-
     def __init__(self, procedure_class, x_axis, y_axis, z_axis=None, inputs=(), displays=(),
                  log_channel='', log_level=logging.INFO, parent=None):
         super().__init__(parent)
         app = QtCore.QCoreApplication.instance()
         app.aboutToQuit.connect(self.quit)
         self.procedure_class = procedure_class
         self.inputs = inputs
@@ -642,14 +678,17 @@
 
         self.main.setLayout(vbox)
         self.setCentralWidget(self.main)
         self.main.show()
         self.resize(1000, 800)
 
     def quit(self, evt=None):
+        if self.manager.is_running():
+            self.abort()
+
         self.close()
 
     def browser_item_changed(self, item, column):
         if column == 0:
             state = item.checkState(0)
             experiment = self.manager.experiments.with_browser_item(item)
             if state == 0:
@@ -753,17 +792,28 @@
         if color.isValid():
             pixelmap = QtGui.QPixmap(24, 24)
             pixelmap.fill(color)
             experiment.browser_item.setIcon(0, QtGui.QIcon(pixelmap))
             experiment.curve.setPen(pg.mkPen(color=color, width=2))
 
     def open_file_externally(self, filename):
-        # TODO: Make this function OS-agnostic
-        import subprocess
-        proc = subprocess.Popen([self.EDITOR, filename])
+        """ Method to open the datafile using an external editor or viewer. Uses the default
+        application to open a datafile of this filetype, but can be overridden by the child
+        class in order to open the file in another application of choice.
+        """
+        system = platform.system()
+        if (system == 'Windows'):
+            # The empty argument after the start is needed to be able to cope correctly with filenames with spaces
+            proc = subprocess.Popen(['start', '', filename], shell=True)
+        elif (system == 'Linux'):
+            proc = subprocess.Popen(['xdg-open', filename])
+        elif (system == 'Darwin'):
+            proc = subprocess.Popen(['open', filename])
+        else:
+            raise Exception("{cls} method open_file_externally does not support {system} OS".format(cls=type(self).__name__,system=system))
 
     def make_procedure(self):
         if not isinstance(self.inputs, InputsWidget):
             raise Exception("ManagedWindow can not make a Procedure"
                             " without an InputsWidget type")
         return self.inputs.get_procedure()
```

### Comparing `PyMeasure-0.8.0/pymeasure/errors.py` & `PyMeasure-0.9.0/pymeasure/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/experiment/__init__.py` & `PyMeasure-0.9.0/pymeasure/experiment/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/experiment/config.py` & `PyMeasure-0.9.0/pymeasure/experiment/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -42,9 +42,10 @@
     return config
 
 
 # noinspection PyProtectedMember
 def set_mpl_rcparams(config):
     if 'matplotlib.rcParams' in config._sections.keys():
         import matplotlib
+        from cycler import cycler
         for key in config._sections['matplotlib.rcParams']:
             matplotlib.rcParams[key] = eval(config._sections['matplotlib.rcParams'][key])
```

### Comparing `PyMeasure-0.8.0/pymeasure/experiment/experiment.py` & `PyMeasure-0.9.0/pymeasure/experiment/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -35,14 +35,15 @@
 from .results import unique_filename
 from .config import get_config, set_mpl_rcparams
 from pymeasure.log import setup_logging, console_log
 from pymeasure.experiment import Results, Worker
 from .parameters import Measurable
 import time, signal
 import numpy as np
+import pandas as pd
 import tempfile
 import gc
 
 
 def get_array(start, stop, step):
     """Returns a numpy array from start to stop"""
     step = np.sign(stop - start) * abs(step)
@@ -177,14 +178,15 @@
                 self.figs.append(ax.get_figure())
             self._user_interrupt = False
 
     def clear_plot(self):
         """Clear the figures and plot lists."""
         for fig in self.figs:
             fig.clf()
+        for pl in self.plots:
             pl.close()
         self.figs = []
         self.plots = []
         gc.collect()
 
     def update_plot(self):
         """Update the plots in the plots list with new data from the experiment.data
@@ -198,15 +200,15 @@
                     x, y = plot['args'][0], plot['args'][1]
                     if type(y) == str:
                         y = [y]
                     for yname, line in zip(y, ax.lines):
                         self.update_line(ax, line, x, yname)
                 if plot['type'] == 'pcolor':
                     x, y, z = plot['x'], plot['y'], plot['z']
-                    update_pcolor(ax, x, y, z)
+                    self.update_pcolor(ax, x, y, z)
 
             display.clear_output(wait=True)
             display.display(*self.figs)
             time.sleep(0.1)
         except KeyboardInterrupt:
             display.clear_output(wait=True)
             display.display(*self.figs)
@@ -217,14 +219,15 @@
         Store the plots in a plots list attribute."""
         title = self.title
         x, y, z = self._data[xname], self._data[yname], self._data[zname]
         shape = (len(y.unique()), len(x.unique()))
         diff = shape[0] * shape[1] - len(z)
         Z = np.concatenate((z.values, np.zeros(diff))).reshape(shape)
         df = pd.DataFrame(Z, index=y.unique(), columns=x.unique())
+        # TODO: Remove seaborn dependencies
         ax = sns.heatmap(df)
         pl.title(title)
         pl.xlabel(xname)
         pl.ylabel(yname)
         ax.invert_yaxis()
         pl.plt.show()
         self.plots.append(
@@ -237,14 +240,15 @@
         """Update a pcolor graph with new data."""
         x, y, z = self._data[xname], self._data[yname], self._data[zname]
         shape = (len(y.unique()), len(x.unique()))
         diff = shape[0] * shape[1] - len(z)
         Z = np.concatenate((z.values, np.zeros(diff))).reshape(shape)
         df = pd.DataFrame(Z, index=y.unique(), columns=x.unique())
         cbar_ax = ax.get_figure().axes[1]
+        # TODO: Remove seaborn dependencies
         sns.heatmap(df, ax=ax, cbar_ax=cbar_ax)
         ax.set_xlabel(xname)
         ax.set_ylabel(yname)
         ax.invert_yaxis()
 
     def update_line(self, ax, hl, xname, yname):
         """Update a line in a matplotlib graph with new data."""
```

### Comparing `PyMeasure-0.8.0/pymeasure/experiment/listeners.py` & `PyMeasure-0.9.0/pymeasure/experiment/listeners.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -103,7 +103,13 @@
         for filename in results.data_filenames:
             fh = FileHandler(filename=filename, **kwargs)
             fh.setFormatter(results.formatter)
             fh.setLevel(logging.NOTSET)
             handlers.append(fh)
 
         super().__init__(queue, *handlers)
+
+    def stop(self):
+        for handler in self.handlers:
+            handler.close()
+
+        super().stop()
```

### Comparing `PyMeasure-0.8.0/pymeasure/experiment/parameters.py` & `PyMeasure-0.9.0/pymeasure/experiment/parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -89,14 +89,20 @@
         if self.is_set():
             return int(self._value)
         else:
             raise ValueError("Parameter value is not set")
 
     @value.setter
     def value(self, value):
+        if isinstance(value, str):
+            value, _, units = value.strip().partition(" ")
+            if units != "" and units != self.units:
+                raise ValueError("Units included in string (%s) do not match"
+                                 "the units of the IntegerParameter (%s)" % (units, self.units))
+
         try:
             value = int(value)
         except ValueError:
             raise ValueError("IntegerParameter given non-integer value of "
                              "type '%s'" % type(value))
         if value < self.minimum:
             raise ValueError("IntegerParameter value is below the minimum")
@@ -134,50 +140,68 @@
         if self.is_set():
             return self._value
         else:
             raise ValueError("Parameter value is not set")
 
     @value.setter
     def value(self, value):
-        try:
+        if isinstance(value, str):
+            if value.lower() == "true":
+                self._value = True
+            elif value.lower() == "false":
+                self._value = False
+            else:
+                raise ValueError("BooleanParameter given string value of '%s'" % value)
+        elif isinstance(value, (int, float)) and value in [0, 1]:
             self._value = bool(value)
-        except ValueError:
+        elif isinstance(value, bool):
+            self._value = value
+        else:
             raise ValueError("BooleanParameter given non-boolean value of "
                              "type '%s'" % type(value))
 
 
 class FloatParameter(Parameter):
     """ :class:`.Parameter` sub-class that uses the floating point
     type to store the value.
 
     :var value: The floating point value of the parameter
 
     :param name: The parameter name
     :param units: The units of measure for the parameter
     :param minimum: The minimum allowed value (default: -1e9)
     :param maximum: The maximum allowed value (default: 1e9)
+    :param decimals: The number of decimals considered (default: 15)
     :param default: The default floating point value
     :param ui_class: A Qt class to use for the UI of this parameter
     """
 
-    def __init__(self, name, units=None, minimum=-1e9, maximum=1e9, **kwargs):
+    def __init__(self, name, units=None, minimum=-1e9, maximum=1e9,
+                 decimals=15, **kwargs):
         super().__init__(name, **kwargs)
         self.units = units
         self.minimum = minimum
         self.maximum = maximum
+        self.decimals = decimals
 
     @property
     def value(self):
         if self.is_set():
             return float(self._value)
         else:
             raise ValueError("Parameter value is not set")
 
     @value.setter
     def value(self, value):
+        if isinstance(value, str):
+            value, _, units = value.strip().partition(" ")
+            if units != "" and units != self.units:
+                raise ValueError("Units included in string (%s) do not match"
+                                 "the units of the FloatParameter (%s)" % (units, self.units))
+
         try:
             value = float(value)
         except ValueError:
             raise ValueError("FloatParameter given non-float value of "
                              "type '%s'" % type(value))
         if value < self.minimum:
             raise ValueError("FloatParameter value is below the minimum")
@@ -222,16 +246,20 @@
         if self.is_set():
             return [float(ve) for ve in self._value]
         else:
             raise ValueError("Parameter value is not set")
 
     @value.setter
     def value(self, value):
-        # Strip initial and final brackets
         if isinstance(value, str):
+            # strip units if included
+            if self.units is not None and value.endswith(" " + self.units):
+                value = value[:-len(self.units)].strip()
+
+            # Strip initial and final brackets
             if (value[0] != '[') or (value[-1] != ']'):
                 raise ValueError("VectorParameter must be passed a vector"
                                  " denoted by square brackets if initializing"
                                  " by string.")
             raw_list = value[1:-1].split(",")
         elif isinstance(value, (list, tuple)):
             raw_list = value
@@ -283,14 +311,19 @@
         if self.is_set():
             return self._value
         else:
             raise ValueError("Parameter value is not set")
 
     @value.setter
     def value(self, value):
+        # strip units if included
+        if isinstance(value, str):
+            if self.units is not None and value.endswith(" " + self.units):
+                value = value[:-len(self.units)].strip()
+
         if self._choices is not None and value in self._choices:
             self._value = value
         else:
             raise ValueError("Invalid choice for parameter. "
                              "Must be one of %s" % str(self._choices))
 
     @property
@@ -324,16 +357,20 @@
         if self.is_set():
             return [float(ve) for ve in self._value]
         else:
             raise ValueError("Parameter value is not set")
 
     @value.setter
     def value(self, value):
-        # Strip initial and final brackets
         if isinstance(value, str):
+            # strip units if included
+            if self.units is not None and value.endswith(" " + self.units):
+                value = value[:-len(self.units)].strip()
+
+            # Strip initial and final brackets
             if (value[0] != '[') or (value[-1] != ']'):
                 raise ValueError("VectorParameter must be passed a vector"
                                  " denoted by square brackets if initializing"
                                  " by string.")
             raw_list = value[1:-1].split(",")
         elif isinstance(value, (list, tuple)):
             raw_list = value
```

### Comparing `PyMeasure-0.8.0/pymeasure/experiment/procedure.py` & `PyMeasure-0.9.0/pymeasure/experiment/procedure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/experiment/results.py` & `PyMeasure-0.9.0/pymeasure/experiment/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -230,56 +230,44 @@
                                  "uncommented sections")
             if line.startswith("Procedure"):
                 regex = r"<(?:(?P<module>[^>]+)\.)?(?P<class>[^.>]+)>"
                 search = re.search(regex, line)
                 procedure_module = search.group("module")
                 procedure_class = search.group("class")
             elif line.startswith("\t"):
-                regex = (r"\t(?P<name>[^:]+):\s(?P<value>[^\s]+)"
-                         r"(?:\s(?P<units>.+))?")
-                search = re.search(regex, line)
-                if search is None:
-                    raise Exception("Error parsing header line %s." % line)
+                separator = ": "
+                partitioned_line = line[1:].partition(separator)
+                if partitioned_line[1] != separator:
+                    raise Exception("Error partitioning header line %s." % line)
                 else:
-                    parameters[search.group("name")] = (
-                        search.group("value"),
-                        search.group("units")
-                    )
+                    parameters[partitioned_line[0]] = partitioned_line[2]
+
         if procedure is None:
             if procedure_class is None:
                 raise ValueError("Header does not contain the Procedure class")
             try:
                 from importlib import import_module
                 procedure_module = import_module(procedure_module)
                 procedure_class = getattr(procedure_module, procedure_class)
                 procedure = procedure_class()
             except ImportError:
                 procedure = UnknownProcedure(parameters)
                 log.warning("Unknown Procedure being used")
             except Exception as e:
                 raise e
 
-        def units_found(parameter, units):
-            return (hasattr(parameter, 'units') and
-                    parameter.units is None and
-                    isinstance(parameter, Parameter) and
-                    units is not None)
-
         # Fill the procedure with the parameters found
         for name, parameter in procedure.parameter_objects().items():
             if parameter.name in parameters:
-                value, units = parameters[parameter.name]
-
-                if units_found(parameter, units):
-                    # Force full string to be matched
-                    value = value + " " + str(units)
+                value = parameters[parameter.name]
                 setattr(procedure, name, value)
             else:
                 raise Exception("Missing '%s' parameter when loading '%s' class" % (
                     parameter.name, procedure_class))
+
         procedure.refresh_parameters()  # Enforce update of meta data
         return procedure
 
     @staticmethod
     def load(data_filename, procedure_class=None):
         """ Returns a Results object with the associated Procedure object and
         data
```

### Comparing `PyMeasure-0.8.0/pymeasure/experiment/workers.py` & `PyMeasure-0.9.0/pymeasure/experiment/workers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,29 +18,18 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from ..errors import RangeError, RangeException
-from .instrument import Instrument
-from .mock import Mock
-from .resources import list_resources
-from .validators import discreteTruncate
-
-from . import advantest
-from . import agilent
-from . import ametek
-from . import anritsu
-from . import deltaelektronika
-from . import danfysik
-from . import fwbell
-from . import hp
-from . import keithley
-from . import lakeshore
-from . import parker
-from . import signalrecovery
-from . import srs
-from . import tektronix
-from . import thorlabs
-from . import yokogawa
+from .agilent8257D import Agilent8257D
+from .agilent8722ES import Agilent8722ES
+from .agilentE4408B import AgilentE4408B
+from .agilentE4980 import AgilentE4980
+from .agilent34410A import Agilent34410A
+from .agilent34450A import Agilent34450A
+from .agilent4156 import Agilent4156
+from .agilent33220A import Agilent33220A
+from .agilent33500 import Agilent33500
+from .agilent33521A import Agilent33521A
+from .agilentB1500 import AgilentB1500
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/advantest/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/advantest/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/advantest/advantestR3767CG.py` & `PyMeasure-0.9.0/pymeasure/instruments/advantest/advantestR3767CG.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/fwbell/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,16 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from .agilent8257D import Agilent8257D
-from .agilent8722ES import Agilent8722ES
-from .agilentE4408B import AgilentE4408B
-from .agilentE4980 import AgilentE4980
-from .agilent34410A import Agilent34410A
-from .agilent4156 import Agilent4156
-from .agilent33220A import Agilent33220A
-from .agilent33500 import Agilent33500
-from .agilent33521A import Agilent33521A
+from .fwbell5080 import FWBell5080
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent33220A.py` & `PyMeasure-0.9.0/pymeasure/instruments/anritsu/anritsuMS9710C.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,311 +17,327 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
-
 import logging
+from time import sleep
+import numpy as np
+from pymeasure.instruments import Instrument
+from pymeasure.instruments.validators import (
+    strict_discrete_set,
+    truncated_discrete_set,
+    truncated_range,
+    joined_validators
+)
+import re
+
 log = logging.getLogger(__name__)
 log.addHandler(logging.NullHandler())
 
-from pymeasure.instruments import Instrument
-from pymeasure.instruments.validators import strict_discrete_set,\
-    strict_range, joined_validators
-from time import time
-from pyvisa.errors import VisaIOError
+# Analysis Results with Units, ie -24.5DBM -> (-24.5, 'DBM')
+r_value_units = re.compile(r"([-\d]*\.\d*)(.*)")
 
+# Join validators to allow for special sets of characters
+truncated_range_or_off = joined_validators(strict_discrete_set, truncated_range)
 
-# Capitalize string arguments to allow for better conformity with other WFG's
-def capitalize_string(string: str, *args, **kwargs):
-    return string.upper()
 
+def _int_or_neg_one(v):
+    try:
+        return int(v)
+    except ValueError:
+        return -1
 
-# Combine the capitalize function and validator
-string_validator = joined_validators(capitalize_string, strict_discrete_set)
 
+def _parse_trace_peak(vals):
+    """Parse the returned value from a trace peak query."""
+    l, p = vals
+    res = [l]
+    m = r_value_units.match(p)
+    if m is not None:
+        data = list(m.groups())
+        data[0] = float(data[0])
+        res.extend(data)
+    else:
+        res.append(float(p))
+    return res
 
-class Agilent33220A(Instrument):
-    """Represents the Agilent 33220A Arbitrary Waveform Generator.
 
-    .. code-block:: python
+class AnritsuMS9710C(Instrument):
+    """Anritsu MS9710C Optical Spectrum Analyzer."""
 
-        # Default channel for the Agilent 33220A
-        wfg = Agilent33220A("GPIB::10")
+    #############
+    #  Mappings #
+    #############
+    ONOFF = ["ON", "OFF"]
+    ONOFF_MAPPING = {True: 'ON', False: 'OFF', 1: 'ON', 0: 'OFF'}
 
-        wfg.shape = "SINUSOID"          # Sets a sine waveform
-        wfg.frequency = 4.7e3           # Sets the frequency to 4.7 kHz
-        wfg.amplitude = 1               # Set amplitude of 1 V
-        wfg.offset = 0                  # Set the amplitude to 0 V
+    ######################
+    #  Status Registers  #
+    ######################
 
-        wfg.burst = True                # Enable burst mode
-        wfg.burst_ncycles = 10e3        # A burst will consist of 10 cycles
-        wfg.burst_mode = "TRIGGERED"    # A burst will be applied on a trigger
-        wfg.trigger_source = "BUS"      # A burst will be triggered on TRG*
+    ese2 = Instrument.control(
+        "ESE2?", "ESE2 %d",
+        "Extended Event Status Enable Register 2",
+        get_process=int
+    )
 
-        wfg.output = True               # Enable output of waveform generator
-        wfg.trigger()                   # Trigger a burst
-        wfg.wait_for_trigger()          # Wait until the triggering is finished
-        wfg.beep()                      # "beep"
+    esr2 = Instrument.control(
+        "ESR2?", "ESR2 %d",
+        "Extended Event Status Register 2",
+        get_process=_int_or_neg_one
+    )
 
-        wfg.check_errors()              # Get the error queue
+    ###########
+    #  Modes  #
+    ###########
 
-    """
+    measure_mode = Instrument.measurement(
+        "MOD?", "Returns the current Measure Mode the OSA is in.",
+        values={None: 0, "SINGLE": 1.0, "AUTO": 2.0, "POWER": 3.0},
+        map_values=True
+    )
 
-    def __init__(self, adapter, **kwargs):
-        super(Agilent33220A, self).__init__(
-            adapter,
-            "Agilent 33220A Arbitrary Waveform generator",
-            **kwargs
-        )
+    ####################################
+    # Spectrum Parameters - Wavelength #
+    ####################################
+    wavelength_center = Instrument.control('CNT?', 'CNT %g', "Center Wavelength of Spectrum Scan in nm.")
 
-    shape = Instrument.control(
-        "FUNC?", "FUNC %s",
-        """ A string property that controls the output waveform. Can be set to:
-        SIN<USOID>, SQU<ARE>, RAMP, PULS<E>, NOIS<E>, DC, USER. """,
-        validator=string_validator,
-        values=["SINUSOID", "SIN", "SQUARE", "SQU", "RAMP",
-                "PULSE", "PULS", "NOISE", "NOIS", "DC", "USER"],
-    )
-
-    frequency = Instrument.control(
-        "FREQ?", "FREQ %s",
-        """ A floating point property that controls the frequency of the output
-        waveform in Hz, from 1e-6 (1 uHz) to 20e+6 (20 MHz), depending on the
-        specified function. Can be set. """,
-        validator=strict_range,
-        values=[1e-6, 5e+6],
-    )
-
-    amplitude = Instrument.control(
-        "VOLT?", "VOLT %f",
-        """ A floating point property that controls the voltage amplitude of the
-        output waveform in V, from 10e-3 V to 10 V. Can be set. """,
-        validator=strict_range,
-        values=[10e-3, 10],
-    )
-
-    amplitude_unit = Instrument.control(
-        "VOLT:UNIT?", "VOLT:UNIT %s",
-        """ A string property that controls the units of the amplitude. Valid
-        values are Vpp (default), Vrms, and dBm. Can be set. """,
-        validator=string_validator,
-        values=["VPP", "VRMS", "DBM"],
-    )
-
-    offset = Instrument.control(
-        "VOLT:OFFS?", "VOLT:OFFS %f",
-        """ A floating point property that controls the voltage offset of the
-        output waveform in V, from 0 V to 4.995 V, depending on the set
-        voltage amplitude (maximum offset = (10 - voltage) / 2). Can be set.
-        """,
-        validator=strict_range,
-        values=[-4.995, +4.995],
-    )
-
-    voltage_high = Instrument.control(
-        "VOLT:HIGH?", "VOLT:HIGH %f",
-        """ A floating point property that controls the upper voltage of the
-        output waveform in V, from -4.990 V to 5 V (must be higher than low
-        voltage). Can be set. """,
-        validator=strict_range,
-        values=[-4.99, 5],
-    )
-
-    voltage_low = Instrument.control(
-        "VOLT:LOW?", "VOLT:LOW %f",
-        """ A floating point property that controls the lower voltage of the
-        output waveform in V, from -5 V to 4.990 V (must be lower than high
-        voltage). Can be set. """,
-        validator=strict_range,
-        values=[-5, 4.99],
-    )
-
-    square_dutycycle = Instrument.control(
-        "FUNC:SQU:DCYC?", "FUNC:SQU:DCYC %f",
-        """ A floating point property that controls the duty cycle of a square
-        waveform function in percent. Can be set. """,
-        validator=strict_range,
-        values=[20, 80],
-    )
-
-    ramp_symmetry = Instrument.control(
-        "FUNC:RAMP:SYMM?", "FUNC:RAMP:SYMM %f",
-        """ A floating point property that controls the symmetry percentage
-        for the ramp waveform. Can be set. """,
-        validator=strict_range,
-        values=[0, 100],
-    )
-
-    pulse_period = Instrument.control(
-        "PULS:PER?", "PULS:PER %f",
-        """ A floating point property that controls the period of a pulse
-        waveform function in seconds, ranging from 200 ns to 2000 s. Can be set
-        and overwrites the frequency for *all* waveforms. If the period is
-        shorter than the pulse width + the edge time, the edge time and pulse
-        width will be adjusted accordingly. """,
-        validator=strict_range,
-        values=[200e-9, 2e3],
-    )
-
-    pulse_hold = Instrument.control(
-        "FUNC:PULS:HOLD?", "FUNC:PULS:HOLD %s",
-        """ A string property that controls if either the pulse width or the
-        duty cycle is retained when changing the period or frequency of the
-        waveform. Can be set to: WIDT<H> or DCYC<LE>. """,
-        validator=string_validator,
-        values=["WIDT", "WIDTH", "DCYC", "DCYCLE"],
-    )
-
-    pulse_width = Instrument.control(
-        "FUNC:PULS:WIDT?", "FUNC:PULS:WIDT %f",
-        """ A floating point property that controls the width of a pulse
-        waveform function in seconds, ranging from 20 ns to 2000 s, within a
-        set of restrictions depending on the period. Can be set. """,
-        validator=strict_range,
-        values=[20e-9, 2e3],
-    )
-
-    pulse_dutycycle = Instrument.control(
-        "FUNC:PULS:DCYC?", "FUNC:PULS:DCYC %f",
-        """ A floating point property that controls the duty cycle of a pulse
-        waveform function in percent. Can be set. """,
-        validator=strict_range,
-        values=[0, 100],
-    )
-
-    pulse_transition = Instrument.control(
-        "FUNC:PULS:TRAN?", "FUNC:PULS:TRAN %f",
-        """ A floating point property that controls the the edge time in
-        seconds for both the rising and falling edges. It is defined as the
-        time between 0.1 and 0.9 of the threshold. Valid values are between
-        5 ns to 100 ns. Can be set. """,
-        validator=strict_range,
-        values=[5e-9, 100e-9],
-    )
-
-    output = Instrument.control(
-        "OUTP?", "OUTP %d",
-        """ A boolean property that turns on (True) or off (False) the output
-        of the function generator. Can be set. """,
+    wavelength_span = Instrument.control('SPN?', 'SPN %g', "Wavelength Span of Spectrum Scan in nm.")
+
+    wavelength_start = Instrument.control('STA?', 'STA %g', "Wavelength Start of Spectrum Scan in nm.")
+
+    wavelength_stop = Instrument.control('STO?', 'STO %g', "Wavelength Stop of Spectrum Scan in nm.")
+
+    wavelength_marker_value = Instrument.control(
+        'MKV?', 'MKV %s',
+        "Wavelength Marker Value (wavelength or freq.?)",
         validator=strict_discrete_set,
-        map_values=True,
-        values={True: 1, False: 0},
+        values=["WL", "FREQ"]
     )
 
-    burst_state = Instrument.control(
-        "BURS:STAT?", "BURS:STAT %d",
-        """ A boolean property that controls whether the burst mode is on
-        (True) or off (False). Can be set. """,
+    wavelength_value_in = Instrument.control(
+        'WDP?', 'WDP %s',
+        "Wavelength value in Vacuum or Air",
         validator=strict_discrete_set,
-        map_values=True,
-        values={True: 1, False: 0},
+        values=["VACUUM", "AIR"]
+    )
+
+    level_scale = Instrument.measurement(
+        'LVS?', "Current Level Scale",
+        values=["LOG", "LIN"]
+    )
+
+    level_log = Instrument.control(
+        "LOG?", "LOG %f", "Level Log Scale (/div)",
+        validator=truncated_range, values=[0.1, 10.0]
+    )
+
+    level_lin = Instrument.control(
+        "LIN?", "LIN %f", "Level Linear Scale (/div)",
+        validator=truncated_range, values=[1e-12, 1]
     )
 
-    burst_mode = Instrument.control(
-        "BURS:MODE?", "BURS:MODE %s",
-        """ A string property that controls the burst mode. Valid values
-        are: TRIG<GERED>, GAT<ED>. This setting can be set. """,
-        validator=string_validator,
-        values=["TRIG", "TRIGGERED", "GAT", "GATED"],
-    )
-
-    burst_ncycles = Instrument.control(
-        "BURS:NCYC?", "BURS:NCYC %d",
-        """ An integer property that sets the number of cycles to be output
-        when a burst is triggered. Valid values are 1 to 50000. This can be
-        set. """,
+    level_opt_attn = Instrument.control(
+        "ATT?", "ATT %s", "Optical Attenuation Status (ON/OFF)",
         validator=strict_discrete_set,
-        values=range(1, 50001),
+        values=ONOFF
     )
 
-    def trigger(self):
-        """ Send a trigger signal to the function generator. """
-        self.write("*TRG;*WAI")
+    resolution = Instrument.control(
+        "RES?", "RES %f", "Resolution (nm)",
+        validator=truncated_discrete_set,
+        values=[0.05, 0.07, 0.1, 0.2, 0.5, 1.0]
+    )
 
-    def wait_for_trigger(self, timeout=3600, should_stop=lambda: False):
-        """ Wait until the triggering has finished or timeout is reached.
+    resolution_actual = Instrument.control(
+        "ARES?", "ARES %s", "Resolution Actual (ON/OFF)",
+        validator=strict_discrete_set,
+        values=ONOFF,
+        map_values=True
 
-        :param timeout: The maximum time the waiting is allowed to take. If
-                        timeout is exceeded, a TimeoutError is raised. If
-                        timeout is set to zero, no timeout will be used.
-        :param should_stop: Optional function (returning a bool) to allow the
-                            waiting to be stopped before its end.
+    )
 
-        """
-        self.write("*OPC?")
+    resolution_vbw = Instrument.control(
+        "VBW?", "VBW %s", "Video Bandwidth Resolution",
+        validator=strict_discrete_set,
+        values=["1MHz", "100kHz", "10kHz", "1kHz", "100Hz", "10Hz"]
+    )
 
-        t0 = time()
-        while True:
-            try:
-                ready = bool(self.read())
-            except VisaIOError:
-                ready = False
-
-            if ready:
-                return
-
-            if timeout != 0 and time() - t0 > timeout:
-                raise TimeoutError(
-                    "Timeout expired while waiting for the Agilent 33220A" +
-                    " to finish the triggering."
-                )
-
-            if should_stop:
-                return
-
-    trigger_source = Instrument.control(
-        "TRIG:SOUR?", "TRIG:SOUR %s",
-        """ A string property that controls the trigger source. Valid values
-        are: IMM<EDIATE> (internal), EXT<ERNAL> (rear input), BUS (via trigger
-        command). This setting can be set. """,
-        validator=string_validator,
-        values=["IMM", "IMMEDIATE", "EXT", "EXTERNAL", "BUS"],
-    )
-
-    trigger_state = Instrument.control(
-        "OUTP:TRIG?", "OUTP:TRIG %d",
-        """ A boolean property that controls whether the output is triggered
-        (True) or not (False). Can be set. """,
+    average_point = Instrument.control(
+        "AVT?", "AVT %d",
+        "Number of averages to take on each point (2-1000), or OFF",
+        validator=truncated_range_or_off,
+        values=[["OFF"], [2, 1000]]
+    )
+
+    average_sweep = Instrument.control(
+        "AVS?", "AVS %d",
+        "Number of averages to make on a sweep (2-1000) or OFF",
+        validator=truncated_range_or_off,
+        values=[["OFF"], [2, 1000]]
+    )
+
+    sampling_points = Instrument.control(
+        "MPT?", "MPT %d", "Number of sampling points",
+        validator=truncated_discrete_set,
+        values=[51, 101, 251, 501, 1001, 2001, 5001],
+        get_process=lambda v: int(v)
+    )
+
+    #####################################
+    #  Analysis Peak Search Parameters  #
+    #####################################
+
+    peak_search = Instrument.control(
+        "PKS?", "PKS %s", "Peak Search Mode",
         validator=strict_discrete_set,
-        map_values=True,
-        values={True: 1, False: 0},
+        values=["PEAK", "NEXT", "LAST", "LEFT", "RIGHT"]
     )
 
-    remote_local_state = Instrument.setting(
-        "SYST:COMM:RLST %s",
-        """ A string property that controls the remote/local state of the
-        function generator. Valid values are: LOC<AL>, REM<OTE>, RWL<OCK>.
-        This setting can only be set. """,
-        validator=string_validator,
-        values=["LOC", "LOCAL", "REM", "REMOTE", "RWL", "RWLOCK"],
-    )
-
-    def check_errors(self):
-        """ Read all errors from the instrument. """
-
-        errors = []
-        while True:
-            err = self.values("SYST:ERR?")
-            if int(err[0]) != 0:
-                errmsg = "Agilent 33220A: %s: %s" % (err[0], err[1])
-                log.error(errmsg + '\n')
-                errors.append(errmsg)
-            else:
-                break
+    dip_search = Instrument.control(
+        "DPS?", "DPS %s", "Dip Search Mode",
+        validator=strict_discrete_set,
+        values=["DIP", "NEXT", "LAST", "LEFT", "RIGHT"]
+    )
+
+    analysis = Instrument.control(
+        "ANA?", "ANA %s", "Analysis Control"
+    )
 
-        return errors
+    analysis_result = Instrument.measurement(
+        "ANAR?", "Read back anaysis result from current scan."
+    )
+
+    ##########################
+    #  Data Memory Commands  #
+    ##########################
+
+    data_memory_a_size = Instrument.measurement(
+        'DBA?',
+        "Returns the number of points sampled in data memory register A."
+    )
+
+    data_memory_b_size = Instrument.measurement(
+        'DBB?',
+        "Returns the number of points sampled in data memory register B."
+    )
+
+    data_memory_a_condition = Instrument.measurement(
+        "DCA?",
+        """Returns the data condition of data memory register A.
+        Starting wavelength, and a sampling point (l1, l2, n)."""
+    )
+
+    data_memory_b_condition = Instrument.measurement(
+        "DCB?",
+        """Returns the data condition of data memory register B.
+        Starting wavelength, and a sampling point (l1, l2, n)."""
+    )
+
+    data_memory_a_values = Instrument.measurement(
+        "DMA?",
+        "Reads the binary data from memory register A."
+    )
 
-    beeper_state = Instrument.control(
-        "SYST:BEEP:STAT?", "SYST:BEEP:STAT %d",
-        """ A boolean property that controls the state of the beeper. Can
-        be set. """,
+    data_memory_b_values = Instrument.measurement(
+        "DMA?",
+        "Reads the binary data from memory register B."
+    )
+
+    data_memory_select = Instrument.control(
+        "MSL?", "MSL %s",
+        "Memory Data Select.",
         validator=strict_discrete_set,
+        values=["A", "B"]
+    )
+
+    ###########################
+    #  Trace Marker Commands  #
+    ###########################
+
+    trace_marker_center = Instrument.setting(
+        "TMC %s", "Trace Marker at Center. Set to 1 or True to initiate command",
         map_values=True,
-        values={True: 1, False: 0},
+        values={True: ''}
+    )
+
+    trace_marker = Instrument.control(
+        "TMK?", "TMK %f",
+        "Sets the trace marker with a wavelength.  Returns the trace wavelength and power.",
+        get_process=_parse_trace_peak
     )
 
-    def beep(self):
-        """ Causes a system beep. """
-        self.write("SYST:BEEP")
+    def __init__(self, adapter, **kwargs):
+        """Constructor."""
+        self.analysis_mode = None
+        super(AnritsuMS9710C, self).__init__(adapter, "Anritsu MS9710C Optical Spectrum Analyzer", **kwargs)
+
+    @property
+    def wavelengths(self):
+        """Return a numpy array of the current wavelengths of scans."""
+        return np.linspace(
+            self.wavelength_start,
+            self.wavelength_stop,
+            self.sampling_points
+        )
+
+    def read_memory(self, slot="A"):
+        """Read the scan saved in a memory slot."""
+        cond_attr = "data_memory_{}_condition".format(slot.lower())
+        data_attr = "data_memory_{}_values".format(slot.lower())
+
+        scan = getattr(self, cond_attr)
+        wavelengths = np.linspace(scan[0], scan[1], int(scan[2]))
+        power = np.fromstring(getattr(self, data_attr), sep="\r\n")
+
+        return wavelengths, power
+
+    def wait(self, n=3, delay=1):
+        """Query OPC Command and waits for appropriate response."""
+        log.info("Wait for OPC")
+        res = self.adapter.ask("*OPC?")
+        n_attempts = n
+        while(res == ''):
+            log.debug("Empty OPC Repsonse. {} remaining".format(n_attempts))
+            if n_attempts == 0:
+                break
+            n_attempts -= 1
+            sleep(delay)
+            res = self.adapter.read().strip()
+
+        log.debug(res)
+
+    def wait_for_sweep(self, n=20, delay=0.5):
+        """Wait for a sweep to stop.
+
+        This is performed by checking bit 1 of the ESR2.
+        """
+        log.debug("Waiting for spectrum sweep")
+
+        while(self.esr2 != 3 and n > 0):
+            log.debug("Wait for sweep [{}]".format(n))
+            # log.debug("ESR2: {}".format(esr2))
+            sleep(delay)
+            n -= 1
+
+        if n <= 0:
+            log.warning("Sweep Timeout Occurred ({} s)".format(int(delay * n)))
+
+    def single_sweep(self, **kwargs):
+        """Perform a single sweep and wait for completion."""
+        log.debug("Performing a Spectrum Sweep")
+        self.clear()
+        self.write('SSI')
+        self.wait_for_sweep(**kwargs)
+
+    def center_at_peak(self, **kwargs):
+        """Center the spectrum at the measured peak."""
+        self.write("PKC")
+        self.wait(**kwargs)
+
+    def measure_peak(self):
+        """Measure the peak and return the trace marker."""
+        self.peak_search = "PEAK"
+        return self.trace_marker
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent33500.py` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent33500.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent33521A.py` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent33521A.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent34410A.py` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent34410A.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -39,11 +39,11 @@
     
     current_ac = Instrument.measurement("MEAS:CURR:AC? DEF,DEF", "AC current, in Amps")
     
     resistance = Instrument.measurement("MEAS:RES? DEF,DEF", "Resistance, in Ohms")
     
     resistance_4w = Instrument.measurement("MEAS:FRES? DEF,DEF", "Four-wires (remote sensing) resistance, in Ohms")
     
-    def __init__(self, adapter, delay=0.02, **kwargs):
+    def __init__(self, adapter, **kwargs):
         super(Agilent34410A, self).__init__(
             adapter, "HP/Agilent/Keysight 34410A Multimeter", **kwargs
         )
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent4156.py` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent4156.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -528,15 +528,15 @@
         self.check_errors()
 
     @property
     def compliance(self):
         """ This command sets the *constant* compliance value of SMU<n>. If the SMU channel is setup as a variable (VAR1, VAR2, VARD) then compliance limits are set by the variable definition.
 
         - Value: Voltage in (-200V, 200V) and current in (-1A, 1A) based
-        on :meth:`~.SMU.channel_mode`.
+          on :meth:`~.SMU.channel_mode`.
 
         .. code-block:: python
 
             instr.smu1.compliance = 0.1
         """
         if Agilent4156.analyzer_mode.fget(self) == "SWEEP":
             value = self.ask(":PAGE:MEAS:CONS:{}:COMP?".format(self.channel))
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent8257D.py` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent8257D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -73,15 +73,15 @@
     )
     start_power = Instrument.control(
         ":SOUR:POW:STAR?", ":SOUR:POW:STAR %e dBm",
         """ A floating point property that represents the start power
         in dBm. This property can be set.
         """
     )
-    start_power = Instrument.control(
+    stop_power = Instrument.control(
         ":SOUR:POW:STOP?", ":SOUR:POW:STOP %e dBm",
         """ A floating point property that represents the stop power
         in dBm. This property can be set.
         """
     )
     dwell_time = Instrument.control(
         ":SOUR:SWE:DWEL1?", ":SOUR:SWE:DWEL1 %.3f",
@@ -241,15 +241,15 @@
         which can take the values: 'sine', 'triangle', 'square', 'ramp', 'noise',
         'dual-sine', and 'swept-sine'. """,
         validator=strict_discrete_set,
         values=INTERNAL_SHAPES,
         map_values=True
     )
 
-    def __init__(self, adapter, delay=0.02, **kwargs):
+    def __init__(self, adapter, **kwargs):
         super(Agilent8257D, self).__init__(
             adapter, "Agilent 8257D RF Signal Generator", **kwargs
         )
 
     def enable(self):
         """ Enables the output of the signal. """
         self.write(":OUTPUT ON;")
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/agilent8722ES.py` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/agilent8722ES.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,18 +19,20 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 from pymeasure.instruments import Instrument, discreteTruncate, RangeException
+from pyvisa import VisaIOError
 
 import numpy as np
 import re
 from io import BytesIO
+import warnings
 
 
 class Agilent8722ES(Instrument):
     """ Represents the Agilent8722ES Vector Network Analyzer
     and provides a high-level interface for taking scans of the
     scattering parameters.
     """
@@ -53,14 +55,27 @@
     )
     sweep_time = Instrument.control(
         "SWET?", "SWET%.2e",
         """ A floating point property that represents the sweep time
         in seconds. This property can be set.
         """
     )
+    averages = Instrument.control(
+        "AVERFACT?", "AVERFACT%d",
+        """ An integer representing the number of averages to take. Note that
+        averaging must be enabled for this to take effect. This property can be set.
+        """,
+        cast=lambda x: int(float(x))  # int() doesn't like converting scientific notation values directly from strings
+    )
+    averaging_enabled = Instrument.control(
+        "AVERO?", "AVERO%d",
+        """ A bool that indicates whether or not averaging is enabled. This property
+        can be set.""",
+        cast=bool
+    )
 
     def __init__(self, resourceName, **kwargs):
         super(Agilent8722ES, self).__init__(
             resourceName,
             "Agilent 8722ES Vector Network Analyzer",
             **kwargs
         )
@@ -117,56 +132,67 @@
         if bandwidth:
             self.write("IFBW%d" % bandwidth)
         else:
             raise RangeException("Maximum IF bandwidth (6000) for Agilent "
                                  "8722ES exceeded")
 
     def set_averaging(self, averages):
-        """ Turns on averaging of a specific number between 0 and 999
-        """
-        if int(averages) > 999 or int(averages) < 0:
-            raise RangeException("Averaging must be in the range 0 to 999")
-        else:
-            self.write("AVERO1")
-            self.write("AVERFACT%d" % int(averages))
+        """Sets the number of averages and enables/disables averaging. Should be
+        between 1 and 999"""
+        averages = int(averages)
+        if not 1 <= averages <= 999:
+            assert RangeException("Set", averages, "must be in the range 1 to 999")
+        self.averages = averages
+        self.averaging_enabled = (averages > 1)
 
     def disable_averaging(self):
-        """ Disables averaging """
-        self.write("AVERO0")
+        """Disables averaging"""
+        warnings.warn("Don't use disable_averaging(), use averaging_enabled = False instead", FutureWarning)
+        self.averaging_enabled = False
+
+    def enable_averaging(self):
+        """Enables averaging"""
+        warnings.warn("Don't use enable_averaging(), use averaging_enabled = True instead", FutureWarning)
+        self.averaging_enabled = True
 
     def is_averaging(self):
         """ Returns True if averaging is enabled """
-        return self.ask("AVERO?") == '1\n'
+        warnings.warn("Don't use is_averaging(), use averaging_enabled instead", FutureWarning)
+        return self.averaging_enabled
 
     def restart_averaging(self, averages):
-        if int(averages) > 999 or int(averages) < 0:
-            raise RangeException("Averaging must be in the range 0 to 999")
-        else:
-            self.write("NUMG%d" % averages)
+        warnings.warn("Don't use restart_averaging(), use scan_single() instead", FutureWarning)
+        self.scan_single()
 
-    def scan(self, averages=1, blocking=True, timeout=25, delay=0.1):
+    def scan(self, averages=None, blocking=None, timeout=None, delay=None):
         """ Initiates a scan with the number of averages specified and
-        blocks until the operation is complete if blocking is True
+        blocks until the operation is complete.
         """
-        if averages == 1:
-            self.disableAveraging()
-            self.setSingleSweep()
-        else:
-            self.setAveraging(averages)
-            self.write("*CLS;SRE 4;ESNB 1;")
-            self.restartAveraging(averages)
-            if blocking:
-                self.adapter.wait_for_srq(timeout, delay)
-
-    def is_scan_complete():
-        pass  # TODO: Implement method for determining if the scan is completed
+        if averages is not None or blocking is not None or timeout is not None or delay is not None:
+            warnings.warn("averages, blocking, timeout, and delay arguments are no longer used by scan()", FutureWarning)
+        self.write("*CLS")
+        self.scan_single()
+        # All queries will block until the scan is done, so use NOOP? to check.
+        # These queries will time out after several seconds though, 
+        # so query repeatedly until the scan finishes.
+        while True:
+            try:
+                self.ask("NOOP?")
+            except VisaIOError as e:
+                if e.abbreviation != "VI_ERROR_TMO":
+                    raise e
+            else:
+                break
 
     def scan_single(self):
         """ Initiates a single scan """
-        self.write("SING")
+        if self.averaging_enabled:
+            self.write("NUMG%d" % self.averages)
+        else:
+            self.write("SING")
 
     def scan_continuous(self):
         """ Initiates a continuous scan """
         self.write("CONT")
 
     @property
     def frequencies(self):
@@ -175,35 +201,65 @@
         return np.linspace(
             self.start_frequency,
             self.stop_frequency,
             num=self.scan_points
         )
 
     @property
-    def data(self):
-        """ Returns the real and imaginary data from the last scan
+    def data_complex(self):
+        """ Returns the complex power from the last scan
         """
         # TODO: Implement binary transfer instead of ASCII
         data = np.loadtxt(
-            BytesIO(self.ask("FORM4;OUTPDATA")),
+            BytesIO(self.ask("FORM4;OUTPDATA").encode()),
             delimiter=',',
             dtype=np.float32
         )
-        return data[:, 0], data[:, 1]
+        data_complex = data[:, 0] + 1j * data[:, 1]
+        return data_complex
+
+    @property
+    def data_log_magnitude(self):
+        """ Returns the absolute magnitude values in dB from the last scan
+        """
+        return 20*np.log10(self.data_magnitude)
+
+    @property
+    def data_magnitude(self):
+        """ Returns the absolute magnitude values from the last scan
+        """
+        return np.abs(self.data_complex)
+
+    @property
+    def data_phase(self):
+        """ Returns the phase in degrees from the last scan
+        """
+        return np.degrees(np.angle(self.data_complex))
+    
+    @property
+    def data(self):
+        """ Returns the real and imaginary data from the last scan
+        """
+        warnings.warn("Don't use this function, use data_complex instead", FutureWarning)
+        data_complex = self.data_complex
+        return data_complex.real, data_complex.complex
 
     def log_magnitude(self, real, imaginary):
         """ Returns the magnitude in dB from a real and imaginary
         number or numpy arrays
         """
+        warnings.warn("Don't use log_magnitude(), use data_log_magnitude instead", FutureWarning)
         return 20*np.log10(self.magnitude(real, imaginary))
 
     def magnitude(self, real, imaginary):
         """ Returns the magnitude from a real and imaginary
         number or numpy arrays
         """
+        warnings.warn("Don't use magnitude(), use data_magnitude", FutureWarning)
         return np.sqrt(real**2 + imaginary**2)
 
     def phase(self, real, imaginary):
         """ Returns the phase in degrees from a real and imaginary
         number or numpy arrays
         """
+        warnings.warn("Don't use phase(), use data_phase instead", FutureWarning)
         return np.arctan2(imaginary, real)*180/np.pi
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/agilentE4408B.py` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/agilentE4408B.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/agilent/agilentE4980.py` & `PyMeasure-0.9.0/pymeasure/instruments/agilent/agilentE4980.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/ametek/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/ametek/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/ametek/ametek7270.py` & `PyMeasure-0.9.0/pymeasure/instruments/ametek/ametek7270.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/ami/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/ami/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/ami/ami430.py` & `PyMeasure-0.9.0/pymeasure/instruments/ami/ami430.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -61,15 +61,15 @@
         magnet.ramp_to_current(5)             # Ramps the current to 5 A
 
         magnet.shutdown()                     # Ramps the current to zero and disables output
 
     """
     def __init__(self, resourceName, **kwargs):
         adapter = VISAAdapter(resourceName, read_termination='\n')
-        super(ami430, self).__init__(
+        super(AMI430, self).__init__(
             adapter,
             "AMI superconducting magnet power supply.",
             includeSCPI=True,
             **kwargs
         )
         # Read twice in order to remove welcome/connect message
         self.read()
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/anritsu/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/anritsu/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/anritsu/anritsuMG3692C.py` & `PyMeasure-0.9.0/pymeasure/instruments/anritsu/anritsuMG3692C.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/comedi.py` & `PyMeasure-0.9.0/pymeasure/instruments/comedi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/danfysik/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/danfysik/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/danfysik/adapters.py` & `PyMeasure-0.9.0/pymeasure/instruments/danfysik/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/danfysik/danfysik8500.py` & `PyMeasure-0.9.0/pymeasure/instruments/danfysik/danfysik8500.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/deltaelektronika/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/deltaelektronika/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/deltaelektronika/sm7045d.py` & `PyMeasure-0.9.0/pymeasure/instruments/deltaelektronika/sm7045d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/fwbell/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/oxfordinstruments/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,8 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from .fwbell5080 import FWBell5080
+from .itc503 import ITC503
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/fwbell/fwbell5080.py` & `PyMeasure-0.9.0/pymeasure/instruments/fwbell/fwbell5080.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/hp/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/hp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/hp/hp33120A.py` & `PyMeasure-0.9.0/pymeasure/instruments/hp/hp33120A.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/hp/hp34401A.py` & `PyMeasure-0.9.0/pymeasure/instruments/hp/hp34401A.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/instrument.py` & `PyMeasure-0.9.0/pymeasure/instruments/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -314,15 +314,15 @@
 class FakeInstrument(Instrument):
     """ Provides a fake implementation of the Instrument class
     for testing purposes.
     """
 
     def __init__(self, adapter=None, name=None, includeSCPI=False, **kwargs):
         super().__init__(
-            FakeAdapter(),
+            FakeAdapter(**kwargs),
             name or "Fake Instrument",
             includeSCPI=includeSCPI,
             **kwargs
         )
 
     @staticmethod
     def control(get_command, set_command, docs,
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/keithley/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/keithley/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,7 +24,8 @@
 
 from .keithley2000 import Keithley2000
 from .keithley2400 import Keithley2400
 from .keithley2450 import Keithley2450
 from .keithley2700 import Keithley2700
 from .keithley6221 import Keithley6221
 from .keithley2750 import Keithley2750
+from .keithley6517b import Keithley6517B
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/keithley/buffer.py` & `PyMeasure-0.9.0/pymeasure/instruments/keithley/buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2000.py` & `PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2000.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2400.py` & `PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2400.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -299,14 +299,66 @@
         ":TRIG:SEQ:DEL?", ":TRIG:SEQ:DEL %g",
         """ A floating point property that controls the trigger delay
         in seconds, which can take values from 0 to 999.9999 s. """,
         validator=truncated_range,
         values=[0, 999.9999]
     )
 
+    ###########
+    # Filters #
+    ###########
+
+    filter_type = Instrument.control(
+        ":SENS:AVER:TCON?", ":SENS:AVER:TCON %s",
+        """ A String property that controls the filter's type.
+        REP : Repeating filter
+        MOV : Moving filter""",
+        validator=strict_discrete_set,
+        values=['REP', 'MOV'],
+        map_values=False)
+
+    filter_count = Instrument.control(
+        ":SENS:AVER:COUNT?", ":SENS:AVER:COUNT %d",
+        """ A integer property that controls the number of readings that are 
+        acquired and stored in the filter buffer for the averaging""",
+        validator=truncated_range,
+        values=[1, 100],
+        cast=int)
+
+    filter_state = Instrument.control(
+        ":SENS:AVER?", ":SENS:AVER %s",
+        """ A string property that controls if the filter is active.""",
+        validator=strict_discrete_set,
+        values=['ON', 'OFF'],
+        map_values=False)
+
+
+    #####################
+    # Output subsystem #
+    #####################
+
+    output_off_state = Instrument.control(
+        ":OUTP:SMOD?", ":OUTP:SMOD %s",
+        """ Select the output-off state of the SourceMeter.
+        HIMP : output relay is open, disconnects external circuitry.
+        NORM : V-Source is selected and set to 0V, Compliance is set to 0.5% 
+        full scale of the present current range.
+        ZERO : V-Source is selected and set to 0V, compliance is set to the 
+        programmed Source I value or to 0.5% full scale of the present current
+        range, whichever is greater.
+        GUAR : I-Source is selected and set to 0A""",
+        validator=strict_discrete_set,
+        values=['HIMP', 'NORM', 'ZERO', 'GUAR'],
+        map_values=False)
+
+    
+    ####################
+    # Methods        #
+    ####################
+    
     def __init__(self, adapter, **kwargs):
         super(Keithley2400, self).__init__(
             adapter, "Keithley 2400 SourceMeter", **kwargs
         )
 
     def enable_source(self):
         """ Enables the source of current or voltage depending on the
@@ -620,15 +672,15 @@
     def mean_resistance(self):
         """ Returns the mean resistance from the buffer """
         return self.means[2]
 
     @property
     def max_resistance(self):
         """ Returns the maximum resistance from the buffer """
-        return self.maximums()[2]
+        return self.maximums[2]
 
     @property
     def min_resistance(self):
         """ Returns the minimum resistance from the buffer """
         return self.minimums[2]
 
     @property
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2450.py` & `PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2450.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -119,14 +119,32 @@
         ":SOUR:CURR:RANG?", ":SOUR:CURR:RANG:AUTO 0;:SOUR:CURR:RANG %g",
         """ A floating point property that controls the source current
         range in Amps, which can take values between -1.05 and +1.05 A.
         Auto-range is disabled when this property is set. """,
         validator=truncated_range,
         values=[-1.05, 1.05]
     )
+    
+    source_current_delay = Instrument.control(
+        ":SOUR:CURR:DEL?", ":SOUR:CURR:DEL %g",
+        """ A floating point property that sets a manual delay for the source
+        after the output is turned on before a measurement is taken. When this
+        property is set, the auto delay is turned off. Valid values are
+        between 0 [seconds] and 999.9999 [seconds].""",
+        validator=truncated_range,
+        values=[0, 999.9999],
+    )
+
+    source_current_delay_auto = Instrument.control(
+        ":SOUR:CURR:DEL:AUTO?", ":SOUR:CURR:DEL:AUTO %d",
+        """ A boolean property that enables or disables auto delay. Valid
+        values are True and False. """,
+        values={True: 1, False: 0},
+        map_values=True,
+    )
 
     ###############
     # Voltage (V) #
     ###############
 
     voltage = Instrument.measurement(":READ?",
         """ Reads the voltage in Volts, if configured for this reading.
@@ -168,14 +186,32 @@
         ":SOUR:VOLT:RANG?", ":SOUR:VOLT:RANG:AUTO 0;:SOUR:VOLT:RANG %g",
         """ A floating point property that controls the source voltage
         range in Volts, which can take values from -210 to 210 V.
         Auto-range is disabled when this property is set. """,
         validator=truncated_range,
         values=[-210, 210]
     )
+    
+    source_voltage_delay = Instrument.control(
+        ":SOUR:VOLT:DEL?", ":SOUR:VOLT:DEL %g",
+        """ A floating point property that sets a manual delay for the source
+        after the output is turned on before a measurement is taken. When this
+        property is set, the auto delay is turned off. Valid values are
+        between 0 [seconds] and 999.9999 [seconds].""",
+        validator=truncated_range,
+        values=[0, 999.9999],
+    )
+
+    source_voltage_delay_auto = Instrument.control(
+        ":SOUR:VOLT:DEL:AUTO?", ":SOUR:VOLT:DEL:AUTO %d",
+        """ A boolean property that enables or disables auto delay. Valid
+        values are True and False. """,
+        values={True: 1, False: 0},
+        map_values=True,
+    )
 
     ####################
     # Resistance (Ohm) #
     ####################
 
 
     resistance = Instrument.measurement(":READ?",
@@ -239,14 +275,92 @@
 
     standard_devs = Instrument.measurement(
         ":TRACe:STATistics:STDDev?",
         """ Returns the calculated standard deviations for voltage,
         current, and resistance from the buffer data as a list. """
     )
 
+    ###########
+    # Filters #
+    ###########
+
+    current_filter_type = Instrument.control(
+        ":SENS:CURR:AVER:TCON?", ":SENS:CURR:AVER:TCON %s",
+        """ A String property that controls the filter's type for the current.
+        REP : Repeating filter
+        MOV : Moving filter""",
+        validator=strict_discrete_set,
+        values=['REP', 'MOV'],
+        map_values=False)
+
+    current_filter_count = Instrument.control(
+        ":SENS:CURR:AVER:COUNT?", ":SENS:CURR:AVER:COUNT %d",
+        """ A integer property that controls the number of readings that are 
+        acquired and stored in the filter buffer for the averaging""",
+        validator=truncated_range,
+        values=[1, 100],
+        cast=int)
+
+    current_filter_state = Instrument.control(
+        ":SENS:CURR:AVER?", ":SENS:CURR:AVER %s",
+        """ A string property that controls if the filter is active.""",
+        validator=strict_discrete_set,
+        values=['ON', 'OFF'],
+        map_values=False)
+
+    voltage_filter_type = Instrument.control(
+        ":SENS:VOLT:AVER:TCON?", ":SENS:VOLT:AVER:TCON %s",
+        """ A String property that controls the filter's type for the current.
+        REP : Repeating filter
+        MOV : Moving filter""",
+        validator=strict_discrete_set,
+        values=['REP', 'MOV'],
+        map_values=False)
+
+    voltage_filter_count = Instrument.control(
+        ":SENS:VOLT:AVER:COUNT?", ":SENS:VOLT:AVER:COUNT %d",
+        """ A integer property that controls the number of readings that are 
+        acquired and stored in the filter buffer for the averaging""",
+        validator=truncated_range,
+        values=[1, 100],
+        cast=int)
+
+    #####################
+    # Output subsystem #
+    #####################
+
+    current_output_off_state = Instrument.control(
+        ":OUTP:CURR:SMOD?", ":OUTP:CURR:SMOD %s",
+        """ Select the output-off state of the SourceMeter.
+        HIMP : output relay is open, disconnects external circuitry.
+        NORM : V-Source is selected and set to 0V, Compliance is set to 0.5% 
+        full scale of the present current range.
+        ZERO : V-Source is selected and set to 0V, compliance is set to the 
+        programmed Source I value or to 0.5% full scale of the present current
+        range, whichever is greater.
+        GUAR : I-Source is selected and set to 0A""",
+        validator=strict_discrete_set,
+        values=['HIMP', 'NORM', 'ZERO', 'GUAR'],
+        map_values=False)
+
+    voltage_output_off_state = Instrument.control(
+        ":OUTP:VOLT:SMOD?", ":OUTP:VOLT:SMOD %s",
+        """ Select the output-off state of the SourceMeter.
+        HIMP : output relay is open, disconnects external circuitry.
+        NORM : V-Source is selected and set to 0V, Compliance is set to 0.5% 
+        full scale of the present current range.
+        ZERO : V-Source is selected and set to 0V, compliance is set to the 
+        programmed Source I value or to 0.5% full scale of the present current
+        range, whichever is greater.
+        GUAR : I-Source is selected and set to 0A""",
+        validator=strict_discrete_set,
+        values=['HIMP', 'NORM', 'ZERO', 'GUAR'],
+        map_values=False)
+
+
     ####################
     # Methods        #
     ####################
 
     def __init__(self, adapter, **kwargs):
         super(Keithley2450, self).__init__(
             adapter, "Keithley 2450 SourceMeter", **kwargs
@@ -498,15 +612,15 @@
     def mean_resistance(self):
         """ Returns the mean resistance from the buffer """
         return self.means[2]
 
     @property
     def max_resistance(self):
         """ Returns the maximum resistance from the buffer """
-        return self.maximums()[2]
+        return self.maximums[2]
 
     @property
     def min_resistance(self):
         """ Returns the minimum resistance from the buffer """
         return self.minimums[2]
 
     @property
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2700.py` & `PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2700.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -167,49 +167,50 @@
                 connected to the DMM backplane (input and sense respectively).
                 """
                 channels = range(1, 51)
             else:
                 log.warning(
                     "Card type %s at slot %s is not yet implemented." % (card, slot)
                 )
+                continue
 
             channels = [100 * slot + ch for ch in channels]
 
             self.CLIST_VALUES.extend(channels)
 
     def close_rows_to_columns(self, rows, columns, slot=None):
         """ Closes (connects) the channels between column(s) and row(s)
         of the 7709 connection matrix.
-        Only one of the parameters `rows' or 'columns' can be "all"
+        Only one of the parameters 'rows' or 'columns' can be "all"
 
         :param rows: row number or list of numbers; can also be "all"
         :param columns: column number or list of numbers; can also be "all"
         :param slot: slot number (1 or 2) of the 7709 card to be used
         """
 
         channels = self.channels_from_rows_columns(rows, columns, slot)
         self.closed_channels = channels
 
     def open_rows_to_columns(self, rows, columns, slot=None):
         """ Opens (disconnects) the channels between column(s) and row(s)
         of the 7709 connection matrix.
-        Only one of the parameters `rows' or 'columns' can be "all"
+        Only one of the parameters 'rows' or 'columns' can be "all"
 
         :param rows: row number or list of numbers; can also be "all"
         :param columns: column number or list of numbers; can also be "all"
         :param slot: slot number (1 or 2) of the 7709 card to be used
         """
 
         channels = self.channels_from_rows_columns(rows, columns, slot)
         self.open_channels = channels
 
     def channels_from_rows_columns(self, rows, columns, slot=None):
         """ Determine the channel numbers between column(s) and row(s) of the
         7709 connection matrix. Returns a list of channel numbers.
-        Only one of the parameters `rows' or 'columns' can be "all"
+        Only one of the parameters 'rows' or 'columns' can be "all"
 
         :param rows: row number or list of numbers; can also be "all"
         :param columns: column number or list of numbers; can also be "all"
         :param slot: slot number (1 or 2) of the 7709 card to be used
 
         """
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley2750.py` & `PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley2750.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/keithley/keithley6221.py` & `PyMeasure-0.9.0/pymeasure/instruments/keithley/keithley6221.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/keysight/keysightN5767A.py` & `PyMeasure-0.9.0/pymeasure/instruments/keysight/keysightN5767A.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/lakeshore/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/lakeshore/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/lakeshore/adapters.py` & `PyMeasure-0.9.0/pymeasure/instruments/lakeshore/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/lakeshore/lakeshore331.py` & `PyMeasure-0.9.0/pymeasure/instruments/lakeshore/lakeshore331.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/lakeshore/lakeshore425.py` & `PyMeasure-0.9.0/pymeasure/instruments/lakeshore/lakeshore425.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/mock.py` & `PyMeasure-0.9.0/pymeasure/instruments/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/newport/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/newport/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/newport/esp300.py` & `PyMeasure-0.9.0/pymeasure/instruments/newport/esp300.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/ni/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/ni/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/ni/daqmx.py` & `PyMeasure-0.9.0/pymeasure/instruments/ni/daqmx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/ni/nidaq.py` & `PyMeasure-0.9.0/pymeasure/instruments/ni/nidaq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/ni/virtualbench.py` & `PyMeasure-0.9.0/pymeasure/instruments/ni/virtualbench.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 # pyvirtualbench library: Copyright (c) 2015 Charles Armstrap <charles@armstrap.org>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
@@ -32,27 +32,27 @@
                     c_int64, c_uint64, c_wchar, c_wchar_p, Structure, c_int,
                     cdll, byref)
 from datetime import datetime, timezone, timedelta
 import numpy as np
 import pandas as pd
 
 from pymeasure.instruments import Instrument, RangeException
-from pymeasure.instruments.validators import (strict_discrete_set,
-                                              truncated_discrete_set,
-                                              strict_range)
+from pymeasure.instruments.validators import (
+    strict_discrete_set, strict_discrete_range,
+    truncated_discrete_set, strict_range
+)
 
 log = logging.getLogger(__name__)
 log.addHandler(logging.NullHandler())
 
 try:
     # Requires 'pyvirtualbench' package:
     # https://github.com/armstrap/armstrap-pyvirtualbench
     import pyvirtualbench as pyvb
 except ModuleNotFoundError as err:
-    # catch here for logging
     log.info('Failed loading the pyvirtualbench package. '
              + 'Check the NI VirtualBench documentation on how to '
              + 'install this external dependency. '
              + 'ImportError: {}'.format(err))
     raise
 
 
@@ -97,15 +97,16 @@
           for pymeasure yet
         - Inter Integrated Circuit (I2C) -> not implemented for pymeasure yet
 
     For every module exist methods to save/load the configuration to file.
     These methods are not wrapped so far, checkout the pyvirtualbench file.
 
     All calibration methods and classes are not wrapped so far, since these
-    are not required on a very regular basis.
+    are not required on a very regular basis. Also the connections via network
+    are not yet implemented.
     Check the pyvirtualbench file, if you need the functionality.
 
     :param str device_name: Full unique device name
     :param str name: Name for display in pymeasure
     """
 
     def __init__(self, device_name='', name='VirtualBench'):
@@ -200,55 +201,14 @@
         :type names_in: str
         :return: Channel string with all channels separated by comma,
                  number of channels
         :rtype: (str, int)
         """
         return self.vb.expand_channel_string(names_in)
 
-    """
-    Wrappers not implented yet:
-    -   Handling Network Device
-    -   Setting Calibration Information
-
-    def add_network_device(self, ip_or_hostname, timeout_in_ms):
-        ''' Adds a networked device to the system.
-        '''
-
-    def remove_device(self, device_name = ''):
-        ''' Removes a device from the system. The device must not be connected
-            via USB to be removed.
-        '''
-
-    def login(self, device_name = '', username = 'admin', password = ''):
-        ''' Attempts to log in to a networked device. Logging in to
-        a device grants access to the permissions set for the
-        specified user in NI Web-Based Monitoring and Configuration.
-        '''
-
-    def logout(self, device_name = ''):
-        ''' Logs out of a networked device that you are logged in to.
-        Logging out of a device revokes access to the permissions set
-        for the specified user in NI Web-Based Monitoring and
-        Configuration.
-        '''
-
-    def set_calibration_information(self, calibration_date,
-                                    calibration_interval, device_name = '',
-                                    password = ''):
-        ''' Sets calibration information for the specified device.
-        '''
-
-    def set_calibration_password(self, current_password, new_password,
-                                 device_name = ''):
-        ''' Sets a new calibration password for the specified device. This
-            method requires the current password for the device, and returns an
-            error if the specified password is incorrect.
-        '''
-    """
-
     def get_calibration_information(self):
         """ Returns calibration information for the specified device,
         including the last calibration date and calibration interval.
 
         :return: Calibration date, recommended calibration interval in months,
                  calibration interval in months
         :rtype: (pyvb.Timestamp, int, int)
@@ -261,15 +221,16 @@
 
         :param lines: Lines to acquire, reading is possible on all lines
         :type lines: str
         :param reset: Reset DIO module, defaults to False
         :type reset: bool, optional
         """
         reset = strict_discrete_set(reset, [True, False])
-        self.dio = self.DigitalInputOutput(self.vb, lines, reset, vb_name=self.name)
+        self.dio = self.DigitalInputOutput(self.vb, lines, reset,
+                                           vb_name=self.name)
 
     def acquire_power_supply(self, reset=False):
         """ Establishes communication with the PS module. This method should be
         called once per session.
 
         :param reset: Reset the PS module, defaults to False
         :type reset: bool, optional
@@ -291,27 +252,68 @@
         """ Establishes communication with the MSO module. This method should
         be called once per session.
 
         :param reset: Reset the MSO module, defaults to False
         :type reset: bool, optional
         """
         reset = strict_discrete_set(reset, [True, False])
-        self.mso = self.MixedSignalOscilloscope(self.vb, reset, vb_name=self.name)
+        self.mso = self.MixedSignalOscilloscope(self.vb, reset,
+                                                vb_name=self.name)
 
     def acquire_digital_multimeter(self, reset=False):
         """ Establishes communication with the DMM module. This method should
         be called once per session.
 
         :param reset: Reset the DMM module, defaults to False
         :type reset: bool, optional
         """
         reset = strict_discrete_set(reset, [True, False])
-        self.dmm = self.DigitalMultimeter(self.vb, reset=reset, vb_name=self.name)
+        self.dmm = self.DigitalMultimeter(self.vb, reset=reset,
+                                          vb_name=self.name)
+
+    class VirtualBenchInstrument():
+        def __init__(self, acquire_instr, reset,
+                     instr_identifier, vb_name=''):
+            """Initialize instrument of VirtualBench device.
+            Sets class variables and provides basic methods
+            common to all VB instruments.
+
+            :param acquire_instr: Method to acquire the instrument
+            :type acquire_instr: method
+            :param reset: Resets the instrument
+            :type reset: bool
+            :param instr_identifier: Shorthand identifier, e.g. mso or fgen
+            :type instr_identifier: str
+            :param vb_name: Name of VB device for logging, defaults to ''
+            :type vb_name: str, optional
+            """
+            # Parameters & Handle of VirtualBench Instance
+            self._vb_handle = acquire_instr.__self__
+            self._device_name = self._vb_handle.device_name
+            self.name = (vb_name + " " + instr_identifier.upper()).strip()
+            log.info("Initializing %s." % self.name)
+            self._instrument_handle = acquire_instr(self._device_name, reset)
+            self.isShutdown = False
+
+        def __del__(self):
+            """ Ensures the connection is closed upon deletion
+            """
+            if self.isShutdown is not True:
+                self._instrument_handle.release()
+
+        def shutdown(self):
+            ''' Removes the session and deallocates any resources acquired
+            during the session. If output is enabled on any channels, they
+            remain in their current state.
+            '''
+            log.info("Shutting down %s" % self.name)
+            self._instrument_handle.release()
+            self.isShutdown = True
 
-    class DigitalInputOutput():
+    class DigitalInputOutput(VirtualBenchInstrument):
         """ Represents Digital Input Output (DIO) Module of Virtual Bench
         device. Allows to read/write digital channels and/or set channels
         to export the start signal of FGEN module or trigger of MSO module.
         """
         def __init__(self, virtualbench, lines, reset, vb_name=''):
             """ Acquire DIO module
 
@@ -330,35 +332,22 @@
             # store line names & numbers for future reference
             (self._line_names, self._line_numbers) = self.validate_lines(
                 lines, return_single_lines=True, validate_init=False)
             # Create DIO Instance
             log.info("Initializing %s." % self.name)
             self.dio = self._vb_handle.acquire_digital_input_output(
                 self._line_names, reset)
+            # for methods provided by super class
+            self._instrument_handle = self.dio
             self.isShutdown = False
 
-        def __del__(self):
-            """ Ensures the connection is closed upon deletion
-            """
-            if self.isShutdown is not True:
-                self.dio.release()
-
-        def shutdown(self):
-            ''' Stops the session and deallocates any resources acquired during
-                the session. If output is enabled on any channels, they remain
-                in their current state and continue to output data.
-            '''
-            log.info("Shutting down %s" % self.name)
-            self.dio.release()
-            self.isShutdown = True
-
         def validate_lines(self, lines, return_single_lines=False,
                            validate_init=False):
-            """ Validate lines string
-                Allowed patterns (case sensitive):
+            """Validate lines string
+            Allowed patterns (case sensitive):
 
                 - ``'VBxxxx-xxxxxxx/dig/0:7'``
                 - ``'VBxxxx-xxxxxxx/dig/0'``
                 - ``'dig/0'``
                 - ``'VBxxxx-xxxxxxx/trig'``
                 - ``'trig'``
 
@@ -388,15 +377,17 @@
             for line in lines:
                 if line == 'trig':
                     device = self._device_name
                 # otherwise (device_name/)dig/line or device_name/trig
                 else:
                     # split off line number by last '/'
                     try:
-                        (device, line) = re.match(r'(.*)(?:/)(.+)', line).groups()
+                        (device, line) = re.match(
+                            r'(.*)(?:/)(.+)',
+                            line).groups()
                     except IndexError:
                         error()
                 if (line == 'trig') and (device == self._device_name):
                     single_lines.append('trig')
                     return_lines.append(self._device_name + '/' + line)
                 elif int(line) in range(0, 8):
                     line = int(line)
@@ -509,49 +500,31 @@
 
         def reset_instrument(self):
             ''' Resets the session configuration to default values, and
             resets the device and driver software to a known state.
             '''
             self.dio.reset_instrument()
 
-    class DigitalMultimeter():
+    class DigitalMultimeter(VirtualBenchInstrument):
         """ Represents Digital Multimeter (DMM) Module of Virtual Bench
         device. Allows to measure either DC/AC voltage or current,
         Resistance or Diodes.
         """
         def __init__(self, virtualbench, reset, vb_name=''):
             """ Acquire DMM module
 
             :param virtualbench: Instance of the VirtualBench class
             :type virtualbench: VirtualBench
             :param reset: Resets the instrument
             :type reset: bool
             """
-            # Parameters & Handle of VirtualBench Instance
-            self._device_name = virtualbench.device_name
-            self._vb_handle = virtualbench
-            self.name = vb_name + " DMM"
-            log.info("Initializing %s." % self.name)
-            self.dmm = self._vb_handle.acquire_digital_multimeter(
-                self._device_name, reset)
-            self.isShutdown = False
-
-        def __del__(self):
-            """ Ensures the connection is closed upon deletion
-            """
-            if self.isShutdown is not True:
-                self.dmm.release()
-
-        def shutdown(self):
-            """ Stops the DMM session and deallocates any resources
-            acquired during the session.
-            """
-            log.info("Shutting down %s" % self.name)
-            self.dmm.release()
-            self.isShutdown = True
+            super().__init__(
+                virtualbench.acquire_digital_multimeter,
+                reset, 'dmm', vb_name)
+            self.dmm = self._instrument_handle
 
         @staticmethod
         def validate_range(dmm_function, range):
             """ Checks if ``range`` is valid for the chosen ``dmm_function``
 
             :param int dmm_function: DMM Function
             :param range: Range value, e.g. maximum value to measure
@@ -584,15 +557,15 @@
             :return: DMM function index to pass to the instrument
             :rtype: int
             """
             try:
                 pyvb.DmmFunction(dmm_function)
             except Exception:
                 try:
-                    dmm_function = pyvb.DmmFunction[dmm_function.Upper()]
+                    dmm_function = pyvb.DmmFunction[dmm_function.upper()]
                 except Exception:
                     raise ValueError(
                         "DMM Function may be 0-5, 'DC_VOLTS'," +
                         " 'AC_VOLTS', 'DC_CURRENT', 'AC_CURRENT'," +
                         " 'RESISTANCE' or 'DIODE'")
             return dmm_function
 
@@ -608,15 +581,15 @@
             :rtype: int
             """
             try:
                 pyvb.DmmCurrentTerminal(auto_range_terminal)
             except Exception:
                 try:
                     auto_range_terminal = pyvb.DmmCurrentTerminal[
-                        auto_range_terminal.Upper()]
+                        auto_range_terminal.upper()]
                 except Exception:
                     raise ValueError(
                         "Current Auto Range Terminal may be 0, 1," +
                         " 'LOW' or 'HIGH'")
             return auto_range_terminal
 
         def configure_measurement(self, dmm_function, auto_range=True,
@@ -649,15 +622,15 @@
             :type dmm_input_resistance: int or str
             """
             try:
                 pyvb.DmmInputResistance(dmm_input_resistance)
             except Exception:
                 try:
                     dmm_input_resistance = pyvb.DmmInputResistance[
-                        dmm_input_resistance.Upper()]
+                        dmm_input_resistance.upper()]
                 except Exception:
                     raise ValueError(
                         "Input Resistance may be 0, 1," +
                         " 'TEN_MEGA_OHM' or 'TEN_GIGA_OHM'")
             self.dmm.configure_dc_voltage(dmm_input_resistance)
 
         def configure_dc_current(self, auto_range_terminal):
@@ -712,56 +685,37 @@
             self.dmm.read()
 
         def reset_instrument(self):
             """ Reset the DMM module to defaults
             """
             self.dmm.reset_instrument()
 
-    class FunctionGenerator():
+    class FunctionGenerator(VirtualBenchInstrument):
         """ Represents Function Generator (FGEN) Module of Virtual
         Bench device.
         """
         def __init__(self, virtualbench, reset, vb_name=''):
             """ Acquire FGEN module
 
             :param virtualbench: Instance of the VirtualBench class
             :type virtualbench: VirtualBench
             :param reset: Resets the instrument
             :type reset: bool
             """
-            # Parameters & Handle of VirtualBench Instance
-            self._device_name = virtualbench.device_name
-            self._vb_handle = virtualbench
-            self.name = vb_name + " FGEN"
-            log.info("Initializing %s." % self.name)
-            self.fgen = self._vb_handle.acquire_function_generator(
-                self._device_name, reset)
+            super().__init__(
+                virtualbench.acquire_function_generator,
+                reset, 'fgen', vb_name)
+            self.fgen = self._instrument_handle
 
             self._waveform_functions = {"SINE": 0, "SQUARE": 1,
                                         "TRIANGLE/RAMP": 2, "DC": 3}
             # self._waveform_functions_index = {
             # v: k for k, v in self._waveform_functions.items()}
             self._max_frequency = {"SINE": 20000000, "SQUARE": 5000000,
                                    "TRIANGLE/RAMP": 1000000, "DC": 20000000}
-            self.isShutdown = False
-
-        def __del__(self):
-            """ Ensures the connection is closed upon deletion
-            """
-            if self.isShutdown is not True:
-                self.fgen.release()
-
-        def shutdown(self):
-            ''' Stops the session and deallocates any resources acquired during
-            the session. If output is enabled on any channels, they remain
-            in their current state and continue to output data.
-            '''
-            log.info("Shutting down %s" % self.name)
-            self.fgen.release()
-            self.isShutdown = True
 
         def configure_standard_waveform(self, waveform_function, amplitude,
                                         dc_offset, frequency, duty_cycle):
             """ Configures the instrument to output a standard waveform.
             Check instrument manual for maximum ratings which depend on load.
 
             :param waveform_function: Waveform function (``"SINE", "SQUARE",
@@ -777,58 +731,52 @@
             :type duty_cycle: int
             """
             waveform_function = strict_discrete_set(
                 waveform_function.upper(), self._waveform_functions)
             max_frequency = self._max_frequency[waveform_function.upper()]
             waveform_function = self._waveform_functions[
                 waveform_function.upper()]
-            amplitude = strict_range(
-                amplitude, [x/100 for x in range(0, 2401)])
-            dc_offset = strict_range(
-                dc_offset, [x/100 for x in range(-1201, 1201)])
+            amplitude = strict_range(amplitude, (0, 24))
+            dc_offset = strict_range(dc_offset, (-12, 12))
             if (amplitude/2 + abs(dc_offset)) > 12:
                 raise ValueError(
                     "Amplitude and DC Offset may not exceed +/-12V")
-            duty_cycle = strict_range(duty_cycle, range(0, 101))
-            frequency = strict_range(
-                frequency, [x/1000 for x in range(0, max_frequency*1000 + 1)])
+            duty_cycle = strict_range(duty_cycle, (0, 100))
+            frequency = strict_range(frequency, (0, max_frequency))
             self.fgen.configure_standard_waveform(
                 waveform_function, amplitude, dc_offset, frequency, duty_cycle)
 
         def configure_arbitrary_waveform(self, waveform, sample_period):
             """ Configures the instrument to output a waveform. The waveform is
             output either after the end of the current waveform if output
             is enabled, or immediately after output is enabled.
 
             :param waveform: Waveform as list of values
             :type waveform: list
             :param sample_period: Time between two waveform points
                                   (maximum of 125MS/s, which equals 80ns)
             :type sample_period: float
             """
-            strict_range(len(waveform), range(1, 1000001))  # 1MS
-            if not ((sample_period >= 8e-8) and (sample_period <= 1)):
-                raise ValueError(
-                    "Sample Period allows a maximum of 125MS/s (80ns)")
+            strict_range(len(waveform), (1, 1e6))  # 1MS
+            sample_period = strict_range(sample_period, (8e-8, 1))
             self.fgen.configure_arbitrary_waveform(waveform, sample_period)
 
         def configure_arbitrary_waveform_gain_and_offset(self, gain,
                                                          dc_offset):
             """ Configures the instrument to output an arbitrary waveform with
             a specified gain and offset value. The waveform is output either
             after the end of the current waveform if output is enabled, or
             immediately after output is enabled.
 
             :param gain: Gain, multiplier of waveform values
             :type gain: float
             :param dc_offset: DC offset in volts
             :type dc_offset: float
             """
-            dc_offset = strict_range(
-                dc_offset, [x/100 for x in range(-1201, 1201)])
+            dc_offset = strict_range(dc_offset, (-12, 12))
             self.fgen.configure_arbitrary_waveform_gain_and_offset(
                 gain, dc_offset)
 
         @property
         def filter(self):
             ''' Enables or disables the filter on the instrument.
 
@@ -837,25 +785,14 @@
             return self.fgen.query_filter
 
         @filter.setter
         def filter(self, enable_filter):
             enable_filter = strict_discrete_set(enable_filter, [True, False])
             self.fgen.enable_filter(enable_filter)
 
-        # def enable_filter(self, enable_filter):
-        #     ''' Enables or disables the filter on the instrument.
-        #     '''
-        #     enable_filter = strict_discrete_set(enable_filter,[True,False])
-        #     self.fgen.enable_filter(enable_filter)
-
-        # def query_filter(self):
-        #     ''' Indicates whether the filter is enabled on the instrument.
-        #     '''
-        #     self.fgen.query_filter()
-
         def query_waveform_mode(self):
             """ Indicates whether the waveform output by the instrument is a
             standard or arbitrary waveform.
 
             :return: Waveform mode
             :rtype: enum
             """
@@ -918,50 +855,53 @@
 
         def reset_instrument(self):
             ''' Resets the session configuration to default values, and resets
             the device and driver software to a known state.
             '''
             self.fgen.reset_instrument()
 
-    class MixedSignalOscilloscope():
+    class MixedSignalOscilloscope(VirtualBenchInstrument):
         """ Represents Mixed Signal Oscilloscope (MSO) Module of Virtual Bench
         device. Allows to measure oscilloscope data from analog and digital
         channels.
+
+        Methods from pyvirtualbench not implemented in pymeasure yet:
+
+            - ``enable_digital_channels``
+            - ``configure_digital_threshold``
+            - ``configure_advanced_digital_timing``
+            - ``configure_state_mode``
+            - ``configure_digital_edge_trigger``
+            - ``configure_digital_pattern_trigger``
+            - ``configure_digital_glitch_trigger``
+            - ``configure_digital_pulse_width_trigger``
+            - ``query_digital_channel``
+            - ``query_enabled_digital_channels``
+            - ``query_digital_threshold``
+            - ``query_advanced_digital_timing``
+            - ``query_state_mode``
+            - ``query_digital_edge_trigger``
+            - ``query_digital_pattern_trigger``
+            - ``query_digital_glitch_trigger``
+            - ``query_digital_pulse_width_trigger``
+            - ``read_digital_u64``
         """
+
         def __init__(self, virtualbench, reset, vb_name=''):
-            """ Acquire FGEN module
+            """ Acquire MSO module
 
             :param virtualbench: Instance of the VirtualBench class
             :type virtualbench: VirtualBench
             :param reset: Resets the instrument
             :type reset: bool
             """
-            # Parameters & Handle of VirtualBench Instance
-            self._device_name = virtualbench.device_name
-            self._vb_handle = virtualbench
-            self.name = vb_name + " MSO"
-            log.info("Initializing %s." % self.name)
-            self.mso = self._vb_handle.acquire_mixed_signal_oscilloscope(
-                self._device_name, reset)
-            self.isShutdown = False
-
-        def __del__(self):
-            """ Ensures the connection is closed upon deletion
-            """
-            if self.isShutdown is not True:
-                self.mso.release()
-
-        def shutdown(self):
-            ''' Removes the session and deallocates any resources acquired
-            during the session. If output is enabled on any channels, they
-            remain in their current state.
-            '''
-            log.info("Shutting down %s" % self.name)
-            self.mso.release()
-            self.isShutdown = True
+            super().__init__(
+                virtualbench.acquire_mixed_signal_oscilloscope,
+                reset, 'mso', vb_name)
+            self.mso = self._instrument_handle
 
         @staticmethod
         def validate_trigger_instance(trigger_instance):
             """ Check if ``trigger_instance`` is a valid choice
 
             :param trigger_instance: Trigger instance (``'A'`` or ``'B'``)
             :type trigger_instance: int or str
@@ -969,25 +909,20 @@
             :rtype: int
             """
             try:
                 pyvb.MsoTriggerInstance(trigger_instance)
             except Exception:
                 try:
                     trigger_instance = pyvb.MsoTriggerInstance[
-                        trigger_instance.Upper()]
+                        trigger_instance.upper()]
                 except Exception:
                     raise ValueError(
                         "Trigger Instance may be 0, 1, 'A' or 'B'")
             return trigger_instance
 
-        def auto_setup(self):
-            """ Automatically configure the instrument
-            """
-            self.mso.auto_setup()
-
         def validate_channel(self, channel):
             """ Check if ``channel`` is a correct specification
 
             :param str channel: Channel string
             :return: Channel string
             :rtype: str
             """
@@ -1021,57 +956,69 @@
                     if not device == self._device_name:
                         error()
                 # constructing line references for output
                 return_value.append('mso/' + channel)
 
             return_value = ', '.join(return_value)
             return_value = self._vb_handle.collapse_channel_string(
-                return_value)
+                return_value)[0]  # drop number of channels
             return return_value
 
+        # --------------------------
+        # Configure Instrument
+        # --------------------------
+
+        def auto_setup(self):
+            """ Automatically configure the instrument
+            """
+            self.mso.auto_setup()
+
         def configure_analog_channel(self, channel, enable_channel,
                                      vertical_range, vertical_offset,
                                      probe_attenuation, vertical_coupling):
             """ Configure analog measurement channel
 
             :param str channel: Channel string
             :param bool enable_channel: Enable/Disable channel
-            :param float vertical_range: Vertical measurement range (0V - 20V)
+            :param float vertical_range: Vertical measurement range (0V - 20V),
+                the instrument discretizes to these ranges:
+                ``[20, 10, 5, 2, 1, 0.5, 0.2, 0.1, 0.05]``
+                which are 5x the values shown in the native UI.
             :param float vertical_offset: Vertical offset to correct for
                                           (inverted compared to VB native UI,
-                                          -20V - +20V)
+                                          -20V - +20V, resolution 0.1mV)
             :param probe_attenuation: Probe attenuation (``'ATTENUATION_10X'``
                                       or ``'ATTENUATION_1X'``)
             :type probe_attenuation: int or str
             :param vertical_coupling: Vertical coupling (``'AC'`` or ``'DC'``)
             :type vertical_coupling: int or str
             """
             channel = self.validate_channel(channel)
             enable_channel = strict_discrete_set(
                 enable_channel, [True, False])
-            if (vertical_range < 0) or (vertical_range > 20):
-                raise ValueError("Vertical Range takes value 0 to 20V")
-            if (vertical_offset < -20) or (vertical_offset > 20):
-                raise ValueError("Vertical Offset takes value -20 to +20V")
+            vertical_range = strict_range(vertical_range, (0, 20))
+            vertical_offset = strict_discrete_range(
+                vertical_offset, [-20, 20], 1e-4
+            )
             try:
                 pyvb.MsoProbeAttenuation(probe_attenuation)
             except Exception:
                 try:
                     probe_attenuation = pyvb.MsoProbeAttenuation[
-                        probe_attenuation.Upper()]
+                        probe_attenuation.upper()]
                 except Exception:
                     raise ValueError(
                         "Probe Attenuation may be 1, 10," +
                         " 'ATTENUATION_10X' or 'ATTENUATION_1X'")
             try:
                 pyvb.MsoCoupling(vertical_coupling)
             except Exception:
                 try:
                     vertical_coupling = pyvb.MsoCoupling[
-                        vertical_coupling.Upper()]
+                        vertical_coupling.upper()]
                 except Exception:
                     raise ValueError(
                         "Probe Attenuation may be 0, 1, 'AC' or 'DC'")
 
             self.mso.configure_analog_channel(
                 channel, enable_channel, vertical_range, vertical_offset,
                 probe_attenuation, vertical_coupling)
@@ -1089,77 +1036,52 @@
             """
             channel = self.validate_channel(channel)
             try:
                 pyvb.MsoInputImpedance(input_impedance)
             except Exception:
                 try:
                     input_impedance = pyvb.MsoInputImpedance[
-                        input_impedance.Upper()]
+                        input_impedance.upper()]
                 except Exception:
                     raise ValueError(
                         "Probe Attenuation may be 0, 1," +
                         " 'ONE_MEGA_OHM' or 'FIFTY_OHMS'")
             bandwidth_limit = strict_discrete_set(
                 bandwidth_limit, [100000000, 20000000])  # 100 Mhz or 20Mhz
             self.mso.configure_analog_channel_characteristics(
                 channel, input_impedance, bandwidth_limit)
 
-        # def enable_digital_channels(self, channel, enable_channel):
-        #     ''' Enables or disables the specified digital channels.
-        #     '''
-
-        # def configure_digital_threshold(self, threshold):
-        #     ''' Configures the threshold level for logic analyzer lines.
-        #     '''
-
         def configure_timing(self, sample_rate, acquisition_time,
                              pretrigger_time, sampling_mode):
             """ Configure timing settings of the MSO
 
-            :param int sample_rate: Sample rate (15.26kS - 1MS)
+            :param int sample_rate: Sample rate (15.26kS - 1GS)
             :param float acquisition_time: Acquisition time (1ns - 68.711s)
             :param float pretrigger_time: Pretrigger time (0s - 10s)
             :param sampling_mode: Sampling mode (``'SAMPLE'`` or
                                   ``'PEAK_DETECT'``)
             """
-            sample_rate = strict_range(sample_rate, range(15260, 1000000001))
-            if not ((acquisition_time >= 1e-09) and
-                    (acquisition_time <= 68.711)):
-                raise ValueError(
-                    "Acquisition Time must be between 1ns and 68.7s")
+            sample_rate = strict_range(sample_rate, (15260, 1e9))
+            acquisition_time = strict_discrete_range(
+                acquisition_time, (1e-09, 68.711), 1e-09)
             # acquisition is also limited by buffer size,
             # which depends on sample rate as well as acquisition time
-            if not ((pretrigger_time >= 0) and (pretrigger_time <= 10)):
-                raise ValueError("Pretrigger Time must be between 1ns and 10s")
+            pretrigger_time = strict_range(pretrigger_time, (0, 10))
             try:
                 pyvb.MsoSamplingMode(sampling_mode)
             except Exception:
                 try:
-                    sampling_mode = pyvb.MsoSamplingMode[sampling_mode.Upper()]
+                    sampling_mode = pyvb.MsoSamplingMode[sampling_mode.upper()]
                 except Exception:
                     raise ValueError(
                         "Sampling Mode may be 0, 1, 'SAMPLE' or 'PEAK_DETECT'")
 
             self.mso.configure_timing(
                 sample_rate, acquisition_time, pretrigger_time, sampling_mode)
 
-        # def configure_advanced_digital_timing(self,
-        #   digital_sample_rate_control,
-        #   digital_sample_rate, buffer_control, buffer_pretrigger_percent):
-        #     ''' Configures the rate and buffer settings of the logic
-        #     analyzer.
-        #         This method allows for more advanced configuration options
-        #     than MSO Configure Timing.
-        #     '''
-
-        # def configure_state_mode(self, enable, clock_channel, clock_edge):
-        #     ''' Configures how to clock data on the logic analyzer channels
-        #         that are enabled.
-        #     '''
-
         def configure_immediate_trigger(self):
             """ Configures a trigger to immediately activate on the specified
             channels after the pretrigger time has expired.
             """
             self.mso.configure_immediate_trigger()
 
         def configure_analog_edge_trigger(self, trigger_source, trigger_slope,
@@ -1178,52 +1100,24 @@
             :type trigger_instance: int or str
             """
             trigger_source = self.validate_channel(trigger_source)
             try:
                 pyvb.EdgeWithEither(trigger_slope)
             except Exception:
                 try:
-                    trigger_slope = pyvb.EdgeWithEither[trigger_slope.Upper()]
+                    trigger_slope = pyvb.EdgeWithEither[trigger_slope.upper()]
                 except Exception:
                     raise ValueError(
                         "Trigger Slope may be 0, 1, 2, 'RISING'," +
                         " 'FALLING' or 'EITHER'")
             trigger_instance = self.validate_trigger_instance(trigger_instance)
             self.mso.configure_analog_edge_trigger(
                 trigger_source, trigger_slope, trigger_level,
                 trigger_hysteresis, trigger_instance)
 
-        # def configure_digital_edge_trigger(self, trigger_source,
-        #   trigger_slope, trigger_instance):
-        #     ''' Configures a trigger to activate on the specified source when
-        #         the digital edge reaches the specified levels.
-        #     '''
-
-        # def configure_digital_pattern_trigger(self, trigger_source,
-        #   trigger_pattern, trigger_instance):
-        #     ''' Configures a trigger to activate on the specified channels
-        #         when
-        #         a digital pattern is matched. A trigger is produced when
-        #         every
-        #         level (high/low) requirement specified in Trigger Pattern is
-        #         met, and when at least one toggling (toggle/fall/rise)
-        #         requirement is met. If no toggling requirements are set, then
-        #         only the level requirements must be met to produce a trigger.
-        #     '''
-
-        # def configure_digital_glitch_trigger(self, trigger_source,
-        #   trigger_instance):
-        #     ''' Configures a trigger to activate on the specified channels
-        #         when
-        #         a digital glitch occurs. A glitch occurs when a channel in
-        #         Trigger Source toggles between two edges of the sample clock,
-        #         but has the same state for both samples. This may happen when
-        #         the sampling rate is less than 1 GHz.
-        #     '''
-
         def configure_analog_pulse_width_trigger(self, trigger_source,
                                                  trigger_polarity,
                                                  trigger_level,
                                                  comparison_mode, lower_limit,
                                                  upper_limit,
                                                  trigger_instance):
             """ Configures a trigger to activate on the specified source when
@@ -1248,46 +1142,36 @@
             """
             trigger_source = self.validate_channel(trigger_source)
             try:
                 pyvb.MsoTriggerPolarity(trigger_polarity)
             except Exception:
                 try:
                     trigger_polarity = pyvb.MsoTriggerPolarity[
-                        trigger_polarity.Upper()]
+                        trigger_polarity.upper()]
                 except Exception:
                     raise ValueError(
                         "Comparison Mode may be 0, 1, 2, 3," +
                         " 'GREATER_THAN_UPPER_LIMIT'," +
                         " 'LESS_THAN_LOWER_LIMIT'," +
                         " 'INSIDE_LIMITS' or 'OUTSIDE_LIMITS'")
             try:
                 pyvb.MsoComparisonMode(comparison_mode)
             except Exception:
                 try:
                     comparison_mode = pyvb.MsoComparisonMode[
-                        comparison_mode.Upper()]
+                        comparison_mode.upper()]
                 except Exception:
                     raise ValueError(
                         "Trigger Polarity may be 0, 1," +
                         " 'POSITIVE' or 'NEGATIVE'")
             trigger_instance = self.validate_trigger_instance(trigger_instance)
             self.mso.configure_analog_pulse_width_trigger(
                 trigger_source, trigger_polarity, trigger_level,
                 comparison_mode, lower_limit, upper_limit, trigger_instance)
 
-        def configure_digital_pulse_width_trigger(self, trigger_source,
-                                                  trigger_polarity,
-                                                  comparison_mode,
-                                                  lower_limit, upper_limit,
-                                                  trigger_instance):
-            ''' Configures a trigger to activate on the specified source when
-            the digital edge reaches the specified levels within a specified
-            window of time.
-            '''
-
         def configure_trigger_delay(self, trigger_delay):
             """ Configures the amount of time to wait after a trigger condition
             is met before triggering.
 
                 :param float trigger_delay: Trigger delay (0s - 17.1799s)
             """
             self.mso.configure_trigger_delay(trigger_delay)
@@ -1317,27 +1201,14 @@
             applied to the channel.
 
                 :return: Input impedance, bandwidth limit
                 :rtype: (enum, float)
             """
             return self.mso.query_analog_channel_characteristics(channel)
 
-        # def query_digital_channel(self):
-        #     ''' Indicates whether the specified digital channel is enabled.
-        #     '''
-
-        # def query_enabled_digital_channels(self):
-        #     ''' No documentation
-        #     '''
-
-        # def query_digital_threshold(self):
-        #     ''' Indicates the threshold configuration of the logic analyzer
-        #         channels.
-        #     '''
-
         def query_timing(self):
             """ Indicates the timing configuration of the MSO.
             Call directly before measurement to read the actual timing
             configuration and write it to the corresponding class variables.
             Necessary to interpret the measurement data, since it contains no
             time information.
 
@@ -1347,22 +1218,14 @@
             """
             (self.sample_rate, self.acquisition_time,
              self.pretrigger_time,
              self.sampling_mode) = self.mso.query_timing()
             return (self.sample_rate, self.acquisition_time,
                     self.pretrigger_time, self.sampling_mode)
 
-        # def query_advanced_digital_timing(self):
-        #     ''' Indicates the buffer configuration of the logic analyzer.
-        #     '''
-
-        # def query_state_mode(self, clockChannelSize):
-        #     ''' Indicates the clock configuration of the logic analyzer.
-        #     '''
-
         def query_trigger_type(self, trigger_instance):
             """ Indicates the trigger type of the specified instance.
 
             :param trigger_instance: Trigger instance (``'A'`` or ``'B'``)
             :return: Trigger type
             :rtype: str
             """
@@ -1375,37 +1238,14 @@
             :return: Trigger source, trigger slope, trigger level, trigger
                      hysteresis
             :rtype: (str, enum, float, float)
             """
             trigger_instance = self.validate_trigger_instance(trigger_instance)
             return self.mso.query_analog_edge_trigger(trigger_instance)
 
-        # def query_digital_edge_trigger(self, trigger_instance):
-        #     ''' Indicates the digital trigger configuration of the specified
-        #         instance.
-        #     '''
-
-        # def query_digital_pattern_trigger(self, trigger_instance):
-        #     ''' Indicates the digital pattern trigger configuration of the
-        #         specified instance. A trigger is produced when every level
-        #         (high/low) requirement specified in Trigger Pattern is met,
-        #         and
-        #         when at least one toggling (toggle/fall/rise) requirement is
-        #         met. If no toggling requirements are set, then only the level
-        #         requirements must be met to produce a trigger.
-        #     '''
-
-        # def query_digital_glitch_trigger(self, trigger_instance):
-        #     ''' Indicates the digital glitch trigger configuration of the
-        #         specified instance. A glitch occurs when a channel in Trigger
-        #         Source toggles between two edges of the sample clock. This
-        #         may
-        #         happen when the sampling rate is less than 1 GHz.
-        #     '''
-
         def query_trigger_delay(self):
             """ Indicates the trigger delay setting of the MSO.
 
             :return: Trigger delay
             :rtype: float
             """
             return self.mso.query_trigger_delay()
@@ -1417,24 +1257,23 @@
             :return: Trigger source, trigger polarity, trigger level,
                      comparison mode, lower limit, upper limit
             :rtype: (str, enum, float, enum, float, float)
             """
             trigger_instance = self.validate_trigger_instance(trigger_instance)
             return self.mso.query_analog_pulse_width_trigger(trigger_instance)
 
-        # def query_digital_pulse_width_trigger(self, trigger_instance):
-        #     ''' Indicates the digital pulse width trigger configuration of
-        #         the specified instance.
-        #     '''
-
         def query_acquisition_status(self):
             """ Returns the status of a completed or ongoing acquisition.
             """
             return self.mso.query_acquisition_status()
 
+        # --------------------------
+        # Measurement Control
+        # --------------------------
+
         def run(self, autoTrigger=True):
             """ Transitions the acquisition from the Stopped state to the
             Running state. If the current state is Triggered, the
             acquisition is first transitioned to the Stopped state before
             transitioning to the Running state. This method returns an
             error if too much power is applied to any enabled channel.
 
@@ -1450,35 +1289,14 @@
 
         def stop(self):
             """ Transitions the acquisition from either the Triggered or
             Running state to the Stopped state.
             """
             self.mso.stop()
 
-        # def read_analog(self, data_size):
-        #     ''' Transfers data from the instrument as long as the acquisition
-        #     state is Acquisition Complete. If the state is either Running or
-        #     Triggered, this method will wait until the state transitions to
-        #     Acquisition Complete. If the state is Stopped, this method
-        #     returns an error.
-        #     '''
-        #     #return (data.value, data_stride.value, initial_timestamp,
-        #              trigger_timestamp,
-        #              MsoTriggerReason(trigger_reason.value))
-
-        # def read_digital_u64(self, data_size, sample_timestamps_size):
-        #     ''' Transfers data from the instrument as long as the acquisition
-        #         state is Acquisition Complete. If the state is either
-        #         Running or
-        #         Triggered, this method will wait until the state transitions
-        #         to
-        #         Acquisition Complete. If the state is Stopped, this method
-        #         returns an error.
-        #     '''
-
         def read_analog_digital_u64(self):
             """ Transfers data from the instrument as long as the acquisition
             state is Acquisition Complete. If the state is either Running or
             Triggered, this method will wait until the state transitions to
             Acquisition Complete. If the state is Stopped, this method
             returns an error.
 
@@ -1497,94 +1315,63 @@
 
             :return: Dataframe with time and measurement data
             :rtype: pd.DataFrame
             """
             (analog_data_out, analog_data_stride
              # , analog_t0, digital_data_out, digital_timestamps_out,
              # digital_t0, trigger_timestamp, trigger_reason
-             ) = self.read_analog_digital_u64()[0:1]
+             ) = self.read_analog_digital_u64()[0:2]
 
             number_of_samples = int(self.sample_rate *
                                     self.acquisition_time) + 1
             if not number_of_samples == (len(analog_data_out) /
                                          analog_data_stride):
                 # try updating timing parameters
                 self.query_timing()
                 number_of_samples = int(self.sample_rate *
                                         self.acquisition_time) + 1
                 if not number_of_samples == (len(analog_data_out) /
                                              analog_data_stride):
                     raise ValueError(
                         "Length of Analog Data does not match" +
                         " Timing Parameters")
+
             pretrigger_samples = int(self.sample_rate * self.pretrigger_time)
             times = (
                 list(range(-pretrigger_samples, 0))
-                + list(range(0, number_of_samples - pretrigger_samples + 1)))
+                + list(range(0, number_of_samples - pretrigger_samples)))
             times = [list(map(lambda x: x*1/self.sample_rate, times))]
 
             np_array = np.array(analog_data_out)
             np_array = np.split(np_array, analog_data_stride)
             np_array = np.append(np.array(times), np_array, axis=0)
             np_array = np.transpose(np_array)
             return pd.DataFrame(data=np_array)
 
         def reset_instrument(self):
             """ Resets the session configuration to default values, and resets
             the device and driver software to a known state.
             """
             self.mso.reset()
 
-        # def export_configuration(self, configuration_filename):
-        #     ''' Exports a configuration file for use with the MSO.
-        #     '''
-
-        # def import_configuration(self, configuration_filename):
-        #     ''' Imports a configuration file for use with the MSO. You can
-        #         import PNG files exported from the VirtualBench Application
-        #         or
-        #         files created from MSO Export Configuration.
-        #     '''
-
-    class PowerSupply():
+    class PowerSupply(VirtualBenchInstrument):
         """ Represents Power Supply (PS) Module of Virtual Bench device
         """
         def __init__(self, virtualbench, reset, vb_name=''):
             """ Acquire PS module
 
             :param virtualbench: Instance of the VirtualBench class
             :type virtualbench: VirtualBench
             :param reset: Resets the instrument
             :type reset: bool
             """
-            # Parameters & Handle of VirtualBench Instance
-            self._device_name = virtualbench.device_name
-            self._vb_handle = virtualbench
-            self.name = vb_name + " PS"
-            # Create DIO Instance
-            reset = strict_discrete_set(reset, [True, False])
-            log.info("Initializing %s." % self.name)
-            self.ps = self._vb_handle.acquire_power_supply(
-                self._device_name, reset)
-            self.isShutdown = False
-
-        def __del__(self):
-            """ Ensures the connection is closed upon deletion
-            """
-            if self.isShutdown is not True:
-                self.ps.release()
-
-        def shutdown(self):
-            ''' Stops the session and deallocates any resources acquired during
-            the session. If output is enabled on any channels, they remain
-            in their current state and continue to output data.
-            '''
-            log.info("Releasing %s" % self.name)
-            self.ps.release()
-            self.isShutdown = True
+            super().__init__(
+                virtualbench.acquire_power_supply,
+                reset, 'ps', vb_name)
+            self.ps = self._instrument_handle
 
         def validate_channel(self, channel, current=False, voltage=False):
             """ Check if channel string is valid and if output current/voltage
             are within the output ranges of the channel
 
             :param channel: Channel string (``"ps/+6V","ps/+25V","ps/-25V"``)
             :type channel: str
@@ -1598,25 +1385,23 @@
             if current is False and voltage is False:
                 return strict_discrete_set(
                     channel, ["ps/+6V", "ps/+25V", "ps/-25V"])
             else:
                 channel = strict_discrete_set(
                     channel, ["ps/+6V", "ps/+25V", "ps/-25V"])
                 if channel == "ps/+6V":
-                    current_range = range(0, 1001)
-                    voltage_range = range(0, 6001)
+                    current_range = (0, 1)
+                    voltage_range = (0, 6)
                 else:
-                    current_range = range(0, 501)
-                    voltage_range = range(0, 25001)
+                    current_range = (0, 5)
+                    voltage_range = (0, 25)
                     if channel == "ps/-25V":
-                        voltage_range = map(lambda x: -x, voltage_range)
-                current_range = map(lambda x: x/1000, current_range)
-                voltage_range = map(lambda x: x/1000, voltage_range)
-                current = strict_range(current, current_range)
-                voltage = strict_range(voltage, voltage_range)
+                        voltage_range = (0, -25)
+                current = strict_discrete_range(current, current_range, 1e-3)
+                voltage = strict_discrete_range(voltage, voltage_range, 1e-3)
                 return (channel, current, voltage)
 
         def configure_voltage_output(self, channel, voltage_level,
                                      current_limit):
             ''' Configures a voltage output on the specified channel. This
             method should be called once for every channel you want to
             configure to output voltage.
@@ -1661,27 +1446,14 @@
         @outputs_enabled.setter
         def outputs_enabled(self, enable_outputs):
             enable_outputs = strict_discrete_set(
                 enable_outputs, [True, False])
             log.info("%s Output %s." % (self.name, enable_outputs))
             self.ps.enable_all_outputs(enable_outputs)
 
-        # def enable_all_outputs(self, enable_outputs):
-        #     ''' Enables or disables all outputs on all channels of the
-        #         instrument.
-        #     '''
-        #     enable_outputs = strict_discrete_set(
-        #       enable_outputs, [True,False])
-        #     self.ps.enable_all_outputs(enable_outputs)
-
-        # def query_outputs_enabled(self):
-        #     ''' Indicates whether the outputs are enabled for the instrument.
-        #     '''
-        #     self.ps.query_outputs_enabled()
-
         @property
         def tracking(self):
             ''' Enables or disables tracking between the positive and negative
             25V channels. If enabled, any configuration change on the
             positive 25V channel is mirrored to the negative 25V channel,
             and any writes to the negative 25V channel are ignored.
 
@@ -1691,31 +1463,14 @@
 
         @tracking.setter
         def tracking(self, enable_tracking):
             enable_tracking = strict_discrete_set(
                 enable_tracking, [True, False])
             self.ps.enable_tracking(enable_tracking)
 
-        # def query_tracking(self):
-        #     ''' Indicates whether voltage tracking is enabled on
-        #       the instrument.
-        #     '''
-        #     self.ps.query_tracking()
-
-        # def enable_tracking(self, enable_tracking):
-        #     ''' Enables or disables tracking between the positive and
-        #           negative
-        #         25V channels. If enabled, any configuration change on the
-        #         positive 25V channel is mirrored to the negative 25V channel,
-        #         and any writes to the negative 25V channel are ignored.
-        #     '''
-        #     enable_tracking = strict_discrete_set(
-        #       enable_tracking,[True,False])
-        #     self.ps.enable_tracking(enable_tracking)
-
         def read_output(self, channel):
             ''' Reads the voltage and current levels and outout mode of the
             specified channel.
             '''
             channel = self.validate_channel(channel)
             return self.ps.read_output()
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/oxfordinstruments/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/signalrecovery/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,8 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from .itc503 import ITC503
+from .dsp7265 import DSP7265
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/oxfordinstruments/itc503.py` & `PyMeasure-0.9.0/pymeasure/instruments/oxfordinstruments/itc503.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,22 +18,29 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
+
+import logging
 from time import sleep, time
 import numpy
 
 from pymeasure.instruments import Instrument
 from pymeasure.instruments.validators import strict_discrete_set, \
     truncated_range, strict_range
 
 
+# Setup logging
+log = logging.getLogger(__name__)
+log.addHandler(logging.NullHandler())
+
+
 class ITC503(Instrument):
     """Represents the Oxford Intelligent Temperature Controller 503.
 
     .. code-block:: python
 
         itc = ITC503("GPIB::24")        # Default channel for the ITC503
 
@@ -43,14 +50,15 @@
 
         print(itc.temperature_setpoint) # Print the current set-point
         itc.temperature_setpoint = 300  # Change the set-point to 300 K
         itc.wait_for_temperature()      # Wait for the temperature to stabilize
         print(itc.temperature_1)        # Print the temperature at sensor 1
 
     """
+    _T_RANGE = [0, 301]
 
     control_mode = Instrument.control(
         "X", "$C%d",
         """ A string property that sets the ITC in LOCAL or REMOTE and LOCKES,
         or UNLOCKES, the LOC/REM button. Allowed values are:
         LL: LOCAL & LOCKED
         RL: REMOTE & LOCKED
@@ -72,14 +80,34 @@
         AUTO: HEATER AUTO, GAS AUTO. """,
         get_process=lambda v: int(v[3:4]),
         validator=strict_discrete_set,
         values={"MANUAL": 0, "AM": 1, "MA": 2, "AUTO": 3},
         map_values=True,
     )
 
+    heater = Instrument.control(
+        "R5", "$O%f",
+        """ A floating point property that sets the required heater output when
+        in manual mode. The parameter is expressed as a percentage of the
+        maximum voltage. Valid values are in range 0 [off] to 99.9 [%]. """,
+        get_process=lambda v: float(v[1:]),
+        validator=truncated_range,
+        values=[0, 99.9]
+    )
+
+    gasflow = Instrument.control(
+        "R7", "$G%f",
+        """ A floating point property that controls gas flow when in manual
+        mode. The value is expressed as a percentage of the maximum gas flow.
+        Valid values are in range 0 [off] to 99.9 [%]. """,
+        get_process=lambda v: float(v[1:]),
+        validator=truncated_range,
+        values=[0, 99.9]
+    )
+
     auto_pid = Instrument.control(
         "X", "$L%d",
         """ A boolean property that sets the Auto-PID mode on (True) or off (False).
         """,
         get_process=lambda v: int(v[12:13]),
         validator=strict_discrete_set,
         values={True: 1, False: 0},
@@ -100,15 +128,15 @@
 
     temperature_setpoint = Instrument.control(
         "R0", "$T%f",
         """ A floating point property that controls the temperature set-point of
         the ITC in kelvin. """,
         get_process=lambda v: float(v[1:]),
         validator=truncated_range,
-        values=[0, 301]
+        values=_T_RANGE
     )
 
     temperature_1 = Instrument.measurement(
         "R1",
         """ Reads the temperature of the sensor 1 in Kelvin. """,
         get_process=lambda v: float(v[1:]),
     )
@@ -159,32 +187,37 @@
         "r", "$s%f",
         """ A property that sets values in the sweep table. Relies on the
         xpointer and ypointer to point at the location in the table that
         is to be set. """,
         get_process=lambda v: float(v[1:]),
     )
 
-    def __init__(self, resourceName, clear_buffer=True, **kwargs):
+    def __init__(self, resourceName, clear_buffer=True,
+                 max_temperature=301, min_temperature=0, **kwargs):
         super(ITC503, self).__init__(
             resourceName,
             "Oxford ITC503",
             includeSCPI=False,
             send_end=True,
             read_termination="\r",
             **kwargs
         )
 
         # Clear the buffer in order to prevent communication problems
         if clear_buffer:
             self.adapter.connection.clear()
 
+        self._T_RANGE[0] = min_temperature
+        self._T_RANGE[1] = max_temperature
+
     def wait_for_temperature(self, error=0.01, timeout=3600,
                              check_interval=0.5, stability_interval=10,
                              thermalize_interval=300,
-                             should_stop=lambda: False):
+                             should_stop=lambda: False,
+                             max_comm_errors=None):
         """
         Wait for the ITC to reach the set-point temperature.
 
         :param error: The maximum error in Kelvin under which the temperature
                       is considered at set-point
         :param timeout: The maximum time the waiting is allowed to take. If
                         timeout is exceeded, a TimeoutError is raised. If
@@ -192,38 +225,55 @@
         :param check_interval: The time between temperature queries to the ITC.
         :param stability_interval: The time over which the temperature_error is
                                    to be below error to be considered stable.
         :param thermalize_interval: The time to wait after stabilizing for the
                                     system to thermalize.
         :param should_stop: Optional function (returning a bool) to allow the
                             waiting to be stopped before its end.
+        :param max_comm_errors: The maximum number of communication errors that
+                                are allowed before the wait is stopped. if set
+                                to None (default), no maximum will be used.
         """
 
         number_of_intervals = int(stability_interval / check_interval)
         stable_intervals = 0
         attempt = 0
+        comm_errors = 0
 
         t0 = time()
         while True:
-
-            if abs(self.temperature_error) < error:
-                stable_intervals += 1
+            try:
+                temp_error = self.temperature_error
+            except ValueError:
+                comm_errors += 1
+                log.error(
+                    "No temperature-error returned. "
+                    "Communication error # %d." % comm_errors
+                )
             else:
-                stable_intervals = 0
-                attempt += 1
+                if abs(temp_error) < error:
+                    stable_intervals += 1
+                else:
+                    stable_intervals = 0
+                    attempt += 1
 
             if stable_intervals >= number_of_intervals:
                 break
 
-            if timeout >= 0 and (time() - t0) > timeout:
+            if timeout > 0 and (time() - t0) > timeout:
                 raise TimeoutError(
                     "Timeout expired while waiting for the Oxford ITC305 to \
                     reach the set-point temperature"
                 )
 
+            if max_comm_errors is not None and comm_errors > max_comm_errors:
+                raise ValueError(
+                    "Too many communication errors have occurred."
+                )
+
             if should_stop():
                 return
 
             sleep(check_interval)
 
         if attempt == 0:
             return
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/parker/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/attocube/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,8 +18,9 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from .parkerGV6 import ParkerGV6
+from .adapters import AttocubeConsoleAdapter
+from .anc300 import ANC300Controller
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/parker/parkerGV6.py` & `PyMeasure-0.9.0/pymeasure/instruments/parker/parkerGV6.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/resources.py` & `PyMeasure-0.9.0/pymeasure/instruments/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,15 +18,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-import visa
+import pyvisa
 
 
 def list_resources():
     """
     Prints the available resources, and returns a list of VISA resource names
     
     .. code-block:: python
@@ -34,27 +34,27 @@
         resources = list_resources()
         #prints (e.g.)
             #0 : GPIB0::22::INSTR : Agilent Technologies,34410A,******
             #1 : GPIB0::26::INSTR : Keithley Instruments Inc., Model 2612, *****
         dmm = Agilent34410(resources[0])
     
     """
-    rm = visa.ResourceManager()
+    rm = pyvisa.ResourceManager()
     instrs = rm.list_resources()
     for n, instr in enumerate(instrs):
         # trying to catch errors in comunication
         try:
             res = rm.open_resource(instr)
             # try to avoid errors from *idn?
             try:
                 # noinspection PyUnresolvedReferences
                 idn = res.ask('*idn?')[:-1]
-            except visa.Error:
+            except pyvisa.Error:
                 idn = "Not known"
             finally:
                 res.close()
                 print(n, ":", instr, ":", idn)
-        except visa.VisaIOError as e:
+        except pyvisa.VisaIOError as e:
             print(n, ":", instr, ":", "Visa IO Error: check connections")
             print(e)
     rm.close()
     return instrs
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/signalrecovery/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/yokogawa/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,8 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from .dsp7265 import DSP7265
+from .yokogawa7651 import Yokogawa7651
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/signalrecovery/dsp7265.py` & `PyMeasure-0.9.0/pymeasure/instruments/signalrecovery/dsp7265.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/srs/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/srs/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,7 +20,8 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 from .sr830 import SR830
 from .sg380 import SG380
+from .sr860 import SR860
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/srs/sg380.py` & `PyMeasure-0.9.0/pymeasure/instruments/srs/sg380.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/srs/sr830.py` & `PyMeasure-0.9.0/pymeasure/instruments/srs/sr830.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -349,20 +349,24 @@
         """
         return int(self.ask("LIAS?2")) == 1
 
     def quick_range(self):
         """ While the magnitude is out of range, increase
         the sensitivity by one setting
         """
+        self.write('LIAE 2,1')
         while self.is_out_of_range():
             self.write("SENS%d" % (int(self.ask("SENS?"))+1))
             time.sleep(5.0*self.time_constant)
             self.write("*CLS")
         # Set the range as low as possible
-        self.sensitivity(1.15*abs(self.R))
+        newsensitivity = 1.15*abs(self.magnitude)
+        if self.input_config in('I (1 MOhm)','I (100 MOhm)'):
+            newsensitivity = newsensitivity*1e6
+        self.sensitivity = newsensitivity
 
     @property
     def buffer_count(self):
         query = self.ask("SPTS?")
         if query.count("\n") > 1:
             return int(re.match(r"\d+\n$", query, re.MULTILINE).group(0))
         else:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/tektronix/__init__.py` & `PyMeasure-0.9.0/pymeasure/instruments/tektronix/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/tektronix/afg3152c.py` & `PyMeasure-0.9.0/pymeasure/instruments/tektronix/afg3152c.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/tektronix/tds2000.py` & `PyMeasure-0.9.0/pymeasure/instruments/tektronix/tds2000.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/thorlabs/__init__.py` & `PyMeasure-0.9.0/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-#
-# This file is part of the PyMeasure package.
-#
-# Copyright (c) 2013-2020 PyMeasure Developers
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-# THE SOFTWARE.
-#
+Copyright (c) 2013-2021 PyMeasure Developers
 
-from .thorlabspm100usb import ThorlabsPM100USB
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/thorlabs/thorlabspm100usb.py` & `PyMeasure-0.9.0/pymeasure/instruments/thorlabs/thorlabspm100usb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/validators.py` & `PyMeasure-0.9.0/pymeasure/instruments/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/yokogawa/__init__.py` & `PyMeasure-0.9.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,8 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from .yokogawa7651 import Yokogawa7651
+import pytest
```

### Comparing `PyMeasure-0.8.0/pymeasure/instruments/yokogawa/yokogawa7651.py` & `PyMeasure-0.9.0/pymeasure/instruments/yokogawa/yokogawa7651.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -156,29 +156,29 @@
         self.write("O1;E")
 
     def disable_source(self):
         """ Disables the source of current or voltage depending on the
         configuration of the instrument. """
         self.write("O0;E")
 
-    def apply_current(self, max_current=1e-3, complinance_voltage=1):
+    def apply_current(self, max_current=1e-3, compliance_voltage=1):
         """ Configures the instrument to apply a source current, which can
         take optional parameters that defer to the :attr:`~.Yokogawa7651.source_current_range`
         and :attr:`~.Yokogawa7651.compliance_voltage` properties. """
         self.source_mode = 'current'
         self.source_current_range = max_current
-        self.complinance_voltage = complinance_voltage
+        self.compliance_voltage = compliance_voltage
 
-    def apply_voltage(self, max_voltage=1, complinance_current=10e-3):
+    def apply_voltage(self, max_voltage=1, compliance_current=10e-3):
         """ Configures the instrument to apply a source voltage, which can
         take optional parameters that defer to the :attr:`~.Yokogawa7651.source_voltage_range`
         and :attr:`~.Yokogawa7651.compliance_current` properties. """
         self.source_mode = 'voltage'
         self.source_voltage_range = max_voltage
-        self.complinance_current = compliance_current
+        self.compliance_current = compliance_current
 
     def ramp_to_current(self, current, steps=25, duration=0.5):
         """ Ramps the current to a value in Amps by traversing a linear spacing
         of current steps over a duration, defined in seconds.
 
         :param steps: A number of linear steps to traverse
         :param duration: A time in seconds over which to ramp
```

### Comparing `PyMeasure-0.8.0/pymeasure/log.py` & `PyMeasure-0.9.0/pymeasure/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -95,15 +95,15 @@
     if file_kwargs is None:
         file_kwargs = {}
 
     logger.handlers = []
     if console:
         console_log(logger, level=getattr(logging, console_level))
         logger.info('Set up console logging')
-    if filename is not filename:
+    if filename is not None:
         file_log(logger, filename, level=getattr(logging, file_level), **file_kwargs)
         logger.info('Set up file logging')
 
     scribe = Scribe(queue)
     return scribe
```

### Comparing `PyMeasure-0.8.0/pymeasure/process.py` & `PyMeasure-0.9.0/pymeasure/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/pymeasure/thread.py` & `PyMeasure-0.9.0/pymeasure/thread.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,27 +21,45 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 import logging
 
 from threading import Thread, Event
+from time import time
 
 log = logging.getLogger(__name__)
 log.addHandler(logging.NullHandler())
 
 
+class InterruptableEvent(Event):
+    """
+    This subclass solves the problem indicated in bug
+    https://bugs.python.org/issue35935 that prevents the
+    wait of an Event to be interrupted by a KeyboardInterrupt.
+    """
+
+    def wait(self, timeout=None):
+        if timeout is None:
+            while not super().wait(0.1):
+                pass
+        else:
+            timeout_start = time()
+            while not super().wait(0.1) and time() <= timeout_start + timeout:
+                pass
+
+
 class StoppableThread(Thread):
     """ Base class for Threads which require the ability
     to be stopped by a thread-safe method call
     """
 
     def __init__(self):
         super().__init__()
-        self._should_stop = Event()
+        self._should_stop = InterruptableEvent()
         self._should_stop.clear()
 
     def join(self, timeout=0):
         """ Joins the current thread and forces it to stop after
         the timeout if necessary
 
         :param timeout: Timeout duration in seconds
```

### Comparing `PyMeasure-0.8.0/setup.py` & `PyMeasure-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -23,20 +23,20 @@
 #
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='PyMeasure',
-    version='0.8.0',
+    version='0.9.0',
     author='PyMeasure Developers',
     packages=find_packages(),
     scripts=[],
-    url='https://github.com/ralph-group/pymeasure',
-    download_url='https://github.com/ralph-group/pymeasure/tarball/v0.8.0',
+    url='https://github.com/pymeasure/pymeasure',
+    download_url='https://github.com/pymeasure/pymeasure/tarball/v0.9.0',
     license='MIT License',
     description='Scientific measurement library for instruments, experiments, and live-plotting',
     long_description=open('README.rst').read() + "\n\n" + open('CHANGES.txt').read(),
     install_requires=[
         "numpy >= 1.6.1",
         "pandas >= 0.14",
         "pyvisa >= 1.8",
@@ -52,26 +52,27 @@
         'python-vxi11': ['python-vxi11 >= 0.9']
     },
     setup_requires=[
         'pytest-runner'
     ],
     tests_require=[
         'pytest >= 2.9.1',
-        'pytest-qt >= 2.4.0'
+        'pytest-qt >= 2.4.0',
+        'pyvisa-sim >= 0.4.0',
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering",
     ],
     keywords="measure instrument experiment control automate graph plot"
 )
```

### Comparing `PyMeasure-0.8.0/tests/adapters/test_adapter.py` & `PyMeasure-0.9.0/tests/test_thread.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,22 +18,22 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-import logging
+from pymeasure.thread import StoppableThread
 
-from pymeasure.adapters import FakeAdapter
 
-log = logging.getLogger(__name__)
-log.addHandler(logging.NullHandler())
+def test_thread_stopping():
+    t = StoppableThread()
+    t.start()
+    t.stop()
+    assert t.should_stop() is True
+    t.join()
 
-
-def test_adapter_values():
-    a = FakeAdapter()
-    assert a.values("5,6,7") == [5, 6, 7]
-    assert a.values("5,6,7", cast=str) == ['5', '6', '7']
-    assert a.values("X,Y,Z") == ['X', 'Y', 'Z']
-    assert a.values("X,Y,Z", cast=str) == ['X', 'Y', 'Z']
-    assert a.values("X.Y.Z", separator='.') == ['X', 'Y', 'Z']
+def test_thread_joining():
+    t = StoppableThread()
+    t.start()
+    t.join()
+    assert t.should_stop() is True
```

### Comparing `PyMeasure-0.8.0/tests/adapters/test_visa.py` & `PyMeasure-0.9.0/tests/experiment/test_listeners.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,11 +18,23 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from pymeasure.adapters import VISAAdapter
+import time
+from queue import Queue
 
-def test_visa_version():
-  assert VISAAdapter.has_supported_version()
+from pymeasure.experiment.listeners import Listener, Recorder
+from pymeasure.experiment.results import Results
+
+# TODO: Make results_for_testing.csv
+# TODO: Make procedure_for_testing.py
+
+"""
+def test_recorder_stop():
+    q = Queue()
+    d = Results.load('results_for_testing.csv')
+    r = Recorder(d, q)
+    r.
+"""
```

### Comparing `PyMeasure-0.8.0/tests/conftest.py` & `PyMeasure-0.9.0/pymeasure/instruments/anapico/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,8 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-import pytest
+from .apsin12G import APSIN12G
```

### Comparing `PyMeasure-0.8.0/tests/display/test_inputs.py` & `PyMeasure-0.9.0/tests/display/test_inputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -27,24 +27,34 @@
 
 from pymeasure.display.Qt import QtGui, QtCore
 from pymeasure.display.inputs import ScientificInput, BooleanInput, ListInput
 from pymeasure.experiment.parameters import BooleanParameter, ListParameter, FloatParameter
 
 @pytest.mark.parametrize("default_value", [True, False])
 class TestBooleanInput:
-    def test_init_from_param(self, qtbot, default_value):
+    @pytest.mark.parametrize("value_remains_default", [True, False])
+    def test_init_from_param(self, qtbot, default_value, value_remains_default):
         # set up BooleanInput
         bool_param = BooleanParameter('potato', default=default_value)
+
+        if (value_remains_default):
+            # Enable check that the value is initialized to default_value
+            check_value = default_value
+        else:
+            # Set to a non default value
+            bool_param.value = not default_value
+            # Enable check that the value is changed after initialization to a non default value
+            check_value = not default_value
+
         bool_input = BooleanInput(bool_param)
         qtbot.addWidget(bool_input)
 
         # test
         assert bool_input.text() == bool_param.name
-        assert bool_input.value() == default_value
-
+        assert bool_input.value() == check_value
 
     def test_setValue_should_update_value(self, qtbot, default_value):
 
         # set up BooleanInput
         bool_param = BooleanParameter('potato', default=default_value)
         bool_input = BooleanInput(bool_param)
         qtbot.addWidget(bool_input)
@@ -57,14 +67,18 @@
         # set up BooleanInput
         bool_param = BooleanParameter('potato', default=default_value)
 
         with mock.patch('test_inputs.BooleanParameter.value',
                 new_callable=mock.PropertyMock,
                 return_value=default_value) as p:
             bool_input = BooleanInput(bool_param)
+
+            # Clear any call to property 'value' during initialization
+            p.reset_mock()
+
             qtbot.addWidget(bool_input)
             bool_input.show()
 
             # TODO: fix: fails to toggle on Windows
             #qtbot.mouseClick(bool_input, QtCore.Qt.LeftButton)
             bool_input.setValue(not default_value)
 
@@ -75,24 +89,35 @@
 
 class TestListInput:
     @pytest.mark.parametrize("choices,default_value", [
         (["abc", "def", "ghi"], "abc"), # strings
         ([123, 456, 789], 123), # numbers
         (["abc", "def", "ghi"], "def") # default not first value
     ])
-    def test_init_from_param(self, qtbot, choices, default_value):
+    @pytest.mark.parametrize("value_remains_default", [True, False])
+    def test_init_from_param(self, qtbot, choices, default_value, value_remains_default):
         list_param = ListParameter('potato',
                 choices=choices,
                 default=default_value,
                 units='m')
+
+        if (value_remains_default):
+            # Enable check that the value is initialized to default_value
+            check_value = default_value
+        else:
+            # Set to a non default value
+            list_param.value = choices[2]
+            # Enable check that the value is changed after initialization to a non default_value
+            check_value = choices[2]
+
         list_input = ListInput(list_param)
         qtbot.addWidget(list_input)
 
         assert list_input.isEditable() == False
-        assert list_input.value() == default_value
+        assert list_input.value() == check_value
 
     def test_setValue_should_update_value(self, qtbot):
         # Test write-read loop: verify value -> index -> value conversion
         choices = [123, 'abc', 0]
         list_param = ListParameter('potato', choices=choices, default=123)
         list_input = ListInput(list_param)
         qtbot.addWidget(list_input)
@@ -132,28 +157,41 @@
         with pytest.raises(ValueError):
             list_input.setValue(789)
 
 class TestScientificInput:
     @pytest.mark.parametrize("min_,max_,default_value", [
         [0, 20, 12],
         [0, 1000, 200], # regression #118: default above default max 99.99
-        [-1000, 1000, -10] # regression #118: default below default min 0
+        [-1000, 1000, -10], # regression #118: default below default min 0
+        [0.004, 5.5, 3.3],  # minimum #225: 0 < minimum < 0.005
+        [0, 0.01, 0.002]  # default #233: default <0.01 changes to 0
     ])
-    def test_init_from_param(self, qtbot, min_, max_, default_value):
+    @pytest.mark.parametrize("value_remains_default", [True, False])
+    def test_init_from_param(self, qtbot, min_, max_, default_value, value_remains_default):
         float_param = FloatParameter('potato',
                 minimum=min_,
                 maximum=max_,
                 default=default_value,
                 units='m')
+
+        if (value_remains_default):
+            # Enable check that the value is initialized to default_value
+            check_value = default_value
+        else:
+            # Set to a non default value
+            float_param.value = min_
+            # Enable check that the value is changed after initialization to a non default value
+            check_value = min_
+
         sci_input = ScientificInput(float_param)
         qtbot.addWidget(sci_input)
 
         assert sci_input.minimum() == min_
         assert sci_input.maximum() == max_
-        assert sci_input.value() == default_value
+        assert sci_input.value() == check_value
         assert sci_input.suffix() == ' m'
 
     def test_setValue_within_range_should_set(self, qtbot):
         float_param = FloatParameter('potato',
             minimum=-10, maximum=10, default=0)
         sci_input = ScientificInput(float_param)
         qtbot.addWidget(sci_input)
```

### Comparing `PyMeasure-0.8.0/tests/display/test_plotter.py` & `PyMeasure-0.9.0/tests/display/test_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/tests/display/test_windows.py` & `PyMeasure-0.9.0/tests/display/test_windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/tests/experiment/data/procedure_for_testing.py` & `PyMeasure-0.9.0/tests/experiment/data/procedure_for_testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/tests/experiment/test_listeners.py` & `PyMeasure-0.9.0/pymeasure/instruments/razorbill/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,23 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-import time
-from queue import Queue
-
-from pymeasure.experiment.listeners import Listener, Recorder
-from pymeasure.experiment.results import Results
-
-# TODO: Make results_for_testing.csv
-# TODO: Make procedure_for_testing.py
-
-"""
-def test_recorder_stop():
-    q = Queue()
-    d = Results.load('results_for_testing.csv')
-    r = Recorder(d, q)
-    r.
-"""
+from .razorbillRP100 import razorbillRP100
```

### Comparing `PyMeasure-0.8.0/tests/experiment/test_parameters.py` & `PyMeasure-0.9.0/tests/experiment/test_parameters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,38 +24,47 @@
 
 import pytest
 
 from pymeasure.experiment.parameters import Parameter
 from pymeasure.experiment.parameters import IntegerParameter
 from pymeasure.experiment.parameters import BooleanParameter
 from pymeasure.experiment.parameters import FloatParameter
+from pymeasure.experiment.parameters import ListParameter
+from pymeasure.experiment.parameters import VectorParameter
 
 
 def test_parameter_default():
     p = Parameter('Test', default=5)
     assert p.value == 5
 
 
 def test_integer_units():
     p = IntegerParameter('Test', units='V')
     assert p.units == 'V'
 
 
 def test_integer_value():
-    p = IntegerParameter('Test')
+    p = IntegerParameter('Test', units='tests')
     with pytest.raises(ValueError):
         v = p.value  # not set
     with pytest.raises(ValueError):
         p.value = 'a'  # not an integer
     p.value = 0.5  # a float
     assert p.value == 0
     p.value = False  # a boolean
     assert p.value == 0
     p.value = 10
     assert p.value == 10
+    p.value = '5'
+    assert p.value == 5
+    p.value = '11 tests'
+    assert p.value == 11
+    assert p.units == 'tests'
+    with pytest.raises(ValueError):
+        p.value = '31 incorrect units'  # not the correct units
 
 
 def test_integer_bounds():
     p = IntegerParameter('Test', minimum=0, maximum=10)
     p.value = 10
     assert p.value == 10
     with pytest.raises(ValueError):
@@ -64,39 +73,99 @@
         p.value = -100  # below minimum
 
 
 def test_boolean_value():
     p = BooleanParameter('Test')
     with pytest.raises(ValueError):
         v = p.value  # not set
-    p.value = 'a'  # a string
+    with pytest.raises(ValueError):
+        p.value = 'a'  # a string
+    with pytest.raises(ValueError):
+        p.value = 10  # a number other than 0 or 1
+    p.value = "True"
+    assert p.value == True
+    p.value = "False"
+    assert p.value == False
+    p.value = "true"
     assert p.value == True
-    p.value = 10  # a number
+    p.value = "false"
+    assert p.value == False
+    p.value = 1  # a number
     assert p.value == True
     p.value = 0  # zero
     assert p.value == False
     p.value = True
     assert p.value == True
 
 
 def test_float_value():
-    p = FloatParameter('Test')
+    p = FloatParameter('Test', units='tests')
     with pytest.raises(ValueError):
         v = p.value  # not set
     with pytest.raises(ValueError):
         p.value = 'a'  # not a float
     p.value = False  # boolean
     assert p.value == 0.0
     p.value = 100
     assert p.value == 100.0
+    p.value = '1.06'
+    assert p.value == 1.06
+    p.value = '11.3 tests'
+    assert p.value == 11.3
+    assert p.units == 'tests'
+    with pytest.raises(ValueError):
+        p.value = '31.3 incorrect units'  # not the correct units
 
 
 def test_float_bounds():
     p = FloatParameter('Test', minimum=0.1, maximum=0.5)
     p.value = 0.3
     assert p.value == 0.3
     with pytest.raises(ValueError):
         p.value = 10  # above maximum
     with pytest.raises(ValueError):
         p.value = -10  # below minimum
 
-# TODO: Add tests for VectorParameter, ListParamter, and Measurable
+
+def test_list_value():
+    # TODO: check against setting the string version of the numeric choices
+    p = ListParameter('Test', choices=[1, 2.2, 'three', 'and four'])
+    p.value = 1
+    assert p.value == 1
+    p.value = 2.2
+    assert p.value == 2.2
+    p.value = 'three'
+    assert p.value == 'three'
+    p.value = 'and four'
+    assert p.value == 'and four'
+    with pytest.raises(ValueError):
+        p.value = 5
+
+
+def test_list_value_with_units():
+    # TODO: check against setting the string version (with units) of the numeric choices
+    p = ListParameter('Test', choices=[1, 2.2, 'three', 'and four'], units='tests')
+    p.value = 'three tests'
+    assert p.value == 'three'
+    p.value = 'and four tests'
+    assert p.value == 'and four'
+
+
+def test_vector():
+    p = VectorParameter('test', length=3, units='tests')
+    p.value = [1, 2, 3]
+    assert p.value == [1, 2, 3]
+    p.value = '[4, 5, 6]'
+    assert p.value == [4, 5, 6]
+    p.value = '[7, 8, 9] tests'
+    assert p.value == [7, 8, 9]
+    with pytest.raises(ValueError):
+        p.value = '[0, 1, 2] wrong unit'
+    with pytest.raises(ValueError):
+        p.value = [1, 2]
+    with pytest.raises(ValueError):
+        p.value = ['a', 'b']
+    with pytest.raises(ValueError):
+        p.value = '0, 1, 2'
+
+
+# TODO: Add tests for Measurable
```

### Comparing `PyMeasure-0.8.0/tests/experiment/test_procedure.py` & `PyMeasure-0.9.0/tests/experiment/test_procedure.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/tests/experiment/test_results.py` & `PyMeasure-0.9.0/tests/experiment/test_results.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -29,14 +29,15 @@
 import tempfile
 import pickle
 from importlib.machinery import SourceFileLoader
 import pandas as pd
 import numpy as np
 from pymeasure.experiment.results import Results, CSVFormatter
 from pymeasure.experiment.procedure import Procedure, Parameter
+from pymeasure.experiment import BooleanParameter
 
 # Load the procedure, without it being in a module
 #data_path = os.path.join(os.path.dirname(__file__), 'data/procedure_for_testing.py')
 #RandomProcedure = SourceFileLoader('procedure', data_path).load_module().RandomProcedure
 from data.procedure_for_testing import RandomProcedure
 
 
@@ -109,7 +110,31 @@
         procedure = DummyProcedure()
         procedure.par = np.linspace(1,100,17)
         filename = os.path.join(str(tmpdir), 'header_linebreak_test.csv')
         result = Results(procedure, filename)
         result.reload() # assert no error
         pd.read_csv(filename, comment="#") # assert no error
         assert (result.parameters['par'].value == np.linspace(1,100,17)).all()
+
+
+def test_parameter_reading():
+    data_path = os.path.join(os.path.dirname(__file__), "data/results_for_testing_parameters.csv")
+    test_string = "/test directory with space/test_filename.csv"
+    iterations = 101
+    delay = 0.0005
+    seed = '54321'
+
+    class DummyProcedure(RandomProcedure):
+        check_false = BooleanParameter('checkbox False')
+        check_true = BooleanParameter('checkbox True')
+        check_dir = Parameter('Directory string')
+
+    results = Results.load(data_path, procedure_class=DummyProcedure)
+
+    # Check if all parameters are correctly read from file
+    assert results.parameters["iterations"].value == iterations
+    assert results.parameters["delay"].value == delay
+    assert results.parameters["seed"].value == seed
+
+    assert results.parameters["check_true"].value == True
+    assert results.parameters["check_false"].value == False
+    assert results.parameters["check_dir"].value == test_string
```

### Comparing `PyMeasure-0.8.0/tests/experiment/test_workers.py` & `PyMeasure-0.9.0/tests/experiment/test_workers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -65,7 +65,20 @@
     worker.start()
     worker.join(timeout=5)
 
     assert not worker.is_alive()
 
     new_results = Results.load(file, procedure_class=RandomProcedure)
     assert new_results.data.shape == (100, 2)
+
+def test_worker_closes_file_after_finishing():
+    procedure = RandomProcedure()
+    procedure.iterations = 100
+    procedure.delay = 0.001
+    file = tempfile.mktemp()
+    results = Results(procedure, file)
+    worker = Worker(results)
+    worker.start()
+    worker.join(timeout=5)
+
+    # Test if the file has been properly closed by removing the file
+    os.remove(file)
```

### Comparing `PyMeasure-0.8.0/tests/instruments/keithley/test_keithley2750.py` & `PyMeasure-0.9.0/tests/instruments/keithley/test_keithley2750.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/tests/instruments/test_instrument.py` & `PyMeasure-0.9.0/tests/instruments/test_instrument.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,14 +19,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 import pytest
+from pymeasure.adapters import FakeAdapter
 from pymeasure.instruments.instrument import Instrument, FakeInstrument
 from pymeasure.instruments.validators import strict_discrete_set, strict_range
 
 
 def test_fake_instrument():
     fake = FakeInstrument()
     fake.write("Testing")
@@ -146,14 +147,55 @@
     fake = Fake()
     fake.x = 5
     assert fake.read() == 'JUNK5'
     fake.x = 5
     assert fake.x == 5
 
 
+def test_control_preprocess_reply_property():
+    # test setting preprocess_reply at property-level
+    class Fake(FakeInstrument):
+        x = Instrument.control(
+            "", "JUNK%d",
+            "",
+            preprocess_reply=lambda v: v.replace('JUNK', ''),
+            cast=int
+        )
+
+    fake = Fake()
+    fake.x = 5
+    assert fake.read() == 'JUNK5'
+    # notice that read returns the full reply since preprocess_reply is only
+    # called inside Adapter.values()
+    fake.x = 5
+    assert fake.x == 5
+    fake.x = 5
+    assert type(fake.x) == int
+
+
+def test_control_preprocess_reply_adapter():
+    # test setting preprocess_reply at Adapter-level
+    class Fake(FakeInstrument):
+        def __init__(self):
+            super().__init__(preprocess_reply=lambda v: v.replace('JUNK', ''))
+
+        x = Instrument.control(
+            "", "JUNK%d", "",
+            cast=int
+        )
+
+    fake = Fake()
+    fake.x = 5
+    assert fake.read() == 'JUNK5'
+    # notice that read returns the full reply since preprocess_reply is only
+    # called inside Adapter.values()
+    fake.x = 5
+    assert fake.x == 5
+
+
 def test_measurement_dict_str_map():
     class Fake(FakeInstrument):
         x = Instrument.measurement(
             "", "",
             values={'X': 1, 'Y': 2, 'Z': 3},
             map_values=True,
         )
```

### Comparing `PyMeasure-0.8.0/tests/instruments/test_validators.py` & `PyMeasure-0.9.0/tests/instruments/test_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/tests/test_log.py` & `PyMeasure-0.9.0/tests/test_log.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,16 +19,21 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 import time
+import sys
+from unittest import mock
+
+import pytest
+
 from pymeasure.process import context
-from pymeasure.log import Scribe
+from pymeasure.log import Scribe, setup_logging
 
 
 # TODO: Add tests for logging convenience functions and TopicQueueHandler
 
 def test_scribe_stop():
     q = context.Queue()
     s = Scribe(q)
@@ -42,7 +47,16 @@
     q = context.Queue()
     s = Scribe(q)
     s.start()
     assert s.is_alive() is True
     q.put(None)
     time.sleep(0.1)
     assert s.is_alive() is False
+
+
+@pytest.mark.skipif(sys.version_info < (3, 6), reason='Mock.assert_called_once requires python 3.6')
+def test_setup_file_logging():
+    with mock.patch('pymeasure.log.file_log') as mocked_file_log:
+        setup_logging()
+        mocked_file_log.assert_not_called()
+        setup_logging(filename='log.txt')
+        mocked_file_log.assert_called_once()
```

### Comparing `PyMeasure-0.8.0/tests/test_process.py` & `PyMeasure-0.9.0/tests/test_process.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `PyMeasure-0.8.0/tests/test_thread.py` & `PyMeasure-0.9.0/pymeasure/instruments/thorlabs/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the PyMeasure package.
 #
-# Copyright (c) 2013-2020 PyMeasure Developers
+# Copyright (c) 2013-2021 PyMeasure Developers
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,22 +18,9 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from pymeasure.thread import StoppableThread
-
-
-def test_thread_stopping():
-    t = StoppableThread()
-    t.start()
-    t.stop()
-    assert t.should_stop() is True
-    t.join()
-
-def test_thread_joining():
-    t = StoppableThread()
-    t.start()
-    t.join()
-    assert t.should_stop() is True
+from .thorlabspm100usb import ThorlabsPM100USB
+from .thorlabspro8000 import ThorlabsPro8000
```

