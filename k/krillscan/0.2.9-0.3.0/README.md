# Comparing `tmp/krillscan-0.2.9.tar.gz` & `tmp/krillscan-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krillscan-0.2.9.tar", last modified: Sun Apr 23 13:33:32 2023, max compression
+gzip compressed data, was "krillscan-0.3.0.tar", last modified: Wed May 22 13:47:35 2024, max compression
```

## Comparing `krillscan-0.2.9.tar` & `krillscan-0.3.0.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.107857 krillscan-0.2.9/
--rw-rw-rw-   0        0        0     8325 2023-04-23 13:33:32.107857 krillscan-0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.938557 krillscan-0.2.9/krillscan/
--rw-rw-rw-   0        0        0      121 2023-04-21 13:49:36.000000 krillscan-0.2.9/krillscan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.954179 krillscan-0.2.9/krillscan/echolab2/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.954179 krillscan-0.2.9/krillscan/echolab2/instruments/
--rw-rw-rw-   0        0        0   159358 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/EK60.py
--rw-rw-rw-   0        0        0   193943 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/EK80.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/__init__.py
--rw-rw-rw-   0        0        0     3283 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/echosounder.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.985430 krillscan-0.2.9/krillscan/echolab2/instruments/util/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/__init__.py
--rw-rw-rw-   0        0        0     5456 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/annotation_data.py
--rw-rw-rw-   0        0        0     8274 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/bottom_data.py
--rw-rw-rw-   0        0        0     6783 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/date_conversion.py
--rw-rw-rw-   0        0        0     3698 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/ek80_datagram_example.py
--rw-rw-rw-   0        0        0     8616 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/motion_data.py
--rw-rw-rw-   0        0        0    24904 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/nmea_data.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.991943 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/
--rw-rw-rw-   0        0        0      410 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/_version.py
--rw-rw-rw-   0        0        0     7181 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea.py
--rw-rw-rw-   0        0        0     2014 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea_file.py
--rw-rw-rw-   0        0        0     3415 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea_utils.py
--rw-rw-rw-   0        0        0      902 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/seatalk_utils.py
--rw-rw-rw-   0        0        0     2050 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/stream.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.991943 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/
--rw-rw-rw-   0        0        0       85 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.007587 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/
--rw-rw-rw-   0        0        0      127 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/__init__.py
--rw-rw-rw-   0        0        0     3937 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ash.py
--rw-rw-rw-   0        0        0     1382 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/grm.py
--rw-rw-rw-   0        0        0      634 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py
--rw-rw-rw-   0        0        0     1196 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/srf.py
--rw-rw-rw-   0        0        0     3675 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py
--rw-rw-rw-   0        0        0     3404 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py
--rw-rw-rw-   0        0        0     2099 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py
--rw-rw-rw-   0        0        0    34150 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/talker.py
--rw-rw-rw-   0        0        0     1141 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/read_idx_example.py
--rw-rw-rw-   0        0        0    26010 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_calibration.py
--rw-rw-rw-   0        0        0    78275 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_parsers.py
--rw-rw-rw-   0        0        0    21140 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_raw_file.py
--rw-rw-rw-   0        0        0    11377 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_signal_proc.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.007587 krillscan-0.2.9/krillscan/echolab2/instruments/util/vincenty/
--rw-rw-rw-   0        0        0     3179 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/vincenty/__init__.py
--rw-rw-rw-   0        0        0    67919 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/ping_data.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.023211 krillscan-0.2.9/krillscan/echolab2/plotting/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.023211 krillscan-0.2.9/krillscan/echolab2/plotting/matplotlib/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/matplotlib/__init__.py
--rw-rw-rw-   0        0        0    16178 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/matplotlib/echogram.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.023211 krillscan-0.2.9/krillscan/echolab2/plotting/qt/
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.054457 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/
--rw-rw-rw-   0        0        0    26210 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py
--rw-rw-rw-   0        0        0    19146 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py
--rw-rw-rw-   0        0        0    20595 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py
--rw-rw-rw-   0        0        0    20668 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py
--rw-rw-rw-   0        0        0    15704 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVGrid.py
--rw-rw-rw-   0        0        0     6629 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVHudText.py
--rw-rw-rw-   0        0        0     7732 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVLine.py
--rw-rw-rw-   0        0        0    17957 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarker.py
--rw-rw-rw-   0        0        0     7030 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py
--rw-rw-rw-   0        0        0    13085 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygon.py
--rw-rw-rw-   0        0        0    12899 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py
--rw-rw-rw-   0        0        0    12600 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py
--rw-rw-rw-   0        0        0    12009 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer.py
--rw-rw-rw-   0        0        0    12665 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py
--rw-rw-rw-   0        0        0    61143 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QViewerBase.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/__init__.py
--rw-rw-rw-   0        0        0     8890 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py
--rw-rw-rw-   0        0        0     7787 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.054457 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/__init__.py
--rw-rw-rw-   0        0        0    17722 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py
--rw-rw-rw-   0        0        0    14034 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py
--rw-rw-rw-   0        0        0     1615 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.054457 krillscan-0.2.9/krillscan/echolab2/plotting/qt/ui/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/ui/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/ui/ui_echogram_viewer.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.070084 krillscan-0.2.9/krillscan/echolab2/processing/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/__init__.py
--rw-rw-rw-   0        0        0    10904 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/afsc_bot_detector.py
--rw-rw-rw-   0        0        0     3347 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/batch_utils.py
--rw-rw-rw-   0        0        0     9669 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/grid.py
--rw-rw-rw-   0        0        0    21422 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/line.py
--rw-rw-rw-   0        0        0    22367 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/mask.py
--rw-rw-rw-   0        0        0    75289 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/processed_data.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.107857 krillscan-0.2.9/krillscan/echopy/
--rw-rw-rw-   0        0        0      758 2023-04-21 13:50:02.000000 krillscan-0.2.9/krillscan/echopy/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/cmaps.py
--rw-rw-rw-   0        0        0      267 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/correct_absorption.py
--rw-rw-rw-   0        0        0      248 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/correct_es60triangle.py
--rw-rw-rw-   0        0        0      250 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/correct_soundspeed.py
--rw-rw-rw-   0        0        0     3372 2023-04-21 13:50:19.000000 krillscan-0.2.9/krillscan/echopy/get_background.py
--rw-rw-rw-   0        0        0     5966 2023-04-21 13:50:51.000000 krillscan-0.2.9/krillscan/echopy/mask_attenuated.py
--rw-rw-rw-   0        0        0     7763 2023-04-21 13:51:06.000000 krillscan-0.2.9/krillscan/echopy/mask_impulse.py
--rw-rw-rw-   0        0        0     1358 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/mask_multifrequency.py
--rw-rw-rw-   0        0        0     2609 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/mask_range.py
--rw-rw-rw-   0        0        0    21355 2023-04-21 13:51:18.000000 krillscan-0.2.9/krillscan/echopy/mask_seabed.py
--rw-rw-rw-   0        0        0    10771 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/mask_shoals.py
--rw-rw-rw-   0        0        0     2511 2023-04-21 13:51:29.000000 krillscan-0.2.9/krillscan/echopy/mask_signal2noise.py
--rw-rw-rw-   0        0        0      873 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/mask_stationary.py
--rw-rw-rw-   0        0        0     7131 2023-04-21 13:51:37.000000 krillscan-0.2.9/krillscan/echopy/mask_transient.py
--rw-rw-rw-   0        0        0    13405 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/read_calibration.py
--rw-rw-rw-   0        0        0    17793 2023-04-21 13:50:29.000000 krillscan-0.2.9/krillscan/echopy/resample.py
--rw-rw-rw-   0        0        0     5841 2023-04-21 13:50:38.000000 krillscan-0.2.9/krillscan/echopy/transform.py
--rw-rw-rw-   0        0        0    57129 2023-04-23 13:30:28.000000 krillscan-0.2.9/krillscan/krillscan.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.954179 krillscan-0.2.9/krillscan.egg-info/
--rw-rw-rw-   0        0        0     8325 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4821 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 13:33:32.107857 krillscan-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-04-23 13:32:41.000000 krillscan-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:35.145266 krillscan-0.3.0/
+-rw-rw-rw-   0        0        0    11918 2024-05-22 13:47:35.145266 krillscan-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:33.967634 krillscan-0.3.0/echolab2/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.014510 krillscan-0.3.0/echolab2/instruments/
+-rw-rw-rw-   0        0        0   159358 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/EK60.py
+-rw-rw-rw-   0        0        0   193943 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/EK80.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/__init__.py
+-rw-rw-rw-   0        0        0     3283 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/echosounder.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.186418 krillscan-0.3.0/echolab2/instruments/util/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/__init__.py
+-rw-rw-rw-   0        0        0     5456 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/annotation_data.py
+-rw-rw-rw-   0        0        0     8274 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/bottom_data.py
+-rw-rw-rw-   0        0        0     6783 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/date_conversion.py
+-rw-rw-rw-   0        0        0     3698 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/ek80_datagram_example.py
+-rw-rw-rw-   0        0        0     8616 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/motion_data.py
+-rw-rw-rw-   0        0        0    24904 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/nmea_data.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.285883 krillscan-0.3.0/echolab2/instruments/util/pynmea2/
+-rw-rw-rw-   0        0        0      410 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/_version.py
+-rw-rw-rw-   0        0        0     7181 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea.py
+-rw-rw-rw-   0        0        0     2014 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea_file.py
+-rw-rw-rw-   0        0        0     3415 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea_utils.py
+-rw-rw-rw-   0        0        0      902 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/seatalk_utils.py
+-rw-rw-rw-   0        0        0     2050 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/stream.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.332761 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/
+-rw-rw-rw-   0        0        0       85 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.457760 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/
+-rw-rw-rw-   0        0        0      127 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/__init__.py
+-rw-rw-rw-   0        0        0     3937 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/ash.py
+-rw-rw-rw-   0        0        0     1382 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/grm.py
+-rw-rw-rw-   0        0        0      634 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py
+-rw-rw-rw-   0        0        0     1196 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/srf.py
+-rw-rw-rw-   0        0        0     3675 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py
+-rw-rw-rw-   0        0        0     3404 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py
+-rw-rw-rw-   0        0        0     2099 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py
+-rw-rw-rw-   0        0        0    34150 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/talker.py
+-rw-rw-rw-   0        0        0     1141 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/read_idx_example.py
+-rw-rw-rw-   0        0        0    26010 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/simrad_calibration.py
+-rw-rw-rw-   0        0        0    78275 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/simrad_parsers.py
+-rw-rw-rw-   0        0        0    21140 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/simrad_raw_file.py
+-rw-rw-rw-   0        0        0    11377 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/simrad_signal_proc.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.473438 krillscan-0.3.0/echolab2/instruments/util/vincenty/
+-rw-rw-rw-   0        0        0     3179 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/vincenty/__init__.py
+-rw-rw-rw-   0        0        0    67919 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/ping_data.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.473438 krillscan-0.3.0/echolab2/plotting/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.504636 krillscan-0.3.0/echolab2/plotting/matplotlib/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/matplotlib/__init__.py
+-rw-rw-rw-   0        0        0    16178 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/matplotlib/echogram.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.504636 krillscan-0.3.0/echolab2/plotting/qt/
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.754638 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/
+-rw-rw-rw-   0        0        0    26210 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py
+-rw-rw-rw-   0        0        0    19146 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py
+-rw-rw-rw-   0        0        0    20595 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py
+-rw-rw-rw-   0        0        0    20668 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py
+-rw-rw-rw-   0        0        0    15704 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVGrid.py
+-rw-rw-rw-   0        0        0     6629 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVHudText.py
+-rw-rw-rw-   0        0        0     7732 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVLine.py
+-rw-rw-rw-   0        0        0    17957 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVMarker.py
+-rw-rw-rw-   0        0        0     7030 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py
+-rw-rw-rw-   0        0        0    13085 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVPolygon.py
+-rw-rw-rw-   0        0        0    12899 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py
+-rw-rw-rw-   0        0        0    12600 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py
+-rw-rw-rw-   0        0        0    12009 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QImageViewer.py
+-rw-rw-rw-   0        0        0    12665 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py
+-rw-rw-rw-   0        0        0    61143 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QViewerBase.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/__init__.py
+-rw-rw-rw-   0        0        0     8890 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py
+-rw-rw-rw-   0        0        0     7787 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.817138 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/__init__.py
+-rw-rw-rw-   0        0        0    17722 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py
+-rw-rw-rw-   0        0        0    14034 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py
+-rw-rw-rw-   0        0        0     1615 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.832764 krillscan-0.3.0/echolab2/plotting/qt/ui/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/ui/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/ui/ui_echogram_viewer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.926514 krillscan-0.3.0/echolab2/processing/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/__init__.py
+-rw-rw-rw-   0        0        0    10904 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/afsc_bot_detector.py
+-rw-rw-rw-   0        0        0     3347 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/batch_utils.py
+-rw-rw-rw-   0        0        0     9669 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/grid.py
+-rw-rw-rw-   0        0        0    21422 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/line.py
+-rw-rw-rw-   0        0        0    22367 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/mask.py
+-rw-rw-rw-   0        0        0    75289 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/processed_data.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:35.098391 krillscan-0.3.0/echopy/
+-rw-rw-rw-   0        0        0      758 2023-04-21 13:50:02.000000 krillscan-0.3.0/echopy/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/cmaps.py
+-rw-rw-rw-   0        0        0      267 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/correct_absorption.py
+-rw-rw-rw-   0        0        0      248 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/correct_es60triangle.py
+-rw-rw-rw-   0        0        0      250 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/correct_soundspeed.py
+-rw-rw-rw-   0        0        0     3372 2023-04-21 13:50:19.000000 krillscan-0.3.0/echopy/get_background.py
+-rw-rw-rw-   0        0        0     5966 2023-04-21 13:50:51.000000 krillscan-0.3.0/echopy/mask_attenuated.py
+-rw-rw-rw-   0        0        0     7763 2023-04-21 13:51:06.000000 krillscan-0.3.0/echopy/mask_impulse.py
+-rw-rw-rw-   0        0        0     1358 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/mask_multifrequency.py
+-rw-rw-rw-   0        0        0     2609 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/mask_range.py
+-rw-rw-rw-   0        0        0    21355 2023-04-21 13:51:18.000000 krillscan-0.3.0/echopy/mask_seabed.py
+-rw-rw-rw-   0        0        0    10771 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/mask_shoals.py
+-rw-rw-rw-   0        0        0     2511 2023-04-21 13:51:29.000000 krillscan-0.3.0/echopy/mask_signal2noise.py
+-rw-rw-rw-   0        0        0      873 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/mask_stationary.py
+-rw-rw-rw-   0        0        0     7131 2023-04-21 13:51:37.000000 krillscan-0.3.0/echopy/mask_transient.py
+-rw-rw-rw-   0        0        0    13405 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/read_calibration.py
+-rw-rw-rw-   0        0        0    17793 2023-04-21 13:50:29.000000 krillscan-0.3.0/echopy/resample.py
+-rw-rw-rw-   0        0        0     5841 2023-04-21 13:50:38.000000 krillscan-0.3.0/echopy/transform.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:35.145266 krillscan-0.3.0/krillscan/
+-rw-rw-rw-   0        0        0      123 2023-04-27 09:16:18.000000 krillscan-0.3.0/krillscan/__init__.py
+-rw-rw-rw-   0        0        0    37891 2024-04-24 08:37:15.000000 krillscan-0.3.0/krillscan/inspect.py
+-rw-rw-rw-   0        0        0    67697 2024-05-13 12:02:29.000000 krillscan-0.3.0/krillscan/process.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:35.145266 krillscan-0.3.0/krillscan.egg-info/
+-rw-rw-rw-   0        0        0    11918 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3950 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 13:47:35.145266 krillscan-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      906 2024-05-22 13:45:47.000000 krillscan-0.3.0/setup.py
```

### Comparing `krillscan-0.2.9/PKG-INFO` & `krillscan-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 Metadata-Version: 2.1
 Name: krillscan
-Version: 0.2.9
+Version: 0.3.0
 Summary: A python module for automatic analysis of backscatter data from vessels of opportunity
 Home-page: 
 Author: Sebastian Menze
 Author-email: sebastian.menze@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+Requires-Dist: lxml
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: future
+Requires-Dist: pyproj
+Requires-Dist: scikit_image
+Requires-Dist: scipy
+Requires-Dist: toml
+Requires-Dist: geopy
+Requires-Dist: tables
+Requires-Dist: xarray
+Requires-Dist: netcdf4
+Requires-Dist: pyqtdarktheme
 
 
 
-# Krillscan - A python module for automatic  analysis of backscatter data from fishing vessels to implement feedback management of the Antarctic krill fishery
+# Krillscan - A python module for automatic analysis of backscatter data from fishing vessels to implement feedback management of the Antarctic krill fishery
 
