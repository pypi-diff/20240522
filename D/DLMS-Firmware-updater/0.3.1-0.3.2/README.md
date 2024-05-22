# Comparing `tmp/DLMS_Firmware_updater-0.3.1.tar.gz` & `tmp/DLMS_Firmware_updater-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_Firmware_updater-0.3.1.tar", last modified: Thu May  2 07:45:32 2024, max compression
+gzip compressed data, was "DLMS_Firmware_updater-0.3.2.tar", last modified: Wed May 22 08:56:45 2024, max compression
```

## Comparing `DLMS_Firmware_updater-0.3.1.tar` & `DLMS_Firmware_updater-0.3.2.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.429392 DLMS_Firmware_updater-0.3.1/
--rw-rw-rw-   0        0        0        8 2024-04-08 10:22:40.000000 DLMS_Firmware_updater-0.3.1/.gitignore
--rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      569 2024-05-02 07:45:32.428393 DLMS_Firmware_updater-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.3.1/README.md
--rw-rw-rw-   0        0        0     1115 2024-05-02 07:42:25.000000 DLMS_Firmware_updater-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-02 07:45:32.429392 DLMS_Firmware_updater-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.035391 DLMS_Firmware_updater-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.063392 DLMS_Firmware_updater-0.3.1/src/DLMSFirmwareUpdater/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.3.1/src/DLMSFirmwareUpdater/__init__.py
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.3.1/src/DLMSFirmwareUpdater/config.toml
--rw-rw-rw-   0        0        0     3724 2024-05-02 06:52:12.000000 DLMS_Firmware_updater-0.3.1/src/DLMSFirmwareUpdater/main.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.078400 DLMS_Firmware_updater-0.3.1/src/DLMS_Firmware_updater.egg-info/
--rw-rw-rw-   0        0        0      569 2024-05-02 07:45:31.000000 DLMS_Firmware_updater-0.3.1/src/DLMS_Firmware_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5356 2024-05-02 07:45:31.000000 DLMS_Firmware_updater-0.3.1/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 07:45:31.000000 DLMS_Firmware_updater-0.3.1/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-02 07:45:31.000000 DLMS_Firmware_updater-0.3.1/src/DLMS_Firmware_updater.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2024-05-02 07:45:31.000000 DLMS_Firmware_updater-0.3.1/src/DLMS_Firmware_updater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-02 07:45:31.000000 DLMS_Firmware_updater-0.3.1/src/DLMS_Firmware_updater.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.089392 DLMS_Firmware_updater-0.3.1/test/
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.091392 DLMS_Firmware_updater-0.3.1/test/Firmwares/
--rw-rw-rw-   0        0        0  2737171 2024-01-16 06:35:27.000000 DLMS_Firmware_updater-0.3.1/test/Firmwares/firmwares.dat
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.042391 DLMS_Firmware_updater-0.3.1/test/Types/
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.038391 DLMS_Firmware_updater-0.3.1/test/Types/101/
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.153393 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/
--rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.14.typ
--rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.16.typ
--rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.26.typ
--rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.39.typ
--rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.43.typ
--rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.45.typ
--rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.46.typ
--rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.48.typ
--rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.49.typ
--rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.53.typ
--rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.54.typ
--rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.1.0.typ
--rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.2.0.typ
--rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.3.0.typ
--rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.3.30.typ
--rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.3.7.typ
--rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.3.9.typ
--rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.4.0.typ
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.039391 DLMS_Firmware_updater-0.3.1/test/Types/102/
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.209394 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/
--rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.20.typ
--rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.26.typ
--rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.39.typ
--rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.41.typ
--rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.43.typ
--rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.45.typ
--rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.48.typ
--rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.49.typ
--rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.53.typ
--rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.1.0.typ
--rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.2.0.typ
--rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.0.typ
--rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.30.typ
--rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.5.typ
--rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.7.typ
--rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.040391 DLMS_Firmware_updater-0.3.1/test/Types/103/
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.255391 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/
--rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.16.typ
--rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.26.typ
--rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.39.typ
--rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.43.typ
--rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.45.typ
--rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.48.typ
--rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.49.typ
--rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.1.0.typ
--rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.2.0.typ
--rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.3.0.typ
--rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.3.30.typ
--rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.3.7.typ
--rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.041391 DLMS_Firmware_updater-0.3.1/test/Types/104/
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.297392 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/
--rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.20.typ
--rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.26.typ
--rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.39.typ
--rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.43.typ
--rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.45.typ
--rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.48.typ
--rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.49.typ
--rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.1.0.typ
--rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.2.0.typ
--rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.3.0.typ
--rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.3.30.typ
--rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.3.7.typ
--rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.300392 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.329400 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.0.typ
--rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.15.typ
--rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.16.typ
--rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.17.typ
--rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.5.0.typ
--rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.5.3.typ
--rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.5.7.typ
--rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.6.1.typ
--rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.357401 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.0.typ
--rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.10.typ
--rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.12.typ
--rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.15.typ
--rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.16.typ
--rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.17.typ
--rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.5.0.typ
--rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.5.7.typ
--rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.379394 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
--rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
--rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
--rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
--rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
--rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
--rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.401392 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
--rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
--rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
--rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
--rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
--rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
--rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:32.425393 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
--rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
--rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
--rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
--rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
--rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
--rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
--rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.1/test/Types/KPZ/image_transfer_1.typ
--rw-rw-rw-   0        0        0  1785889 2024-05-02 07:38:01.000000 DLMS_Firmware_updater-0.3.1/test/client_log.txt
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.3.1/test/config.toml
--rw-rw-rw-   0        0        0      399 2024-05-02 07:02:25.000000 DLMS_Firmware_updater-0.3.1/test/test_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.815377 DLMS_Firmware_updater-0.3.2/
+-rw-rw-rw-   0        0        0        8 2024-04-08 10:22:40.000000 DLMS_Firmware_updater-0.3.2/.gitignore
+-rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      569 2024-05-22 08:56:45.812379 DLMS_Firmware_updater-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.3.2/README.md
+-rw-rw-rw-   0        0        0     1116 2024-05-22 07:48:34.000000 DLMS_Firmware_updater-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 08:56:45.816378 DLMS_Firmware_updater-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.499375 DLMS_Firmware_updater-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.526408 DLMS_Firmware_updater-0.3.2/src/DLMSFirmwareUpdater/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.3.2/src/DLMSFirmwareUpdater/__init__.py
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.3.2/src/DLMSFirmwareUpdater/config.toml
+-rw-rw-rw-   0        0        0     3882 2024-05-22 07:33:03.000000 DLMS_Firmware_updater-0.3.2/src/DLMSFirmwareUpdater/main.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.539410 DLMS_Firmware_updater-0.3.2/src/DLMS_Firmware_updater.egg-info/
+-rw-rw-rw-   0        0        0      569 2024-05-22 08:56:45.000000 DLMS_Firmware_updater-0.3.2/src/DLMS_Firmware_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5356 2024-05-22 08:56:45.000000 DLMS_Firmware_updater-0.3.2/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 08:56:45.000000 DLMS_Firmware_updater-0.3.2/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-22 08:56:45.000000 DLMS_Firmware_updater-0.3.2/src/DLMS_Firmware_updater.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-05-22 08:56:45.000000 DLMS_Firmware_updater-0.3.2/src/DLMS_Firmware_updater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-22 08:56:45.000000 DLMS_Firmware_updater-0.3.2/src/DLMS_Firmware_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.547376 DLMS_Firmware_updater-0.3.2/test/
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.549378 DLMS_Firmware_updater-0.3.2/test/Firmwares/
+-rw-rw-rw-   0        0        0  2737171 2024-01-16 06:35:27.000000 DLMS_Firmware_updater-0.3.2/test/Firmwares/firmwares.dat
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.504376 DLMS_Firmware_updater-0.3.2/test/Types/
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.501375 DLMS_Firmware_updater-0.3.2/test/Types/101/
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.596407 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/
+-rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.14.typ
+-rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.16.typ
+-rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.26.typ
+-rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.39.typ
+-rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.43.typ
+-rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.45.typ
+-rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.46.typ
+-rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.48.typ
+-rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.49.typ
+-rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.53.typ
+-rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.54.typ
+-rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.1.0.typ
+-rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.2.0.typ
+-rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.3.0.typ
+-rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.3.30.typ
+-rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.3.7.typ
+-rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.3.9.typ
+-rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.4.0.typ
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.502376 DLMS_Firmware_updater-0.3.2/test/Types/102/
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.636376 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/
+-rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.20.typ
+-rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.26.typ
+-rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.39.typ
+-rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.41.typ
+-rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.43.typ
+-rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.45.typ
+-rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.48.typ
+-rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.49.typ
+-rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.53.typ
+-rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.1.0.typ
+-rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.2.0.typ
+-rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.0.typ
+-rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.30.typ
+-rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.5.typ
+-rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.7.typ
+-rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.503376 DLMS_Firmware_updater-0.3.2/test/Types/103/
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.670376 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/
+-rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.16.typ
+-rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.26.typ
+-rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.39.typ
+-rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.43.typ
+-rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.45.typ
+-rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.48.typ
+-rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.49.typ
+-rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.1.0.typ
+-rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.2.0.typ
+-rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.3.0.typ
+-rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.3.30.typ
+-rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.3.7.typ
+-rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.504376 DLMS_Firmware_updater-0.3.2/test/Types/104/
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.705383 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/
+-rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.20.typ
+-rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.26.typ
+-rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.39.typ
+-rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.43.typ
+-rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.45.typ
+-rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.48.typ
+-rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.49.typ
+-rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.1.0.typ
+-rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.2.0.typ
+-rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.3.0.typ
+-rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.3.30.typ
+-rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.3.7.typ
+-rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.707377 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.729377 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.0.typ
+-rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.15.typ
+-rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.16.typ
+-rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.17.typ
+-rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.5.0.typ
+-rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.5.3.typ
+-rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.5.7.typ
+-rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.6.1.typ
+-rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.751377 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.0.typ
+-rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.10.typ
+-rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.12.typ
+-rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.15.typ
+-rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.16.typ
+-rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.17.typ
+-rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.5.0.typ
+-rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.5.7.typ
+-rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.768410 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
+-rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
+-rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
+-rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
+-rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
+-rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
+-rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.787377 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
+-rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
+-rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
+-rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
+-rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
+-rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
+-rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-05-22 08:56:45.810379 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
+-rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
+-rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
+-rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
+-rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
+-rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
+-rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
+-rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.2/test/Types/KPZ/image_transfer_1.typ
+-rw-rw-rw-   0        0        0  1820496 2024-05-22 07:19:49.000000 DLMS_Firmware_updater-0.3.2/test/client_log.txt
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.3.2/test/config.toml
+-rw-rw-rw-   0        0        0      399 2024-05-02 07:02:25.000000 DLMS_Firmware_updater-0.3.2/test/test_updater.py
```

### Comparing `DLMS_Firmware_updater-0.3.1/PKG-INFO` & `DLMS_Firmware_updater-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_Firmware_updater
-Version: 0.3.1
+Version: 0.3.2
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.3.1/pyproject.toml` & `DLMS_Firmware_updater-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 [tool.setuptools.package-data]
 DLMSFirmwareUpdater = ["*.toml", "*.dat", "*.typ"]
 #exclude = ["test*", "dummy"]  # alternatively: `exclude = ["additional*"]`
 #namespaces = false
 
 [project]
 name = "DLMS_Firmware_updater"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
