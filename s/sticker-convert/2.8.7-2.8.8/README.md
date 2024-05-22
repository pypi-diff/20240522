# Comparing `tmp/sticker_convert-2.8.7.tar.gz` & `tmp/sticker_convert-2.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sticker_convert-2.8.7.tar", last modified: Sat Apr 20 06:55:05 2024, max compression
+gzip compressed data, was "sticker_convert-2.8.8.tar", last modified: Wed May 22 08:36:03 2024, max compression
```

## Comparing `sticker_convert-2.8.7.tar` & `sticker_convert-2.8.8.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    50061 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.748997 sticker_convert-2.8.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.752997 sticker_convert-2.8.7/src/sticker_convert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18621 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.752997 sticker_convert-2.8.7/src/sticker_convert/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3980 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_viber.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30707 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.752997 sticker_convert-2.8.7/src/sticker_convert/gui_components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/comp_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/config_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/control_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/cred_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/input_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/output_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/progress_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/right_clicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/gui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31964 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/advanced_compression_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/base_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/line_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.748997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
--rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.748997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.748997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
--rwxr-xr-x   0 runner    (1001) docker     (127)    25775 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7732 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/job_option.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/NotoColorEmoji.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/appicon.icns
--rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/appicon.ico
--rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/appicon.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12156 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/compression.json
--rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/emoji.json
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/help.json
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/input.json
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/output.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/uploaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/compress_wastickers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6396 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15695 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_telegram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/xcode_imessage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/utils/auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_kakao_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_line_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_signal_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/utils/files/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/cache_store.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/json_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/json_resources_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10100 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/metadata_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/run_bin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/sanitize_filename.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/utils/media/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/media/apple_png_normalize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/media/codec_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/media/decrypt_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/media/format_verify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      840 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/url_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/src/sticker_convert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50061 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    14721 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/tests/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.890105 sticker_convert-2.8.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    50061 2024-05-22 08:36:03.890105 sticker_convert-2.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:36:03.890105 sticker_convert-2.8.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.862105 sticker_convert-2.8.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.866105 sticker_convert-2.8.8/src/sticker_convert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18621 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.866105 sticker_convert-2.8.8/src/sticker_convert/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4041 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_viber.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30707 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.866105 sticker_convert-2.8.8/src/sticker_convert/gui_components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/comp_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/config_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/control_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/cred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/input_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/output_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/progress_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/right_clicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/gui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31964 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/advanced_compression_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/line_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.862105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
+-rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.862105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.862105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25775 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7732 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/job_option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/NotoColorEmoji.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/appicon.icns
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/appicon.ico
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/appicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12156 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/compression.json
+-rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/emoji.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/help.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/output.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/compress_wastickers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6396 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15695 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_telegram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/xcode_imessage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/utils/auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_kakao_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_line_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_signal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/utils/files/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/cache_store.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/json_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/json_resources_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10100 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/metadata_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/run_bin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/sanitize_filename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/utils/media/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/media/apple_png_normalize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/media/codec_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/media/decrypt_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/media/format_verify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      840 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/url_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50061 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14721 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/tests/test_export.py
```

### Comparing `sticker_convert-2.8.7/LICENSE` & `sticker_convert-2.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/PKG-INFO` & `sticker_convert-2.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.7
+Version: 2.8.8
 Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, Viber, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -365,27 +365,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiolimiter~=1.1.0
 Requires-Dist: anyio~=4.3.0
 Requires-Dist: apngasm_python~=1.2.3
 Requires-Dist: av~=12.0.0
 Requires-Dist: beautifulsoup4~=4.12.3
-Requires-Dist: rookiepy~=0.4.0
+Requires-Dist: rookiepy~=0.5.1
 Requires-Dist: imagequant~=1.1.1
 Requires-Dist: memory-tempfile~=2.2.3
 Requires-Dist: mergedeep~=1.3.4
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: Pillow~=10.3.0
 Requires-Dist: pyoxipng~=9.0.0
 Requires-Dist: python-telegram-bot~=21.1
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rlottie_python~=1.3.4
 Requires-Dist: signalstickers-client-fork-laggykiller~=3.3.0.post1
 Requires-Dist: sqlcipher3-wheels~=0.5.2.post1
-Requires-Dist: tqdm~=4.66.2
+Requires-Dist: tqdm~=4.66.4
 Requires-Dist: ttkbootstrap-fork-laggykiller~=1.5.1
 Requires-Dist: webp~=0.3.0
 
 # sticker-convert
 ![imgs/banner.png](imgs/banner.png)
 ![imgs/screenshot](imgs/screenshot.png)
```

### Comparing `sticker_convert-2.8.7/README.md` & `sticker_convert-2.8.8/README.md`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/pyproject.toml` & `sticker_convert-2.8.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/cli.py` & `sticker_convert-2.8.8/src/sticker_convert/cli.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/converter.py` & `sticker_convert-2.8.8/src/sticker_convert/converter.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/definitions.py` & `sticker_convert-2.8.8/src/sticker_convert/definitions.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_base.py` & `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
+from functools import partial
 from pathlib import Path
 from typing import Any, List, Optional, Tuple
 
 import anyio
 import requests
 
 from sticker_convert.job_option import CredOption
@@ -25,15 +26,17 @@
         self.opt_cred = opt_cred
         self.cb = cb
         self.cb_return = cb_return
 
     def download_multiple_files(
         self, targets: List[Tuple[str, Path]], retries: int = 3, **kwargs: Any
     ) -> None:
-        anyio.run(self.download_multiple_files_async, targets, retries, **kwargs)
+        anyio.run(
+            partial(self.download_multiple_files_async, targets, retries, **kwargs)
+        )
 
     async def download_multiple_files_async(
         self, targets: List[Tuple[str, Path]], retries: int = 3, **kwargs: Any
     ) -> None:
         # targets format: [(url1, dest2), (url2, dest2), ...]
         self.cb.put(
             ("bar", None, {"set_progress_mode": "determinate", "steps": len(targets)})
```