-- Automatically processes and analyzees EK60 and EK80 echosounder data 
+- Automatically processes and analyzes EK60 and EK80 echosounder data 
 - stores echograms and NASC tables as NetCDF, HDF or .csv files
 - detects krill swarms and can send near-real-time acoustic registrations via email
 
 ![dataflow](dataflow.JPG)
 
 ## Installation
 
@@ -50,34 +64,35 @@
 sv_SNR_threshold_db = 3
 swarm_sv_threshold_db = -70
 dbdiff_sv_threshold_db = 3
 seafloor_offset_m= 10
 seafloor_sv_threshold_db= -38
 surface_exclusion_depth_m = 20
 maximum_depth_m = 250
+write_mask_as_csv= 0
 
 [EMAIL]
 email_send = 0
 email_from = *Enter a mail address here*
 email_to = *Enter a mail address here*
 pw = *Enter IMAP password address here*
 files_per_email = 6
 send_echograms = 1
 echogram_resolution_in_seconds = 1
 ```
 
-This settings.ini file must be located in the same working directory as your python prompt. To send emails set email_send=1 (or True).
+This location of the settings.ini file must be passed to krillscan when starting the processing. To send emails set email_send=1 (or True).
 
- To start the processing type:
+To start the processing type:
 
 ```python
-import krillscan as ks
-ks.krillscan.ks.start()
+from krillscan import process
+process.ks.start('settings.ini')
 # to stop the processing: 
-# ks.krillscan.ks.stop()
+# process.ks.stop( )
 ```
 This starts two threads, one that looks for new data, processes and stores it and another that scans for recently processed data and sends them out via email. This is an ad-hoc solution so far, future versions of krillscan will transfer data directly to a cloud storage. 
 
 
 ### Output format
 
 Krillscan will store the raw and processed echograms, detection masks and NASC tables in 10-min long snippets, with the filename containing the start date of each snippet:
@@ -88,15 +103,24 @@
 D20140125-T060417_mask_dbdiff.h5
 D20140125-T060417_mask_swarm.h5
 D20140125-T060417_nasctable.csv
 D20140125-T060417_nasctable.h5
 D20140125-T060417_rawechogram.nc
 ```
 
+NASC stands for Nautical area backscattering coefficient has the unit m^2 nmi^-2 and is the vertical integral (sum) of volume backscatter normalized to 1x1 nautical mile area:
+
+```python
+sv_lin=np.power(10, Sv120sw /10)  
+sv_downsampled=  resize_local_mean(sv_lin,[ len(r_new) , Sv120sw.shape[1] ] ,grid_mode =True)
+sa =  integrate.trapezoid(sv_downsampled,sv_dep,axis=0)  
+nasc =  4*np.pi*1852**2 * sa
+```
 Here is an example of the contents of the echogram files, they are stored and read using the xarray module:
+
 ```python
 import xarray as xr
 file="D20140125-T055416_rawechogram.nc"
 xr_sv = xr.open_dataarray(file)
 print(xr_sv)
 ```
 ```
@@ -104,15 +128,15 @@
 [854000 values with dtype=float32]
 Coordinates:
   * time       (time) datetime64[ns] 2014-01-25T05:54:16.770000 ... 2014-01-2...
   * depth      (depth) float64 0.0 0.5 1.0 1.5 2.0 ... 498.0 498.5 499.0 499.5
   * frequency  (frequency) float64 3.8e+04 1.2e+05
 ```
 
-Here is an example of the contents of the mask files, they are stored and read as pandas DataFrames:
+Here is an example of the contents of the mask files, they are stored and read as pandas DataFrames. if you want the mask files as csv in addition to hdf you must change settings.ini to "write_mask_as_csv= True". 
 
 ```python
 import pandas as pd
 file="D20140125-T060417_mask_swarm.h5"
 df = pd.read_hdf(file,key='df')
 print(df)
 ```
@@ -157,25 +181,26 @@
 2014-01-25 06:04:11.395 -60.004037 -48.374469  ...   334.853738          0.0
 2014-01-25 06:04:12.797 -60.004021 -48.374597  ...  1719.993121          0.0
 2014-01-25 06:04:14.199 -60.004004 -48.374726  ...     0.000000          0.0
 
 [427 rows x 7 columns]
 ```
 
-Here is an example for 1-month of echosunder data from a krill fishing vessel, processed entirely automatic using the swarm detection method.
+Here is an example for 1-month of echosounder data from a krill fishing vessel, processed entirely automatic using the swarm detection method.
 
 ![timeseries_endurance_jan2022](timeseries_endurance_jan2022.jpg)
 
 
 ### Visual inspection of processed echograms
 
 Krillscan also contains a GUI tool (PyQT5) that lets you inspect the automatically processed echograms and correct the swarm detection masks by adding or removing areas. To start the GUI enter:
 
 ```python
