# Comparing `tmp/YouTube-Driver-1.0.7.tar.gz` & `tmp/youtube_driver-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YouTube-Driver-1.0.7.tar", last modified: Sat May 14 01:00:09 2022, max compression
+gzip compressed data, was "youtube_driver-1.0.8.tar", last modified: Wed May 22 01:51:45 2024, max compression
```

## Comparing `YouTube-Driver-1.0.7.tar` & `youtube_driver-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 mharoon   (1000) mharoon   (1000)        0 2022-05-14 01:00:09.698163 YouTube-Driver-1.0.7/
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)     1072 2022-05-11 04:46:15.000000 YouTube-Driver-1.0.7/LICENSE
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)     1499 2022-05-14 01:00:09.698163 YouTube-Driver-1.0.7/PKG-INFO
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)     1073 2022-05-11 04:57:41.000000 YouTube-Driver-1.0.7/README.md
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)       79 2022-05-14 01:00:09.698163 YouTube-Driver-1.0.7/setup.cfg
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)      723 2022-05-14 00:58:43.000000 YouTube-Driver-1.0.7/setup.py
-drwxrwxr-x   0 mharoon   (1000) mharoon   (1000)        0 2022-05-14 01:00:09.698163 YouTube-Driver-1.0.7/src/
-drwxrwxr-x   0 mharoon   (1000) mharoon   (1000)        0 2022-05-14 01:00:09.698163 YouTube-Driver-1.0.7/src/YouTube_Driver.egg-info/
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)     1499 2022-05-14 01:00:09.000000 YouTube-Driver-1.0.7/src/YouTube_Driver.egg-info/PKG-INFO
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)      343 2022-05-14 01:00:09.000000 YouTube-Driver-1.0.7/src/YouTube_Driver.egg-info/SOURCES.txt
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)        1 2022-05-14 01:00:09.000000 YouTube-Driver-1.0.7/src/YouTube_Driver.egg-info/dependency_links.txt
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)       26 2022-05-14 01:00:09.000000 YouTube-Driver-1.0.7/src/YouTube_Driver.egg-info/requires.txt
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)        9 2022-05-14 01:00:09.000000 YouTube-Driver-1.0.7/src/YouTube_Driver.egg-info/top_level.txt
-drwxrwxr-x   0 mharoon   (1000) mharoon   (1000)        0 2022-05-14 01:00:09.698163 YouTube-Driver-1.0.7/src/ytdriver/
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)    10120 2022-05-11 04:47:26.000000 YouTube-Driver-1.0.7/src/ytdriver/YTDriver.py
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)      127 2022-05-11 04:54:02.000000 YouTube-Driver-1.0.7/src/ytdriver/__init__.py
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)      581 2022-05-11 04:46:15.000000 YouTube-Driver-1.0.7/src/ytdriver/example.py
--rw-rw-r--   0 mharoon   (1000) mharoon   (1000)      963 2022-05-14 00:58:22.000000 YouTube-Driver-1.0.7/src/ytdriver/helpers.py
+drwxr-xr-x   0 mharoon    (501) staff       (20)        0 2024-05-22 01:51:45.692739 youtube_driver-1.0.8/
+-rw-r--r--   0 mharoon    (501) staff       (20)     1072 2024-05-22 00:25:51.000000 youtube_driver-1.0.8/LICENSE
+-rw-r--r--   0 mharoon    (501) staff       (20)     1557 2024-05-22 01:51:45.692657 youtube_driver-1.0.8/PKG-INFO
+-rw-r--r--   0 mharoon    (501) staff       (20)     1073 2024-05-22 00:25:51.000000 youtube_driver-1.0.8/README.md
+-rw-r--r--   0 mharoon    (501) staff       (20)       79 2024-05-22 01:51:45.692942 youtube_driver-1.0.8/setup.cfg
+-rw-r--r--   0 mharoon    (501) staff       (20)      741 2024-05-22 01:48:16.000000 youtube_driver-1.0.8/setup.py
+drwxr-xr-x   0 mharoon    (501) staff       (20)        0 2024-05-22 01:51:45.690533 youtube_driver-1.0.8/src/
+drwxr-xr-x   0 mharoon    (501) staff       (20)        0 2024-05-22 01:51:45.692450 youtube_driver-1.0.8/src/YouTube_Driver.egg-info/
+-rw-r--r--   0 mharoon    (501) staff       (20)     1557 2024-05-22 01:51:45.000000 youtube_driver-1.0.8/src/YouTube_Driver.egg-info/PKG-INFO
+-rw-r--r--   0 mharoon    (501) staff       (20)      362 2024-05-22 01:51:45.000000 youtube_driver-1.0.8/src/YouTube_Driver.egg-info/SOURCES.txt
+-rw-r--r--   0 mharoon    (501) staff       (20)        1 2024-05-22 01:51:45.000000 youtube_driver-1.0.8/src/YouTube_Driver.egg-info/dependency_links.txt
+-rw-r--r--   0 mharoon    (501) staff       (20)       33 2024-05-22 01:51:45.000000 youtube_driver-1.0.8/src/YouTube_Driver.egg-info/requires.txt
+-rw-r--r--   0 mharoon    (501) staff       (20)        9 2024-05-22 01:51:45.000000 youtube_driver-1.0.8/src/YouTube_Driver.egg-info/top_level.txt
+drwxr-xr-x   0 mharoon    (501) staff       (20)        0 2024-05-22 01:51:45.692266 youtube_driver-1.0.8/src/ytdriver/
+-rw-r--r--   0 mharoon    (501) staff       (20)     2200 2024-05-22 01:45:48.000000 youtube_driver-1.0.8/src/ytdriver/Video.py
+-rw-r--r--   0 mharoon    (501) staff       (20)    10364 2024-05-22 01:38:33.000000 youtube_driver-1.0.8/src/ytdriver/YTDriver.py
+-rw-r--r--   0 mharoon    (501) staff       (20)      125 2024-05-22 01:37:27.000000 youtube_driver-1.0.8/src/ytdriver/__init__.py
+-rw-r--r--   0 mharoon    (501) staff       (20)      705 2024-05-22 01:47:41.000000 youtube_driver-1.0.8/src/ytdriver/example.py
+-rw-r--r--   0 mharoon    (501) staff       (20)      256 2024-05-22 01:37:14.000000 youtube_driver-1.0.8/src/ytdriver/util.py
```

### Comparing `YouTube-Driver-1.0.7/LICENSE` & `youtube_driver-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `YouTube-Driver-1.0.7/PKG-INFO` & `youtube_driver-1.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: YouTube-Driver
-Version: 1.0.7
+Version: 1.0.8
 Summary: Programmatically interact with YouTube's interface.
 Home-page: https://github.com/ucdavis-noyce/YouTube-Driver
 Download-URL: https://github.com/ucdavis-noyce/YouTube-Driver/archive/refs/tags/v1.0.7.tar.gz
 Author: Muhammad Haroon
 Author-email: mharoon@ucdavis.edu
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: selenium
+Requires-Dist: pyvirtualdisplay
+Requires-Dist: yt-dlp
 
 # YouTube-Driver
 This package provides a high-level abstraction over selenium to allow programmatic interaction with YouTube's interface.
 
 ## Installation
 1. Install the package using `pip install --upgrade YouTube-Driver`.
 2. Download [youtube-dl](https://youtube-dl.org/) to a location in your PATH.
@@ -25,9 +27,7 @@
 - See [`example.py`](https://github.com/ucdavis-noyce/YouTube-Driver/blob/main/src/ytdriver/example.py) for a quick overview on how to use the package.
 - Read the [documentation](https://ucdavis-noyce.github.io/YouTube-Driver/ytdriver).
 
 ## Acknowledgements
 This tool was developed as part of an effort by researchers at UC Davis to audit the recommendations on YouTube. Read more about it [here](https://youtubeaudit.com).
 
 The primary maintainer is [Muhammad Haroon](https://github.com/haroon96).
-
-
```

