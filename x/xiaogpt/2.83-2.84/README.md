# Comparing `tmp/xiaogpt-2.83.tar.gz` & `tmp/xiaogpt-2.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.83.tar", last modified: Mon May 20 10:52:11 2024, max compression
+gzip compressed data, was "xiaogpt-2.84.tar", last modified: Wed May 22 11:21:55 2024, max compression
```

## Comparing `xiaogpt-2.83.tar` & `xiaogpt-2.84.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1063 2024-05-20 10:52:02.458185 xiaogpt-2.83/LICENSE
--rw-r--r--   0        0        0    23909 2024-05-20 10:52:02.458185 xiaogpt-2.83/README.md
--rw-r--r--   0        0        0     3861 2024-05-20 10:52:11.946170 xiaogpt-2.83/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1160 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3660 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     2773 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/doubao_bot.py
--rw-r--r--   0        0        0     2516 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0      708 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/llama_bot.py
--rw-r--r--   0        0        0      822 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/moonshot_bot.py
--rw-r--r--   0        0        0     3657 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0      784 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/yi_bot.py
--rw-r--r--   0        0        0     5711 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/cli.py
--rw-r--r--   0        0        0     6734 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      145 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4665 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1095 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1058 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/tts/tetos.py
--rw-r--r--   0        0        0     2072 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/utils.py
--rw-r--r--   0        0        0    16525 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    29678 1970-01-01 00:00:00.000000 xiaogpt-2.83/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-22 11:21:51.764859 xiaogpt-2.84/LICENSE
+-rw-r--r--   0        0        0    24015 2024-05-22 11:21:51.764859 xiaogpt-2.84/README.md
+-rw-r--r--   0        0        0     3994 2024-05-22 11:21:55.396825 xiaogpt-2.84/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1160 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3660 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     2773 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/doubao_bot.py
+-rw-r--r--   0        0        0     2516 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0      708 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/llama_bot.py
+-rw-r--r--   0        0        0      822 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/moonshot_bot.py
+-rw-r--r--   0        0        0     3657 2024-05-22 11:21:51.764859 xiaogpt-2.84/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0      784 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/bot/yi_bot.py
+-rw-r--r--   0        0        0     5711 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6734 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4665 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1058 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2668 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/utils.py
+-rw-r--r--   0        0        0    16153 2024-05-22 11:21:51.768859 xiaogpt-2.84/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    29950 1970-01-01 00:00:00.000000 xiaogpt-2.84/PKG-INFO
```

### Comparing `xiaogpt-2.83/LICENSE` & `xiaogpt-2.84/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/README.md` & `xiaogpt-2.84/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -302,17 +302,18 @@
 
 ```shell
 docker run -v <your-config-dir>:/config -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> yihong0618/xiaogpt --config=/config/config.yaml
 ```
 
 注意端口必须映射为与容器内一致，XIAOGPT_HOSTNAME 需要设置为宿主机的 IP 地址，否则小爱无法正常播放语音。
 
