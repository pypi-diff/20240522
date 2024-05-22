# Comparing `tmp/you-get-0.4.990.tar.gz` & `tmp/you-get-0.4.995.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/you-get-0.4.990.tar", last modified: Sat Dec  2 00:37:55 2017, max compression
+gzip compressed data, was "dist/you-get-0.4.995.tar", last modified: Mon Dec  4 03:19:49 2017, max compression
```

## Comparing `you-get-0.4.990.tar` & `you-get-0.4.995.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:55.000000 you-get-0.4.990/
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1265 2017-04-01 19:55:49.000000 you-get-0.4.990/you-get.json
--rwxr-xr-x   0 soimort   (1000) soimort   (1000)      477 2016-10-14 18:26:29.000000 you-get-0.4.990/you-get
--rw-r--r--   0 soimort   (1000) soimort   (1000)    19552 2017-12-02 00:35:52.000000 you-get-0.4.990/README.md
--rw-r--r--   0 soimort   (1000) soimort   (1000)      805 2016-10-14 18:26:29.000000 you-get-0.4.990/Makefile
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2476 2016-10-14 18:26:29.000000 you-get-0.4.990/README.rst
--rw-r--r--   0 soimort   (1000) soimort   (1000)      100 2017-12-02 00:37:55.000000 you-get-0.4.990/setup.cfg
--rwxr-xr-x   0 soimort   (1000) soimort   (1000)     1218 2016-10-14 18:26:29.000000 you-get-0.4.990/setup.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:54.000000 you-get-0.4.990/src/
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get/
--rw-r--r--   0 soimort   (1000) soimort   (1000)      371 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/__init__.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     9957 2017-10-13 21:45:38.000000 you-get-0.4.990/src/you_get/extractor.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get/cli_wrapper/
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/__init__.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get/cli_wrapper/player/
--rw-r--r--   0 soimort   (1000) soimort   (1000)       46 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/player/__init__.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)       22 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/player/vlc.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/player/dragonplayer.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/player/wmp.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/player/mplayer.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      150 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/cli_wrapper/player/__main__.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/player/gnome_mplayer.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get/cli_wrapper/transcoder/
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/transcoder/__init__.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/transcoder/mencoder.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/transcoder/libav.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/transcoder/ffmpeg.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get/cli_wrapper/downloader/
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/downloader/__init__.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get/cli_wrapper/openssl/
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/cli_wrapper/openssl/__init__.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1599 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/json_output.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:55.000000 you-get-0.4.990/src/you_get/processor/
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1711 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/processor/rtmpdump.py
--rwxr-xr-x   0 soimort   (1000) soimort   (1000)    10222 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/processor/join_flv.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1624 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/processor/join_ts.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      135 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/processor/__init__.py
--rwxr-xr-x   0 soimort   (1000) soimort   (1000)     9783 2017-11-27 20:40:22.000000 you-get-0.4.990/src/you_get/processor/ffmpeg.py
--rwxr-xr-x   0 soimort   (1000) soimort   (1000)    30413 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/processor/join_mp4.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2578 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/__main__.py
--rwxr-xr-x   0 soimort   (1000) soimort   (1000)    48296 2017-12-02 00:35:52.000000 you-get-0.4.990/src/you_get/common.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:55.000000 you-get-0.4.990/src/you_get/extractors/
--rw-r--r--   0 soimort   (1000) soimort   (1000)     7799 2017-07-08 00:58:49.000000 you-get-0.4.990/src/you_get/extractors/netease.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1560 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/qingting.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      863 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/ted.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2731 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/extractors/douyutv.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2676 2017-05-21 12:11:28.000000 you-get-0.4.990/src/you_get/extractors/imgur.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1652 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/qq_egame.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2952 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/extractors/sohu.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)    15351 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/extractors/icourses.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      726 2017-02-01 22:34:42.000000 you-get-0.4.990/src/you_get/extractors/_jpopsuki.py
--rwxr-xr-x   0 soimort   (1000) soimort   (1000)     2378 2017-10-13 21:45:38.000000 you-get-0.4.990/src/you_get/extractors/instagram.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1213 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/dailymotion.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1623 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/mtv81.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1280 2017-04-16 10:25:45.000000 you-get-0.4.990/src/you_get/extractors/yizhibo.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1760 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/ifeng.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2968 2017-02-01 22:34:42.000000 you-get-0.4.990/src/you_get/extractors/_thvideo.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      828 2017-10-13 21:45:38.000000 you-get-0.4.990/src/you_get/extractors/giphy.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      616 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/archive.py
--rwxr-xr-x   0 soimort   (1000) soimort   (1000)     1898 2017-11-27 20:40:22.000000 you-get-0.4.990/src/you_get/extractors/__init__.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1414 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/suntv.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)    14352 2017-11-27 20:40:22.000000 you-get-0.4.990/src/you_get/extractors/bilibili.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1946 2017-04-16 10:25:45.000000 you-get-0.4.990/src/you_get/extractors/nanagogo.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      997 2016-11-03 15:56:05.000000 you-get-0.4.990/src/you_get/extractors/huomaotv.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      617 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/cbs.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     3952 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/extractors/yixia.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1439 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/kuwo.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     3675 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/showroom.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4510 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/extractors/universal.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1190 2015-10-05 19:03:54.000000 you-get-0.4.990/src/you_get/extractors/_videobam.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1483 2015-10-05 19:03:54.000000 you-get-0.4.990/src/you_get/extractors/_songtaste.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     3731 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/extractors/twitter.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2281 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/huaban.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      605 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/alive.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     6600 2016-08-26 17:15:53.000000 you-get-0.4.990/src/you_get/extractors/_bilibili.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4336 2017-04-16 10:25:45.000000 you-get-0.4.990/src/you_get/extractors/dilidili.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     5924 2017-11-27 20:40:22.000000 you-get-0.4.990/src/you_get/extractors/mgtv.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     5443 2017-05-21 12:11:28.000000 you-get-0.4.990/src/you_get/extractors/ucas.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     8971 2017-09-16 09:35:32.000000 you-get-0.4.990/src/you_get/extractors/google.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2398 2017-01-10 16:46:09.000000 you-get-0.4.990/src/you_get/extractors/lizhi.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      748 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/bandcamp.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1177 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/vidto.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     6516 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/extractors/qq.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      806 2017-01-10 16:46:09.000000 you-get-0.4.990/src/you_get/extractors/magisto.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2901 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/qie_video.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1998 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/kugou.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4301 2015-10-05 19:03:54.000000 you-get-0.4.990/src/you_get/extractors/_coursera.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     3514 2017-04-16 10:25:45.000000 you-get-0.4.990/src/you_get/extractors/ckplayer.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     6989 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/vimeo.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2711 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/tucao.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)    11838 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/iqiyi.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4211 2017-05-21 12:11:28.000000 you-get-0.4.990/src/you_get/extractors/ximalaya.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      865 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/metacafe.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      965 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/facebook.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1576 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/videomega.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2400 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/bigthink.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      988 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/theplatform.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2137 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/miaopai.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)    23977 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/youtube.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1176 2017-11-27 20:40:22.000000 you-get-0.4.990/src/you_get/extractors/vine.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2305 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/zhanqi.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1447 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/w56.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4859 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/extractors/acfun.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1902 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/yinyuetai.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     7704 2017-07-23 21:09:38.000000 you-get-0.4.990/src/you_get/extractors/flickr.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     3376 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/bokecc.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      666 2015-10-05 19:03:54.000000 you-get-0.4.990/src/you_get/extractors/_blip.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4687 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/extractors/tumblr.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1211 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/baomihua.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1438 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/veoh.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      892 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/iqilu.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      847 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/quanmin.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      508 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/khan.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     3605 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/qie.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     3886 2017-11-27 20:40:22.000000 you-get-0.4.990/src/you_get/extractors/coub.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     8715 2017-10-13 21:45:38.000000 you-get-0.4.990/src/you_get/extractors/xiami.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2707 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/cntv.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      663 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/freesound.py
--rwxr-xr-x   0 soimort   (1000) soimort   (1000)     4860 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/wanmen.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1324 2017-02-01 22:34:42.000000 you-get-0.4.990/src/you_get/extractors/_qianmo.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1955 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/miomio.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     5515 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/embed.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     8143 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/funshion.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2966 2015-10-05 19:03:54.000000 you-get-0.4.990/src/you_get/extractors/_catfun.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     6363 2017-05-21 12:11:28.000000 you-get-0.4.990/src/you_get/extractors/le.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)    10348 2017-10-13 21:45:38.000000 you-get-0.4.990/src/you_get/extractors/pptv.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4564 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/sina.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1975 2017-02-01 22:34:42.000000 you-get-0.4.990/src/you_get/extractors/_dongting.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1598 2017-09-16 09:47:00.000000 you-get-0.4.990/src/you_get/extractors/soundcloud.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1555 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/panda.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)    11648 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/baidu.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      694 2015-10-05 19:03:54.000000 you-get-0.4.990/src/you_get/extractors/_vid48.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1440 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/iwara.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1015 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/musicplayon.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4429 2017-10-13 13:02:31.000000 you-get-0.4.990/src/you_get/extractors/tudou.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2362 2017-11-27 20:40:22.000000 you-get-0.4.990/src/you_get/extractors/toutiao.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1898 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/infoq.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1353 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/naver.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     3798 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/pixnet.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      861 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/heavymusic.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1729 2017-07-23 21:09:38.000000 you-get-0.4.990/src/you_get/extractors/nicovideo.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2339 2016-11-19 19:47:48.000000 you-get-0.4.990/src/you_get/extractors/douban.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1110 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/interest.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1110 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/ehow.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      891 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/mixcloud.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1507 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/joy.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1894 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/fantasy.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2796 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/ku6.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2439 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/fc2video.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2430 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/extractors/vk.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1628 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/extractors/pinterest.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)    12310 2017-12-02 00:35:52.000000 you-get-0.4.990/src/you_get/extractors/youku.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:55.000000 you-get-0.4.990/src/you_get/util/
--rw-r--r--   0 soimort   (1000) soimort   (1000)      303 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/util/term.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)      765 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/util/strings.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/util/__init__.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     2585 2017-09-11 13:33:09.000000 you-get-0.4.990/src/you_get/util/log.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1049 2017-11-17 16:14:52.000000 you-get-0.4.990/src/you_get/util/fs.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1489 2016-10-14 18:26:29.000000 you-get-0.4.990/src/you_get/util/git.py
--rw-r--r--   0 soimort   (1000) soimort   (1000)       71 2017-12-02 00:35:52.000000 you-get-0.4.990/src/you_get/version.py
-drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get.egg-info/
--rw-r--r--   0 soimort   (1000) soimort   (1000)     5095 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get.egg-info/SOURCES.txt
--rw-r--r--   0 soimort   (1000) soimort   (1000)        8 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get.egg-info/top_level.txt
--rw-r--r--   0 soimort   (1000) soimort   (1000)       51 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get.egg-info/entry_points.txt
--rw-r--r--   0 soimort   (1000) soimort   (1000)        1 2015-11-11 21:26:02.000000 you-get-0.4.990/src/you_get.egg-info/zip-safe
--rw-r--r--   0 soimort   (1000) soimort   (1000)        1 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get.egg-info/dependency_links.txt
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4279 2017-12-02 00:37:54.000000 you-get-0.4.990/src/you_get.egg-info/PKG-INFO
--rw-r--r--   0 soimort   (1000) soimort   (1000)     1254 2017-04-01 19:55:49.000000 you-get-0.4.990/LICENSE.txt
--rw-r--r--   0 soimort   (1000) soimort   (1000)      100 2016-10-14 18:26:29.000000 you-get-0.4.990/MANIFEST.in
--rw-r--r--   0 soimort   (1000) soimort   (1000)    10866 2016-10-14 18:26:29.000000 you-get-0.4.990/CHANGELOG.rst
--rw-r--r--   0 soimort   (1000) soimort   (1000)     4279 2017-12-02 00:37:55.000000 you-get-0.4.990/PKG-INFO
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:49.000000 you-get-0.4.995/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1265 2017-04-01 19:55:49.000000 you-get-0.4.995/you-get.json
+-rwxr-xr-x   0 soimort   (1000) soimort   (1000)      477 2016-10-14 18:26:29.000000 you-get-0.4.995/you-get
+-rw-r--r--   0 soimort   (1000) soimort   (1000)    19588 2017-12-04 03:18:49.000000 you-get-0.4.995/README.md
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      805 2016-10-14 18:26:29.000000 you-get-0.4.995/Makefile
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2476 2016-10-14 18:26:29.000000 you-get-0.4.995/README.rst
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      100 2017-12-04 03:19:49.000000 you-get-0.4.995/setup.cfg
+-rwxr-xr-x   0 soimort   (1000) soimort   (1000)     1218 2016-10-14 18:26:29.000000 you-get-0.4.995/setup.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:48.000000 you-get-0.4.995/src/
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:48.000000 you-get-0.4.995/src/you_get/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      371 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/__init__.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     9957 2017-12-04 02:46:59.000000 you-get-0.4.995/src/you_get/extractor.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:48.000000 you-get-0.4.995/src/you_get/cli_wrapper/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/__init__.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:48.000000 you-get-0.4.995/src/you_get/cli_wrapper/player/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)       46 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/player/__init__.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)       22 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/player/vlc.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/player/dragonplayer.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/player/wmp.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/player/mplayer.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      150 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/cli_wrapper/player/__main__.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/player/gnome_mplayer.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:48.000000 you-get-0.4.995/src/you_get/cli_wrapper/transcoder/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/transcoder/__init__.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/transcoder/mencoder.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/transcoder/libav.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/transcoder/ffmpeg.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:48.000000 you-get-0.4.995/src/you_get/cli_wrapper/downloader/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/downloader/__init__.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:48.000000 you-get-0.4.995/src/you_get/cli_wrapper/openssl/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/cli_wrapper/openssl/__init__.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1599 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/json_output.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:49.000000 you-get-0.4.995/src/you_get/processor/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1711 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/processor/rtmpdump.py
+-rwxr-xr-x   0 soimort   (1000) soimort   (1000)    10222 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/processor/join_flv.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1624 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/processor/join_ts.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      135 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/processor/__init__.py
+-rwxr-xr-x   0 soimort   (1000) soimort   (1000)     9783 2017-11-27 20:40:22.000000 you-get-0.4.995/src/you_get/processor/ffmpeg.py
+-rwxr-xr-x   0 soimort   (1000) soimort   (1000)    30413 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/processor/join_mp4.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2578 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/__main__.py
+-rwxr-xr-x   0 soimort   (1000) soimort   (1000)    48296 2017-12-03 21:27:58.000000 you-get-0.4.995/src/you_get/common.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:49.000000 you-get-0.4.995/src/you_get/extractors/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     7799 2017-07-08 00:58:49.000000 you-get-0.4.995/src/you_get/extractors/netease.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1560 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/qingting.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      863 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/ted.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2731 2017-11-17 16:14:52.000000 you-get-0.4.995/src/you_get/extractors/douyutv.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2676 2017-05-21 12:11:28.000000 you-get-0.4.995/src/you_get/extractors/imgur.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1652 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/qq_egame.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2952 2017-11-17 16:14:52.000000 you-get-0.4.995/src/you_get/extractors/sohu.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)    15351 2017-11-17 16:14:52.000000 you-get-0.4.995/src/you_get/extractors/icourses.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      726 2017-02-01 22:34:42.000000 you-get-0.4.995/src/you_get/extractors/_jpopsuki.py
+-rwxr-xr-x   0 soimort   (1000) soimort   (1000)     2378 2017-10-13 21:45:38.000000 you-get-0.4.995/src/you_get/extractors/instagram.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1213 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/dailymotion.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1623 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/mtv81.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1280 2017-04-16 10:25:45.000000 you-get-0.4.995/src/you_get/extractors/yizhibo.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1760 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/ifeng.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2968 2017-02-01 22:34:42.000000 you-get-0.4.995/src/you_get/extractors/_thvideo.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      828 2017-10-13 21:45:38.000000 you-get-0.4.995/src/you_get/extractors/giphy.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      616 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/archive.py
+-rwxr-xr-x   0 soimort   (1000) soimort   (1000)     1898 2017-11-27 20:40:22.000000 you-get-0.4.995/src/you_get/extractors/__init__.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1414 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/suntv.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)    14210 2017-12-04 03:18:49.000000 you-get-0.4.995/src/you_get/extractors/bilibili.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1946 2017-04-16 10:25:45.000000 you-get-0.4.995/src/you_get/extractors/nanagogo.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      997 2016-11-03 15:56:05.000000 you-get-0.4.995/src/you_get/extractors/huomaotv.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      617 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/cbs.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     3952 2017-11-17 16:14:52.000000 you-get-0.4.995/src/you_get/extractors/yixia.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1439 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/kuwo.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     3675 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/showroom.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4510 2017-12-03 21:30:54.000000 you-get-0.4.995/src/you_get/extractors/universal.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1190 2015-10-05 19:03:54.000000 you-get-0.4.995/src/you_get/extractors/_videobam.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1483 2015-10-05 19:03:54.000000 you-get-0.4.995/src/you_get/extractors/_songtaste.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     3731 2017-11-17 16:14:52.000000 you-get-0.4.995/src/you_get/extractors/twitter.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2281 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/huaban.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      605 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/alive.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     6600 2016-08-26 17:15:53.000000 you-get-0.4.995/src/you_get/extractors/_bilibili.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4336 2017-04-16 10:25:45.000000 you-get-0.4.995/src/you_get/extractors/dilidili.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     5924 2017-11-27 20:40:22.000000 you-get-0.4.995/src/you_get/extractors/mgtv.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     5443 2017-05-21 12:11:28.000000 you-get-0.4.995/src/you_get/extractors/ucas.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     8971 2017-09-16 09:35:32.000000 you-get-0.4.995/src/you_get/extractors/google.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2398 2017-01-10 16:46:09.000000 you-get-0.4.995/src/you_get/extractors/lizhi.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      748 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/bandcamp.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1177 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/vidto.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     6516 2017-11-17 16:14:52.000000 you-get-0.4.995/src/you_get/extractors/qq.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      806 2017-01-10 16:46:09.000000 you-get-0.4.995/src/you_get/extractors/magisto.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2901 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/qie_video.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1998 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/kugou.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4301 2015-10-05 19:03:54.000000 you-get-0.4.995/src/you_get/extractors/_coursera.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     3514 2017-04-16 10:25:45.000000 you-get-0.4.995/src/you_get/extractors/ckplayer.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     6989 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/vimeo.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2711 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/tucao.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)    11838 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/iqiyi.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4211 2017-05-21 12:11:28.000000 you-get-0.4.995/src/you_get/extractors/ximalaya.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      865 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/metacafe.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      965 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/facebook.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1576 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/videomega.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2400 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/bigthink.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      988 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/theplatform.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2137 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/miaopai.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)    23977 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/youtube.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1176 2017-11-27 20:40:22.000000 you-get-0.4.995/src/you_get/extractors/vine.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2305 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/zhanqi.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1447 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/w56.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4859 2017-11-17 16:14:52.000000 you-get-0.4.995/src/you_get/extractors/acfun.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1902 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/yinyuetai.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     7704 2017-07-23 21:09:38.000000 you-get-0.4.995/src/you_get/extractors/flickr.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     3376 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/bokecc.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      666 2015-10-05 19:03:54.000000 you-get-0.4.995/src/you_get/extractors/_blip.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4687 2017-11-17 16:14:52.000000 you-get-0.4.995/src/you_get/extractors/tumblr.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1211 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/baomihua.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1438 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/veoh.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      892 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/iqilu.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      847 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/quanmin.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      508 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/khan.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     3605 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/qie.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     3886 2017-11-27 20:40:22.000000 you-get-0.4.995/src/you_get/extractors/coub.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     8715 2017-10-13 21:45:38.000000 you-get-0.4.995/src/you_get/extractors/xiami.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2707 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/cntv.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      663 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/freesound.py
+-rwxr-xr-x   0 soimort   (1000) soimort   (1000)     4860 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/wanmen.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1324 2017-02-01 22:34:42.000000 you-get-0.4.995/src/you_get/extractors/_qianmo.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1955 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/miomio.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     5515 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/embed.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     8143 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/funshion.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2966 2015-10-05 19:03:54.000000 you-get-0.4.995/src/you_get/extractors/_catfun.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     6363 2017-05-21 12:11:28.000000 you-get-0.4.995/src/you_get/extractors/le.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)    10348 2017-10-13 21:45:38.000000 you-get-0.4.995/src/you_get/extractors/pptv.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4564 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/sina.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1975 2017-02-01 22:34:42.000000 you-get-0.4.995/src/you_get/extractors/_dongting.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1598 2017-09-16 09:47:00.000000 you-get-0.4.995/src/you_get/extractors/soundcloud.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1555 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/panda.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)    11648 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/baidu.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      694 2015-10-05 19:03:54.000000 you-get-0.4.995/src/you_get/extractors/_vid48.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1440 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/iwara.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1015 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/musicplayon.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4429 2017-10-13 13:02:31.000000 you-get-0.4.995/src/you_get/extractors/tudou.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2362 2017-11-27 20:40:22.000000 you-get-0.4.995/src/you_get/extractors/toutiao.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1898 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/infoq.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1353 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/naver.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     3798 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/pixnet.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      861 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/heavymusic.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1729 2017-07-23 21:09:38.000000 you-get-0.4.995/src/you_get/extractors/nicovideo.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2339 2016-11-19 19:47:48.000000 you-get-0.4.995/src/you_get/extractors/douban.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1110 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/interest.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1110 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/ehow.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      891 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/mixcloud.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1507 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/joy.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1894 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/fantasy.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2796 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/ku6.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2439 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/fc2video.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2430 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/extractors/vk.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1628 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/extractors/pinterest.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)    12310 2017-12-04 03:18:49.000000 you-get-0.4.995/src/you_get/extractors/youku.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:49.000000 you-get-0.4.995/src/you_get/util/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      303 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/util/term.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      765 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/util/strings.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        0 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/util/__init__.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     2585 2017-09-11 13:33:09.000000 you-get-0.4.995/src/you_get/util/log.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1049 2017-11-17 16:14:52.000000 you-get-0.4.995/src/you_get/util/fs.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1489 2016-10-14 18:26:29.000000 you-get-0.4.995/src/you_get/util/git.py
+-rw-r--r--   0 soimort   (1000) soimort   (1000)       71 2017-12-04 03:18:49.000000 you-get-0.4.995/src/you_get/version.py
+drwxr-xr-x   0 soimort   (1000) soimort   (1000)        0 2017-12-04 03:19:48.000000 you-get-0.4.995/src/you_get.egg-info/
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     5095 2017-12-04 03:19:48.000000 you-get-0.4.995/src/you_get.egg-info/SOURCES.txt
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        8 2017-12-04 03:19:47.000000 you-get-0.4.995/src/you_get.egg-info/top_level.txt
+-rw-r--r--   0 soimort   (1000) soimort   (1000)       51 2017-12-04 03:19:47.000000 you-get-0.4.995/src/you_get.egg-info/entry_points.txt
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        1 2015-11-11 21:26:02.000000 you-get-0.4.995/src/you_get.egg-info/zip-safe
+-rw-r--r--   0 soimort   (1000) soimort   (1000)        1 2017-12-04 03:19:47.000000 you-get-0.4.995/src/you_get.egg-info/dependency_links.txt
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4279 2017-12-04 03:19:47.000000 you-get-0.4.995/src/you_get.egg-info/PKG-INFO
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     1254 2017-04-01 19:55:49.000000 you-get-0.4.995/LICENSE.txt
+-rw-r--r--   0 soimort   (1000) soimort   (1000)      100 2016-10-14 18:26:29.000000 you-get-0.4.995/MANIFEST.in
+-rw-r--r--   0 soimort   (1000) soimort   (1000)    10866 2016-10-14 18:26:29.000000 you-get-0.4.995/CHANGELOG.rst
+-rw-r--r--   0 soimort   (1000) soimort   (1000)     4279 2017-12-04 03:19:49.000000 you-get-0.4.995/PKG-INFO
```

### Comparing `you-get-0.4.990/you-get.json` & `you-get-0.4.995/you-get.json`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/README.md` & `you-get-0.4.995/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,31 @@
 
 [![PyPI version](https://img.shields.io/pypi/v/you-get.svg)](https://pypi.python.org/pypi/you-get/)
 [![Build Status](https://travis-ci.org/soimort/you-get.svg)](https://travis-ci.org/soimort/you-get)
 [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/soimort/you-get?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 [You-Get](https://you-get.org/) is a tiny command-line utility to download media contents (videos, audios, images) from the Web, in case there is no other handy way to do it.
 
-Here's how you use `you-get` to download a video from [this web page](http://www.fsf.org/blogs/rms/20140407-geneva-tedx-talk-free-software-free-society):
+Here's how you use `you-get` to download a video from [YouTube](https://www.youtube.com/watch?v=jNQXAC9IVRw):
 
 ```console