-    "DLMS_SPODES_client == 0.8.9",
+    "DLMS_SPODES_client == 0.8.15",
     "pyinstaller >= 6.2",
     "build >= 1.2.1"
 ]
 description="dlms-spodes"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords=["dlms", "spodes", "client", "firmware", "update"]
```

### Comparing `DLMS_Firmware_updater-0.3.1/src/DLMSFirmwareUpdater/config.toml` & `DLMS_Firmware_updater-0.3.2/src/DLMSFirmwareUpdater/config.toml`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/src/DLMSFirmwareUpdater/main.py` & `DLMS_Firmware_updater-0.3.2/src/DLMSFirmwareUpdater/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import argparse
 import time
-
 from DLMS_SPODES_client.servers import TransactionServer, Result
 from DLMS_SPODES_client import task, services
 from DLMS_SPODES_client.client import Client, logL, IDFactory
 from DLMS_SPODES_communications import AsyncSerial, AsyncNetwork
 
-
 id_factory = IDFactory("#")
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Update Firmware Program for DLMS meters")
     parser.add_argument(
@@ -85,15 +83,15 @@
         if len(args.p) == 1:
             clients = services.get_client_from_csv(
                 file_name=args.p[0],
                 id_factory=id_factory)
         else:
             raise ValueError("-p for \"File\" must have 1 file name")
     else:
-         raise ValueError(F"unknown {source=}")
+        raise ValueError(F"unknown {source=}")
     t_server = TransactionServer(
         clients=clients,
         tsk=task.Loop(
             task=task.UpdateFirmware(),
             func=lambda res: res,
             delay=args.loop_delay,
             attempt_amount=args.n_loops
@@ -102,18 +100,23 @@
     t_server.start()
     results = list(t_server.results)
     with open(
             file=args.file,
             mode="w+",
             encoding="utf-8") as file:
         while results:
-            time.sleep(3)
+            try:
+                time.sleep(3)
+            except KeyboardInterrupt:
+                t_server.abort()
+                print("Abort")
+                raise SystemExit
             for res in results:
                 res: Result
                 if res.complete:
                     results.remove(res)
                     res.client.log(logL.INFO, F"Для {res.client} обновление: {'Удачно' if res.value else 'Неудачно'}")
-                    file.write(F"{res.client} {res.value}")
+                    file.write(F"{res.client} {res.value}\n")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DLMS_Firmware_updater-0.3.1/src/DLMS_Firmware_updater.egg-info/PKG-INFO` & `DLMS_Firmware_updater-0.3.2/src/DLMS_Firmware_updater.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-Firmware-updater
-Version: 0.3.1
+Version: 0.3.2
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.3.1/src/DLMS_Firmware_updater.egg-info/SOURCES.txt` & `DLMS_Firmware_updater-0.3.2/src/DLMS_Firmware_updater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Firmwares/firmwares.dat` & `DLMS_Firmware_updater-0.3.2/test/Firmwares/firmwares.dat`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.14.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.14.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.16.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.26.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.39.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.43.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.45.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.46.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.46.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.48.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.49.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.53.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/0.0.54.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/0.0.54.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.1.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.1.9.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.2.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.2.5.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.3.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.3.30.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.3.7.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.3.9.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/101/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/101/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.20.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.26.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.39.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.41.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.41.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.43.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.45.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.48.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.49.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/0.0.53.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.1.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.1.9.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.2.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.2.5.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.30.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.5.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.7.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/102/09054d324d5f33/1.3.9.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/102/09054d324d5f33/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.16.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.26.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.39.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.43.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.45.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.48.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.49.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/0.0.53.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.1.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.1.9.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.2.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.2.5.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.3.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.3.30.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.3.7.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/103/09064d324d5f3153/1.3.9.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/103/09064d324d5f3153/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.20.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.26.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.39.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.43.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.45.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.48.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.49.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/0.0.53.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.1.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.1.9.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.2.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.2.5.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.3.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.3.30.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.3.7.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/104/09064d324d5f3353/1.3.9.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/104/09064d324d5f3353/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.15.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.16.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.17.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.4.22.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.5.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.5.3.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.5.3.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.5.7.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.6.1.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.6.1.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f31/1.6.2.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f31/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.10.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.10.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.12.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.15.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.16.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.17.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.4.22.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.5.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.5.7.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09054d324d5f33/1.6.2.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09054d324d5f33/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.15.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.16.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.17.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.4.22.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.5.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.5.7.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3153/1.6.2.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3153/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.15.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.16.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.17.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.4.22.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.5.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.5.7.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3353/1.6.2.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3353/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.12.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.15.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.16.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.17.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.4.22.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.5.0.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.5.7.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/09064d324d5f3354/1.6.2.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/09064d324d5f3354/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/Types/KPZ/image_transfer_1.typ` & `DLMS_Firmware_updater-0.3.2/test/Types/KPZ/image_transfer_1.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.3.1/test/client_log.txt` & `DLMS_Firmware_updater-0.3.2/test/client_log.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3044,7 +3044,96 @@
 #2: 02.05 10:37 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
 #2: 02.05 10:37 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
 #1: 02.05 10:37 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
 #1: 02.05 10:37 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
 #2: 02.05 10:37 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
 #1: 02.05 10:37 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для #1 обновление: Неудачно
 #2: 02.05 10:38 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для #2 обновление: Неудачно