### Comparing `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_kakao.py` & `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_line.py` & `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_line.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_signal.py` & `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_signal.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_telegram.py` & `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_telegram.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_viber.py` & `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_viber.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui.py` & `sticker_convert-2.8.8/src/sticker_convert/gui.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/comp_frame.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/comp_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/config_frame.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/config_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/control_frame.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/control_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/cred_frame.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/cred_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/input_frame.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/input_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/output_frame.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/output_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/progress_frame.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/progress_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/right_clicker.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/right_clicker.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/gui_utils.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/gui_utils.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/advanced_compression_window.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/advanced_compression_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/base_window.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/base_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/line_get_auth_window.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/line_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/signal_get_auth_window.py` & `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/signal_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate` & `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/job.py` & `sticker_convert-2.8.8/src/sticker_convert/job.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/job_option.py` & `sticker_convert-2.8.8/src/sticker_convert/job_option.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/resources/NotoColorEmoji.ttf` & `sticker_convert-2.8.8/src/sticker_convert/resources/NotoColorEmoji.ttf`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/resources/appicon.icns` & `sticker_convert-2.8.8/src/sticker_convert/resources/appicon.icns`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/resources/appicon.ico` & `sticker_convert-2.8.8/src/sticker_convert/resources/appicon.ico`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/resources/appicon.png` & `sticker_convert-2.8.8/src/sticker_convert/resources/appicon.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/resources/compression.json` & `sticker_convert-2.8.8/src/sticker_convert/resources/compression.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/resources/emoji.json` & `sticker_convert-2.8.8/src/sticker_convert/resources/emoji.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/resources/help.json` & `sticker_convert-2.8.8/src/sticker_convert/resources/help.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/resources/input.json` & `sticker_convert-2.8.8/src/sticker_convert/resources/input.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/resources/output.json` & `sticker_convert-2.8.8/src/sticker_convert/resources/output.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/uploaders/compress_wastickers.py` & `sticker_convert-2.8.8/src/sticker_convert/uploaders/compress_wastickers.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_base.py` & `sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_base.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_signal.py` & `sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_signal.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_telegram.py` & `sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_telegram.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/uploaders/xcode_imessage.py` & `sticker_convert-2.8.8/src/sticker_convert/uploaders/xcode_imessage.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_kakao_auth.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_kakao_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_line_auth.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_line_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_signal_auth.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_signal_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/callback.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/callback.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/files/cache_store.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/files/cache_store.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/files/json_manager.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/files/json_manager.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/files/json_resources_loader.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/files/json_resources_loader.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/files/metadata_handler.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/files/metadata_handler.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/files/run_bin.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/files/run_bin.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/files/sanitize_filename.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/files/sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/media/apple_png_normalize.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/media/apple_png_normalize.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/media/codec_info.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/media/codec_info.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/media/decrypt_kakao.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/media/decrypt_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/media/format_verify.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/media/format_verify.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert/utils/url_detect.py` & `sticker_convert-2.8.8/src/sticker_convert/utils/url_detect.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/src/sticker_convert.egg-info/PKG-INFO` & `sticker_convert-2.8.8/src/sticker_convert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.7
+Version: 2.8.8
 Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, Viber, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -365,27 +365,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiolimiter~=1.1.0
 Requires-Dist: anyio~=4.3.0
 Requires-Dist: apngasm_python~=1.2.3
 Requires-Dist: av~=12.0.0
 Requires-Dist: beautifulsoup4~=4.12.3
-Requires-Dist: rookiepy~=0.4.0
+Requires-Dist: rookiepy~=0.5.1
 Requires-Dist: imagequant~=1.1.1
 Requires-Dist: memory-tempfile~=2.2.3
 Requires-Dist: mergedeep~=1.3.4
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: Pillow~=10.3.0
 Requires-Dist: pyoxipng~=9.0.0
 Requires-Dist: python-telegram-bot~=21.1
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rlottie_python~=1.3.4
 Requires-Dist: signalstickers-client-fork-laggykiller~=3.3.0.post1
 Requires-Dist: sqlcipher3-wheels~=0.5.2.post1
-Requires-Dist: tqdm~=4.66.2
+Requires-Dist: tqdm~=4.66.4
 Requires-Dist: ttkbootstrap-fork-laggykiller~=1.5.1
 Requires-Dist: webp~=0.3.0
 
 # sticker-convert
 ![imgs/banner.png](imgs/banner.png)
 ![imgs/screenshot](imgs/screenshot.png)
```

### Comparing `sticker_convert-2.8.7/src/sticker_convert.egg-info/SOURCES.txt` & `sticker_convert-2.8.8/src/sticker_convert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/tests/test_compression.py` & `sticker_convert-2.8.8/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/tests/test_download.py` & `sticker_convert-2.8.8/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.7/tests/test_export.py` & `sticker_convert-2.8.8/tests/test_export.py`

 * *Files identical despite different names*