### Comparing `YouTube-Driver-1.0.7/README.md` & `youtube_driver-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `YouTube-Driver-1.0.7/setup.py` & `youtube_driver-1.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="YouTube-Driver",
-    version="1.0.7",
+    version="1.0.8",
     packages=["ytdriver"],
     license="MIT",
     author="Muhammad Haroon",
     author_email="mharoon@ucdavis.edu",
     url="https://github.com/ucdavis-noyce/YouTube-Driver",
     download_url="https://github.com/ucdavis-noyce/YouTube-Driver/archive/refs/tags/v1.0.7.tar.gz",
     description="Programmatically interact with YouTube's interface.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     package_dir={"": "src"},
     install_requires=[
         'selenium',
-        'pyvirtualdisplay'
+        'pyvirtualdisplay',
+        'yt-dlp'
     ]
 )
```

### Comparing `YouTube-Driver-1.0.7/src/YouTube_Driver.egg-info/PKG-INFO` & `youtube_driver-1.0.8/src/YouTube_Driver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: YouTube-Driver
-Version: 1.0.7
+Version: 1.0.8
 Summary: Programmatically interact with YouTube's interface.
 Home-page: https://github.com/ucdavis-noyce/YouTube-Driver
 Download-URL: https://github.com/ucdavis-noyce/YouTube-Driver/archive/refs/tags/v1.0.7.tar.gz
 Author: Muhammad Haroon
 Author-email: mharoon@ucdavis.edu
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: selenium
+Requires-Dist: pyvirtualdisplay
+Requires-Dist: yt-dlp
 
 # YouTube-Driver
 This package provides a high-level abstraction over selenium to allow programmatic interaction with YouTube's interface.
 
 ## Installation
 1. Install the package using `pip install --upgrade YouTube-Driver`.
 2. Download [youtube-dl](https://youtube-dl.org/) to a location in your PATH.
@@ -25,9 +27,7 @@
 - See [`example.py`](https://github.com/ucdavis-noyce/YouTube-Driver/blob/main/src/ytdriver/example.py) for a quick overview on how to use the package.
 - Read the [documentation](https://ucdavis-noyce.github.io/YouTube-Driver/ytdriver).
 
 ## Acknowledgements
 This tool was developed as part of an effort by researchers at UC Davis to audit the recommendations on YouTube. Read more about it [here](https://youtubeaudit.com).
 
 The primary maintainer is [Muhammad Haroon](https://github.com/haroon96).
-
-
```

### Comparing `YouTube-Driver-1.0.7/src/ytdriver/YTDriver.py` & `youtube_driver-1.0.8/src/ytdriver/YTDriver.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 from selenium.webdriver.firefox.service import Service
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import WebDriverException
 from time import sleep
-from .helpers import Video, VideoUnavailableException, time2seconds
+from .Video import Video, VideoUnavailableException
+from .util import time2seconds
 from pyvirtualdisplay import Display
 import os
 
 class YTDriver:
 
+    AD_CLASSNAMES = [
+        'ytp-preview-ad',
+        'ytp-ad-preview-container'
+    ]
+
     def __init__(self, browser='chrome', profile_dir=None, use_virtual_display=False, headless=False, verbose=False):
         """
         Initializes the webdriver and virtual display
 
         ### Arguments:
         - `browser`: Specify `chrome` or `firefox` to launch the corresponding webdriver.
         - `profile_dir`: Specify a directory to save the browser profile so it can be loaded later. Set to `None` to not save the profile.
@@ -42,15 +48,15 @@
 
     def close(self):
         """
         Close the underlying webdriver.
         """
         self.driver.close()
 
-    def get_homepage(self, scroll_times=0):
+    def get_homepage_recommendations(self, scroll_times=0) -> list[Video]:
         """
         Collect videos from the YouTube homepage.
 
         ### Arguments:
         - `scroll_times`: Number of times to scroll the homepage.
 
         ### Returns:
@@ -83,15 +89,15 @@
             a = video.find_elements(By.TAG_NAME, 'a')[0]
             href = a.get_attribute('href')
             if href is not None and href.startswith('https://www.youtube.com/watch?'):
                 homepage.append(Video(a, href))
 
         return homepage
 
-    def get_recommendations(self, topn=5):
+    def get_upnext_recommendations(self, topn=5) -> list[Video]:
 
         """
         Collect up-next recommendations for the currently playing video.
 
         ### Arguments:
         - `topn`: Number of recommendations to return.
 
@@ -106,15 +112,15 @@
         elems = WebDriverWait(self.driver, 30).until(
             EC.presence_of_all_elements_located((By.TAG_NAME, 'ytd-compact-video-renderer'))
         )
 
         # recommended videos array
         return [Video(elem, elem.find_elements(By.TAG_NAME, 'a')[0].get_attribute('href')) for elem in elems[:topn]]
 
-    def search_videos(self, query, scroll_times=0):
+    def search_videos(self, query, scroll_times=0) -> list[Video]:
         """
         Search for videos.
 
         ### Arguments:
         - `query` (`str`): Search query.
 
         ### Returns:
@@ -218,29 +224,29 @@
 
     def __handle_ads(self):
         # handle multiple ads
         while True:
             sleep(1)
 
             # check if ad is being shown
-            preview = self.driver.find_elements(By.CLASS_NAME, 'ytp-ad-preview-container')
-            if len(preview) == 0:
+            xpath = '//div[%s]' % (' or '.join(["@class='%s'" % i for i in YTDriver.AD_CLASSNAMES]))
+            ad_elems = self.driver.find_elements(By.XPATH, xpath)
+            if len(ad_elems) == 0:
                 self.__log('Ad not detected')
                 # ad is not shown, return
                 return
 
             self.__log('Ad detected')
             
-            sleep(1)
-            preview = preview[0]
             # an ad is being shown
             # grab preview text to determine ad type
+            preview = ad_elems[0]
             text = preview.text.replace('\n', ' ')
             wait = 0
-            if 'after ad' in text:
+            if 'after ad' in text or 'plays soon' in text:
                 # unskippable ad, grab ad length
                 length = self.driver.find_elements(By.CLASS_NAME, 'ytp-ad-duration-remaining')[0].text
                 wait = time2seconds(length)
                 self.__log('Unskippable ad. Waiting %d seconds...' % wait)
             elif 'begin in' in text or 'end in' in text:
                 # short ad
                 wait = int(text.split()[-1])
@@ -250,15 +256,15 @@
                 wait = int(text)
                 self.__log('Skippable ad. Skipping after %d seconds...' % wait)
 
             # wait for ad to finish
             sleep(wait)
 
             # click skip button if available
-            skip = self.driver.find_elements(By.CLASS_NAME, 'ytp-ad-skip-button-container')
+            skip = self.driver.find_elements(By.CLASS_NAME, 'ytp-skip-ad-button')
             if len(skip) > 0:
                 skip[0].click()
 
     def __clear_prompts(self):
         try:
             sleep(1)
             self.driver.find_element(By.XPATH, '/html/body/ytd-app/ytd-popup-container/tp-yt-iron-dropdown/div/yt-tooltip-renderer/div[2]/div[1]/yt-button-renderer/a/tp-yt-paper-button/yt-formatted-string').click()
```

