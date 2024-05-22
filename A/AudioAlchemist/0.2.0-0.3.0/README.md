# Comparing `tmp/audioalchemist-0.2.0.tar.gz` & `tmp/audioalchemist-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioalchemist-0.2.0.tar", last modified: Wed May 22 13:22:44 2024, max compression
+gzip compressed data, was "audioalchemist-0.3.0.tar", last modified: Wed May 22 13:54:07 2024, max compression
```

## Comparing `audioalchemist-0.2.0.tar` & `audioalchemist-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:22:44.675733 audioalchemist-0.2.0/
-drwxrwxrwx   0        0        0        0 2024-05-22 13:22:44.660079 audioalchemist-0.2.0/AudioAlchemist/
--rw-rw-rw-   0        0        0       43 2024-05-22 12:04:05.000000 audioalchemist-0.2.0/AudioAlchemist/__int__.py
--rw-rw-rw-   0        0        0     1337 2024-05-22 12:19:34.000000 audioalchemist-0.2.0/AudioAlchemist/audio_alchemist.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:22:44.671731 audioalchemist-0.2.0/AudioAlchemist.egg-info/
--rw-rw-rw-   0        0        0     2313 2024-05-22 13:22:44.000000 audioalchemist-0.2.0/AudioAlchemist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-22 13:22:44.000000 audioalchemist-0.2.0/AudioAlchemist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:22:44.000000 audioalchemist-0.2.0/AudioAlchemist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-22 13:22:44.000000 audioalchemist-0.2.0/AudioAlchemist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-22 13:22:44.000000 audioalchemist-0.2.0/AudioAlchemist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2313 2024-05-22 13:22:44.673729 audioalchemist-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 13:22:44.676730 audioalchemist-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1421 2024-05-22 13:21:26.000000 audioalchemist-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:54:07.045963 audioalchemist-0.3.0/
+drwxrwxrwx   0        0        0        0 2024-05-22 13:54:07.030199 audioalchemist-0.3.0/AudioAlchemist/
+-rw-rw-rw-   0        0        0       43 2024-05-22 12:04:05.000000 audioalchemist-0.3.0/AudioAlchemist/__int__.py
+-rw-rw-rw-   0        0        0     2607 2024-05-22 13:52:00.000000 audioalchemist-0.3.0/AudioAlchemist/audio_alchemist.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:54:07.045963 audioalchemist-0.3.0/AudioAlchemist.egg-info/
+-rw-rw-rw-   0        0        0     2308 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2308 2024-05-22 13:54:07.045963 audioalchemist-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 13:54:07.045963 audioalchemist-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2024-05-22 13:50:31.000000 audioalchemist-0.3.0/setup.py
```

### Comparing `audioalchemist-0.2.0/AudioAlchemist.egg-info/PKG-INFO` & `audioalchemist-0.3.0/AudioAlchemist.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAlchemist
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convert all files directly under the directory to any music file.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Kohki Suto
 Author-email: s2222019@stu.musashino-u.ac.jp
 Maintainer: Kohki Suto
 Maintainer-email: s2222019@stu.musashino-u.ac.jp
@@ -19,39 +19,39 @@
 
 ## リードミーファイル
 
 **# 音色変換**
 
 **## 概要**
 
-音色変換は、Pydub を利用した音声変換ツールです。WAV ファイルを MP3 ファイルなどの形式に変換することができます。
+音色変換は、Pydub を利用した音声変換ツールです。WAVやm4aを MP3 ファイルなどの形式に変換することができます。
 
 **## 機能**
 
-* WAV ファイルを MP3 ファイルなどの形式に変換する
+* WAVやm4aを MP3 ファイルなどの形式に変換する
 * 複数のファイルをまとめて変換する
 * 変換後のファイル名を連番で出力
 
 **## インストール**
 
 ```
-pip install AudioAlchemist
+pip3 install AudioAlchemist
 ```
 