-ks.ks.inspect()
+from krillscan import inspect
+inspect.gui()
 ```
 
 The GUI looks like this: A  menu bar lets you open processed NetCDF files, show the data folder, undo changes and quite the GUI. The Main window shows the echogram for each 10-min long NetCDF and the ping-by-ping NASC (black line) and 1-min NASC average (blue line). 
 
 ![menuebar](menuebar.JPG)
 
 The tool bar below the menu bar has these functions:
@@ -188,15 +213,55 @@
 
 - You can add or remove areas of the detection mask (shown as red overlay) using double clicks to draw a polygon of you choice. Once finished with drawing press enter to apply the change and update the NASC accordingly.
 
 ![fig_inspect](fig_inspect.png)
 
 
 
+### Data Transfer
+
+So far I have implemented simple email sending as data transfer method. The echogram NetCDF and detection mask Hdf files are down sampled in time to a desired resolution (in setting.ini) and than compressed into a zip file. This is rather efficient, for a 10-min snippet in 1-s resolution the files echogram files are between 10-30 MB (depending on the number of frequencies) but the zip file is only around 800 kB. In addition to the echogram and mask the ping-by-ping NASC table is sent as Hdf file and the setting.ini file. Here is an example:
+
+![mail_content](mail_content.JPG)
+
+You can open and edit these echogram / detection mask files with the inspection GUI, but the "view raw" mode will not work. 
+
+### Parallel post-processing of data
+
+If you have a lot of raw files that need to be processed, it can be better to use parallel processing instead of the serial real-time processing. This is also implemented in krillscan using the multiprocessing module This will process and store the data in their original file length and not 10-min snippets. To start the parallel post-processing you can use the same ini file, the module will detect the amount of cores available and distribute tasks across all of them.
+
+```python
+from krillscan import process
+process.ks.start_para_processing('settings.ini')
+```
+
+### Annotation of echograms using custom labels
+
+```python
+from krillscan import inspect_and_annotate
+inspect_and_annotate.gui()
+```
+
+This opens the PyQt5 GUI with an additional line, here you can write up to 7 custom lables into the fields and mark rectangular patches in the echogram using mouse click and release. To remove the latest rectangle use the right mouse click. To save annotations check the "save changes" box and move on to the next snippet. You can toggle if the swarm detection mask should show or not using the "show mask" box. Annotations are saved as .csv for each snippet using UNIX timestamps as left and right border and depth as upper and lower border.
+
+```
+,t1,t2,d1,d2,label
+0,19092.83217844115,19092.83316209359,-241.50554015402548,-62.35334814153828,Predator
+1,19092.83269467859,19092.834692351964,-46.36452080694602,-24.86553958551312,
+```
+
+![ks_with_annot](ks_with_annot.JPG)
+
 ## Acknowledgements
 
+This software relies on packages and functions developed by the rapidkrill, echopy, pyecholab and echopype projects. We would like to thank the teams for sharing their useful code! We also thank all developers of python and its many open libraries. 
+
+https://github.com/bas-acoustics/rapidkrill
+
+https://echopype.readthedocs.io/en/stable/index.html
 
+https://github.com/bas-acoustics/echopy
 
+https://github.com/CI-CMG/pyEcholab/tree/master/echolab2
 
 
-## Run krillscan automatic processing from a Docker container
```

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/EK60.py` & `krillscan-0.3.0/echolab2/instruments/EK60.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/EK80.py` & `krillscan-0.3.0/echolab2/instruments/EK80.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/echosounder.py` & `krillscan-0.3.0/echolab2/instruments/echosounder.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/annotation_data.py` & `krillscan-0.3.0/echolab2/instruments/util/annotation_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/bottom_data.py` & `krillscan-0.3.0/echolab2/instruments/util/bottom_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/date_conversion.py` & `krillscan-0.3.0/echolab2/instruments/util/date_conversion.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/ek80_datagram_example.py` & `krillscan-0.3.0/echolab2/instruments/util/ek80_datagram_example.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/motion_data.py` & `krillscan-0.3.0/echolab2/instruments/util/motion_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/nmea_data.py` & `krillscan-0.3.0/echolab2/instruments/util/nmea_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea_file.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea_file.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea_utils.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea_utils.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/seatalk_utils.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/seatalk_utils.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/stream.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/stream.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ash.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/ash.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/grm.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/grm.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/srf.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/srf.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/talker.py` & `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/talker.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/read_idx_example.py` & `krillscan-0.3.0/echolab2/instruments/util/read_idx_example.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_calibration.py` & `krillscan-0.3.0/echolab2/instruments/util/simrad_calibration.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_parsers.py` & `krillscan-0.3.0/echolab2/instruments/util/simrad_parsers.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_raw_file.py` & `krillscan-0.3.0/echolab2/instruments/util/simrad_raw_file.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_signal_proc.py` & `krillscan-0.3.0/echolab2/instruments/util/simrad_signal_proc.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/instruments/util/vincenty/__init__.py` & `krillscan-0.3.0/echolab2/instruments/util/vincenty/__init__.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/ping_data.py` & `krillscan-0.3.0/echolab2/ping_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/matplotlib/echogram.py` & `krillscan-0.3.0/echolab2/plotting/matplotlib/echogram.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVGrid.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVGrid.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVHudText.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVHudText.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVLine.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVLine.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarker.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVMarker.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygon.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVPolygon.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QImageViewer.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QViewerBase.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QViewerBase.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py` & `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/plotting/qt/ui/ui_echogram_viewer.py` & `krillscan-0.3.0/echolab2/plotting/qt/ui/ui_echogram_viewer.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/processing/afsc_bot_detector.py` & `krillscan-0.3.0/echolab2/processing/afsc_bot_detector.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/processing/batch_utils.py` & `krillscan-0.3.0/echolab2/processing/batch_utils.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/processing/grid.py` & `krillscan-0.3.0/echolab2/processing/grid.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/processing/line.py` & `krillscan-0.3.0/echolab2/processing/line.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/processing/mask.py` & `krillscan-0.3.0/echolab2/processing/mask.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echolab2/processing/processed_data.py` & `krillscan-0.3.0/echolab2/processing/processed_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/__init__.py` & `krillscan-0.3.0/echopy/__init__.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/cmaps.py` & `krillscan-0.3.0/echopy/cmaps.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/get_background.py` & `krillscan-0.3.0/echopy/get_background.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/mask_attenuated.py` & `krillscan-0.3.0/echopy/mask_attenuated.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/mask_impulse.py` & `krillscan-0.3.0/echopy/mask_impulse.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/mask_multifrequency.py` & `krillscan-0.3.0/echopy/mask_multifrequency.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/mask_range.py` & `krillscan-0.3.0/echopy/mask_range.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/mask_seabed.py` & `krillscan-0.3.0/echopy/mask_seabed.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/mask_shoals.py` & `krillscan-0.3.0/echopy/mask_shoals.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/mask_signal2noise.py` & `krillscan-0.3.0/echopy/mask_signal2noise.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/mask_stationary.py` & `krillscan-0.3.0/echopy/mask_stationary.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/mask_transient.py` & `krillscan-0.3.0/echopy/mask_transient.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/read_calibration.py` & `krillscan-0.3.0/echopy/read_calibration.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/resample.py` & `krillscan-0.3.0/echopy/resample.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/echopy/transform.py` & `krillscan-0.3.0/echopy/transform.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.9/krillscan/krillscan.py` & `krillscan-0.3.0/krillscan/process.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 # -*- coding: utf-8 -*-
 """
+Created on Mon Mar 18 16:39:03 2024
+
+@author: a5278
+"""
+
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Jul 25 11:25:10 2023
+
+@author: a5278
+"""
+
+# -*- coding: utf-8 -*-
+"""
 Created on Fri Apr 21 11:01:11 2023
 
 @author: Administrator
 """
 
 
 from skimage.transform import  resize
 from skimage.transform import  resize_local_mean
 import shutil
 from skimage.transform import  resize
 
-from krillscan.echolab2.instruments import EK80, EK60
+# from krillscan.echolab2.instruments import EK80, EK60
 import configparser
 
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import datetime as dt
 import glob 
 import os
+from PIL import Image
 
 # from scipy.ndimage.filters import uniform_filter1d
 
 from scipy.signal import convolve2d
 # from skimage.transform import  resize
 
-from krillscan.echopy import transform as tf
+from krillscan.echopy import transform as transform
 from krillscan.echopy import resample as rs
 from krillscan.echopy import mask_impulse as mIN
 from krillscan.echopy import mask_seabed as mSB
 from krillscan.echopy import get_background as gBN
 from krillscan.echopy import mask_range as mRG
 from krillscan.echopy import mask_shoals as mSH
 from krillscan.echopy import mask_signal2noise as mSN
 
+import echopype as ep
+
+
 from pyproj import Geod
 geod = Geod(ellps="WGS84")
 from pathlib import Path
 
 
 # from matplotlib.colors import ListedColormap
 import re
@@ -59,649 +77,47 @@
 
 import xarray as xr
 from scipy.interpolate import interp1d
 from scipy import integrate
 
 
 
-# from echolab2.instruments import EK80, EK60
-import configparser
-from scipy.signal import find_peaks
-
-import pandas as pd
-import numpy as np
-import matplotlib.pyplot as plt
-import datetime as dt
-import glob 
-import os
-import logging
-
-from scipy.ndimage.filters import uniform_filter1d
-
-from scipy.signal import convolve2d
-from scipy.interpolate import interp1d
-
-
-from skimage.transform import rescale, resize 
-
-from pyproj import Geod
-geod = Geod(ellps="WGS84")
-
-import sys
-import matplotlib
-
-from PyQt5 import QtCore, QtGui, QtWidgets
-
-from matplotlib.gridspec import GridSpec
-from mpl_toolkits.axes_grid1.inset_locator import inset_axes
-
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg, NavigationToolbar2QT as NavigationToolbar
-from matplotlib.figure import Figure
-import qdarktheme
-import time
-
-from matplotlib.path import Path as MPL_Path
-
-from mpl_toolkits.axes_grid1.inset_locator import inset_axes
-
-from matplotlib.colors import ListedColormap
-import re
-import traceback
-import zipfile
-
-import xarray as xr
-import matplotlib.dates as mdates
-#%% inspection GUI
-
-class MplCanvas(FigureCanvasQTAgg ):
-
-    def __init__(self, parent=None, dpi=150):
-        self.fig = Figure(figsize=None, dpi=dpi,facecolor='gray')
-        super(MplCanvas, self).__init__(self.fig)
-
-        
-class MainWindow(QtWidgets.QMainWindow):
-    
-
-    def __init__(self, *args, **kwargs):
-        super(MainWindow, self).__init__(*args, **kwargs)
-
-        self.canvas =  MplCanvas(self, dpi=150)
-                
-        self.echodata=dict()
-        self.echodata_swarm=dict()
-        self.df_nasc=pd.DataFrame([])
-
-        
-        self.filecounter=-1
-        self.filenames = None
-        self.df_files = pd.DataFrame([])
-
-        self.folder_source=''
-        self.statusBar().setStyleSheet("background-color : k")
-
-
-        menuBar = self.menuBar()
-
-        # Creating menus using a title
-        openMenu = menuBar.addAction("Select echogram files")
-        openMenu.triggered.connect(self.openfiles_fun)
-
-        
-        self.showfolderbutton =  menuBar.addAction('Show data folder')
-        # self.showfolderbutton.setEnabled(False)
-        self.showfolderbutton.triggered.connect(self.showfoldefunc)     
-
-        
-        self.showfolderbutton =  menuBar.addAction('Undo mask change')
-        # self.showfolderbutton.setEnabled(False)
-        self.showfolderbutton.triggered.connect(self.undo_mask)     
-  
-        quitMenu = menuBar.addAction("Quit")
-        quitMenu.triggered.connect(self.func_quit)     
-    
-
-        toolbar = QtWidgets.QToolBar()
-
-        self.checkbox_mask=QtWidgets.QCheckBox('Save changes')
-        self.checkbox_mask.setChecked(False)            
-        toolbar.addWidget(self.checkbox_mask)
-        
-        self.checkbox_raw=QtWidgets.QCheckBox('Raw')
-        self.checkbox_raw.setChecked(False)           
-        self.checkbox_raw.clicked.connect(self.choose_raw_changed)          
-        toolbar.addWidget(self.checkbox_raw)
-
-        toolbar.addWidget(QtWidgets.QLabel('Freq.:'))        
-        self.choose_freq = QtWidgets.QComboBox()
-        self.choose_freq.addItem('38')
-        self.choose_freq.addItem('120')
-        self.choose_freq.addItem('200')
-        self.choose_freq.setCurrentIndex(1)
-        toolbar.addWidget(  self.choose_freq)
-        toolbar.addWidget(QtWidgets.QLabel('kHz'))            
-        self.choose_freq.activated[str].connect(self.choose_freq_changed) 
-
-        toolbar.addWidget(QtWidgets.QLabel('Color:'))        
-        self.choose_color = QtWidgets.QComboBox()
-        self.choose_color.addItem('viridis')
-        self.choose_color.addItem('plasma')
-        self.choose_color.addItem('jet')
-        self.choose_color.setCurrentIndex(2)
-        toolbar.addWidget(  self.choose_color)
-        self.choose_color.activated[str].connect(self.choose_color_changed) 
-        
-        
-
-        toolbar.addWidget(QtWidgets.QLabel('Min. depth:'))        
-        self.excl_depth_spin = QtWidgets.QSpinBox()
-        self.excl_depth_spin.setMinimum(0)
-        self.excl_depth_spin.setMaximum(8000)
-        self.excl_depth_spin.setValue(20)
-        toolbar.addWidget(  self.excl_depth_spin)
-        toolbar.addWidget(QtWidgets.QLabel('m'))        
-
-        toolbar.addWidget(QtWidgets.QLabel('Max. depth:'))        
-        self.max_depth_spin = QtWidgets.QSpinBox()
-        self.max_depth_spin.setMinimum(0)
-        self.max_depth_spin.setMaximum(8000)
-        self.max_depth_spin.setValue(500)
-
-        toolbar.addWidget(  self.max_depth_spin)
-        toolbar.addWidget(QtWidgets.QLabel('m'))              
-        
-        self.butt_prev=QtWidgets.QPushButton('<-- previous')
-        self.butt_prev.clicked.connect(self.plot_prev)        
-        toolbar.addWidget(self.butt_prev)
-
-        self.butt_next=QtWidgets.QPushButton('Next -->')
-        self.butt_next.clicked.connect(self.plot_next)        
-        toolbar.addWidget(self.butt_next)
-        
-                #### hotkeys
-        self.msgSc1 = QtWidgets.QShortcut(QtCore.Qt.Key_Right, self)
-        self.msgSc1.activated.connect(self.plot_next)
-        self.msgSc2 = QtWidgets.QShortcut(QtCore.Qt.Key_Left, self)
-        self.msgSc2.activated.connect(self.plot_prev)        
-
-
-        self.butt_removearea=QtWidgets.QPushButton('Remove area')
-        self.butt_removearea.clicked.connect(self.mask_removearea)        
-        toolbar.addWidget(self.butt_removearea)
-        
-        self.butt_addarea=QtWidgets.QPushButton('Add area')
-        self.butt_addarea.clicked.connect(self.mask_addarea)        
-        toolbar.addWidget(self.butt_addarea)
-        
-        toolbar.addSeparator()
-
-         
-        tnav = NavigationToolbar( self.canvas, self)       
-        toolbar.addWidget(tnav)
-       
-        outer_layout = QtWidgets.QVBoxLayout()
-        outer_layout.addWidget(toolbar)
-        outer_layout.addWidget(self.canvas)
-    
-        # Create a placeholder widget to hold our toolbar and canvas.
-        widget = QtWidgets.QWidget()
-        widget.setLayout(outer_layout)
-        self.setCentralWidget(widget)
-        
-        
-        self.show()  
-   
-
-        self.cmap_mask = ListedColormap( np.array([[1,0,0, 1. ]] ) )
-        
-        
-        self.t=[-1,-1]
-        self.plotwindow_startsecond=0
-        self.plotwindow_length=0
-  
-        
-    def settings_edit(self):
-        os.startfile(self.ini_file)    
-   
-                  
-    def showfoldefunc(self):    
-         os.startfile(self.workpath)
-         
-    def openfiles_fun(self):
-        
-        fname_canidates, ok = QtWidgets.QFileDialog.getOpenFileNames(self,"QFileDialog.getOpenFileNames()",'',"Echogram Files (*_echogram.nc)")
-         
-        if len( fname_canidates ) >0:
-            
-            self.filenames = np.array( fname_canidates )   
-            print(  fname_canidates )
-            
-            self.workpath = os.path.dirname( fname_canidates[0])
-        
-            self.filecounter=-1
-               
-            self.plot_next()
-            
-    def choose_color_changed(self):
-        if self.filecounter>=0:        
-            self.plot_echogram()
-
-    def choose_raw_changed(self):
-        if self.filecounter>=0:        
-            self.plot_echogram()
-            
-    def plot_echogram(self):    
-        
-                
-        # breakpoint()
-        
-        ix_f = self.xr_sv.coords['frequency']== int(self.choose_freq.currentText()) *1000
-        sv = np.squeeze( self.xr_sv[ix_f,:,:])
-        
-
-            
-                
-        # sv = sv.interpolate_na( dim='time', method="linear")
-        
-        # sv = sv.interpolate_na(  'depth',max_gap=3,method="linear")
-        # sv = sv.interpolate_na(  'time' ,max_gap=pd.Timedelta(seconds=5))
-        
-        # sv = sv.interp(time=sv.time , depth=sv.depth, method="linear")
-        
-        
-
-        sv_mask=sv.copy()
-        sv_mask.values [~self.mask_manual.values]=np.nan
-
-        
-        cell_thickness=np.abs(np.mean(np.diff( self.xr_sv.coords['depth']) ))        
-        
-        track= pd.DataFrame([])
-        track.index= self.xr_sv.coords['time']      
-        track['nasc_swarm'] =4*np.pi*1852**2 * np.nansum( np.power(10, sv_mask /10)*cell_thickness ,axis=0)   
-          
-        # peak filter
-        x = track['nasc_swarm'].values.copy()
-        peaks, peak_meta = find_peaks(x,prominence=10000,width=[0,2] )
-        # x[peaks]=np.nan
-        
-        ix1 = np.round( peak_meta['left_ips']).astype(int)-1
-        ix2 = np.round( peak_meta['right_ips']).astype(int)+1
-        
-        ix1[ix1<0]=0
-        ix2[ix2>len(x)-1]=len(x)-1
-        
-        for i1,i2 in zip(ix1,ix2):
-            x[i1:i2]=np.nan
-
-        track['nasc_swarm']=x
-        track['nasc_swarm']=track['nasc_swarm'].interpolate()
-        
-        # duration =     ( self.xr_sv.coords['time'][-1] - self.xr_sv.coords['time'][0]).data  / np.timedelta64(1, 's')
-        # dm=self.xr_sv.coords['depth'][-1].data
-        
-        
-        self.canvas.fig.clf() 
-                
-        self.ax = self.canvas.fig.subplots(2, 1, gridspec_kw={'height_ratios': [1, 3]},sharex=True)
-        ax=self.ax
-        
-        ax[0].plot( track['nasc_swarm'] , '-k')
-        ax[0].plot( track['nasc_swarm'].resample('1min').mean(), '.-b')
-        
-        
-        ax[0].grid()
-        # ax[0].set_xlim( self.xr_sv.coords['time'].min() , self.xr_sv.coords['time'].max())
-        ax[0].set_ylabel('NASC')
-        
-        # plt.gca=ax[1]
-        
-        x_lims = mdates.date2num( [  self.xr_sv.coords['time'].min().values , self.xr_sv.coords['time'].max().values ])
-        range_max = self.xr_sv.coords['depth'].max()
-        ext=[x_lims[0] ,x_lims[1],-range_max ,0 ]
-        
-        if self.checkbox_raw.isChecked():
-            fname= self.filenames[self.filecounter]
-            self.xr_sv_raw = xr.open_dataarray(fname[:-12] + '_rawechogram.nc')
-            sv_raw = np.squeeze( self.xr_sv_raw[ix_f,:,:])
-            im = ax[1].imshow( sv_raw,cmap= self.choose_color.currentText()   ,aspect='auto',vmin=-90,vmax=-30,extent=ext)
-            
-        else:    
-            im = ax[1].imshow( sv,cmap= self.choose_color.currentText()   ,aspect='auto',vmin=-90,vmax=-30,extent=ext)
-        
-        masked_data = np.ma.masked_where(self.mask_manual == 1, self.mask_manual)
-        
-        
-        ax[1].imshow( masked_data  ,aspect='auto',extent=ext,cmap=self.cmap_mask,alpha=0.3)
-        
-        # cbar3 = plt.colorbar(im)
-        ax[1].xaxis_date()
-        ax[1].grid()
-        ax[1].set_ylabel('Depth in m')
-        ax[1].set_ylim(-self.max_depth_spin.value(),0)
-
-        ax[1].plot(x_lims,[-self.excl_depth_spin.value(),-self.excl_depth_spin.value()] ,'-r' )
-        
-        
-
-        cbaxes = inset_axes(ax[1], width="15%", height="3%", loc='lower left',  bbox_to_anchor=(0.05, 0.15, 1, 1) ,bbox_transform= ax[1].transAxes) 
-        self.canvas.fig.colorbar(im,cax=cbaxes,label='$s_v$', orientation='horizontal')        
-            
-        
-            #         cbaxes = inset_axes(self.canvas.axes4, width="100%", height="100%", loc=3,bbox_to_anchor=(.05, .15, .4, .04),bbox_transform=self.canvas.axes4.transAxes) 
-            # cbar=self.canvas.fig.colorbar(sc,cax=cbaxes, orientation='horizontal')
-            
-            
+from functools import partial
+import multiprocessing  
 
-        self.canvas.fig.tight_layout()
-        self.canvas.draw()
 
-   
-    def choose_freq_changed(self):
-        if self.filecounter>=0:   
-            self.plot_echogram()
+#%% load unet
 
-        
-    def read_file_and_mask(self):    
-        if self.filecounter>=0:        
-            fname= self.filenames[self.filecounter]
-            
-            
-            self.xr_sv = xr.open_dataarray(fname)
-            
-            # breakpoint()
-            
-            f_list = (self.xr_sv.coords['frequency'].values / 1000).astype(int).astype(str)
-            self.choose_freq.clear()
-            self.choose_freq.addItems(f_list)
-            
-            try:
-                ix_120 = np.where( self.xr_sv.coords['frequency'].values==120000)[0][0] 
-            except:
-                ix_120 = np.argmax( self.xr_sv.coords['frequency'].values)
-                
-            
-            self.choose_freq.setCurrentIndex( ix_120 )
-            # self.choose_freq.setCurrentIndex( np.argmax(self.xr_sv.coords['frequency'].values) )
+# from skimage.transform import rescale, resize, downscale_local_mean
+# from skimage import data, filters, measure, morphology
+# from skimage.morphology import (erosion, dilation, opening, closing,  # noqa
+#                                 white_tophat)
+# from skimage.morphology import disk  # noqa
+# import tensorflow as tf
+# from tensorflow import keras
+# from tensorflow.keras import layers
 
-            if os.path.isfile(fname[:-12] + '_mask_manual.h5' ):     
-                self.mask_manual= np.transpose(  pd.read_hdf( fname[:-12] + '_mask_manual.h5',key='df' ) )
-            else:
-                if os.path.isfile(fname[:-12] + '_mask_swarm.h5' ):     
-                    self.mask_swarm= np.transpose(  pd.read_hdf( fname[:-12] + '_mask_swarm.h5',key='df' ) )
-                    self.mask_manual = self.mask_swarm.copy()
-                    ixdepthvalid= ( self.xr_sv.coords['depth'] >= self.excl_depth_spin.value() ) & ( self.xr_sv.coords['depth']  <= self.max_depth_spin.value())
-                    self.mask_manual.values[~ixdepthvalid,:]=False  
-                else:
-                    
-                    s2=len( self.xr_sv.coords['time'])
-                    s1=len( self.xr_sv.coords['depth'])
-                    self.mask_manual=pd.DataFrame( np.ones([s1,s2]).astype(bool)   )
-                    self.mask_manual.columns=self.xr_sv.coords['time']
-                    self.mask_manual.index=self.xr_sv.coords['depth']
-                    ixdepthvalid= ( self.xr_sv.coords['depth'] >= self.excl_depth_spin.value() ) & ( self.xr_sv.coords['depth']  <= self.max_depth_spin.value())
-                    self.mask_manual.values[~ixdepthvalid,:]=False                  
-          
-            self.mask_manual_old=self.mask_manual.copy() 
-  
-                
-            # self.mask_dbdiff= np.transpose( pd.read_hdf( fname[:-12] + '_mask_dbdiff.h5',key='df' ) )
-            
 
-            
-    def undo_mask(self):
-        self.mask_manual=self.mask_manual_old.copy() 
-        self.plot_echogram()            
-
-                
-    def onclick_draw(self,event):
-            # print('%s click: button=%d, x=%d, y=%d, xdata=%f, ydata=%f' %
-            #       ('double' if event.dblclick else 'single', event.button,
-            #        event.x, event.y, event.xdata, event.ydata))
-            if event.button==1 & event.dblclick:
-                self.draw_x=self.draw_x.append( pd.Series(event.xdata) ,ignore_index=True )
-                self.draw_y=self.draw_y.append( pd.Series(event.ydata) ,ignore_index=True )
-                # self.f_limits=self.canvas.axes.get_ylim()
-                # self.t_limits=self.canvas.axes.get_xlim()   
-                
-                line = self.line_2.pop(0)
-                line.remove()        
-                self.line_2 =self.ax[1].plot(self.draw_x,self.draw_y,'.-r')      
-                self.canvas.draw()    
-                         
-                # func_draw_shape_plot()   
-              
-            if event.button==3:
-                self.draw_x=self.draw_x.head(-1)
-                self.draw_y=self.draw_y.head(-1)
-                # self.f_limits=self.canvas.axes.get_ylim()
-                # self.t_limits=self.canvas.axes.get_xlim()
-                # func_draw_shape_plot()              
-                line = self.line_2.pop(0)
-                line.remove()        
-                self.line_2 =self.ax[1].plot(self.draw_x,self.draw_y,'.-r')     
-                self.canvas.draw()                   
- 
-    def mask_removearea(self):
-            
-        # msg = QtWidgets.QMessageBox()
-        # msg.setIcon(QtWidgets.QMessageBox.Information)   
-        # msg.setText("Add points with double left click.\nRemove latest point with single right click. \nExit draw mode by pushing enter")
-        # msg.setStandardButtons(QtWidgets.QMessageBox.Ok | QtWidgets.QMessageBox.Cancel)
-        # returnValue = msg.exec()    
-        # if returnValue == QtWidgets.QMessageBox.Ok:
-            self.butt_removearea.setEnabled(False)   
-            print('drawing')  
-            self.draw_x=pd.Series(dtype='float')
-            self.draw_y=pd.Series(dtype='float')
-            self.d_limits=self.ax[1].get_ylim()
-            self.t_limits=self.ax[1].get_xlim()
-            self.plot_echogram()
-            
-            # self.canvas.fig.canvas.mpl_disconnect(self.cid1)    
-            self.cid2=self.canvas.fig.canvas.mpl_connect('button_press_event', self.onclick_draw)
-            self.line_2 =self.ax[1].plot(self.draw_x,self.draw_y,'.-r')        
-            # self.plot_echogram()   
-            self.drawexitm = QtWidgets.QShortcut(QtCore.Qt.Key_Return, self)
-            self.drawexitm.activated.connect(self.func_draw_shape_exit_remove)  
-         
-    def func_draw_shape_exit_remove(self):
-        # print('save shape' + str(self.draw_x.shape))
-        self.canvas.fig.canvas.mpl_disconnect(self.cid2)
-        ## deactive shortcut
-        self.drawexitm.setEnabled(False)  
-
-        if self.draw_x.shape[0]>2:
-
-            
-            # breakpoint()
-            
-            m = np.transpose( self.mask_manual )
-            t = mdates.date2num( m.index )
-            d = -m.columns 
-            
-
-            kk_t,kk_d=np.meshgrid( t,d)   
-            # kernel=np.zeros( [ k_f.shape[0] ,k_t.shape[0] ] )
-            x, y = kk_t.flatten(), kk_d.flatten()
-            points = np.vstack((x,y)).T 
-            
-            p = MPL_Path(list(zip( self.draw_x.values , self.draw_y.values))) # make a polygon
-            grid = p.contains_points(points)
-            m_shapemask = grid.reshape(kk_t.shape) # now you have a mask with points inside a polygon  
-            self.mask_manual_old=self.mask_manual.copy() 
-            self.mask_manual.values[ m_shapemask ] = False
-                  
-        self.plot_echogram()
-        self.butt_removearea.setEnabled(True)   
-
-         
-    def func_draw_shape_exit_add(self):
-        # print('save shape' + str(self.draw_x.shape))
-        self.canvas.fig.canvas.mpl_disconnect(self.cid2)
-        ## deactive shortcut
-        self.drawexitm.setEnabled(False)  
-
-        if self.draw_x.shape[0]>2:
-
-            # breakpoint()
-            
-            m = np.transpose( self.mask_manual )
-            t = mdates.date2num( m.index )
-            d = -m.columns 
-            
-
-            kk_t,kk_d=np.meshgrid( t,d)   
-            # kernel=np.zeros( [ k_f.shape[0] ,k_t.shape[0] ] )
-            x, y = kk_t.flatten(), kk_d.flatten()
-            points = np.vstack((x,y)).T 
-            
-            p = MPL_Path(list(zip( self.draw_x.values , self.draw_y.values))) # make a polygon
-            grid = p.contains_points(points)
-            m_shapemask = grid.reshape(kk_t.shape) # now you have a mask with points inside a polygon  
-            self.mask_manual_old=self.mask_manual.copy() 
-            self.mask_manual.values[ m_shapemask ] = True
-                  
-        self.plot_echogram()   
-        self.butt_addarea.setEnabled(True)     
-         
-
-
-    def mask_addarea(self):
-        # msg = QtWidgets.QMessageBox()
-        # msg.setIcon(QtWidgets.QMessageBox.Information)   
-        # msg.setText("Add points with double left click.\nRemove latest point with single right click. \nExit draw mode by pushing enter")
-        # msg.setStandardButtons(QtWidgets.QMessageBox.Ok | QtWidgets.QMessageBox.Cancel)
-        # returnValue = msg.exec()    
-        # if returnValue == QtWidgets.QMessageBox.Ok:
-            self.butt_addarea.setEnabled(False)     
-
-            print('drawing')  
-            self.draw_x=pd.Series(dtype='float')
-            self.draw_y=pd.Series(dtype='float')
-            self.d_limits=self.ax[1].get_ylim()
-            self.t_limits=self.ax[1].get_xlim()
-            self.plot_echogram()
-            
-            # self.canvas.fig.canvas.mpl_disconnect(self.cid1)    
-            self.cid2=self.canvas.fig.canvas.mpl_connect('button_press_event', self.onclick_draw)
-            self.line_2 =self.ax[1].plot(self.draw_x,self.draw_y,'.-g')        
-            # self.plot_echogram()   
-            self.drawexitm = QtWidgets.QShortcut(QtCore.Qt.Key_Return, self)
-            self.drawexitm.activated.connect(self.func_draw_shape_exit_add)  
-        
-        
-        
-    def save_changes(self):
-       
-        
-        m = np.transpose( self.mask_manual )
-        fname= self.filenames[self.filecounter]
-        m.to_hdf( fname[:-12] + '_mask_manual.h5',key='df' )
-        
-        # calc nasc
-        ix_f = self.xr_sv.coords['frequency']== int(self.choose_freq.currentText()) *1000
-        sv_mask = np.squeeze( self.xr_sv[ix_f,:,:]).copy()
-        sv_mask.values [~self.mask_manual.values]=np.nan
-
-        cell_thickness=np.abs(np.mean(np.diff( self.xr_sv.coords['depth']) ))        
-        nasc = 4*np.pi*1852**2 * np.nansum( np.power(10, sv_mask /10)*cell_thickness ,axis=0)   
-
-        # peak filter
-        x = nasc.copy()
-        peaks, peak_meta = find_peaks(x,prominence=10000,width=[0,2] )
-        # x[peaks]=np.nan
-       
-        ix1 = np.floor( peak_meta['left_ips']).astype(int)-1
-        ix2 = np.ceil( peak_meta['right_ips']).astype(int)+1         
-        ix1[ix1<0]=0
-        ix2[ix2>len(x)-1]=len(x)-1
-         
-        for i1,i2 in zip(ix1,ix2):
-             x[i1:i2]=np.nan
-        
-        track=  pd.read_hdf( fname[:-12] + '_nasctable.h5',key='df' ) 
-
-        track['nasc_manual']=x
-        track['nasc_manual']=track['nasc_manual'].interpolate()
-
-
-        # track['nasc_manual'] =nasc
-        track.to_hdf( fname[:-12] + '_nasctable.h5',key='df'  )
-        
-        
-        
-    def plot_next(self):
-         if len(self.filenames)>0:
-            print('old filecounter is: '+str(self.filecounter))
-            
-            if self.checkbox_mask.isChecked():
-                self.save_changes()
-                
-           
-            self.filecounter=self.filecounter+1
-            if self.filecounter>len(self.filenames)-1:
-                self.filecounter=len(self.filenames)-1
-                print('That was it')
-            self.read_file_and_mask()
-            self.plot_echogram()
-            
-            
-
-    def plot_prev(self):
-         if len(self.filenames)>0:   
-            print('old filecounter is: '+str(self.filecounter))
-            
-            if self.checkbox_mask.isChecked():
-                self.save_changes()
-
-         
-            self.filecounter=self.filecounter-1
-            if self.filecounter<0:
-                self.filecounter=0
-                print('That was it')
-            # new file    
-            # self.filecounter=self.filecounter+1
-            self.read_file_and_mask()
-            self.plot_echogram()
-                
-         
-     
-######
-             
-
-    def func_quit(self):
-        self.statusBar().setStyleSheet("background-color : k")
-        # self.statusBar().removeWidget(self.label_1)   
-        # self.startautoMenu.setEnabled(True)
-        # self.exitautoMenu.setEnabled(False)     
-        QtWidgets.QApplication.instance().quit()     
-        # QCoreApplication.quit()
-        self.close()    
-        
+# model = tf.keras.models.load_model('tensorflow_unet.h5')
 
+# image_n_pixels = 256
 
+# num_classes=5
 
 
 #%% automatic processing
 
 
 class RepeatTimer(Timer):
     def run(self):
         while not self.finished.wait(self.interval):
             self.function(*self.args, **self.kwargs)
 
 class krillscan_class():
     
-    def inspect(self):
-        app = QtWidgets.QApplication(sys.argv)
-        app.setApplicationName("Krillscan")    
-        app.setStyleSheet(qdarktheme.load_stylesheet())
-        w = MainWindow()
-        sys.exit(app.exec_())
              
     
     def start(self,ini_file):
         print('start')
         self.ini_file = ini_file
         self.callback_process_active=False
         self.callback_email_active=False
@@ -709,20 +125,23 @@
         self.df_files=pd.DataFrame([])
         # self.echogram=pd.DataFrame([])    
         self.positions=pd.DataFrame([])    
         
         config = configparser.ConfigParser()
         config.read(self.ini_file)            
         self.workpath=  str(config['GENERAL']['target_folder'])  
+        os.makedirs(self.workpath, exist_ok=True)
+
         
         print('work dir: ' +os.getcwd())
         print('source dir: ' + str(config['GENERAL']['source_folder'])  )
         print('target dir: ' +self.workpath)
                
-
+        # self.start_para_processing()
+        
         self.timer_process = RepeatTimer(10, self.callback_process_raw)
         self.timer_process.start()
         self.timer_email = RepeatTimer(30, self.callback_email)
         self.timer_email.start()  
         
         # doc.add_periodic_callback( self.callback_process_raw,1000 ) 
         # doc.add_periodic_callback( self.callback_plot,3000 ) 
@@ -733,157 +152,303 @@
         self.timer_process.cancel()
         self.timer_email.cancel()  
         print('Krillscan stopped')
 
 
     def read_raw(self,rawfile):       
         # df_sv=pd.DataFrame( [] )
-        positions=pd.DataFrame( []  )
+        # positions=pd.DataFrame( []  )
                 
         # breakpoint()
         
         # print('Echsounder data are: ')
         self.config = configparser.ConfigParser()
         self.config.read(self.ini_file)   
         
-        # rawfile=r"E:\KRILL-2023\D20230129-T065613.raw"
+        # rawfile=r"C:\Users\a5278\Documents\postdoc_krill\krillscan\source_folder\D20220410-T195719.raw"
         # rawfile=r"./source_folder\D20230128-T105149.raw"
    
         try:     
-            raw_obj = EK80.EK80()
-            raw_obj.read_raw(rawfile)
-            print(raw_obj)
+            ed = ep.open_raw(rawfile, sonar_model='EK80')  # for EK80 file
+            # compute Sv values from raw input data
+            try: 
+                edSv = ep.calibrate.compute_Sv(ed, waveform_mode="CW", encode_mode="complex")
+            except:
+                edSv = ep.calibrate.compute_Sv(ed, waveform_mode="CW", encode_mode="power")
         except Exception as e:            
             print(e)       
             try:     
-                raw_obj = EK60.EK60()
-                raw_obj.read_raw(rawfile)
-                print(raw_obj)
+                ed = ep.open_raw(rawfile, sonar_model='EK60')  # for EK80 file
+                # compute Sv values from raw input data
+                edSv = ep.calibrate.compute_Sv(ed)
             except Exception as e:
                 print(e)       
+    
+                    
+        #breakpoint()                           
+        frequencies = np.unique(edSv.frequency_nominal.values)
+        frequencies = frequencies[~np.isnan(frequencies)]
                 
-                                           
+        # from echopype.commongrid.utils import compute_raw_MVBS
+        # from echopype import open_raw
+        # from echopype.calibrate import compute_Sv
+
+
+
+        # compute Sv values from raw input data
+        # edSv = ep.calibrate.compute_Sv(ed, waveform_mode="CW", encode_mode="power")
+
+        # remove depths>500m for faster processing
+        # edSv = edSv.where(edSv.echo_range < 501, drop = True)
+
+        # Convert the array of depth bins into an interval index
+        edSv['echo_range'].max()
+        
+        maxDepth =         edSv['echo_range'].max()
+
+     
+        # range_interval = pd.IntervalIndex.from_breaks(np.linspace(0, maxDepth, edSv.Sv.shape[2]))
+        # r = np.linspace(0, maxDepth, edSv.Sv.shape[2])
+        
+        r=np.arange( 0 , maxDepth , 0.5 )
+     
+            # t=sv_obj.ping_time
+     
+            
+            
+
+        # range_interval = pd.IntervalIndex.from_breaks(np.arange(0, maxDepth + range_meter_bin, range_meter_bin))
+
+        # time_interval = pd.interval_range(start=pd.to_datetime(edSv["ping_time"].min().values),
+        #                                   end = pd.to_datetime(edSv["ping_time"].max().values), 
+        #                                   freq=pd.Timedelta(seconds = 1))
+        t= edSv["ping_time"].values
+        # resampledSv = ep.commongrid.utils.compute_raw_MVBS(edSv,
+        #             range_interval=range_interval,
+        #             ping_interval= edSv["ping_time"],
+        #             range_var='echo_range')
+        
+        # resampledSv = ep.commongrid.compute_MVBS(
+        #   edSv,
+        #   range_bin='.5m')
+
+        frequencies = np.unique(edSv.frequency_nominal.values)
+        frequencies = frequencies[~np.isnan(frequencies)]
+
+        # extract locations for raw file and save to csv file
+        gps_loc = ed['Platform'][['latitude','longitude']]
+        gps_loc = gps_loc.sortby('time1')
+        gps_loc = gps_loc.drop_duplicates(dim='time1')
+        gps_loc = gps_loc.resample(time1='1s').mean()
+        gps_loc = gps_loc.to_dataframe() 
+        
+        la= np.interp(  edSv["ping_time"].values.astype(float) , gps_loc.index.values.astype(float), gps_loc['latitude'])
+        lo= np.interp(  edSv["ping_time"].values.astype(float) , gps_loc.index.values.astype(float), gps_loc['longitude'])
+        
+        positions = pd.DataFrame([])     
+        positions['ping_time']=edSv["ping_time"].values
+        positions['latitude'] = la
+        positions['longitude'] = lo
+        
+        # positions.index
+        
+        raw_freq= frequencies
+        
+        # breakpoint()
         
-        raw_freq= list(raw_obj.frequency_map.keys())
         
         
         # self.ekdata=dict()
         
         # for f in raw_freq:
         # f=float(self.config['GENERAL']['scrutinization_frequency'])
-        print(raw_freq)
+        # print(raw_freq)
         
         for f in raw_freq:
-            print(raw_obj.frequency_map[f])
+        #     # print(raw_obj.frequency_map[f])
             
-            raw_data = raw_obj.raw_data[raw_obj.frequency_map[f][0]][0]  
-    
-            if np.shape(raw_data)[0]>1:                     
-                cal_obj = raw_data.get_calibration()
-                
-                try: 
-                   cal_obj.gain=float(self.config['CALIBRATION']['gain']       )
-                except:
-                    pass
-                try: 
-                   cal_obj.sa_correction=float(self.config['CALIBRATION']['sa_correction']       )
-                except:
-                    pass
-                try: 
-                   cal_obj.beam_width_alongship=float(self.config['CALIBRATION']['beam_width_alongship']       )
-                except:
-                    pass
-                try: 
-                   cal_obj.beam_width_athwartship=float(self.config['CALIBRATION']['beam_width_athwartship']       )
-                except:
-                    pass
-                try: 
-                   cal_obj.angle_offset_alongship=float(self.config['CALIBRATION']['angle_offset_alongship']       )
-                except:
-                    pass
-                try: 
-                   cal_obj.angle_offset_athwartship=float(self.config['CALIBRATION']['angle_offset_athwartship']       )
-                except:
-                    pass
-                    
-                
-                sv_obj = raw_data.get_sv(calibration = cal_obj)    
-                sv_obj = raw_data.get_sv()    
+        #     # single ping storage issue
+        #     if len( raw_obj.raw_data[raw_obj.frequency_map[f][0]][:]) >1:
+        #           raw_data = raw_obj.raw_data[raw_obj.frequency_map[f][0]][:]  
                   
-                # positions =pd.DataFrame(  raw_obj.nmea_data.interpolate(sv_obj, 'GGA')[1] )
-               
-                svr = np.transpose( 10*np.log10( sv_obj.data ) )
-
-                # print(sv_obj.range.max())
-                # r=np.arange( sv_obj.range.min() , sv_obj.range.max() , 0.5 )
-                r=np.arange( 0 , sv_obj.range.max() , 0.5 )
-        
-                t=sv_obj.ping_time
+        #           # new code:
+        #           maxSamples = max([sublist.n_samples for sublist in raw_data])
+        #           svr = np.empty([maxSamples , raw_obj.n_pings])   
+                   
+        #           for k in range(len(raw_data)):
+        #               svr[list(range(0,(raw_data[k].power.size))),k] = raw_data[k].power
+      
+        #     else:
+            
+        #         raw_data = raw_obj.raw_data[raw_obj.frequency_map[f][0]][0]  
         
-                sv=  resize(svr,[ len(r) , len(t) ] )
-                
-               # print(sv.shape)
-               
-               # Clean impulse noise      
-                sv_im, m120in_ = mIN.wang(sv, thr=(-70,-40), erode=[(3,3)],
-                                dilate=[(7,7)], median=[(7,7)])
-                
-                if f== float(self.config['GENERAL']['scrutinization_frequency'] ):
+        #         if np.shape(raw_data)[0]>1:                     
+        #             cal_obj = raw_data.get_calibration()
+                    
+        #             try: 
+        #                 cal_obj.gain=float(self.config['CALIBRATION']['gain']       )
+        #             except:
+        #                 pass
+        #             try: 
+        #                 cal_obj.sa_correction=float(self.config['CALIBRATION']['sa_correction']       )
+        #             except:
+        #                 pass
+        #             try: 
+        #                 cal_obj.beam_width_alongship=float(self.config['CALIBRATION']['beam_width_alongship']       )
+        #             except:
+        #                 pass
+        #             try: 
+        #                 cal_obj.beam_width_athwartship=float(self.config['CALIBRATION']['beam_width_athwartship']       )
+        #             except:
+        #                 pass
+        #             try: 
+        #                 cal_obj.angle_offset_alongship=float(self.config['CALIBRATION']['angle_offset_alongship']       )
+        #             except:
+        #                 pass
+        #             try: 
+        #                 cal_obj.angle_offset_athwartship=float(self.config['CALIBRATION']['angle_offset_athwartship']       )
+        #             except:
+        #                 pass
+                        
                     
-                    positions =pd.DataFrame(  raw_obj.nmea_data.interpolate(sv_obj, 'GGA')[1] )
+        #             sv_obj = raw_data.get_sv(calibration = cal_obj)    
+        #             # sv_obj = raw_data.get_sv()    
+                      
+        #             # positions =pd.DataFrame(  raw_obj.nmea_data.interpolate(sv_obj, 'GGA')[1] )
+                   
+        #             svr = np.transpose( 10*np.log10( sv_obj.data ) )
 
-                    seafloor_sv_threshold_db = float(self.config['PROCESSING']['seafloor_sv_threshold_db'] )
+        #         # print(sv_obj.range.max())
+        #         # r=np.arange( sv_obj.range.min() , sv_obj.range.max() , 0.5 )
+        #     r=np.arange( 0 , sv_obj.range.max() , 0.5 )
+     
+        #     t=sv_obj.ping_time
+     
+        #     sv=  resize(svr,[ len(r) , len(t) ] )
+             
+            # print(sv.shape)
+            
+            ix_f= f == frequencies
+            svr =np.squeeze(  edSv.Sv[ix_f,:,:].values.T )
+            
+            sv=  resize(svr,[ len(r) , len(t) ] )
 
-                    mb = mSB.ariza(sv, r, r0=10, r1=1000, roff=0,
-                                      thr=seafloor_sv_threshold_db, ec=1, ek=(3,3), dc=10, dk=(5,15))
-                    
-                    print(mb.sum())
-                    # breakpoint()
-                    # sv_im[mb]=-999
-                    
-                    bottomdepth=[]         
-                    for j in range(mb.shape[1]):
-                        row_1=mb[:,j]
-                        if np.sum(row_1==True)>0:
-                            bottomdepth.append( np.min(r[row_1==True]) )
-                        else:
-                            bottomdepth.append( r.max() )
-                    # print(bottomdepth)   
-                    positions['bottomdepth_m']=bottomdepth
 
+            # r =resampledSv.echo_range_bins
+            
+            # edSv.Sv[ix_f,:,:].values.T
+            
+        # fig= plt.figure(0)
+        # plt.clf()     
+        # plt.imshow(edSv.Sv[ix_f,:,:].values.T ,aspect='auto',vmin=-90,vmax=-30)
+        # plt.colorbar()
+        # plt.grid()
+        # plt.tight_layout()
+        # plt.draw()
+        
+        
+        # fig= plt.figure(1)
+        # plt.clf()     
+        # plt.imshow(resampledSv.Sv[ix_f,:,:].T,aspect='auto',vmin=-90,vmax=-30)
+        # plt.colorbar()
+        # plt.grid()
+        # plt.tight_layout()
+        # plt.draw()
 
-                # estimate and correct background noise       
-                p         = np.arange(len(t))                
-                s         = np.arange(len(r))          
-                bn, m120bn_ = gBN.derobertis(sv, s, p, 5, 20, r, np.mean(cal_obj.absorption_coefficient) ) # whats correct absoprtion?
-                b=pd.DataFrame(bn)
-                bn=  b.interpolate(axis=1).interpolate(axis=0).values                        
-                sv_clean     = tf.log(tf.lin(sv_im) - tf.lin(bn))
-              
-                sv_SNR_threshold_db = float(self.config['PROCESSING']['sv_SNR_threshold_db'] )
-                msn             = mSN.derobertis(sv_clean, bn, thr=sv_SNR_threshold_db)
-                sv_clean[msn] = np.nan
+        # fig= plt.figure(1)
+        # plt.clf()     
+        # plt.imshow(mb,aspect='auto')
+        # plt.colorbar()
+        # plt.grid()
+        # plt.tight_layout()
+        # plt.draw()
+        
+        # fig= plt.figure(1)
+        # plt.clf()     
+        # plt.plot(row_1)
+        # plt.grid()
+        # plt.tight_layout()
+        # plt.draw()
+        
+        
+            # breakpoint()
+            # Clean impulse noise      
+            sv_im, m120in_ = mIN.wang(sv, thr=(-90,0), erode=[(3,3)], # thre was -70 to -40 
+                              dilate=[(7,7)], median=[(7,7)])
+             
+            if f== float(self.config['GENERAL']['scrutinization_frequency'] ):
+                 
+                  # positions =pd.DataFrame(  raw_obj.nmea_data.interpolate(sv_obj, 'GGA')[1] )
+
+                  seafloor_sv_threshold_db = float(self.config['PROCESSING']['seafloor_sv_threshold_db'] )
+
+                  mb = mSB.ariza(sv, r, r0=10, r1=1000, roff=0,
+                                    thr=seafloor_sv_threshold_db, ec=1, ek=(3,3), dc=10, dk=(5,15))
+                 
+                  # print(mb.sum())
+                  # breakpoint()
+                  # sv_im[mb]=-999
+                 
+                  bottomdepth=[]         
+                  for j in range(mb.shape[1]):
+                      row_1=mb[:,j]
+                      if np.sum(row_1==True)>0:
+                          bottomdepth.append( np.min(r[row_1==True]) )
+                      else:
+                          bottomdepth.append( r.max() )
+                  # print(bottomdepth)   
+                  positions['bottomdepth_m']=bottomdepth
+
+
+              # estimate and correct background noise       
+            p         = np.arange(len(t))                
+            s         = np.arange(len(r))          
+            
+            
+            bn, m120bn_ = gBN.derobertis(sv, s, p, 5, 20, r, np.mean(edSv["sound_absorption"].values[ix_f]) ) # whats correct absoprtion?
+            b=pd.DataFrame(bn)
+            bn=  b.interpolate(axis=1).interpolate(axis=0).values                        
+            sv_clean     = transform.log(transform.lin(sv_im) - transform.lin(bn))
+           
+            sv_SNR_threshold_db = float(self.config['PROCESSING']['sv_SNR_threshold_db'] )
+            msn             = mSN.derobertis(sv_clean, bn, thr=sv_SNR_threshold_db)
+            sv_clean[msn] = np.nan
 
-              
-                sv_x = xr.DataArray(sv_clean,coords={"time": t,"depth": r},  dims=("depth","time"))
-                
-                # fill holes
-                # sv_x = sv_x.interpolate_na( dim='time', method="linear",max_gap=pd.Timedelta(seconds=2))
-                sv_x = sv_x.interpolate_na( dim='depth', method="linear",max_gap=3)
-               
-                sv_x_raw = xr.DataArray(sv,coords={"time": t,"depth": r},  dims=("depth","time"))
-                # breakpoint()
+           
+            sv_x = xr.DataArray(sv_clean,coords={"time": t,"depth": r},  dims=("depth","time"))
 
+            sv_x=sv_x.expand_dims(dim='frequency')                
+              # fill holes
+              # sv_x = sv_x.interpolate_na( dim='time', method="linear",max_gap=pd.Timedelta(seconds=2))
+            sv_x = sv_x.interpolate_na( dim='depth', method="linear",max_gap=3)
+
+            sv_x_raw = xr.DataArray(sv,coords={"time": t,"depth": r},  dims=("depth","time"))
+            sv_x_raw=sv_x_raw.expand_dims(dim='frequency')                
+              # breakpoint()
+
+        # fig= plt.figure(1)
+        # plt.clf()     
+        # plt.subplot(211)
+        # plt.imshow(sv_x_raw[0,:,:],aspect='auto',vmin=-90,vmax=-30)
+        # plt.colorbar()
+        # plt.grid()
+        # plt.subplot(212)
+        # plt.imshow(sv_x[0,:,:],aspect='auto',vmin=-90,vmax=-30)
+        # plt.colorbar()
+        # plt.grid()
                 
-                if f==raw_freq[0]:
-                    xr_sv=sv_x
-                    xr_sv_raw=sv_x_raw
-                else:
-                    xr_sv = xr.concat([xr_sv,sv_x], dim="frequency")
-                    xr_sv_raw = xr.concat([xr_sv_raw,sv_x_raw], dim="frequency")
+        # plt.tight_layout()
+        # plt.draw()
+             
+            if f==raw_freq[0]:
+                  xr_sv=sv_x
+                  xr_sv_raw=sv_x_raw
+            else:
+                  xr_sv = xr.concat([xr_sv,sv_x], dim="frequency")
+                  xr_sv_raw = xr.concat([xr_sv_raw,sv_x_raw], dim="frequency")
 
                     
         xr_sv.coords['frequency'] = raw_freq
         xr_sv_raw.coords['frequency'] = raw_freq
         
         # duration =     ( xr_sv.coords['time'][-1] - xr_sv.coords['time'][0]).data  / np.timedelta64(1, 's')
         # dm=xr_sv.coords['depth'][-1].data
@@ -905,14 +470,379 @@
         # plt.tight_layout()
         
         # print(xr_sv)
         # print(positions)
                
         return xr_sv, positions , xr_sv_raw
 
+
+    
+    def calc_absorption(self,
+        frequency,
+        temperature=27,
+        salinity=35,
+        pressure=10,
+        pH=8.1,
+        sound_speed=None,
+        formula_source="AM",
+    ):
+        """
+        Calculate sea water absorption in units [dB/m].
+    
+        Parameters
+        ----------
+        frequency: int or numpy array
+            frequency [Hz]
+        temperature: num
+            temperature [deg C]
+        salinity: num
+            salinity [PSU, part per thousand]
+        pressure: num
+            pressure [dbars]
+        pH: num
+            pH of water
+        formula_source: str, {"AM", "FG", "AZFP"}
+            Source of formula used to calculate sound speed.
+            "AM" (default) uses the formula from Ainslie and McColm (1998).
+            "FG" uses the formula from Francois and Garrison (1982).
+            "AZFP" uses the the formula supplied in the AZFP Matlab code.
+            See Notes below for the references.
+    
+        Returns
+        -------
+        Sea water absorption [dB/m].
+    
+        Notes
+        -----
+        Ainslie MA, McColm JG. (1998). A simplified formula for viscous
+        and chemical absorption in sea water.
+        The Journal of the Acoustical Society of America, 103(3), 1671–1672.
+        https://doi.org/10.1121/1.421258
+    
+        Francois RE, Garrison GR. (1982). Sound absorption based on
+        ocean measurements. Part II: Boric acid contribution and equation
+        for total absorption.
+        The Journal of the Acoustical Society of America, 72(6), 1879–1890.
+        https://doi.org/10.1121/1.388673
+    
+        The accuracy of the simplified formula from Ainslie & McColm 1998
+        compared with the original complicated formula from Francois & Garrison 1982
+        was demonstrated between 100 Hz and 1 MHz.
+        """
+        if formula_source == "FG":
+            f = frequency / 1000.0  # convert from Hz to kHz due to formula
+            if sound_speed is None:
+                c = 1412.0 + 3.21 * temperature + 1.19 * salinity + 0.0167 * pressure
+            else:
+                c = sound_speed
+            A1 = 8.86 / c * 10 ** (0.78 * pH - 5)
+            P1 = 1.0
+            f1 = 2.8 * np.sqrt(salinity / 35) * 10 ** (4 - 1245 / (temperature + 273))
+            A2 = 21.44 * salinity / c * (1 + 0.025 * temperature)
+            P2 = 1.0 - 1.37e-4 * pressure + 6.2e-9 * pressure**2
+            f2 = 8.17 * 10 ** (8 - 1990 / (temperature + 273)) / (1 + 0.0018 * (salinity - 35))
+            P3 = 1.0 - 3.83e-5 * pressure + 4.9e-10 * pressure**2
+            if np.all(temperature < 20):
+                A3 = (
+                    4.937e-4
+                    - 2.59e-5 * temperature
+                    + 9.11e-7 * temperature**2
+                    - 1.5e-8 * temperature**3
+                )
+            else:
+                A3 = (
+                    3.964e-4
+                    - 1.146e-5 * temperature
+                    + 1.45e-7 * temperature**2
+                    - 6.5e-10 * temperature**3
+                )
+            a = (
+                A1 * P1 * f1 * f**2 / (f**2 + f1**2)
+                + A2 * P2 * f2 * f**2 / (f**2 + f2**2)
+                + A3 * P3 * f**2
+            )
+            sea_abs = a / 1000  # formula output is in unit [dB/km]
+    
+        elif formula_source == "AM":
+            freq = frequency / 1000
+            D = pressure / 1000
+            f1 = 0.78 * np.sqrt(salinity / 35) * np.exp(temperature / 26)
+            f2 = 42 * np.exp(temperature / 17)
+            a1 = 0.106 * (f1 * (freq**2)) / ((f1**2) + (freq**2)) * np.exp((pH - 8) / 0.56)
+            a2 = (
+                0.52
+                * (1 + temperature / 43)
+                * (salinity / 35)
+                * (f2 * (freq**2))
+                / ((f2**2) + (freq**2))
+                * np.exp(-D / 6)
+            )
+            a3 = 0.00049 * freq**2 * np.exp(-(temperature / 27 + D))
+            sea_abs = (a1 + a2 + a3) / 1000  # convert to db/m from db/km
+    
+        elif formula_source == "AZFP":
+            temp_k = temperature + 273.0
+            f1 = 1320.0 * temp_k * np.exp(-1700 / temp_k)
+            f2 = 1.55e7 * temp_k * np.exp(-3052 / temp_k)
+    
+            # Coefficients for absorption calculations
+            k = 1 + pressure / 10.0
+            a = 8.95e-8 * (1 + temperature * (2.29e-2 - 5.08e-4 * temperature))
+            b = (
+                (salinity / 35.0)
+                * 4.88e-7
+                * (1 + 0.0134 * temperature)
+                * (1 - 0.00103 * k + 3.7e-7 * k**2)
+            )
+            c = (
+                4.86e-13
+                * (1 + temperature * (-0.042 + temperature * (8.53e-4 - temperature * 6.23e-6)))
+                * (1 + k * (-3.84e-4 + k * 7.57e-8))
+            )
+            if salinity == 0:
+                sea_abs = c * frequency**2
+            else:
+                sea_abs = (
+                    (a * f1 * frequency**2) / (f1**2 + frequency**2)
+                    + (b * f2 * frequency**2) / (f2**2 + frequency**2)
+                    + c * frequency**2
+                )
+        else:
+            ValueError("Unknown formula source")
+    
+        return sea_abs
+
+
+    def parafunc(self,ini_file,df_files,index ):
+        
+        
+        config = configparser.ConfigParser()
+        config.read(ini_file)   
+        
+        row = df_files.iloc[ index ,:]
+
+        rawfile=row['path']
+        print('working on '+rawfile)
+        try:
+            
+            echogram_file, positions_file , echogram_file_raw = self.read_raw(rawfile)
+           
+            # df_nasc_file, mask_swarm, mask_dbdiff = self.detect_krill_swarms(echogram_file,positions_file)   
+            # df_nasc_file, mask_swarm, mask_dbdiff,segmentation_unet  = self.detect_krill_swarms(echogram_file,echogram_file_raw,positions_file)   
+            # mask_unet= segmentation_unet==1
+            df_nasc_file, mask_swarm, mask_dbdiff  = self.detect_krill_swarms(echogram_file,echogram_file_raw,positions_file)   
+            
+            name = os.path.basename( rawfile )
+            # name = t.min().strftime('D%Y%m%d-T%H%M%S' )         
+            print('saving: '+name)
+            # df_sv_swarm[ new_echogram==-999 ] =-999
+            
+            workpath=  str(config['GENERAL']['target_folder'])  
+                        
+            df_nasc_file.to_hdf(workpath+'/'+ name + '_nasctable.h5', key='df', mode='w'  )
+            
+                        # add mask info to xarray
+            t_mask= echogram_file.coords['time']
+            r= echogram_file.coords['depth']
+            
+            # if len(np.shape(mask_dbdiff))>1:
+
+            #     mas = np.stack([mask_swarm,mask_unet,mask_dbdiff],axis=-1)
+            #     nc_masks = xr.DataArray(mas,coords={"time": t_mask,"depth": r,"method": ['Swarms','U-NET','dBdiff']},  dims=("depth","time","method"))
+            # else:
+            #     mas = np.stack([mask_swarm,mask_unet],axis=-1)
+            #     nc_masks = xr.DataArray(mas,coords={"time": t_mask,"depth": r,"method": ['Swarms','U-NET']},  dims=("depth","time","method"))
+            # nc_masks.to_netcdf(self.workpath+'/'+ name + '_krill_masks.nc')             
+            if len(np.shape(mask_dbdiff))>1:
+
+                mas = np.stack([mask_swarm,mask_dbdiff],axis=-1)
+                nc_masks = xr.DataArray(mas,coords={"time": t_mask,"depth": r,"method": ['Swarms','dBdiff']},  dims=("depth","time","method"))
+            else:
+                mas = np.stack([mask_swarm],axis=-1)
+                nc_masks = xr.DataArray(mas,coords={"time": t_mask,"depth": r,"method": ['Swarms']},  dims=("depth","time","method"))
+            nc_masks.to_netcdf(self.workpath+'/'+ name + '_krill_masks.nc')             
+
+
+            
+            # dffloat=df_nasc_file.copy()
+            # formats = {'lat': "{:.6f}", 'lon': "{:.6f}", 'distance_m': "{:.4f}",'bottomdepth_m': "{:.1f}",'nasc_swarm': "{:.2f}",'nasc_dbdiff': "{:.2f}"}
+            # for col, f in formats.items():
+            #     dffloat[col] = dffloat[col].map(lambda x: f.format(x))                           
+            # # dffloat.to_csv( name + '_nasctable.gzip',compression='gzip' )
+            # dffloat.to_csv(workpath+'/'+ name + '_nasctable.csv')
+            
+            # df_sv_swarm.astype('float16').to_hdf(self.workpath+'/'+ name + '_sv_swarm.h5', key='df', mode='w'  )
+            
+
+            # df_mask = pd.DataFrame( np.transpose(mask_swarm))
+            # df_mask.index=t_mask
+            # df_mask.columns=r
+            # df_mask.astype('bool').to_hdf(workpath+'/'+ name + '_mask_swarm.h5', key='df', mode='w'  )
+            # if bool(int(config['PROCESSING']['write_mask_as_csv'])) :
+            #     df_mask.astype('int').to_csv(workpath+'/'+ name + '_mask_swarm.csv' )
+
+            # if len(np.shape(mask_dbdiff))>1:
+            #     df_mask = pd.DataFrame( np.transpose(mask_dbdiff))
+            #     df_mask.index=t_mask
+            #     df_mask.columns=r
+            #     df_mask.astype('bool').to_hdf(workpath+'/'+ name + '_mask_dbdiff.h5', key='df', mode='w'  )
+            #     if bool(int(config['PROCESSING']['write_mask_as_csv'])) :
+            #         df_mask.astype('int').to_csv(workpath+'/'+ name + '_mask_dbdiff.csv' )
+
+
+            
+            echogram_file.to_netcdf(workpath+'/'+ name + '_echogram.nc')    
+            echogram_file_raw.to_netcdf(workpath+'/'+ name + '_rawechogram.nc')    
+                        
+        except Exception as e:
+            print(e)               
+            print(traceback.format_exc())
+            
+    def start_para_processing(self,ini_file):
+        
+        print('start')
+        # ini_file = ini_file
+        self.ini_file = ini_file
+
+        df_files=pd.DataFrame([])
+        positions=pd.DataFrame([])    
+        
+        config = configparser.ConfigParser()
+        config.read(self.ini_file)            
+        workpath=  str(config['GENERAL']['target_folder'])  
+        folder_source=  str(config['GENERAL']['source_folder'])  
+       
+        print('work dir: ' +os.getcwd())
+        print('source dir: ' + str(config['GENERAL']['source_folder'])  )
+        print('target dir: ' +workpath)
+               
+        # self.start_para_processing()
+         
+        new_df_files = pd.DataFrame([])   
+
+        globstr =  os.path.join( glob.escape( folder_source),'*.raw')           
+        new_df_files['path'] = glob.glob( globstr )  
+        print('found '+str(len(new_df_files)) + ' raw files')
+    
+        dates=[]
+        for fname in new_df_files['path']:
+            
+            datetimestring=re.search('D\d\d\d\d\d\d\d\d-T\d\d\d\d\d\d',fname).group()
+            dates.append( pd.to_datetime( datetimestring,format='D%Y%m%d-T%H%M%S' ) )
+        new_df_files['date'] = dates
+    
+    
+        new_df_files['to_do']=True 
+        
+        
+        df_files=pd.concat([df_files,new_df_files])
+        df_files.drop_duplicates(inplace=True)
+        
+        df_files =  df_files.sort_values('date')
+        df_files=df_files.reset_index(drop=True)
+        
+
+        # look for already processed data
+        df_files['to_do']=True    
+        
+        if os.path.isfile(workpath+'/list_of_rawfiles.csv'):
+            df_files_done =  pd.read_csv(workpath+'/list_of_rawfiles.csv',index_col=0)
+            df_files_done=df_files_done.loc[ df_files_done['to_do']==False,: ]
+        
+            names = df_files['path'].apply(lambda x: Path(x).stem)       
+            names_done = df_files_done['path'].apply(lambda x: Path(x).stem)  
+            # breakpoint()
+            
+        # print(names)
+        # print(nasc_done)
+            ix_done= names.isin( names_done  )  
+    
+        # print(ix_done)
+            df_files.loc[ix_done,'to_do'] = False        
+        n_todo=np.sum(df_files['to_do'])
+        print('To do: ' + str(n_todo))
+                
+        # unit_length_min=pd.to_timedelta(10,'min')
+        
+        ix_todo = np.where( df_files['to_do']==True )[0]
+        
+        # breakpoint()
+        
+        ###### parallel processing
+        
+        print( __name__  )
+        if __name__ == 'krillscan.process':
+            cpucounts=multiprocessing.cpu_count()
+            pool = multiprocessing.Pool(processes=cpucounts)
+            index_list=ix_todo
+            pool.map( partial( self.parafunc,ini_file,  df_files), index_list)
+            pool.close   
+
+    def file2netcdf(self,inifile,rawfile):
+        self.ini_file =inifile
+        
+        self.config = configparser.ConfigParser()
+        self.config.read(inifile)   
+        
+        print('working on '+rawfile)
+        try:
+            
+            echogram_file, positions_file , echogram_file_raw = self.read_raw(rawfile)
+           
+            df_nasc_file, mask_swarm, mask_dbdiff = self.detect_krill_swarms(echogram_file,positions_file)   
+            
+            
+            name = os.path.basename( rawfile )
+            # name = t.min().strftime('D%Y%m%d-T%H%M%S' )         
+            print('saving: '+name)
+            # df_sv_swarm[ new_echogram==-999 ] =-999
+            
+            workpath=  str(self.config['GENERAL']['target_folder'])  
+                        
+            df_nasc_file.to_hdf(workpath+'/'+ name + '_nasctable.h5', key='df', mode='w'  )
+            
+            dffloat=df_nasc_file.copy()
+            formats = {'lat': "{:.6f}", 'lon': "{:.6f}", 'distance_m': "{:.4f}",'bottomdepth_m': "{:.1f}",'nasc_swarm': "{:.2f}",'nasc_dbdiff': "{:.2f}"}
+            for col, f in formats.items():
+                dffloat[col] = dffloat[col].map(lambda x: f.format(x))                           
+            # dffloat.to_csv( name + '_nasctable.gzip',compression='gzip' )
+            dffloat.to_csv(workpath+'/'+ name + '_nasctable.csv')
+            
+            # df_sv_swarm.astype('float16').to_hdf(self.workpath+'/'+ name + '_sv_swarm.h5', key='df', mode='w'  )
+            
+            # add mask info to xarray
+            t_mask= echogram_file.coords['time']
+            r= echogram_file.coords['depth']
+            
+            df_mask = pd.DataFrame( np.transpose(mask_swarm))
+            df_mask.index=t_mask
+            df_mask.columns=r
+            df_mask.astype('bool').to_hdf(workpath+'/'+ name + '_mask_swarm.h5', key='df', mode='w'  )
+            if bool(int(self.config['PROCESSING']['write_mask_as_csv'])) :
+                df_mask.astype('int').to_csv(workpath+'/'+ name + '_mask_swarm.csv' )
+
+            if len(np.shape(mask_dbdiff))>1:
+                df_mask = pd.DataFrame( np.transpose(mask_dbdiff))
+                df_mask.index=t_mask
+                df_mask.columns=r
+                df_mask.astype('bool').to_hdf(workpath+'/'+ name + '_mask_dbdiff.h5', key='df', mode='w'  )
+                if bool(int(self.config['PROCESSING']['write_mask_as_csv'])) :
+                    df_mask.astype('int').to_csv(workpath+'/'+ name + '_mask_dbdiff.csv' )
+
+
+            
+            echogram_file.to_netcdf(workpath+'/'+ name + '_echogram.nc')    
+            echogram_file_raw.to_netcdf(workpath+'/'+ name + '_rawechogram.nc')    
+                        
+        except Exception as e:
+            print(e)               
+            print(traceback.format_exc())
+            
+
+                    
     def callback_process_raw(self):
               
       config = configparser.ConfigParser()
       config.read(self.ini_file)            
       self.folder_source=  str(config['GENERAL']['source_folder'])  
         
       if (self.callback_process_active==False) :
@@ -967,14 +897,16 @@
         
         # echogram=pd.DataFrame([])    
         # positions=pd.DataFrame([])    
         
         unit_length_min=pd.to_timedelta(10,'min')
         
         ix_todo = np.where( self.df_files['to_do']==True )[0]
+        
+        
         if self.n_todo>0:
                 index = ix_todo[0]
                 row = self.df_files.iloc[ index ,:]
 
         # for index, row in self.df_files.iterrows():
         #     if self.toggle_proc.active & (row['to_do']==True):
                 rawfile=row['path']
@@ -994,21 +926,24 @@
                         self.echogram_raw=echogram_file_raw
                                             
                     # self.echogram = pd.concat([ self.echogram,echogram_file ])
                     
                     
                     self.positions = pd.concat([ self.positions,positions_file ])
                     self.positions=self.positions.reset_index(drop=True)
+                    
+                    # breakpoint()
+
+                    
                     # t=pd.to_datetime( self.echogram.coords['time'].data )
                     t=pd.to_datetime( self.positions['ping_time'].values )
                     
-                    # breakpoint()
                     # print(echogram)
                     
-                    # print( [ t.max() , t.min() ])
+                    print( [ t.min() , t.max() ])
                     
                     while (t.max() - t.min()) > unit_length_min:
                         
                         print( (t.max() - t.min())  )
                         
                         # print(  (t.min() + unit_length_min) > t)
                         ix_end = np.where( (t.min() + unit_length_min) > t )[0][-1]
@@ -1034,57 +969,99 @@
                             self.echogram = self.echogram[:,:,ix_end+1:]
                             self.positions = self.positions.iloc[ix_end+1:,:]
                             self.echogram_raw = self.echogram_raw[:,:,ix_end+1:]
 
                             t=pd.to_datetime( self.positions['ping_time'].values )
     
                             # try:
-                            df_nasc_file, mask_swarm, mask_dbdiff = self.detect_krill_swarms(new_echogram,new_positions)   
+                            # df_nasc_file, mask_swarm, mask_dbdiff,segmentation_unet,segmentation_unet_and_shapes  = self.detect_krill_swarms(new_echogram,new_echogram_raw,new_positions)   
+                            # mask_unet= segmentation_unet==1
+                            # mask_unet_and_shapes= segmentation_unet_and_shapes==1
+                            df_nasc_file, mask_swarm, mask_dbdiff  = self.detect_krill_swarms(new_echogram,new_echogram_raw,new_positions)   
                             
+
                             name = new_positions['ping_time'].min().strftime('D%Y%m%d-T%H%M%S' )    
                             # name = t.min().strftime('D%Y%m%d-T%H%M%S' )         
                             print('saving: '+name)
                             # df_sv_swarm[ new_echogram==-999 ] =-999
                             
+                            ###### save mask png
+                            # cat_upsample=segmentation_unet.astype('uint8')
+                            
+                            # nam = self.workpath+'/'+ name + '_segmentation.png'                            
+                            # im = Image.fromarray(cat_upsample *50)
+                            # im.save( nam )
+
+                            #####
                                                     
                             df_nasc_file.to_hdf(self.workpath+'/'+ name + '_nasctable.h5', key='df', mode='w'  )
                             
                             dffloat=df_nasc_file.copy()
+                            # formats = {'lat': "{:.6f}", 'lon': "{:.6f}", 'distance_m': "{:.4f}",'bottomdepth_m': "{:.1f}",'nasc_swarm': "{:.2f}",'nasc_dbdiff': "{:.2f}",'nasc_unet': "{:.2f}"}
                             formats = {'lat': "{:.6f}", 'lon': "{:.6f}", 'distance_m': "{:.4f}",'bottomdepth_m': "{:.1f}",'nasc_swarm': "{:.2f}",'nasc_dbdiff': "{:.2f}"}
                             for col, f in formats.items():
                                 dffloat[col] = dffloat[col].map(lambda x: f.format(x))                           
                             # dffloat.to_csv( name + '_nasctable.gzip',compression='gzip' )
                             dffloat.to_csv(self.workpath+'/'+ name + '_nasctable.csv')
                             
                             # df_sv_swarm.astype('float16').to_hdf(self.workpath+'/'+ name + '_sv_swarm.h5', key='df', mode='w'  )
                             
                             # add mask info to xarray
                             t_mask= new_echogram.coords['time']
                             r= new_echogram.coords['depth']
                             
-                            df_mask = pd.DataFrame( np.transpose(mask_swarm))
-                            df_mask.index=t_mask
-                            df_mask.columns=r
-                            df_mask.astype('bool').to_hdf(self.workpath+'/'+ name + '_mask_swarm.h5', key='df', mode='w'  )
+                            # df_mask = pd.DataFrame( np.transpose(mask_swarm))
+                            # df_mask.index=t_mask
+                            # df_mask.columns=r
+                            # df_mask.astype('bool').to_hdf(self.workpath+'/'+ name + '_mask_swarm.h5', key='df', mode='w'  )
+                            # if bool(int(config['PROCESSING']['write_mask_as_csv'])) :
+                            #     df_mask.astype('int').to_csv(self.workpath+'/'+ name + '_mask_swarm.csv' )
                                
+                            ### U-NET
+                            # df_mask = pd.DataFrame( np.transpose(mask_unet))
+                            # df_mask.index=t_mask
+                            # df_mask.columns=r
+                            # df_mask.astype('bool').to_hdf(self.workpath+'/'+ name + '_mask_unet.h5', key='df', mode='w'  )
+                       
+                            
                             
-                            # xx = xr.DataArray(mask_swarm,coords={"time": t,"depth": r,"frequency": 0},  dims=("depth","time"))
                             # new_echogram = xr.concat([new_echogram,xx], dim="frequency")
                             
                             
-                            if len(np.shape(mask_dbdiff))>1:
-                                df_mask = pd.DataFrame( np.transpose(mask_dbdiff))
-                                df_mask.index=t_mask
-                                df_mask.columns=r
-                                df_mask.astype('bool').to_hdf(self.workpath+'/'+ name + '_mask_dbdiff.h5', key='df', mode='w'  )
-                                
+                            # if len(np.shape(mask_dbdiff))>1:
+                            #     df_mask = pd.DataFrame( np.transpose(mask_dbdiff))
+                            #     df_mask.index=t_mask
+                            #     df_mask.columns=r
+                            #     df_mask.astype('bool').to_hdf(self.workpath+'/'+ name + '_mask_dbdiff.h5', key='df', mode='w'  )
+                               
+                            #     if bool(int(config['PROCESSING']['write_mask_as_csv'])) :
+                            #         df_mask.astype('int').to_csv(self.workpath+'/'+ name + '_mask_dbdiff.csv' )
+       
                             #    xx = xr.DataArray(mask_dbdiff,coords={"time": t,"depth": r,"frequency": 1},  dims=("depth","time"))
                             #    new_echogram = xr.concat([new_echogram,xx], dim="frequency")
-                                                         
+                                          
+                            # breakpoint()
+                            if len(np.shape(mask_dbdiff))>1:
+
+                                mas = np.stack([mask_swarm,mask_dbdiff],axis=-1)
+                                nc_masks = xr.DataArray(mas,coords={"time": t_mask,"depth": r,"method": ['Swarms','dBdiff']},  dims=("depth","time","method"))
+                            else:
+                                mas = np.stack([mask_swarm],axis=-1)
+                                nc_masks = xr.DataArray(mas,coords={"time": t_mask,"depth": r,"method": ['Swarms']},  dims=("depth","time","method"))
+                            nc_masks.to_netcdf(self.workpath+'/'+ name + '_krill_masks.nc')             
                             
+                            # if len(np.shape(mask_dbdiff))>1:
+
+                            #     mas = np.stack([mask_swarm,mask_unet,mask_unet_and_shapes,mask_dbdiff],axis=-1)
+                            #     nc_masks = xr.DataArray(mas,coords={"time": t_mask,"depth": r,"method": ['Swarms','U-NET','U-NET and Swarms','dBdiff']},  dims=("depth","time","method"))
+                            # else:
+                            #     mas = np.stack([mask_swarm,mask_unet,mask_unet_and_shapes],axis=-1)
+                            #     nc_masks = xr.DataArray(mas,coords={"time": t_mask,"depth": r,"method": ['Swarms','U-NET','U-NET and Swarms']},  dims=("depth","time","method"))
+                            # nc_masks.to_netcdf(self.workpath+'/'+ name + '_krill_masks.nc')             
+
                             
                             new_echogram.to_netcdf(self.workpath+'/'+ name + '_echogram.nc')    
                             new_echogram_raw.to_netcdf(self.workpath+'/'+ name + '_rawechogram.nc')    
                             # self.df_files.loc[i,'to_do'] = False
                             # except Exception as e:
                             #   print(e)                      
                     self.df_files.loc[index,'to_do']=False            
@@ -1100,167 +1077,322 @@
                     self.df_files.drop_duplicates(inplace=True)
                     self.df_files=self.df_files.reset_index(drop=True)
                     self.df_files.to_csv(self.workpath+'/list_of_rawfiles.csv')                    
                     
                     
         self.callback_process_active==False
                 
-    def detect_krill_swarms(self,xr_sv,positions):
-         # sv= self.echodata[rawfile][ 120000.0] 
-         # sv= self.ekdata[ 120000.0]          
-         # 
-         # breakpoint()
-         
-         config = configparser.ConfigParser()
-         config.read(self.ini_file)            
-         f=float(config['GENERAL']['scrutinization_frequency'])
+    def detect_krill_swarms(self,xr_sv,xr_sv_raw,positions):
+          # sv= self.echodata[rawfile][ 120000.0] 
+          # sv= self.ekdata[ 120000.0]          
+          # 
+          # breakpoint()
+         
+          config = configparser.ConfigParser()
+          config.read(self.ini_file)            
+          f=float(config['GENERAL']['scrutinization_frequency'])
                   
-         surface_exclusion_depth_m    = float(self.config['PROCESSING']['surface_exclusion_depth_m'] )
-         maximum_depth_m    = float(self.config['PROCESSING']['maximum_depth_m'] )
+          surface_exclusion_depth_m    = float(self.config['PROCESSING']['surface_exclusion_depth_m'] )
+          maximum_depth_m    = float(self.config['PROCESSING']['maximum_depth_m'] )
 
          
             
-         t120 =xr_sv.coords['time'].data
-         r120 =xr_sv.coords['depth'].data
+          t120 =xr_sv.coords['time'].data
+          r120 =xr_sv.coords['depth'].data
          
-         # xr_sv.sel(frequency=f).data
+          # xr_sv.sel(frequency=f).data
 
-         Sv120= xr_sv.sel(frequency=f).data.copy() 
+          Sv120= xr_sv.sel(frequency=f).data.copy() 
          
-         # bottom = self.bottom_detection(Sv120,-38,0)
-         # positions['bottom_depth'] = np.take(  r120,bottom.astype(int)  )
+          # bottom = self.bottom_detection(Sv120,-38,0)
+          # positions['bottom_depth'] = np.take(  r120,bottom.astype(int)  )
 
-         # remove bttom
+          # remove bttom
          
-         for i in range(len(t120)):
+          for i in range(len(t120)):
               ix_na = r120>=  positions['bottomdepth_m'].values[i] 
               Sv120[ix_na,i]=-999
 
           # plt.figure(0)
           # plt.clf()
           # plt.imshow(Sv120,aspect='auto',vmin=-80)
           # plt.plot( np.arange(len(bottom)), bottom,'-r')
           # plt.colorbar()
           # plt.draw()
           # plt.savefig('t.png')
        
-         # breakpoint()
+          # breakpoint()
          
-         # # get mask for seabed
-         # sv2 = Sv120.copy()
-         # sv2[np.isnan(sv2)]=-999
+          # # get mask for seabed
+          # sv2 = Sv120.copy()
+          # sv2[np.isnan(sv2)]=-999
          
-         # mb = mSB.ariza(sv2, r120, r0=20, r1=1000, roff=0,
-         #                  thr=-38, ec=1, ek=(3,3), dc=10, dk=(5,15))
+          # mb = mSB.ariza(sv2, r120, r0=20, r1=1000, roff=0,
+          #                  thr=-38, ec=1, ek=(3,3), dc=10, dk=(5,15))
          
-         # print('bottom='+str(mb.sum()))
-         # Sv120[mb]=-999
+          # print('bottom='+str(mb.sum()))
+          # Sv120[mb]=-999
         
-         ## swarm method
+          ## swarm method
 
-         swarm_sv_threshold_db  = float(self.config['PROCESSING']['swarm_sv_threshold_db'] )
+          swarm_sv_threshold_db  = float(self.config['PROCESSING']['swarm_sv_threshold_db'] )
 
-         # get swarms mask
-         k = np.ones((3, 3))/3**2
-         Sv120cvv = tf.log(convolve2d(tf.lin( Sv120 ), k,'same',boundary='symm'))   
+          # get swarms mask
+          k = np.ones((3, 3))/3**2
+          Sv120cvv = transform.log(convolve2d(transform.lin( Sv120 ), k,'same',boundary='symm'))   
  
-         p120           = np.arange(np.shape(Sv120cvv)[1]+1 )                 
-         s120           = np.arange(np.shape(Sv120cvv)[0]+1 )           
-         m120sh, m120sh_ = mSH.echoview(Sv120cvv, s120, p120, thr=swarm_sv_threshold_db ,
+          p120           = np.arange(np.shape(Sv120cvv)[1]+1 )                 
+          s120           = np.arange(np.shape(Sv120cvv)[0]+1 )           
+          m120sh, m120sh_ = mSH.echoview(Sv120cvv, s120, p120, thr=swarm_sv_threshold_db ,
                                     mincan=(3,10), maxlink=(3,15), minsho=(3,15))
 
-         Sv120sw =  Sv120.copy()
-         mask_swarm = m120sh.copy()
+          Sv120sw =  Sv120.copy()
+          mask_swarm = m120sh.copy()
   
-         # Sv120sw[~m120sh] = np.nan  
-         # ixdepthvalid= (r120>=20) & (r120<=500)
-         # Sv120sw[ ~ixdepthvalid,: ] =np.nan 
+          # Sv120sw[~m120sh] = np.nan  
+          # ixdepthvalid= (r120>=20) & (r120<=500)
+          # Sv120sw[ ~ixdepthvalid,: ] =np.nan 
          
-         Sv120sw[~m120sh] = -999  
-         ixdepthvalid= (r120>=surface_exclusion_depth_m) & (r120<=maximum_depth_m )
-         Sv120sw[ ~ixdepthvalid,: ] =-999          
+          Sv120sw[~m120sh] = -999  
+          ixdepthvalid= (r120>=surface_exclusion_depth_m) & (r120<=maximum_depth_m )
+          Sv120sw[ ~ixdepthvalid,: ] =-999          
          
-         cell_thickness=np.abs(np.mean(np.diff( r120) ))               
+          cell_thickness=np.abs(np.mean(np.diff( r120) ))               
 
-         r_new = np.arange(0,r120.max(),10)
-         # t_new= np.arange(0,Sv120sw.shape[1],10)
+          r_new = np.arange(0,r120.max(),10)
+          # t_new= np.arange(0,Sv120sw.shape[1],10)
         
         
-         sv_lin=np.power(10, Sv120sw /10)
+          sv_lin=np.power(10, Sv120sw /10)
         
-         sv_downsampled=  resize_local_mean(sv_lin,[ len(r_new) , Sv120sw.shape[1] ] ,grid_mode =True)
+          sv_downsampled=  resize_local_mean(sv_lin,[ len(r_new) , Sv120sw.shape[1] ] ,grid_mode =True)
 
-         sv_dep=np.transpose(  np.tile(r_new,[sv_downsampled.shape[1],1] ) )
+          sv_dep=np.transpose(  np.tile(r_new,[sv_downsampled.shape[1],1] ) )
                           
-         sa =  integrate.trapezoid(sv_downsampled,sv_dep,axis=0)  
-         nasc_swarm =  4*np.pi*1852**2 * sa
+          sa =  integrate.trapezoid(sv_downsampled,sv_dep,axis=0)  
+          nasc_swarm_rs =  4*np.pi*1852**2 * sa
          
-         nasc_swarm_rs =nasc_swarm
+          # nasc_swarm_rs =nasc_swarm
 
 
-         df_sv_swarm=pd.DataFrame( np.transpose(Sv120) )
-         df_sv_swarm.index=t120
-         df_sv_swarm.columns=r120
+          df_sv_swarm=pd.DataFrame( np.transpose(Sv120) )
+          df_sv_swarm.index=t120
+          df_sv_swarm.columns=r120
           # print('df_sv')
          
-         df_nasc_file=pd.DataFrame([])
-         # df_nasc_file['time']=positions['ping_time']
-         df_nasc_file['lat']=positions['latitude']
-         df_nasc_file['lon']=positions['longitude']
-         df_nasc_file['distance_m']=np.append(np.array([0]),geod.line_lengths(lons=positions['longitude'],lats=positions['latitude']) )
-         df_nasc_file['bottomdepth_m']=positions['bottomdepth_m']
-         
-         # # breakpoint()
-         # bottomdepth=[]         
-         # for j in range(Sv120.shape[1]):
-         #     row_1=Sv120[:,j]
-         #     if np.sum(row_1==-999)>0:
-         #         bottomdepth.append( np.min(r120[row_1==-999]) )
-         #     else:
-         #         bottomdepth.append( r120.max() )
-         # # print(bottomdepth)   
-         # df_nasc_file['bottomdepth_m']=bottomdepth
+          df_nasc_file=pd.DataFrame([])
+          # df_nasc_file['time']=positions['ping_time']
+          df_nasc_file['lat']=positions['latitude']
+          df_nasc_file['lon']=positions['longitude']
+          df_nasc_file['distance_m']=np.append(np.array([0]),geod.line_lengths(lons=positions['longitude'],lats=positions['latitude']) )
+          df_nasc_file['bottomdepth_m']=positions['bottomdepth_m']
+         
+          # # breakpoint()
+          # bottomdepth=[]         
+          # for j in range(Sv120.shape[1]):
+          #     row_1=Sv120[:,j]
+          #     if np.sum(row_1==-999)>0:
+          #         bottomdepth.append( np.min(r120[row_1==-999]) )
+          #     else:
+          #         bottomdepth.append( r120.max() )
+          # # print(bottomdepth)   
+          # df_nasc_file['bottomdepth_m']=bottomdepth
             
            
-         df_nasc_file['nasc_swarm']=nasc_swarm_rs
-         df_nasc_file.index=positions['ping_time']
+          df_nasc_file['nasc_swarm']=nasc_swarm_rs
+          df_nasc_file.index=positions['ping_time']
          
-         # df_nasc_file=df_nasc_file.resample('5s').mean()
-         print('Krill detection complete: '+str(np.mean(nasc_swarm)) ) 
+          # df_nasc_file=df_nasc_file.resample('5s').mean()
+          # print('Krill detection complete: '+str(np.mean(nasc_swarm)) ) 
          
          
-         ## db difference method
-         dbdiff_sv_threshold_db   = float(self.config['PROCESSING']['dbdiff_sv_threshold_db'] )
+          ## db difference method
+          dbdiff_sv_threshold_db   = float(self.config['PROCESSING']['dbdiff_sv_threshold_db'] )
 
-         if np.sum( np.isin( [38000.0, 120000.0],xr_sv.coords['frequency'].data ) ) ==2 :
+          if np.sum( np.isin( [38000.0, 120000.0],xr_sv.coords['frequency'].data ) ) ==2 :
          
-             Sv38= xr_sv.sel(frequency=38000.0).data 
-             # remove bttom
-             for i in range(len(t120)):
-                 ix_na = r120>=  positions['bottomdepth_m'].values[i]-10 
-                 Sv38[ix_na,i]=np.nan 
+              Sv38= xr_sv.sel(frequency=38000.0).data 
+              # remove bttom
+              for i in range(len(t120)):
+                  ix_na = r120>=  positions['bottomdepth_m'].values[i]-10 
+                  Sv38[ix_na,i]=np.nan 
              
-             db_diff= Sv120 -Sv38
+              db_diff= Sv120 -Sv38
              
-             mask_dbdiff = db_diff>dbdiff_sv_threshold_db 
+              mask_dbdiff = db_diff>dbdiff_sv_threshold_db 
              
-             Sv120db=Sv120.copy()
-             Sv120db[~mask_dbdiff]=np.nan
+              Sv120db=Sv120.copy()
+              Sv120db[~mask_dbdiff]=np.nan
              
-             ixdepthvalid= (r120>=surface_exclusion_depth_m) & (r120<=maximum_depth_m )
-             Sv120db[~ixdepthvalid,:]=np.nan
+              ixdepthvalid= (r120>=surface_exclusion_depth_m) & (r120<=maximum_depth_m )
+              Sv120db[~ixdepthvalid,:]=np.nan
              
-             cell_thickness=np.abs(np.mean(np.diff( r120) ))               
-             nasc_dbdiff=4*np.pi*1852**2 * np.nansum( np.power(10, Sv120db /10)*cell_thickness ,axis=0)   
-             df_nasc_file['nasc_dbdiff']=nasc_dbdiff
-         else:
-             df_nasc_file['nasc_dbdiff']=np.nan
-             mask_dbdiff=np.nan
+              cell_thickness=np.abs(np.mean(np.diff( r120) ))               
+              nasc_dbdiff=4*np.pi*1852**2 * np.nansum( np.power(10, Sv120db /10)*cell_thickness ,axis=0)   
+              df_nasc_file['nasc_dbdiff']=nasc_dbdiff
+          else:
+              df_nasc_file['nasc_dbdiff']=np.nan
+              mask_dbdiff=np.nan
+              
+          ########## U-NET
+          
+          # # f =  xr_sv_raw.coords['frequency'].max().data
+          # sv_threshold_low=-90
+          # sv_threshold_high=-20
+         
+          # sv= xr_sv_raw.sel(frequency=f).data.copy() 
+          # r=xr_sv_raw.coords['depth'].values
+          # t=xr_sv_raw.coords['time'].values
+          
+        
+          #  # estimate and correct background noise       
+          # p         = np.arange(len(t))                
+          # s         = np.arange(len(r))          
+ 
+          # bn, m120bn_ = gBN.derobertis(sv, s, p, 5, 20, r, self.calc_absorption(f,6) ) # whats correct absoprtion?
+          # b=pd.DataFrame(bn)
+          # bn=  b.interpolate(axis=1).interpolate(axis=0).values                        
+          # sv_clean     = transform.log(transform.lin(sv) - transform.lin(bn))
+          
+          # sv_SNR_threshold_db = 1
+          # msn             = mSN.derobertis(sv_clean, bn, thr=sv_SNR_threshold_db)
+          # sv_clean[msn] = np.nan
+
+          # ix_f = xr_sv_raw.coords['frequency'] ==  f
+          # ix_d = (xr_sv_raw.coords['depth']>0) & (xr_sv_raw.coords['depth']<500)
+          # sv = np.squeeze( xr_sv_raw[ix_f,ix_d,:].values ) 
+          # sv = np.squeeze( sv_clean[ix_d,:] )
+
+          # sv_normalized = sv.copy()
+          # sv_normalized[sv_normalized>sv_threshold_high]= sv_threshold_high
+          # sv_normalized[sv_normalized<sv_threshold_low]=sv_threshold_low
+          # ix = np.isnan(sv_normalized)
+          # sv_normalized[ix]=sv_threshold_low  
+          # sv_normalized =  (sv_normalized - sv_threshold_low) / ( sv_threshold_high - sv_threshold_low   )
+
+          # image_n_pixels=256  
+          # sv_input= resize(sv_normalized,[image_n_pixels, image_n_pixels])           
+          # img = np.expand_dims(sv_input, axis=0)
+         
+          # # apply unet  
+          # pred_mask = model.predict(img)
+          # pred=pred_mask[0,:,:,:]
+          
+          # #filter predictions
+          # thrs =  [0.95,0.76,0.70,0.43]
+          # minimum_area = [10,10,5,10]
+          # masks=np.zeros(pred.shape)
+
+          # for k in range(4):
+            
+          #   mpred = pred[:,:,k+1]>thrs[k]
+          #   labels =  measure.label(  mpred)
+            
+          #   # probs=measure.regionprops_table(labels,sv120,properties=['label','area','mean_intensity','orientation','major_axis_length','minor_axis_length','weighted_centroid','bbox'])
+        
+          #   probs=measure.regionprops_table(labels,properties=['label','area','orientation','major_axis_length','minor_axis_length','centroid','bbox'])
+        
+          #   ix_del =probs['area']<minimum_area[k]
+            
+          #   if k==1:
+          #       ix_del_swarmtosurface =  probs['bbox-0']>(256/500 * 50) # delete pacthes start start below 50m 
+          #       ix_del[ix_del_swarmtosurface]=True
+          #       # print('del predator ')
+            
+          #   label_del = probs['label'][ix_del]
+          #   for lb in label_del:
+          #       ix = labels==lb
+          #       labels[ix]=0
+          #   m = labels>0
+          #   masks[:,:,k]=m    
+            
+          # footprint = disk(3)
+          # masks[:,:,3] = dilation(    masks[:,:,3], footprint)
+        
+          # mask=np.zeros(pred.shape[0:2])
+          # mask [masks[:,:,3]==1]=4
+          # mask [masks[:,:,2]==1]=3
+          # mask [masks[:,:,1]==1]=2
+          # mask [masks[:,:,0]==1]=1
+        
+          # for ix_t in range( mask.shape[1] ):
+          #   profile=mask[:,ix_t] 
+            
+          #   ix_bottom = np.where(profile==4)[0]
+          #   ix_krill = np.where(profile==1)[0]
+          #   ix_surfacepredator = np.where(profile==2)[0]
+            
+          #   if (len(ix_surfacepredator)>0) & (len(ix_krill)>0):
+          #       ixdel=ix_surfacepredator[ix_surfacepredator > ix_krill.max()]
+          #       mask[ixdel,ix_t]=0
+          #   if (len(ix_surfacepredator)>0) & (len(ix_bottom)>0):
+          #       ixdel=ix_surfacepredator[ix_surfacepredator > ix_bottom.max()]
+          #       mask[ixdel,ix_t]=0
+          #   if (len(ix_krill)>0) & (len(ix_bottom)>0):
+          #       ixdel=ix_krill[ix_krill > ix_bottom.max()]
+          #       mask[ixdel,ix_t]=0
+                
+      
+
+          
+          # n1 =       np.sum(ix_d)
+          # n2 = mask_swarm.shape[1]
+          # segmentation_unet = np.zeros(mask_swarm.shape)
+          # segmentation_unet[ix_d,:]=resize(mask,[n1,n2],preserve_range=True,order=0)  
+          # segmentation_unet=np.round(segmentation_unet)
+          # segmentation_unet=segmentation_unet.astype(int)
+          
+          
+          # # combine unet and shapes, add patches from swarms
+          # segmentation_unet_and_shapes = np.zeros(mask_swarm.shape)
+          # ix = (mask_swarm) & ((segmentation_unet!=2) | (segmentation_unet!=3))
+          # segmentation_unet_and_shapes[ix]=1          
+          # ix = (segmentation_unet==2) 
+          # segmentation_unet_and_shapes[ix]=2      
+          # ix = (segmentation_unet==3) 
+          # segmentation_unet_and_shapes[ix]=3    
+          # ix = (segmentation_unet==4) 
+          # segmentation_unet_and_shapes[ix]=4       
+          
+          # sv_lin=np.power(10, Sv120 /10)
+          # sv_lin[segmentation_unet_and_shapes!=1]=0       
+          # sv_downsampled=  resize_local_mean(sv_lin,[ len(r_new) , Sv120.shape[1] ] ,grid_mode =True)
+          # sv_dep=np.transpose(  np.tile(r_new,[sv_downsampled.shape[1],1] ) )                       
+          # sa =  integrate.trapezoid(sv_downsampled,sv_dep,axis=0)  
+          # nasc_unet =  4*np.pi*1852**2 * sa
+          # df_nasc_file['nasc_unet_and_shapes']=nasc_unet
+          
+                               
+          # # breakpoint()
+          # # nasc unet
+          
+          # sv_lin=np.power(10, Sv120 /10)
+          # sv_lin[segmentation_unet!=1]=0       
+          # sv_downsampled=  resize_local_mean(sv_lin,[ len(r_new) , Sv120.shape[1] ] ,grid_mode =True)
+          # sv_dep=np.transpose(  np.tile(r_new,[sv_downsampled.shape[1],1] ) )                       
+          # sa =  integrate.trapezoid(sv_downsampled,sv_dep,axis=0)  
+          # nasc_unet =  4*np.pi*1852**2 * sa
+          # df_nasc_file['nasc_unet']=nasc_unet
+          
+
+          print('Shapes avg NASC: '+str(df_nasc_file['nasc_swarm'].mean()) ) 
+          # print('U-NET avg NASC: '+str(df_nasc_file['nasc_unet'].mean()) ) 
+
+          
+          print('Shapes: '+ str( np.round((np.sum(mask_swarm) / mask_swarm.size )*100,2)) + ' % krill pixels' )
+          try:
+              print('db diff: '+ str( np.round((np.sum(mask_dbdiff) / mask_dbdiff.size )*100,2)) + ' % krill pixels' )
+          except:
+              pass
+          # print('U-NET: '+ str( np.round((np.sum(mask==1) / mask.size )*100,2)) + ' % krill pixels' )
+
+
+            
              
-         return df_nasc_file, mask_swarm, mask_dbdiff
+          return df_nasc_file, mask_swarm, mask_dbdiff #segmentation_unet #,segmentation_unet_and_shapes
  
         
          
     # def start():
     #     print('start')
 
     def callback_email(self):
@@ -1335,33 +1467,52 @@
                         for fi in files_to_send:      
                             
                             
                             # breakpoint()
 
                             xr_sv = xr.open_dataarray(self.workpath+'/'+fi[-30:-13] + '_echogram.nc')
                             
-                            f=float(self.config['GENERAL']['scrutinization_frequency'])
+                            # f=float(self.config['GENERAL']['scrutinization_frequency'])
 
               
-                            ix_f = np.where( xr_sv.coords['frequency'].values==f)[0][0] 
+                            # ix_f = np.where( xr_sv.coords['frequency'].values==f)[0][0] 
                             
-                            sv = np.transpose( np.squeeze( xr_sv[ix_f,:,:].data) )
+                            xr_mail= xr_sv.resample(time=echogram_resolution_in_seconds+'s').mean()
+                            # xr_mail.astype('float16')
+                            targetname=fi[-30:-13] + '_mail_echogram.nc' 
+                            xr_mail.to_netcdf(targetname)    
+                            zip.write(targetname)                                                      
+                            os.remove(targetname)
+                            
+    
 
-                            df=pd.DataFrame(sv)
-                            df.index= xr_sv.coords['time'].values
-                            df.columns= xr_sv.coords['depth'].values
-                                                        
-                            
-                            df=df.resample(echogram_resolution_in_seconds+'s').mean()
-                            targetname=fi[-30:-13] + '_sv_swarm_mail.h5' 
-                            df.astype('float16').to_hdf(targetname,key='df',mode='w')
-                            # df.astype('float16').to_csv(targetname,compression='gzip')
+                            # sv = np.transpose( np.squeeze( xr_sv[ix_f,:,:].data) )
+
+                            # df=pd.DataFrame(sv)
+                            # df.index= xr_sv.coords['time'].values
+                            # df.columns= xr_sv.coords['depth'].values
+                                                                                    
+                            # df=df.resample(echogram_resolution_in_seconds+'s').mean()
+                            # targetname=fi[-30:-13] + '_sv_swarm_mail.h5' 
+                            # df.astype('float16').to_hdf(targetname,key='df',mode='w')
+                            # # df.astype('float16').to_csv(targetname,compression='gzip')
+                            # zip.write(targetname)                                                      
+                            # os.remove(targetname)
+                            
+                            # resample mask
+                            mask_swarm= pd.read_hdf( self.workpath+'/'+fi[-30:-13] + '_mask_swarm.h5',key='df' ) 
+                            mask_swarm=mask_swarm.resample(echogram_resolution_in_seconds+'s').mean()
+                            mask_swarm[mask_swarm>=0.5]=1
+                            mask_swarm[mask_swarm<0.5]=0
+                            mask_swarm=mask_swarm.astype(bool)                            
+                            targetname=fi[-30:-13] + '_mail_mask_swarm.h5' 
+                            mask_swarm.astype('bool').to_hdf(targetname,key='df',mode='w')
                             zip.write(targetname)                                                      
                             os.remove(targetname)
-                    
+                            
                     zip.close()
                     fp = open(loczip, "rb")
                     attachment = MIMEBase('application', 'x-zip')
                     attachment.set_payload(fp.read())
                     fp.close()
                     encoders.encode_base64(attachment)
                     attachment.add_header("Content-Disposition", "attachment", filename=loczip)
@@ -1395,13 +1546,21 @@
                     except Exception as e:
                         print(e)
                                         
         
         self.callback_email_active==False
         
 #%%
+# os.chdir( r'C:\Users\a5278\Documents\postdoc_krill\krillscan\krillscan_github' )
+
 
 ks=krillscan_class()
-# ks.start('settings.ini')
+# ks.start(r'C:\Users\a5278\Documents\postdoc_krill\krillscan\krillscan_github\settings.ini')
+
+# ks.start(r'C:\Users\a5278\Documents\postdoc_krill\CCAMLR_data\settings_ccamlr.ini')
+# ks.start(r"E:\krillscan_cruise_2024_2\settings2024.ini")
+# ks.start(r"F:\krillscan2016\settings.ini")
 
+# ks.start_para_processing('settings.ini')
 
-# ks.stop()
+# ks.stop()
+# ks.inspect()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `krillscan-0.2.9/krillscan.egg-info/PKG-INFO` & `krillscan-0.3.0/krillscan.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 Metadata-Version: 2.1
 Name: krillscan
-Version: 0.2.9
+Version: 0.3.0
 Summary: A python module for automatic analysis of backscatter data from vessels of opportunity
 Home-page: 
 Author: Sebastian Menze
 Author-email: sebastian.menze@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+Requires-Dist: lxml
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: future
+Requires-Dist: pyproj
+Requires-Dist: scikit_image
+Requires-Dist: scipy
+Requires-Dist: toml
+Requires-Dist: geopy
+Requires-Dist: tables
+Requires-Dist: xarray
+Requires-Dist: netcdf4
+Requires-Dist: pyqtdarktheme
 
 
 
-# Krillscan - A python module for automatic  analysis of backscatter data from fishing vessels to implement feedback management of the Antarctic krill fishery
+# Krillscan - A python module for automatic analysis of backscatter data from fishing vessels to implement feedback management of the Antarctic krill fishery
 
-- Automatically processes and analyzees EK60 and EK80 echosounder data 
+- Automatically processes and analyzes EK60 and EK80 echosounder data 
 - stores echograms and NASC tables as NetCDF, HDF or .csv files
 - detects krill swarms and can send near-real-time acoustic registrations via email
 
 ![dataflow](dataflow.JPG)
 
 ## Installation
 
@@ -50,34 +64,35 @@
 sv_SNR_threshold_db = 3
 swarm_sv_threshold_db = -70
 dbdiff_sv_threshold_db = 3
 seafloor_offset_m= 10
 seafloor_sv_threshold_db= -38
 surface_exclusion_depth_m = 20
 maximum_depth_m = 250
+write_mask_as_csv= 0
 
 [EMAIL]
 email_send = 0
 email_from = *Enter a mail address here*
 email_to = *Enter a mail address here*
 pw = *Enter IMAP password address here*
 files_per_email = 6
 send_echograms = 1
 echogram_resolution_in_seconds = 1
 ```
 
-This settings.ini file must be located in the same working directory as your python prompt. To send emails set email_send=1 (or True).
+This location of the settings.ini file must be passed to krillscan when starting the processing. To send emails set email_send=1 (or True).
 
- To start the processing type:
+To start the processing type:
 
 ```python
-import krillscan as ks
-ks.krillscan.ks.start()
+from krillscan import process
+process.ks.start('settings.ini')
 # to stop the processing: 
-# ks.krillscan.ks.stop()
+# process.ks.stop( )
 ```
 This starts two threads, one that looks for new data, processes and stores it and another that scans for recently processed data and sends them out via email. This is an ad-hoc solution so far, future versions of krillscan will transfer data directly to a cloud storage. 
 
 
 ### Output format
 
 Krillscan will store the raw and processed echograms, detection masks and NASC tables in 10-min long snippets, with the filename containing the start date of each snippet:
@@ -88,15 +103,24 @@
 D20140125-T060417_mask_dbdiff.h5
 D20140125-T060417_mask_swarm.h5
 D20140125-T060417_nasctable.csv
 D20140125-T060417_nasctable.h5
 D20140125-T060417_rawechogram.nc
 ```
 
+NASC stands for Nautical area backscattering coefficient has the unit m^2 nmi^-2 and is the vertical integral (sum) of volume backscatter normalized to 1x1 nautical mile area:
+
+```python
+sv_lin=np.power(10, Sv120sw /10)  
+sv_downsampled=  resize_local_mean(sv_lin,[ len(r_new) , Sv120sw.shape[1] ] ,grid_mode =True)
+sa =  integrate.trapezoid(sv_downsampled,sv_dep,axis=0)  
+nasc =  4*np.pi*1852**2 * sa
+```
 Here is an example of the contents of the echogram files, they are stored and read using the xarray module:
+
 ```python
 import xarray as xr
 file="D20140125-T055416_rawechogram.nc"
 xr_sv = xr.open_dataarray(file)
 print(xr_sv)
 ```
 ```
@@ -104,15 +128,15 @@
 [854000 values with dtype=float32]
 Coordinates:
   * time       (time) datetime64[ns] 2014-01-25T05:54:16.770000 ... 2014-01-2...
   * depth      (depth) float64 0.0 0.5 1.0 1.5 2.0 ... 498.0 498.5 499.0 499.5
   * frequency  (frequency) float64 3.8e+04 1.2e+05
 ```
 
-Here is an example of the contents of the mask files, they are stored and read as pandas DataFrames:
+Here is an example of the contents of the mask files, they are stored and read as pandas DataFrames. if you want the mask files as csv in addition to hdf you must change settings.ini to "write_mask_as_csv= True". 
 
 ```python
 import pandas as pd
 file="D20140125-T060417_mask_swarm.h5"
 df = pd.read_hdf(file,key='df')
 print(df)
 ```
@@ -157,25 +181,26 @@
 2014-01-25 06:04:11.395 -60.004037 -48.374469  ...   334.853738          0.0
 2014-01-25 06:04:12.797 -60.004021 -48.374597  ...  1719.993121          0.0
 2014-01-25 06:04:14.199 -60.004004 -48.374726  ...     0.000000          0.0
 
 [427 rows x 7 columns]
 ```
 
-Here is an example for 1-month of echosunder data from a krill fishing vessel, processed entirely automatic using the swarm detection method.
+Here is an example for 1-month of echosounder data from a krill fishing vessel, processed entirely automatic using the swarm detection method.
 
 ![timeseries_endurance_jan2022](timeseries_endurance_jan2022.jpg)
 
 
 ### Visual inspection of processed echograms
 
 Krillscan also contains a GUI tool (PyQT5) that lets you inspect the automatically processed echograms and correct the swarm detection masks by adding or removing areas. To start the GUI enter:
 
 ```python
-ks.ks.inspect()
+from krillscan import inspect
+inspect.gui()
 ```
 
 The GUI looks like this: A  menu bar lets you open processed NetCDF files, show the data folder, undo changes and quite the GUI. The Main window shows the echogram for each 10-min long NetCDF and the ping-by-ping NASC (black line) and 1-min NASC average (blue line). 
 
 ![menuebar](menuebar.JPG)
 
 The tool bar below the menu bar has these functions:
@@ -188,15 +213,55 @@
 
 - You can add or remove areas of the detection mask (shown as red overlay) using double clicks to draw a polygon of you choice. Once finished with drawing press enter to apply the change and update the NASC accordingly.
 
 ![fig_inspect](fig_inspect.png)
 
 
 
+### Data Transfer
+
+So far I have implemented simple email sending as data transfer method. The echogram NetCDF and detection mask Hdf files are down sampled in time to a desired resolution (in setting.ini) and than compressed into a zip file. This is rather efficient, for a 10-min snippet in 1-s resolution the files echogram files are between 10-30 MB (depending on the number of frequencies) but the zip file is only around 800 kB. In addition to the echogram and mask the ping-by-ping NASC table is sent as Hdf file and the setting.ini file. Here is an example:
+
+![mail_content](mail_content.JPG)
+
+You can open and edit these echogram / detection mask files with the inspection GUI, but the "view raw" mode will not work. 
+
+### Parallel post-processing of data
+
+If you have a lot of raw files that need to be processed, it can be better to use parallel processing instead of the serial real-time processing. This is also implemented in krillscan using the multiprocessing module This will process and store the data in their original file length and not 10-min snippets. To start the parallel post-processing you can use the same ini file, the module will detect the amount of cores available and distribute tasks across all of them.
+
+```python
+from krillscan import process
+process.ks.start_para_processing('settings.ini')
+```
+
+### Annotation of echograms using custom labels
+
+```python
+from krillscan import inspect_and_annotate
+inspect_and_annotate.gui()
+```
+
+This opens the PyQt5 GUI with an additional line, here you can write up to 7 custom lables into the fields and mark rectangular patches in the echogram using mouse click and release. To remove the latest rectangle use the right mouse click. To save annotations check the "save changes" box and move on to the next snippet. You can toggle if the swarm detection mask should show or not using the "show mask" box. Annotations are saved as .csv for each snippet using UNIX timestamps as left and right border and depth as upper and lower border.
+
+```
+,t1,t2,d1,d2,label
+0,19092.83217844115,19092.83316209359,-241.50554015402548,-62.35334814153828,Predator
+1,19092.83269467859,19092.834692351964,-46.36452080694602,-24.86553958551312,
+```
+
+![ks_with_annot](ks_with_annot.JPG)
+
 ## Acknowledgements
 
+This software relies on packages and functions developed by the rapidkrill, echopy, pyecholab and echopype projects. We would like to thank the teams for sharing their useful code! We also thank all developers of python and its many open libraries. 
+
+https://github.com/bas-acoustics/rapidkrill
+
+https://echopype.readthedocs.io/en/stable/index.html
 
+https://github.com/bas-acoustics/echopy
 
+https://github.com/CI-CMG/pyEcholab/tree/master/echolab2
 
 
-## Run krillscan automatic processing from a Docker container
```

### Comparing `krillscan-0.2.9/setup.py` & `krillscan-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 # The text of the README file
 README = (HERE / "readme.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="krillscan",
-    version="0.2.9",
+    version="0.3.0",
     description="A python module for automatic analysis of backscatter data from vessels of opportunity",
     long_description=README,
     long_description_content_type="text/markdown",
     url="",
     author="Sebastian Menze",
     author_email="sebastian.menze@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3.9",
     ],
     packages=find_packages(),
     include_package_data=True,
     install_requires=["lxml","numpy","matplotlib","pandas",
     "future","pyproj","scikit_image","scipy","toml","geopy",
-    "tables","xarray","netcdf4"])
+    "tables","xarray","netcdf4","pyqtdarktheme"])
```