-$ you-get http://www.fsf.org/blogs/rms/20140407-geneva-tedx-talk-free-software-free-society
-Site:       fsf.org
-Title:      TEDxGE2014_Stallman05_LQ
-Type:       WebM video (video/webm)
-Size:       27.12 MiB (28435804 Bytes)
+$ you-get 'https://www.youtube.com/watch?v=jNQXAC9IVRw'
+site:                YouTube
+title:               Me at the zoo
+stream:
+    - itag:          43
+      container:     webm
+      quality:       medium
+      size:          0.5 MiB (564215 bytes)
+    # download-with: you-get --itag=43 [URL]
 
-Downloading TEDxGE2014_Stallman05_LQ.webm ...
-100.0% ( 27.1/27.1 MB) ├████████████████████████████████████████┤[1/1]   12 MB/s
+Downloading Me at the zoo.webm ...
+ 100% (  0.5/  0.5MB) ├██████████████████████████████████┤[1/1]    6 MB/s
+
+Saving Me at the zoo.en.srt ... Done.
 ```
 
 And here's why you might want to use it:
 
 * You enjoyed something on the Internet, and just want to download them for your own pleasure.
 * You watch your favorite videos online from your computer, but you are prohibited from saving them. You feel that you have no control over your own computer. (And it's not how an open Web is supposed to work.)
 * You want to get rid of any closed-source technology or proprietary JavaScript code, and disallow things like Flash running on your computer.
```