+#common: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - Open port communication channel: AsyncSerial(port='COM13', inactivity_timeout=20)
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - c.SA=Address(upper_address=48, lower_address=None) c.DA=Address(upper_address=1, lower_address=16)
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: SNRM_P DA:1/16 SA:48  Info[11]:81 80 08 05 02 07 ee 06 02 07 ee
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:48 SA:1/16  Info[10]:81 80 07 05 01 ef 06 02 04 00
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - negotiation setup: NEGOTIATION: 1024->[info_size]->239 1->[window]->1
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:48  Info[67]:e6 e6 00 60 3e a1 09 06 07 60 85 74 05 08 01 01 8a 02 07 80 8b 07 60 85 74 05 08 02 02 ac 12 80 10 f4 df 37 7f ff eb c1 bc ea 27 04 82 f5 c0 13 f5 be 10 04 0e 01 00 00 00 06 5f 1f 04 00 7f ff ff 04 00
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:48 SA:1/16  Info[79]:e6 e7 00 61 4a a1 09 06 07 60 85 74 05 08 01 01 a2 03 02 01 00 a3 05 a1 03 02 01 0e 88 02 07 80 89 07 60 85 74 05 08 02 02 aa 12 80 10 ea 9b 10 35 75 7e cc c8 aa ea 1d 58 0a 7d 27 59 be 10 04 0e 08 00 06 5f 1f 04 00 00 18 9d 04 00 00 07
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - SET CONFORMANCE: 000000000001100010011101
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S1_R1_PF DA:1/16 SA:48  Info[34]:e6 e6 00 c3 01 c1 00 0f 00 00 28 00 00 ff 01 01 09 10 c3 df ce 0c 5f 6f 55 47 9f 92 cc 28 06 6a d9 86
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S1_R2_PF DA:48 SA:1/16  Info[27]:e6 e7 00 c7 01 c1 00 01 00 09 10 b0 8b 80 fe cf 45 f5 b5 ac e0 f1 0e d0 40 04 8d
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S2_R2_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 2a 00 00 ff 02 00
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S2_R3_PF DA:48 SA:1/16  Info[24]:e6 e7 00 c4 01 c1 00 09 0f 4b 50 5a 31 30 31 30 30 30 30 31 37 34 31 30
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S3_R3_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 60 01 01 ff 02 00
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S3_R4_PF DA:48 SA:1/16  Info[14]:e6 e7 00 c4 01 c1 00 09 05 4d 32 4d 5f 31
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S4_R4_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 00 02 01 ff 02 00
+#0: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S4_R5_PF DA:48 SA:1/16  Info[14]:e6 e7 00 c4 01 c1 00 09 05 31 2e 36 2e 32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - added 253 DLMS objects
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - close
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: DISC_P DA:1/16 SA:48 
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:48 SA:1/16  Info[22]:81 80 13 05 01 ef 06 02 04 00 07 04 00 00 00 01 08 04 00 00 00 01
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - c.SA=Address(upper_address=48, lower_address=None) c.DA=Address(upper_address=1, lower_address=16)
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: SNRM_P DA:1/16 SA:48  Info[10]:81 80 07 05 02 04 00 06 01 ef
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:48 SA:1/16  Info[10]:81 80 07 05 01 ef 06 02 04 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - negotiation setup: NEGOTIATION: 1024->[info_size]->239 1->[window]->1
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:48  Info[67]:e6 e6 00 60 3e a1 09 06 07 60 85 74 05 08 01 01 8a 02 07 80 8b 07 60 85 74 05 08 02 02 ac 12 80 10 04 97 03 4c cb 0e 49 6d 43 38 73 9b d1 5b 94 e0 be 10 04 0e 01 00 00 00 06 5f 1f 04 00 7f ff ff 04 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:48 SA:1/16  Info[79]:e6 e7 00 61 4a a1 09 06 07 60 85 74 05 08 01 01 a2 03 02 01 00 a3 05 a1 03 02 01 0e 88 02 07 80 89 07 60 85 74 05 08 02 02 aa 12 80 10 37 00 50 3f 05 23 0e e0 49 e6 d2 0e 8f 9d 22 5c be 10 04 0e 08 00 06 5f 1f 04 00 00 18 9d 04 00 00 07
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - SET CONFORMANCE: 000000000001100010011101
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S1_R1_PF DA:1/16 SA:48  Info[34]:e6 e6 00 c3 01 c1 00 0f 00 00 28 00 00 ff 01 01 09 10 d1 24 b5 57 30 7d 8b ea 0f 13 04 5f 35 b8 48 b7
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S1_R2_PF DA:48 SA:1/16  Info[27]:e6 e7 00 c7 01 c1 00 01 00 09 10 6c 18 7b 90 53 53 cf 07 56 82 51 88 ed 4f dc 3d
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S2_R2_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 2a 00 00 ff 02 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S2_R3_PF DA:48 SA:1/16  Info[24]:e6 e7 00 c4 01 c1 00 09 0f 4b 50 5a 31 30 31 30 30 30 30 31 37 34 31 30
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S3_R3_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 80 64 00 ff 02 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S3_R4_PF DA:48 SA:1/16  Info[36]:e6 e7 00 c4 01 c1 00 0a 1b 30 30 30 35 50 57 52 4d 5f 4d 32 4d 5f 31 5f 46 34 5f 35 70 70 6d 5f 53 70 76 71
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S4_R4_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 00 ff 02 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S4_R5_PF DA:48 SA:1/16  Info[12]:e6 e7 00 c4 01 c1 00 06 00 00 02 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S5_R5_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 00 ff 06 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S5_R6_PF DA:48 SA:1/16  Info[9]:e6 e7 00 c4 01 c1 00 16 01
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S6_R6_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 80 ff 02 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S6_R7_PF DA:48 SA:1/16  Info[12]:e6 e7 00 c4 01 c1 00 06 00 00 02 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - c.objects.server_ver[0]=AppVersion(1, 6, 2) is actual
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - set image to update suitable_boot=11
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S7_R7_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 80 ff 06 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S7_R0_PF DA:48 SA:1/16  Info[9]:e6 e7 00 c4 01 c1 00 16 06
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 80 ff 07 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:48 SA:1/16  Info[52]:e6 e7 00 c4 01 c1 00 01 01 02 03 06 00 00 3f fc 09 10 f8 d3 22 f8 99 54 21 2d d7 de c3 3c 2d 0f 8b 54 09 10 f8 d3 22 f8 99 54 21 2d d7 de c3 3c 2d 0f 8b 54
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S1_R1_PF DA:1/16 SA:48  Info[41]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 01 01 02 02 09 10 75 76 94 42 dd 91 9f d6 37 71 13 a6 25 78 81 0a 06 00 00 3f f3
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S1_R2_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - Start initiate Image Transfer
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S2_R2_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 80 ff 06 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S2_R3_PF DA:48 SA:1/16  Info[9]:e6 e7 00 c4 01 c1 00 16 01
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Статус блока данных: Передача данных инициированна
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S3_R3_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 00 09 82 02 00 00 00 02 20 c1 03 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 15 04 00 08 15 04 00 08 00 00 00 00 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 15 04 00 08 00 00 00 00 15 04 00 08 15 04 00 08 10 b5 05 4c 23 78 33 b9 04 4b 13 b1 04 48 af f3 00 80 01 23 23 70 10 bd bc 04 00 20 00 00 00 00 68 1e 00 08 08 b5 03 4b 1b b1 03 49 03 48 af f3 00 80 08 bd 00 00 00 00 c0 04 00 20 68 1e 00 08 70 b5 0d 4e 0d 4d 76 1b b6 10 06 d0 00 24 01 34 55 f8 04 3b 98 47 a6 42 f9 d1 09 4e 09 4d 76 1b 01 f0 3e fe b6 10 06 d0 00 24 01 34 55 f8 04 3b 98 47 a6 42 f9 d1 70 bd
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S3_R4_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 0/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S4_R4_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 01 09 82 02 00 38 23 00 08 38 23 00 08 40 23 00 08 38 23 00 08 f0 b4 86 07 43 d0 54 1e 00 2a 3e d0 ca b2 03 46 02 e0 14 f1 ff 34 38 d3 03 f8 01 2b 9d 07 f8 d1 03 2c 2b d9 cd b2 45 ea 05 25 0f 2c 45 ea 05 45 16 d9 a4 f1 10 07 3f 09 03 f1 20 06 06 eb 07 16 03 f1 10 02 42 e9 04 55 42 e9 02 55 10 32 b2 42 f8 d1 04 f0 0f 04 01 37 03 2c 03 eb 07 13 0d d9 1e 46 22 46 04 3a 03 2a 46 f8 04 5b fa d8 22 1f 22 f0 03 02 04 32 13 44 04 f0 03 04 2c b1 c9 b2 1c 44 03 f8 01 1b 9c 42 fb d1 f0 bc 70 47 14 46 03 46 c5 e7 02 4b 13 b1 02 48 00 f0 05 b8 70 47 00 00 00 00 c5 02 00 08 00 23 01 46 1a 46 18 46 00 f0 1e b8 38 b5 0a 4c 0a 4d 64 1b a4 10 0a d0 04 f1 80 43 01 3b 05 eb 83 05 01 3c 55 f8 04 39 98 47 00 2c f9 d1 bd e8 38 40 01 f0 c3 bd 00 bf 44 23 00 08 40 23 00 08 70 47 00 bf 70 47 00 bf 2d e9 f8 43 2b 4d 06 46 28 68 98 46 0f 46 91 46 ff f7 f2 ff 28 4b 1c 68 d4 f8 48 31 00 2b 3d d0 5a 68 1f 2a 0d dc 02 f1 01 0c 16 bb 02 32 c3 f8 04 c0 28 68 43 f8 22 70 ff f7 e0 ff 00 20 bd e8 f8 83 1e 4b 7b b3 4f f4 c8 70 af f3 00 80 03 46 48 b3 d4 f8 48 21 00 21 c0 e9 00 21 4f f0 01 0c c4 f8 48 01 0a 46 c0 f8 88 11 c0 f8 8c 11 00 2e dc d0 03 eb 82 01 01 24 c1 f8 88 90 d3 f8 88 01 94 40 20 43 02 2e c3 f8 88 01 c1 f8 08 81 cd d1 d3 f8 8c 11 0c 43 c3 f8 8c 41 c7 e7 04 f5 a6 73 c4 f8 48 31 bc e7 28 68 ff f7 a8 ff 4f f0 ff 30 c5 e7 00 bf a8 04 00 20 a8 1e 00 08 00 00 00 00 df f8 38 d0 00 f0 a8 f8 00 21 03 e0 0c 4b 5b 58 43 50 04 31 0b 48 0c 4b 42 18 9a 42 f6 d3 0b 4a 02 e0 00 23 42 f8 04 3b 09 4b 9a 42 f9 d3 00 f0 d5 fb ff f7 e9 fe 00 f0 3f fa 70 47 00 00 02 20
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S4_R5_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 1/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S5_R5_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 02 09 82 02 00 44 23 00 08 80 00 00 20 bc 04 00 20 bc 04 00 20 44 09 00 20 00 f0 6e f8 fe e7 00 00 08 b5 2b 4a 13 68 23 f0 0f 03 43 f0 04 03 13 60 13 68 03 f0 0f 03 04 2b 44 d1 26 4a 13 68 43 f4 80 43 13 60 02 f5 e4 32 13 68 43 f4 80 33 13 60 21 4b 1b 68 13 f4 00 3f fa d0 1f 4b 5a 68 1f 49 11 40 1f 4a 0a 43 5a 60 5a 68 22 f4 40 32 5a 60 1a 68 42 f0 80 72 1a 60 17 4b 1b 68 13 f0 00 7f fa d0 15 4b 9a 68 22 f0 f0 02 9a 60 9a 68 22 f4 e0 52 42 f4 a0 52 9a 60 9a 68 22 f4 60 42 42 f4 00 42 9a 60 9a 68 22 f0 03 02 42 f0 02 02 9a 60 09 4b 9b 68 03 f0 0c 03 08 2b f9 d1 09 48 00 f0 51 ff 08 bd 4f f4 bf 71 07 48 01 f0 bf fa b4 e7 00 3c 02 40 00 70 00 40 00 38 02 40 00 80 bf ff 0c 24 40 00 80 d1 f0 08 ac 1e 00 08 08 b5 00 f0 17 ff ff f7 95 ff 08 bd bf f3 4f 8f 05 49 ca 68 02 f4 e0 62 04 4b 13 43 cb 60 bf f3 4f 8f 00 bf fd e7 00 bf 00 ed 00 e0 04 00 fa 05 f0 b5 8d b0 a2 4c 23 6b 43 f0 04 03 23 63 23 6b 03 f0 04 03 05 93 05 9b 0c 23 06 93 00 25 07 95 0a 95 9c 4f 06 a9 38 46 00 f0 d4 fd 4f f4 80 73 06 93 01 26 07 96 0a 95 09 96 06 a9 38 46 00 f0 c9 fd 4f f0 80 73 bb 61 23 6b 33 43 23 63 23 6b 33 40 04 93 04 9b 4f f4 00 43 06 93 07 96 0a 96 09 96 a7 f5 00 67 06 a9 38 46 00 f0 b3 fd 11 23 06 93 07 95 0a 95 06 a9 38 46 00 f0 ab fd 23 6b 43 f0 02 03 23 63 23 6b 03 f0 02 03 03 93 03 9b 02 23 06 93 07 95 0a 95 06 a9 7f 48 00 f0 9a fd 23 6b 43 f0 08 03 23 63 23 6b 03 f0 08 03 02 93 02 9b 06 96 07 96 0a 95 09 95 78 4e 06 a9 30 46 00 f0 88 fd 4f f4 80 33 b3 61 4f f4 00 53 06 93 07 95 0a 95 06 a9 30 46 00 f0 7c fd 23 6c 43 f0 80 53 23 64 23 6c 03 f0
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S5_R6_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 2/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S6_R6_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 03 09 82 02 00 80 53 01 93 01 9b 23 6f 13 f4 00 4f 00 f0 b5 80 67 4b 1b 69 13 f0 02 0f 40 f0 af 80 66 4a 13 68 43 f4 80 73 13 60 65 4b ca 21 59 62 53 21 59 62 99 68 21 f4 80 41 99 60 99 68 21 f4 80 61 99 60 13 68 43 f0 04 03 13 60 5c 4b db 68 13 f0 04 0f fa d0 5a 4b 5b 69 9b b2 11 2b 59 d0 57 4a 53 69 1b 0c 1b 04 43 f0 11 03 53 61 93 68 23 f0 07 03 43 f0 03 03 93 60 51 4b da 68 d2 b2 62 f4 90 62 da 60 9a 68 42 f4 80 42 9a 60 4d 4a 51 68 41 f4 80 01 51 60 91 68 41 f4 80 01 91 60 9a 68 42 f4 80 62 9a 60 ff 21 59 62 43 48 02 68 22 f0 03 02 42 f0 01 02 02 60 43 48 02 69 42 f0 04 02 02 61 20 bf ca 22 5a 62 53 22 5a 62 9a 68 22 f4 80 62 9a 60 59 62 1a 6d 03 f5 f0 33 1b 69 00 2a 00 db db 43 23 f0 10 03 38 49 09 69 01 f0 10 01 0b 43 13 f0 08 0f 2c d0 42 f0 01 01 12 f0 01 0f 0e d0 32 48 04 69 04 34 04 61 44 69 04 34 44 61 20 e0 2a 4b 9b 68 03 f0 07 03 03 2b 9f d1 ab e7 27 49 0e 68 4d 68 12 f4 80 5f 0a d0 42 f0 01 11 27 48 00 24 04 61 44 68 01 34 44 60 86 60 c5 60 08 e0 42 f4 80 51 41 f0 01 01 20 48 86 61 c5 61 ee e7 11 46 13 f0 04 0f 0c d0 41 f0 02 00 12 f0 02 0f 36 d0 1a 4b d9 6a 04 31 d9 62 19 6b 04 31 19 63 01 46 91 42 01 d0 11 4b 19 65 13 4b 1b 69 13 f0 01 0f 04 d0 0b 4b 1b 69 13 f4 00 5f 09 d1 07 4b 4f f4 80 72 9a 61 a3 f5 80 63 1b 69 13 f0 02 0f 2f d0 0d b0 f0 bd 00 bf 00 38 02 40 00 08 02 40 00 04 02 40 00 0c 02 40 00 70 00 40 00 28 00 40 00 3c 01 40 00 ed 00 e0 00 00 02 40 50 28 00 40 24 4b 1d 68 5c 68 12 f4 00 5f 0a d0 41 f0 02 11 21 4b 00 20 d8 62 18 6a 01 30 18 62 5d 62 9c 62 bf e7 41 f4 00 51 41 f0 02 01 1b 4b 5d 63 9c 63
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S6_R7_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 3/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S7_R7_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 04 09 82 02 00 ee e7 00 f0 a5 fd 19 4b 1a 6b 22 f0 01 02 1a 63 1a 6b 22 f0 02 02 1a 63 1a 6b 22 f0 04 02 1a 63 1a 6b 22 f0 08 02 1a 63 a3 f5 02 33 45 f2 55 52 1a 60 03 22 5a 60 40 f6 b8 32 9a 60 00 22 1a 60 4c f6 cc 42 1a 60 0a 4a 13 68 23 f0 03 03 43 f0 02 03 13 60 07 4a 13 69 43 f0 04 03 13 61 30 bf 9f e7 00 bf 00 28 00 40 50 28 00 40 00 38 02 40 00 70 00 40 00 ed 00 e0 08 b5 0b 4b db 78 13 f0 01 0f 0a d0 09 4b 5b 6f 03 f0 7e 43 06 4a 13 60 c3 f3 07 63 6f f3 00 03 d3 70 ff f7 25 fe 01 f0 23 f8 01 f0 31 f8 fc e7 00 00 00 20 00 38 02 40 2d e9 f0 4f 97 b0 8d 4c 63 6c 43 f4 80 43 63 64 63 6c 03 f4 80 43 0f 93 0f 9b 23 6c 43 f0 80 53 23 64 23 6c 03 f0 80 53 0e 93 0e 9b 23 6b 43 f0 04 03 23 63 23 6b 03 f0 04 03 0d 93 0d 9b 23 6b 43 f0 08 03 23 63 23 6b 03 f0 08 03 0c 93 0c 9b 23 6b 43 f0 10 03 23 63 23 6b 03 f0 10 03 0b 93 0b 9b 23 6c 43 f4 80 23 23 64 23 6c 03 f4 80 23 0a 93 0a 9b 4f f4 40 73 10 93 02 27 11 97 4f f0 03 08 cd f8 48 80 00 25 13 95 01 26 14 96 07 23 15 93 df f8 b0 a1 10 a9 50 46 00 f0 cf fb 23 6c 43 f4 00 23 23 64 23 6c 03 f4 00 23 09 93 09 9b 4f f4 40 63 10 93 11 97 cd f8 48 80 13 95 14 96 08 23 15 93 10 a9 5e 48 00 f0 b8 fb 23 6b 43 f0 10 03 23 63 23 6b 03 f0 10 03 08 93 08 9b 4f f0 40 0b cd f8 40 b0 11 96 12 95 13 95 14 95 df f8 58 91 0d eb 0b 01 48 46 00 f0 a0 fb c9 f8 18 b0 23 6b 43 f0 08 03 23 63 23 6b 03 f0 08 03 07 93 07 9b 4f f4 80 53 10 93 11 96 12 95 13 95 14 95 0d eb 0b 01 50 46 00 f0 89 fb 4f f0 80 53 ca f8 18 30 23 6b 33 43 23 63 23 6b 33 40 06 93 06 9b 4f f4 00 43 10 93 11 96 12 95 13 95 14 95 aa f5
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S7_R0_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 4/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 05 09 82 02 00 40 6a 0d eb 0b 01 50 46 00 f0 70 fb 63 6c 43 f0 10 03 63 64 63 6c 03 f0 10 03 05 93 05 9b 10 97 11 96 12 95 13 95 14 97 0d eb 0b 01 48 46 00 f0 5d fb 23 6b 33 43 23 63 23 6b 33 40 04 93 04 9b 60 23 10 93 11 97 cd f8 48 80 13 95 14 96 05 23 15 93 0d eb 0b 01 50 46 00 f0 48 fb 23 6b 3b 43 23 63 23 6b 3b 40 03 93 03 9b 20 23 10 93 df f8 8c 80 0d eb 0b 01 40 46 00 f0 38 fb 23 6b 43 f0 04 03 23 63 23 6b 03 f0 04 03 02 93 02 9b 10 96 11 96 12 95 13 96 14 97 0d eb 0b 01 14 48 00 f0 25 fb 4f f4 80 33 12 4a 93 61 23 6b 3b 43 23 63 23 6b 3b 40 01 93 01 9b c0 27 10 97 11 96 12 95 13 95 14 95 0d eb 0b 01 40 46 00 f0 0f fb c8 f8 18 70 63 6c 43 f4 80 53 63 64 63 6c 03 f4 80 53 00 93 00 9b 17 b0 bd e8 f0 8f 00 bf 00 38 02 40 00 08 02 40 00 0c 02 40 00 10 02 40 00 04 02 40 08 b5 00 f0 8d fb 17 48 00 f0 54 fa 16 48 00 f0 51 fa 16 48 00 f0 4e fa 15 4b 5a 6c 22 f4 80 52 5a 64 1a 6b 22 f0 10 02 1a 63 1a 6b 22 f0 08 02 1a 63 1a 6b 22 f0 04 02 1a 63 1a 6b 22 f0 08 02 1a 63 1a 6b 22 f0 10 02 1a 63 1a 6b 22 f0 01 02 1a 63 1a 6c 22 f0 80 52 1a 64 5a 6c 22 f4 80 42 5a 64 08 bd 00 10 02 40 00 0c 02 40 00 08 02 40 00 38 02 40 08 b5 64 20 00 f0 02 ff 08 bd 08 b5 00 f0 04 ff 08 bd 08 b5 00 f0 70 f8 c0 b2 08 bd 08 b5 00 f0 99 f8 c0 b2 08 bd 00 00 0f 49 d1 f8 88 30 43 f4 70 03 c1 f8 88 30 0d 4b 1a 68 42 f0 01 02 1a 60 00 20 98 60 1a 68 22 f0 84 72 22 f4 80 32 1a 60 07 4a 5a 60 1a 68 22 f4 80 22 1a 60 d8 60 4f f0 00 63 8b 60 70 47 00 bf 00 ed 00 e0 00 38 02 40 10 30 00 24 00 b5 83 b0 02 ab 03 f8 01 0d 01 22 00 21 18 46 00 f0 46 fe 03 b0 5d f8
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 5/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S1_R1_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 06 09 82 02 00 04 fb 08 b5 0a 46 01 46 00 20 00 f0 3d fe 08 bd 00 b5 83 b0 03 0c 8d f8 04 30 03 0a 8d f8 05 30 8d f8 06 00 03 22 00 21 01 a8 00 f0 2d fe 03 b0 5d f8 04 fb 70 b5 06 46 0d 46 14 46 00 f0 46 fe 03 20 ff f7 d1 ff 30 46 ff f7 e2 ff 21 46 28 46 ff f7 d7 ff 00 f0 42 fe 20 46 70 bd 08 b5 4f f4 00 72 00 f5 61 10 ff f7 e5 ff 08 bd 15 4b 9b 68 b3 f1 ff 3f 20 d0 13 4b 1b 68 b3 f1 ff 3f 1d d0 10 4b 5b 68 b3 f1 ff 3f 1a d0 30 b5 85 b0 0d 4c 01 ad 94 e8 07 00 85 e8 07 00 00 22 02 99 00 f0 43 fe 03 90 0c 22 29 46 20 46 01 f0 cd f8 b0 fa 80 f0 40 09 05 b0 30 bd 00 20 70 47 00 20 70 47 00 20 70 47 00 40 00 08 01 20 70 47 83 68 b3 f1 ff 3f 12 d0 03 68 b3 f1 ff 3f 10 d0 0d 4a 93 42 0f d9 0d 4a 93 42 0e d8 43 68 b3 f1 ff 3f 0c d0 0a 4a 93 42 0b d9 00 20 70 47 00 20 70 47 00 20 70 47 00 20 70 47 00 20 70 47 00 20 70 47 01 20 70 47 00 bf ff 41 00 08 00 00 08 08 00 be 07 00 08 b5 00 f0 95 fd 00 f0 17 f9 03 78 1f 2b 08 d0 83 78 16 3b db b2 01 2b 0a d9 07 4b 00 22 1a 60 08 bd 43 78 27 2b f3 d1 03 4b 04 4a 1a 60 f7 e7 01 4b 03 4a 1a 60 f3 e7 20 09 00 20 8d 0f 00 08 5d 0c 00 08 f0 b5 ad f5 0d 7d 2c 22 00 21 81 a8 ff f7 4e fa 47 4b 1b 68 00 2b 00 f0 88 80 01 a9 00 20 98 47 88 b1 01 a8 ff f7 a0 ff 08 b9 00 26 0c e0 81 ac 01 ad 0f cd 0f c4 0f cd 0f c4 95 e8 07 00 84 e8 07 00 01 26 00 e0 00 26 00 24 27 46 00 e0 00 26 82 9b a3 42 18 d9 01 2e 16 d1 35 4b 1b 68 04 f5 00 75 01 a9 28 46 98 47 00 28 f0 d0 82 99 09 1b 3a 46 b1 f5 00 7f 28 bf 4f f4 00 71 01 a8 00 f0 a1 fd 07 46 2c 46 e3 e7 01 2e 0d d0 01 2e 10 d0 01 2e 1b d0 01 2e 3c d0 01 2e 3c d0
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S1_R2_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 6/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S2_R2_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 07 09 82 02 00 01 2e 41 d0 30 46 0d f5 0d 7d f0 bd 83 9b bb 42 ee d0 00 26 ee e7 0c 22 1f 49 81 a8 01 f0 14 f8 00 28 e7 d1 00 f0 20 fe 01 28 e3 d1 00 26 e3 e7 00 f0 0e fe 82 99 81 98 00 f0 12 fe 06 46 db e7 01 aa 4f f4 00 71 04 f1 00 60 00 f5 84 40 00 f0 03 fe 06 46 2c 46 01 2e d0 d1 82 9b a3 42 cd d9 0c 4b 1b 68 04 f5 00 75 01 a9 28 46 98 47 00 28 e6 d1 00 26 ee e7 00 24 ed e7 81 aa 2c 21 06 48 00 f0 ea fd 06 46 bb e7 00 f0 f6 fd ba e7 00 26 b8 e7 00 bf 20 09 00 20 00 40 00 08 00 b5 83 b0 02 ab 03 f8 01 0d 01 22 00 21 18 46 00 f0 ec fc 03 b0 5d f8 04 fb 08 b5 0a 46 01 46 00 20 00 f0 e3 fc 08 bd 00 b5 83 b0 83 09 8d f8 04 30 80 00 c0 b2 c1 f3 01 23 18 43 8d f8 05 00 8d f8 06 10 03 22 00 21 01 a8 00 f0 cf fc 03 b0 5d f8 04 fb 08 b5 06 4b a3 fb 00 23 db 09 03 eb 43 11 0a 01 81 1a 18 46 ff f7 de ff 08 bd 00 bf e1 83 0f 3e f8 b5 07 46 0e 46 14 46 1d 46 00 f0 d7 fc 01 20 ff f7 bc ff 38 46 ff f7 e3 ff 21 46 30 46 ff f7 c2 ff 04 21 28 46 ff f7 be ff 00 f0 cf fc 00 22 21 46 30 46 00 f0 f0 fc 2b 68 83 42 01 d0 00 20 f8 bd 20 1d fc e7 00 00 10 b5 00 f0 b7 fc 9f 20 ff f7 9c ff 04 4c 05 21 20 46 ff f7 a4 ff 00 f0 b5 fc 20 46 10 bd 00 bf d8 04 00 20 43 0a c0 f3 08 00 03 eb c3 13 9a 00 10 44 70 47 10 b5 82 b0 0c 46 00 f5 80 40 ff f7 f1 ff 01 ab 4f f4 00 72 21 46 00 f5 67 10 00 f5 3d 50 30 30 ff f7 b0 ff 02 b0 10 bd 44 4b 98 42 19 d0 44 4b 98 42 22 d0 43 4b 98 42 2b d0 43 4b 98 42 34 d0 42 4b 98 42 3d d0 42 4b 98 42 46 d0 41 4b 98 42 4f d0 41 4b 98 42 58 d0 40 4b 98 42 61 d0 00 20 70 47 03 f5 60 53 1a 69 42 f0 01 02 1a 61 1a 69 22 f0 01 02
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S2_R3_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 7/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S3_R3_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 08 09 82 02 00 1a 61 01 20 70 47 03 f5 50 53 1a 69 42 f0 02 02 1a 61 1a 69 22 f0 02 02 1a 61 01 20 70 47 03 f5 40 53 1a 69 42 f0 04 02 1a 61 1a 69 22 f0 04 02 1a 61 01 20 70 47 03 f5 30 53 1a 69 42 f0 08 02 1a 61 1a 69 22 f0 08 02 1a 61 01 20 70 47 03 f5 20 53 1a 69 42 f0 10 02 1a 61 1a 69 22 f0 10 02 1a 61 01 20 70 47 03 f5 10 53 1a 69 42 f0 20 02 1a 61 1a 69 22 f0 20 02 1a 61 01 20 70 47 03 f5 00 53 1a 69 42 f0 40 02 1a 61 1a 69 22 f0 40 02 1a 61 01 20 70 47 03 f5 e0 53 1a 69 42 f0 80 02 1a 61 1a 69 22 f0 80 02 1a 61 01 20 70 47 03 f5 c0 53 1a 69 42 f4 80 72 1a 61 1a 69 22 f4 80 72 1a 61 01 20 70 47 00 bf 00 00 02 40 00 04 02 40 00 08 02 40 00 0c 02 40 00 10 02 40 00 14 02 40 00 18 02 40 00 1c 02 40 00 20 02 40 f0 b4 0a 68 92 fa a2 f2 b2 fa 82 f2 18 e0 0e 69 c4 68 93 fa a3 f5 b5 fa 85 f5 6d 00 03 27 07 fa 05 f5 24 ea 05 04 93 fa a3 f5 b5 fa 85 f5 6d 00 06 fa 05 f5 2c 43 c4 60 4c 68 02 2c 36 d0 01 32 0b 68 33 fa 02 f4 64 d0 01 24 94 40 23 40 f6 d0 4e 68 04 68 93 fa a3 f5 b5 fa 85 f5 6d 00 03 27 07 fa 05 f5 24 ea 05 04 93 fa a3 f5 b5 fa 85 f5 6d 00 06 fa 05 f5 2c 43 04 60 4c 68 01 3c 01 2c c5 d8 8e 68 84 68 93 fa a3 f5 b5 fa 85 f5 6d 00 07 fa 05 f5 24 ea 05 04 93 fa a3 f5 b5 fa 85 f5 6d 00 06 fa 05 f5 2c 43 84 60 b0 e7 93 fa a3 f4 b4 fa 84 f4 07 2c 15 d8 4d 69 04 6a 93 fa a3 f6 b6 fa 86 f6 b6 00 0f 27 07 fa 06 f6 24 ea 06 04 93 fa a3 f3 b3 fa 83 f3 9b 00 05 fa 03 f3 23 43 03 62 ac e7 4c 69 45 6a 1b 0a 93 fa a3 f6 b6 fa 86 f6 b6 00 0f 27 07 fa 06 f6 25 ea 06 05 93 fa a3 f3 b3 fa 83 f3 9b 00 04 fa 03 f3 2b 43 43 62 95 e7 4a 68
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S3_R4_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 8/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S4_R4_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 09 09 82 02 00 01 3a 01 2a 02 d9 01 20 f0 bc 70 47 c9 68 42 68 22 ea 03 02 01 fb 03 f3 13 43 43 60 f3 e7 00 00 1c 4a 13 68 43 f0 01 03 13 60 1a 4b 1b 68 13 f0 02 0f fa d0 17 4a 00 23 93 60 17 4b 13 60 13 68 23 f0 f8 03 43 f0 80 03 13 60 12 4b 1b 68 13 f0 00 7f fa d1 0f 4b 11 4a 5a 60 11 4a c3 f8 84 20 da 68 22 f4 f8 52 da 60 da 68 22 f4 00 52 da 60 da 68 42 f4 1f 02 da 60 da 68 42 f4 00 12 da 60 5a 6f 22 f0 01 02 5a 67 5a 6f 42 f0 80 72 5a 67 01 20 70 47 00 38 02 40 ff ff f2 fa 10 30 00 24 00 30 00 20 10 b5 09 4b 4f f0 ff 32 1a 62 00 24 1c 62 5a 62 5c 62 1a 61 1c 61 5a 61 5c 61 9a 61 9c 61 ff f7 1d fc 20 46 10 bd 00 bf 00 38 02 40 10 b5 04 46 0e 4b 18 78 4f f4 7a 73 b3 fb f0 f3 0c 4a 10 68 b0 fb f3 f0 00 f0 86 f8 68 b9 0f 2c 01 d9 01 20 0a e0 00 22 21 46 4f f0 ff 30 00 f0 47 f8 05 4b 1c 60 00 20 00 e0 01 20 10 bd 00 bf b0 04 00 20 ac 04 00 20 b4 04 00 20 08 b5 0b 4b 1a 68 42 f4 00 72 1a 60 1a 68 42 f4 80 62 1a 60 1a 68 42 f4 80 72 1a 60 03 20 00 f0 17 f8 00 20 ff f7 c6 ff ff f7 b4 fa 00 20 08 bd 00 3c 02 40 02 4a 13 68 23 f0 02 03 13 60 70 47 10 e0 00 e0 01 4b 18 60 70 47 00 bf ac 04 00 20 07 4a d3 68 23 f4 e0 63 1b 04 1b 0c 00 02 00 f4 e0 60 18 43 40 f0 bf 60 40 f4 00 30 d0 60 70 47 00 ed 00 e0 30 b4 17 4b db 68 c3 f3 02 23 c3 f1 07 04 04 2c 28 bf 04 24 1d 1d 06 2d 18 d9 03 3b 4f f0 ff 35 05 fa 04 f4 21 ea 04 01 99 40 05 fa 03 f3 22 ea 03 03 19 43 00 28 0b db 09 01 c9 b2 00 f1 60 40 00 f5 61 40 80 f8 00 13 30 bc 70 47 00 23 e5 e7 00 f0 0f 00 09 01 c9 b2 02 4b 19 54 f4 e7 00 bf 00 ed 00 e0 14 ed 00 e0 01 38 b0 f1 80 7f 0a d2
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S4_R5_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 9/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S5_R5_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 0a 09 82 02 00 06 4b 58 60 06 4a f0 21 82 f8 23 10 00 20 98 60 07 22 1a 60 70 47 01 20 70 47 00 bf 10 e0 00 e0 00 ed 00 e0 07 4b 1a 69 22 f4 40 72 1a 61 1a 69 42 f0 04 02 1a 61 1a 69 42 ea 00 20 40 f4 80 30 18 61 70 47 00 3c 02 40 10 b4 49 b1 01 29 21 d0 02 29 02 d0 4f f4 40 74 03 e0 4f f4 00 74 00 e0 00 24 0e 4b 19 69 21 f4 40 71 19 61 1a 69 22 43 1a 61 1a 69 22 f0 f8 02 1a 61 1a 69 42 ea c0 00 40 f0 02 00 18 61 1a 69 42 f4 80 32 1a 61 5d f8 04 4b 70 47 4f f4 80 74 e3 e7 00 bf 00 3c 02 40 16 4b 1b 68 13 f4 00 7f 10 d0 14 4b 1a 68 22 f4 00 72 1a 60 1a 68 42 f4 00 62 1a 60 1a 68 22 f4 00 62 1a 60 1a 68 42 f4 00 72 1a 60 0b 4b 1b 68 13 f4 80 6f 10 d0 09 4b 1a 68 22 f4 80 62 1a 60 1a 68 42 f4 80 52 1a 60 1a 68 22 f4 80 52 1a 60 1a 68 42 f4 80 62 1a 60 70 47 00 bf 00 3c 02 40 f8 b5 22 4b 1b 7e 01 2b 3e d0 0e 46 04 46 1f 4b 01 22 1a 76 4c f2 50 30 00 f0 ee f8 07 46 70 bb 4f f0 ff 33 33 60 23 68 01 2b 16 d0 a5 68 e3 68 a2 68 13 44 ab 42 20 d9 21 7c 28 46 ff f7 84 ff 4c f2 50 30 00 f0 d8 f8 11 4a 13 69 23 f0 fa 03 13 61 07 46 80 b9 01 35 e9 e7 61 68 20 7c ff f7 61 ff 4c f2 50 30 00 f0 c7 f8 07 46 08 4a 13 69 23 f0 04 03 13 61 00 e0 35 60 ff f7 91 ff 03 4b 00 22 1a 76 38 46 f8 bd 02 27 fb e7 24 09 00 20 00 3c 02 40 10 b4 09 49 0c 69 24 f4 40 74 0c 61 0c 69 44 f4 40 74 0c 61 0c 69 44 f0 01 04 0c 61 02 60 43 60 5d f8 04 4b 70 47 00 bf 00 3c 02 40 07 4b 1a 69 22 f4 40 72 1a 61 1a 69 42 f4 00 72 1a 61 1a 69 42 f0 01 02 1a 61 01 60 70 47 00 bf 00 3c 02 40 07 4b 1a 69 22 f4 40 72 1a 61 1a 69 42 f4 80 72 1a 61 1a 69 42 f0 01 02 1a 61 01 80
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S5_R6_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 10/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S6_R6_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 0b 09 82 02 00 70 47 00 bf 00 3c 02 40 06 4b 1a 69 22 f4 40 72 1a 61 1a 69 1a 61 1a 69 42 f0 01 02 1a 61 01 70 70 47 00 bf 00 3c 02 40 20 4b db 68 13 f0 10 0f 07 d0 1f 4a d3 69 43 f0 10 03 d3 61 1b 4b 10 22 da 60 1a 4b db 68 13 f0 20 0f 07 d0 18 4a d3 69 43 f0 08 03 d3 61 15 4b 20 22 da 60 13 4b db 68 13 f0 40 0f 07 d0 12 4a d3 69 43 f0 04 03 d3 61 0e 4b 40 22 da 60 0d 4b db 68 13 f0 80 0f 07 d0 0b 4a d3 69 43 f0 02 03 d3 61 08 4b 80 22 da 60 06 4b db 68 13 f0 02 0f 07 d0 05 4a d3 69 43 f0 20 03 d3 61 01 4b 02 22 da 60 70 47 00 3c 02 40 24 09 00 20 09 4b 1b 69 00 2b 01 db 00 20 70 47 06 4b 07 4a 5a 60 02 f1 88 32 5a 60 1b 69 00 2b 01 db 00 20 70 47 01 20 70 47 00 bf 00 3c 02 40 23 01 67 45 03 4a 13 69 43 f0 00 43 13 61 00 20 70 47 00 bf 00 3c 02 40 38 b5 04 46 15 4b 00 22 da 61 00 f0 99 fb 05 46 13 4b db 68 13 f4 80 3f 0a d0 b4 f1 ff 3f f7 d0 cc b1 00 f0 8d fb 40 1b a0 42 f1 d9 03 20 0d e0 0b 4b db 68 13 f0 01 0f 02 d0 09 4b 01 22 da 60 07 4b db 68 13 f0 f2 0f 01 d1 00 20 38 bd ff f7 6f ff 01 20 fa e7 03 20 f8 e7 00 bf 24 09 00 20 00 3c 02 40 f8 b5 1d 4c 24 7e 01 2c 34 d0 1f 46 16 46 0d 46 04 46 19 4b 01 22 1a 76 4c f2 50 30 ff f7 be ff 01 46 98 b9 bc b1 01 2c 1a d0 02 2c 1d d0 32 46 3b 46 28 46 ff f7 00 ff 4c f2 50 30 ff f7 ae ff 01 46 0e 4a 13 69 23 f0 01 03 13 61 0a 4b 00 22 1a 76 08 46 f8 bd f1 b2 28 46 ff f7 27 ff eb e7 b1 b2 28 46 ff f7 10 ff e6 e7 31 46 28 46 ff f7 f9 fe e1 e7 02 21 ec e7 24 09 00 20 00 3c 02 40 02 46 03 68 13 f0 40 0f 2e d1 10 b4 00 68 20 f4 7f 40 20 f0 bf 00 0b 68 4c 68 23 43 8c 68 23 43 cc 68 23 43
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S6_R7_PF DA:48 SA:1/16  Info[10]:e6 e7 00 c7 01 c1 00 01 00 00
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - Level 19 - Передача блока данных: 11/32
+KPZ101000017410: 22.05 10:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S7_R7_PF DA:1/16 SA:48  Info[539]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 80 ff 02 01 02 02 06 00 00 00 0c 09 82 02 00 0c 69 23 43 4c 69 23 43 8c 69 23 43 cc 69 23 43 0c 6a 23 43 03 43 13 60 53 68 23 f0 04 03 c8 8a 03 43 53 60 0b 6a b3 f5 00 5f 07 d0 01 20 d3 69 23 f4 00 63 d3 61 5d f8 04 4b 70 47 8b 8c 13 61 01 20 f4 e7 00 20 d3 69 23 f4 00 63 d3 61 70 47 30 b5 8b b0 6c 46 0a 4d 0f cd 0f c4 0f cd 0f c4 95 e8 03 00 84 e8 03 00 06 4c 69 46 20 46 ff f7 b5 ff 23 68 43 f0 40 03 23 60 0b b0 30 bd 00 bf 80 1e 00 08 00 30 01 40 f8 b5 06 46 0d 46 17 46 00 24 04 e0 00 22 07 e0 00 f0 42 f8 01 34 bc 42 10 d2 00 2e f6 d0 32 5d 07 4b 1a 73 06 4b 9b 68 13 f0 01 0f fa d0 04 4b db 68 db b2 00 2d eb d0 2b 55 e9 e7 f8 bd 00 bf 00 30 01 40 02 4b 4f f4 80 02 9a 61 70 47 00 bf 00 04 02 40 01 4b 40 22 9a 61 70 47 00 04 02 40 08 b5 00 f0 d0 f8 00 f0 13 f8 00 f0 77 fa 00 f0 ab f8 ff f7 11 fa ff f7 31 fa 00 f0 95 f8 08 bd 08 b5 00 f0 09 f8 00 f0 7d fa 00 f0 5f f8 08 bd 08 b5 ff f7 2b f9 08 bd 08 b5 ff f7 2c f9 08 bd 30 b4 d2 43 00 24 08 e0 03 5d 53 40 db b2 05 4d 55 f8 23 30 83 ea 12 22 01 34 8c 42 f4 db d0 43 30 bc 70 47 b4 1e 00 08 04 4b 4f f4 00 42 9a 61 03 f5 40 63 01 22 9a 61 70 47 00 bf 00 00 02 40 04 4b 4f f0 00 42 9a 61 03 f5 40 63 4f f4 80 32 9a 61 70 47 00 00 02 40 01 4b 18 80 70 47 00 bf de 04 00 20 08 b5 00 f0 4b fa 0d 4b 1b 68 98 42 0e d3 0c 4b 1b 78 63 b9 0a 4b 01 22 1a 70 ff f7 df ff 00 f0 3d fa 08 4b 1b 88 18 44 04 4b 18 60 08 bd 04 4b 00 22 1a 70 ff f7 c6 ff f1 e7 00 bf b8 04 00 20 e0 04 00 20 de 04 00 20 08 b5 0b 4b 1b 78 01 2b 00 d0 08 bd 00 f0 22 fa 08 4b 1b 68 08 4a 12 68 13 44 03 f5 fa 73 98 42 f3 d3 03 4b 00 22 1a 70 00 f0 4c f8
```

### Comparing `DLMS_Firmware_updater-0.3.1/test/config.toml` & `DLMS_Firmware_updater-0.3.2/test/config.toml`

 * *Files identical despite different names*