-## 推荐的 fork
+## 推荐的类似项目
 
 - [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
+- [MiGPT](https://github.com/idootop/mi-gpt) -> Node.js 版，支持流式响应和长短期记忆
 
 ## 感谢
 
 - [xiaomi](https://www.mi.com/)
 - [PDM](https://pdm.fming.dev/latest/)
 - [Tetos](https://github.com/frostming/tetos) TTS 云服务支持
 - @[Yonsm](https://github.com/Yonsm) 的 [MiService](https://github.com/Yonsm/MiService)
```

### Comparing `xiaogpt-2.83/pyproject.toml` & `xiaogpt-2.84/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,18 @@
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
     "tetos>=0.2.1",
     "groq>=0.5.0",
     "pyyaml>=6.0.1",
     "langchain-community>=0.0.38",
+    "lingua-language-detector>=2.0.2; python_version < \"3.13\"",
 ]
 dynamic = []
-version = "2.83"
+version = "2.84"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
 
@@ -85,14 +86,15 @@
     "jsonpatch==1.33",
     "jsonpointer==2.4",
     "langchain==0.2.0",
     "langchain-community==0.2.0",
     "langchain-core==0.2.0",
     "langchain-text-splitters==0.2.0",
     "langsmith==0.1.45",
+    "lingua-language-detector==2.0.2 ; python_version < \"3.13\"",
     "markdown-it-py==3.0.0",
     "marshmallow==3.20.1",
     "mdurl==0.1.2",
     "miservice-fork==2.5.0",
     "multidict==6.0.5",
     "mutagen==1.47.0",
     "mypy-extensions==1.0.0",
```

### Comparing `xiaogpt-2.83/xiaogpt/bot/__init__.py` & `xiaogpt-2.84/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/base_bot.py` & `xiaogpt-2.84/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.84/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/doubao_bot.py` & `xiaogpt-2.84/xiaogpt/bot/doubao_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.84/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.84/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.84/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/llama_bot.py` & `xiaogpt-2.84/xiaogpt/bot/llama_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/moonshot_bot.py` & `xiaogpt-2.84/xiaogpt/bot/moonshot_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.84/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/bot/yi_bot.py` & `xiaogpt-2.84/xiaogpt/bot/yi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/cli.py` & `xiaogpt-2.84/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/config.py` & `xiaogpt-2.84/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.84/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/langchain/chain.py` & `xiaogpt-2.84/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.84/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.84/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/tts/base.py` & `xiaogpt-2.84/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/tts/mi.py` & `xiaogpt-2.84/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/tts/tetos.py` & `xiaogpt-2.84/xiaogpt/tts/tetos.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.83/xiaogpt/utils.py` & `xiaogpt-2.84/xiaogpt/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import os
 import re
 import socket
 from http.cookies import SimpleCookie
-from typing import AsyncIterator
+from typing import TYPE_CHECKING, AsyncIterator
 from urllib.parse import urlparse
 
 from requests.utils import cookiejar_from_dict
 
+if TYPE_CHECKING:
+    from lingua import LanguageDetector
+
 
 ### HELP FUNCTION ###
 def parse_cookie_string(cookie_string):
     cookie = SimpleCookie()
     cookie.load(cookie_string)
     cookies_dict = {k: m.value for k, m in cookie.items()}
     return cookiejar_from_dict(cookies_dict, cookiejar=None, overwrite=True)
@@ -65,7 +68,25 @@
 def get_hostname() -> str:
     if "XIAOGPT_HOSTNAME" in os.environ:
         return os.environ["XIAOGPT_HOSTNAME"]
 
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
         s.connect(("8.8.8.8", 80))
         return s.getsockname()[0]
+
+
+def _get_detector() -> LanguageDetector | None:
+    try:
+        from lingua import LanguageDetectorBuilder
+    except ImportError:
+        return None
+    return LanguageDetectorBuilder.from_all_spoken_languages().build()
+
+
+_detector = _get_detector()
+
+
+def detect_language(text: str) -> str:
+    if _detector is None:
+        return "zh"  # default to Chinese if langdetect module is not available
+    lang = _detector.detect_language_of(text)
+    return lang.iso_code_639_1.name.lower() if lang is not None else "zh"
```

### Comparing `xiaogpt-2.83/xiaogpt/xiaogpt.py` & `xiaogpt-2.84/xiaogpt/xiaogpt.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     COOKIE_TEMPLATE,
     LATEST_ASK_API,
     MI_ASK_SIMULATE_DATA,
     WAKEUP_KEYWORD,
     Config,
 )
 from xiaogpt.tts import TTS, MiTTS, TetosTTS
-from xiaogpt.utils import (
-    parse_cookie_string,
-)
+from xiaogpt.utils import detect_language, parse_cookie_string
 
 EOF = object()
 
 
 class MiGPT:
     def __init__(self, config: Config):
         self.config = config
@@ -386,19 +384,14 @@
 
             print("-" * 20)
             print("问题：" + query + "？")
             if not self.chatbot.has_history():
                 query = f"{query}，{self.config.prompt}"
             # some model can not detect the language code, so we need to add it
 
-            if self.config.tts != "mi":  # mi only say Chinese
-                query += (
-                    "，并用本段话的language code作为开头，用|分隔，如：en-US|你好……"
-                )
-
             if self.config.mute_xiaoai:
                 await self.stop_if_xiaoai_is_playing()
             else:
                 # waiting for xiaoai speaker done
                 await asyncio.sleep(8)
             await self.do_tts(f"正在问{self.chatbot.name}请耐心等待")
             try:
@@ -416,26 +409,19 @@
             else:
                 print("回答完毕")
             if self.in_conversation:
                 print(f"继续对话, 或用`{self.config.end_conversation}`结束对话")
                 await self.wakeup_xiaoai()
 
     async def speak(self, text_stream: AsyncIterator[str]) -> None:
-        text = await text_stream.__anext__()
-        # See if the first part contains language code(e.g. en-US|Hello world)
-        lang, _, first_chunk = text.rpartition("|")
-        if len(lang) > 7:
-            # It is not a legal language code, discard it
-            lang, first_chunk = "", text
-
-        lang = (
-            matches[0]
-            if (matches := re.findall(r"([a-z]{2}-[A-Z]{2})", lang))
-            else "zh-CN"
-        )
+        first_chunk = await text_stream.__anext__()
+        # Detect the language from the first chunk
+        # Add suffix '-' because tetos expects it to exist when selecting voices
+        # however, the nation code is never used.
+        lang = detect_language(first_chunk) + "-"
 
         async def gen():  # reconstruct the generator
             yield first_chunk
             async for text in text_stream:
                 yield text
 
         await self.tts.synthesize(lang, gen())
```

### Comparing `xiaogpt-2.83/PKG-INFO` & `xiaogpt-2.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.83
+Version: 2.84
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -21,14 +21,15 @@
 Requires-Dist: google-generativeai
 Requires-Dist: numexpr>=2.8.6
 Requires-Dist: dashscope>=1.10.0
 Requires-Dist: tetos>=0.2.1
 Requires-Dist: groq>=0.5.0
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: langchain-community>=0.0.38
+Requires-Dist: lingua-language-detector>=2.0.2; python_version < "3.13"
 Requires-Dist: aiohttp==3.9.5; extra == "locked"
 Requires-Dist: aiosignal==1.3.1; extra == "locked"
 Requires-Dist: annotated-types==0.6.0; extra == "locked"
 Requires-Dist: anyio==4.3.0; extra == "locked"
 Requires-Dist: async-timeout==4.0.3; python_version < "3.11" and extra == "locked"
 Requires-Dist: attrs==23.2.0; extra == "locked"
 Requires-Dist: azure-cognitiveservices-speech==1.37.0; extra == "locked"
@@ -67,14 +68,15 @@
 Requires-Dist: jsonpatch==1.33; extra == "locked"
 Requires-Dist: jsonpointer==2.4; extra == "locked"
 Requires-Dist: langchain==0.2.0; extra == "locked"
 Requires-Dist: langchain-community==0.2.0; extra == "locked"
 Requires-Dist: langchain-core==0.2.0; extra == "locked"
 Requires-Dist: langchain-text-splitters==0.2.0; extra == "locked"
 Requires-Dist: langsmith==0.1.45; extra == "locked"
+Requires-Dist: lingua-language-detector==2.0.2; python_version < "3.13" and extra == "locked"
 Requires-Dist: markdown-it-py==3.0.0; extra == "locked"
 Requires-Dist: marshmallow==3.20.1; extra == "locked"
 Requires-Dist: mdurl==0.1.2; extra == "locked"
 Requires-Dist: miservice-fork==2.5.0; extra == "locked"
 Requires-Dist: multidict==6.0.5; extra == "locked"
 Requires-Dist: mutagen==1.47.0; extra == "locked"
 Requires-Dist: mypy-extensions==1.0.0; extra == "locked"
@@ -416,17 +418,18 @@
 
 ```shell
 docker run -v <your-config-dir>:/config -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> yihong0618/xiaogpt --config=/config/config.yaml
 ```
 
 注意端口必须映射为与容器内一致，XIAOGPT_HOSTNAME 需要设置为宿主机的 IP 地址，否则小爱无法正常播放语音。
 
-## 推荐的 fork
+## 推荐的类似项目
 
 - [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
+- [MiGPT](https://github.com/idootop/mi-gpt) -> Node.js 版，支持流式响应和长短期记忆
 
 ## 感谢
 
 - [xiaomi](https://www.mi.com/)
 - [PDM](https://pdm.fming.dev/latest/)
 - [Tetos](https://github.com/frostming/tetos) TTS 云服务支持
 - @[Yonsm](https://github.com/Yonsm) 的 [MiService](https://github.com/Yonsm/MiService)
```