### Comparing `you-get-0.4.990/Makefile` & `you-get-0.4.995/Makefile`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/README.rst` & `you-get-0.4.995/README.rst`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/setup.py` & `you-get-0.4.995/setup.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractor.py` & `you-get-0.4.995/src/you_get/extractor.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/json_output.py` & `you-get-0.4.995/src/you_get/json_output.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/processor/rtmpdump.py` & `you-get-0.4.995/src/you_get/processor/rtmpdump.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/processor/join_flv.py` & `you-get-0.4.995/src/you_get/processor/join_flv.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/processor/join_ts.py` & `you-get-0.4.995/src/you_get/processor/join_ts.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/processor/ffmpeg.py` & `you-get-0.4.995/src/you_get/processor/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/processor/join_mp4.py` & `you-get-0.4.995/src/you_get/processor/join_mp4.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/__main__.py` & `you-get-0.4.995/src/you_get/__main__.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/common.py` & `you-get-0.4.995/src/you_get/common.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/netease.py` & `you-get-0.4.995/src/you_get/extractors/netease.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/qingting.py` & `you-get-0.4.995/src/you_get/extractors/qingting.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/ted.py` & `you-get-0.4.995/src/you_get/extractors/ted.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/douyutv.py` & `you-get-0.4.995/src/you_get/extractors/douyutv.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/imgur.py` & `you-get-0.4.995/src/you_get/extractors/imgur.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/qq_egame.py` & `you-get-0.4.995/src/you_get/extractors/qq_egame.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/sohu.py` & `you-get-0.4.995/src/you_get/extractors/sohu.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/icourses.py` & `you-get-0.4.995/src/you_get/extractors/icourses.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_jpopsuki.py` & `you-get-0.4.995/src/you_get/extractors/_jpopsuki.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/instagram.py` & `you-get-0.4.995/src/you_get/extractors/instagram.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/dailymotion.py` & `you-get-0.4.995/src/you_get/extractors/dailymotion.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/mtv81.py` & `you-get-0.4.995/src/you_get/extractors/mtv81.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/yizhibo.py` & `you-get-0.4.995/src/you_get/extractors/yizhibo.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/ifeng.py` & `you-get-0.4.995/src/you_get/extractors/ifeng.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_thvideo.py` & `you-get-0.4.995/src/you_get/extractors/_thvideo.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/giphy.py` & `you-get-0.4.995/src/you_get/extractors/giphy.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/archive.py` & `you-get-0.4.995/src/you_get/extractors/archive.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/__init__.py` & `you-get-0.4.995/src/you_get/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/suntv.py` & `you-get-0.4.995/src/you_get/extractors/suntv.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/bilibili.py` & `you-get-0.4.995/src/you_get/extractors/bilibili.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,45 +83,40 @@
             self.streams[stream_type] = {}
             self.streams[stream_type]['src'] = urls_list
             self.streams[stream_type]['size'] = total_size
             self.streams[stream_type]['container'] = container
 
     def download_by_vid(self, cid, bangumi, **kwargs):
         stream_id = kwargs.get('stream_id')