-**## 使い方**
+**## 使い方 example**
 
 ```
 # フォルダパスを設定
-input_folder = 'C:/Users/data/melody/*.mp3'
+input_folder = 'C:/Users/data/melody/*.wav'
 output_folder = 'C:/Users/data/melody/'
-input_extension = "mp3"
-output_extension = "wav"
+input_extension = "wav"
+output_extension = "mp3"
 
 # 変換処理を実行
-AusioAlchemist(input_folder, output_folder, input_extension, output_extension)
+AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
 ```
 
 このコマンドは、`C:/Users/data/melody` フォルダ内のすべての WAV ファイルを MP3 ファイルに変換し、`C:/Users/data/melody` フォルダに出力します。
 
 **## 注意**
 
 * 変換するファイルが存在していることを確認してください。
@@ -64,8 +64,8 @@
 
 **## ライセンス**
 
 このプログラムは [MIT License](https://choosealicense.com/licenses/mit/) でライセンスされています。
 
 **## バージョン**
 
-0.1.0
+0.3.0
```

### Comparing `audioalchemist-0.2.0/PKG-INFO` & `audioalchemist-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAlchemist
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convert all files directly under the directory to any music file.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Kohki Suto
 Author-email: s2222019@stu.musashino-u.ac.jp
 Maintainer: Kohki Suto
 Maintainer-email: s2222019@stu.musashino-u.ac.jp
@@ -19,39 +19,39 @@
 
 ## リードミーファイル
 
 **# 音色変換**
 
 **## 概要**
 
-音色変換は、Pydub を利用した音声変換ツールです。WAV ファイルを MP3 ファイルなどの形式に変換することができます。
+音色変換は、Pydub を利用した音声変換ツールです。WAVやm4aを MP3 ファイルなどの形式に変換することができます。
 
 **## 機能**
 
-* WAV ファイルを MP3 ファイルなどの形式に変換する
+* WAVやm4aを MP3 ファイルなどの形式に変換する
 * 複数のファイルをまとめて変換する
 * 変換後のファイル名を連番で出力
 
 **## インストール**
 
 ```
-pip install AudioAlchemist
+pip3 install AudioAlchemist
 ```
 
-**## 使い方**
+**## 使い方 example**
 
 ```
 # フォルダパスを設定
-input_folder = 'C:/Users/data/melody/*.mp3'
+input_folder = 'C:/Users/data/melody/*.wav'
 output_folder = 'C:/Users/data/melody/'
-input_extension = "mp3"
-output_extension = "wav"
+input_extension = "wav"
+output_extension = "mp3"
 
 # 変換処理を実行
-AusioAlchemist(input_folder, output_folder, input_extension, output_extension)
+AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
 ```
 
 このコマンドは、`C:/Users/data/melody` フォルダ内のすべての WAV ファイルを MP3 ファイルに変換し、`C:/Users/data/melody` フォルダに出力します。
 
 **## 注意**
 
 * 変換するファイルが存在していることを確認してください。
@@ -64,8 +64,8 @@
 
 **## ライセンス**
 
 このプログラムは [MIT License](https://choosealicense.com/licenses/mit/) でライセンスされています。
 
 **## バージョン**
 
-0.1.0
+0.3.0
```

### Comparing `audioalchemist-0.2.0/setup.py` & `audioalchemist-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = 'Convert all files directly under the directory to any music file.'
 NAME = 'AudioAlchemist'
 AUTHOR = 'Kohki Suto'
 AUTHOR_EMAIL = 's2222019@stu.musashino-u.ac.jp'
 URL = 'https://github.com/Ryomo0797/AudioAlchemist.git'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.2.0'
+VERSION = '0.3.0'
 PYTHON_REQUIRES = '>=3.6'
 INSTALL_REQUIRES = [
     "pandas>=2.2.2",
     "pydub>=0.25.1",
     "ffmpeg>=1.4"
     #ffmpeg-python==0.2.0
 ]
```