-# guard here. if stream_id invalid, fallback as not stream_id
+        # guard here. if stream_id invalid, fallback as not stream_id
         if stream_id and stream_id in self.fmt2qlt:
             quality = stream_id
         else:
             quality = 'hdflv' if bangumi else 'flv'
 
         info_only = kwargs.get('info_only')
-        if not info_only or stream_id:
-# won't be None
-            qlt = self.fmt2qlt.get(quality)
+        for qlt in range(4, -1, -1):
             api_xml = self.api_req(cid, qlt, bangumi, **kwargs)
             self.parse_bili_xml(api_xml)
+        if not info_only or stream_id:
             self.danmuku = get_danmuku_xml(cid)
-        else:
-            for qlt in range(4, 0, -1):
-                api_xml = self.api_req(cid, qlt, bangumi, **kwargs)
-                self.parse_bili_xml(api_xml)
 
     def prepare(self, **kwargs):
         if socket.getdefaulttimeout() == 600: # no timeout specified
             socket.setdefaulttimeout(2) # fail fast, very speedy!
 
         # handle "watchlater" URLs
         if '/watchlater/' in self.url:
             aid = re.search(r'av(\d+)', self.url).group(1)
             self.url = 'http://www.bilibili.com/video/av{}/'.format(aid)
 
         self.ua = fake_headers['User-Agent']
         self.url = url_locations([self.url])[0]
         frag = urllib.parse.urlparse(self.url).fragment
-# http://www.bilibili.com/video/av3141144/index_2.html#page=3
+        # http://www.bilibili.com/video/av3141144/index_2.html#page=3
         if frag:
             hit = re.search(r'page=(\d+)', frag)
             if hit is not None:
                 page = hit.group(1)
                 aid = re.search(r'av(\d+)', self.url).group(1)
                 self.url = 'http://www.bilibili.com/video/av{}/index_{}.html'.format(aid, page)
         self.referer = self.url
@@ -149,33 +144,33 @@
         else:
             self.entry(**kwargs)
 
     def movie_entry(self, **kwargs):
         patt = r"var\s*aid\s*=\s*'(\d+)'"
         aid = re.search(patt, self.page).group(1)
         page_list = json.loads(get_content('http://www.bilibili.com/widget/getPageList?aid={}'.format(aid)))
-# better ideas for bangumi_movie titles?
+        # better ideas for bangumi_movie titles?
         self.title = page_list[0]['pagename']
         self.download_by_vid(page_list[0]['cid'], True, bangumi_movie=True, **kwargs)
 
     def entry(self, **kwargs):
-# tencent player
+        # tencent player
         tc_flashvars = re.search(r'"bili-cid=\d+&bili-aid=\d+&vid=([^"]+)"', self.page)
         if tc_flashvars:
             tc_flashvars = tc_flashvars.group(1)
         if tc_flashvars is not None:
             self.out = True
             qq_download_by_vid(tc_flashvars, self.title, output_dir=kwargs['output_dir'], merge=kwargs['merge'], info_only=kwargs['info_only'])
             return
 
         cid = re.search(r'cid=(\d+)', self.page).group(1)
         if cid is not None:
             self.download_by_vid(cid, False, **kwargs)
         else:
-# flashvars?
+            # flashvars?
             flashvars = re.search(r'flashvars="([^"]+)"', self.page).group(1)
             if flashvars is None:
                 raise Exception('Unsupported page {}'.format(self.url))
             param = flashvars.split('&')[0]
             t, cid = param.split('=')
             t = t.strip()
             cid = cid.strip()
@@ -323,15 +318,15 @@
         return urls_list, total_size
     except Exception as e:
         log.w(e)
         return [], 0
 
 def bilibili_download_playlist_by_url(url, **kwargs):
     url = url_locations([url])[0]
-# a bangumi here? possible?
+    # a bangumi here? possible?
     if 'live.bilibili' in url:
         site.download_by_url(url)
     elif 'bangumi.bilibili' in url:
         bangumi_id = re.search(r'(\d+)', url).group(1)
         bangumi_data = get_bangumi_info(bangumi_id)
         ep_ids = collect_bangumi_epids(bangumi_data)
```

### Comparing `you-get-0.4.990/src/you_get/extractors/nanagogo.py` & `you-get-0.4.995/src/you_get/extractors/nanagogo.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/huomaotv.py` & `you-get-0.4.995/src/you_get/extractors/huomaotv.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/cbs.py` & `you-get-0.4.995/src/you_get/extractors/cbs.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/yixia.py` & `you-get-0.4.995/src/you_get/extractors/yixia.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/kuwo.py` & `you-get-0.4.995/src/you_get/extractors/kuwo.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/showroom.py` & `you-get-0.4.995/src/you_get/extractors/showroom.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/universal.py` & `you-get-0.4.995/src/you_get/extractors/universal.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_videobam.py` & `you-get-0.4.995/src/you_get/extractors/_videobam.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_songtaste.py` & `you-get-0.4.995/src/you_get/extractors/_songtaste.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/twitter.py` & `you-get-0.4.995/src/you_get/extractors/twitter.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/huaban.py` & `you-get-0.4.995/src/you_get/extractors/huaban.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/alive.py` & `you-get-0.4.995/src/you_get/extractors/alive.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_bilibili.py` & `you-get-0.4.995/src/you_get/extractors/_bilibili.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/dilidili.py` & `you-get-0.4.995/src/you_get/extractors/dilidili.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/mgtv.py` & `you-get-0.4.995/src/you_get/extractors/mgtv.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/ucas.py` & `you-get-0.4.995/src/you_get/extractors/ucas.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/google.py` & `you-get-0.4.995/src/you_get/extractors/google.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/lizhi.py` & `you-get-0.4.995/src/you_get/extractors/lizhi.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/bandcamp.py` & `you-get-0.4.995/src/you_get/extractors/bandcamp.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/vidto.py` & `you-get-0.4.995/src/you_get/extractors/vidto.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/qq.py` & `you-get-0.4.995/src/you_get/extractors/qq.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/magisto.py` & `you-get-0.4.995/src/you_get/extractors/magisto.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/qie_video.py` & `you-get-0.4.995/src/you_get/extractors/qie_video.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/kugou.py` & `you-get-0.4.995/src/you_get/extractors/kugou.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_coursera.py` & `you-get-0.4.995/src/you_get/extractors/_coursera.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/ckplayer.py` & `you-get-0.4.995/src/you_get/extractors/ckplayer.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/vimeo.py` & `you-get-0.4.995/src/you_get/extractors/vimeo.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/tucao.py` & `you-get-0.4.995/src/you_get/extractors/tucao.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/iqiyi.py` & `you-get-0.4.995/src/you_get/extractors/iqiyi.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/ximalaya.py` & `you-get-0.4.995/src/you_get/extractors/ximalaya.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/metacafe.py` & `you-get-0.4.995/src/you_get/extractors/metacafe.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/facebook.py` & `you-get-0.4.995/src/you_get/extractors/facebook.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/videomega.py` & `you-get-0.4.995/src/you_get/extractors/videomega.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/bigthink.py` & `you-get-0.4.995/src/you_get/extractors/bigthink.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/theplatform.py` & `you-get-0.4.995/src/you_get/extractors/theplatform.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/miaopai.py` & `you-get-0.4.995/src/you_get/extractors/miaopai.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/youtube.py` & `you-get-0.4.995/src/you_get/extractors/youtube.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/vine.py` & `you-get-0.4.995/src/you_get/extractors/vine.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/zhanqi.py` & `you-get-0.4.995/src/you_get/extractors/zhanqi.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/w56.py` & `you-get-0.4.995/src/you_get/extractors/w56.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/acfun.py` & `you-get-0.4.995/src/you_get/extractors/acfun.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/yinyuetai.py` & `you-get-0.4.995/src/you_get/extractors/yinyuetai.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/flickr.py` & `you-get-0.4.995/src/you_get/extractors/flickr.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/bokecc.py` & `you-get-0.4.995/src/you_get/extractors/bokecc.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_blip.py` & `you-get-0.4.995/src/you_get/extractors/_blip.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/tumblr.py` & `you-get-0.4.995/src/you_get/extractors/tumblr.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/baomihua.py` & `you-get-0.4.995/src/you_get/extractors/baomihua.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/veoh.py` & `you-get-0.4.995/src/you_get/extractors/veoh.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/iqilu.py` & `you-get-0.4.995/src/you_get/extractors/iqilu.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/quanmin.py` & `you-get-0.4.995/src/you_get/extractors/quanmin.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/qie.py` & `you-get-0.4.995/src/you_get/extractors/qie.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/coub.py` & `you-get-0.4.995/src/you_get/extractors/coub.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/xiami.py` & `you-get-0.4.995/src/you_get/extractors/xiami.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/cntv.py` & `you-get-0.4.995/src/you_get/extractors/cntv.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/freesound.py` & `you-get-0.4.995/src/you_get/extractors/freesound.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/wanmen.py` & `you-get-0.4.995/src/you_get/extractors/wanmen.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_qianmo.py` & `you-get-0.4.995/src/you_get/extractors/_qianmo.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/miomio.py` & `you-get-0.4.995/src/you_get/extractors/miomio.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/embed.py` & `you-get-0.4.995/src/you_get/extractors/embed.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/funshion.py` & `you-get-0.4.995/src/you_get/extractors/funshion.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_catfun.py` & `you-get-0.4.995/src/you_get/extractors/_catfun.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/le.py` & `you-get-0.4.995/src/you_get/extractors/le.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/pptv.py` & `you-get-0.4.995/src/you_get/extractors/pptv.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/sina.py` & `you-get-0.4.995/src/you_get/extractors/sina.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_dongting.py` & `you-get-0.4.995/src/you_get/extractors/_dongting.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/soundcloud.py` & `you-get-0.4.995/src/you_get/extractors/soundcloud.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/panda.py` & `you-get-0.4.995/src/you_get/extractors/panda.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/baidu.py` & `you-get-0.4.995/src/you_get/extractors/baidu.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/_vid48.py` & `you-get-0.4.995/src/you_get/extractors/_vid48.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/iwara.py` & `you-get-0.4.995/src/you_get/extractors/iwara.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/musicplayon.py` & `you-get-0.4.995/src/you_get/extractors/musicplayon.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/tudou.py` & `you-get-0.4.995/src/you_get/extractors/tudou.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/toutiao.py` & `you-get-0.4.995/src/you_get/extractors/toutiao.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/infoq.py` & `you-get-0.4.995/src/you_get/extractors/infoq.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/naver.py` & `you-get-0.4.995/src/you_get/extractors/naver.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/pixnet.py` & `you-get-0.4.995/src/you_get/extractors/pixnet.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/heavymusic.py` & `you-get-0.4.995/src/you_get/extractors/heavymusic.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/nicovideo.py` & `you-get-0.4.995/src/you_get/extractors/nicovideo.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/douban.py` & `you-get-0.4.995/src/you_get/extractors/douban.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/interest.py` & `you-get-0.4.995/src/you_get/extractors/interest.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/ehow.py` & `you-get-0.4.995/src/you_get/extractors/ehow.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/mixcloud.py` & `you-get-0.4.995/src/you_get/extractors/mixcloud.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/joy.py` & `you-get-0.4.995/src/you_get/extractors/joy.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/fantasy.py` & `you-get-0.4.995/src/you_get/extractors/fantasy.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/ku6.py` & `you-get-0.4.995/src/you_get/extractors/ku6.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/fc2video.py` & `you-get-0.4.995/src/you_get/extractors/fc2video.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/vk.py` & `you-get-0.4.995/src/you_get/extractors/vk.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/pinterest.py` & `you-get-0.4.995/src/you_get/extractors/pinterest.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/extractors/youku.py` & `you-get-0.4.995/src/you_get/extractors/youku.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.video_list = None
         self.video_next = None
         self.password = None
         self.api_data = None
         self.api_error_code = None
         self.api_error_msg = None
 
-        self.ccode = '0501'
+        self.ccode = '0507'
         self.utid = None
 
     def youku_ups(self):
         url = 'https://ups.youku.com/ups/get.json?vid={}&ccode={}'.format(self.vid, self.ccode)
         url += '&client_ip=192.168.1.1'
         url += '&utid=' + self.utid
         url += '&client_ts=' + str(int(time.time()))
```

### Comparing `you-get-0.4.990/src/you_get/util/strings.py` & `you-get-0.4.995/src/you_get/util/strings.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/util/log.py` & `you-get-0.4.995/src/you_get/util/log.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/util/fs.py` & `you-get-0.4.995/src/you_get/util/fs.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get/util/git.py` & `you-get-0.4.995/src/you_get/util/git.py`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get.egg-info/SOURCES.txt` & `you-get-0.4.995/src/you_get.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/src/you_get.egg-info/PKG-INFO` & `you-get-0.4.995/src/you_get.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: you-get
-Version: 0.4.990
+Version: 0.4.995
 Summary: Dumb downloader that scrapes the web
 Home-page: https://you-get.org/
 Author: Mort Yao
 Author-email: mort.yao@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: You-Get
```

### Comparing `you-get-0.4.990/LICENSE.txt` & `you-get-0.4.995/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/CHANGELOG.rst` & `you-get-0.4.995/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `you-get-0.4.990/PKG-INFO` & `you-get-0.4.995/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: you-get
-Version: 0.4.990
+Version: 0.4.995
 Summary: Dumb downloader that scrapes the web
 Home-page: https://you-get.org/
 Author: Mort Yao
 Author-email: mort.yao@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: You-Get
```

