# Comparing `tmp/efaqa_corpus_zh-1.1.tar.gz` & `tmp/efaqa_corpus_zh-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\efaqa_corpus_zh-1.1.tar", last modified: Wed Nov 15 01:40:59 2023, max compression
+gzip compressed data, was "efaqa_corpus_zh-1.2.tar", last modified: Wed May 22 11:29:03 2024, max compression
```

## Comparing `efaqa_corpus_zh-1.1.tar` & `efaqa_corpus_zh-1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/
--rw-rw-rw-   0        0        0     1990 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/PKG-INFO
--rw-rw-rw-   0        0        0    19794 2023-10-28 00:10:09.000000 efaqa_corpus_zh-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh/
--rw-rw-rw-   0        0        0     3367 2023-11-15 01:40:42.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh/data/
--rw-rw-rw-   0        0        0       13 2023-10-27 09:14:20.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh.egg-info/
--rw-rw-rw-   0        0        0     1990 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/efaqa_corpus_zh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-15 01:40:59.000000 efaqa_corpus_zh-1.1/setup.cfg
--rw-rw-rw-   0        0        0     2162 2023-11-15 01:40:36.000000 efaqa_corpus_zh-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:29:03.841176 efaqa_corpus_zh-1.2/
+-rw-rw-rw-   0        0        0      634 2023-10-27 22:24:17.000000 efaqa_corpus_zh-1.2/LICENSE
+-rw-rw-rw-   0        0        0     1805 2024-05-22 11:29:03.840176 efaqa_corpus_zh-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    20494 2024-01-13 04:11:29.000000 efaqa_corpus_zh-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 11:29:03.837177 efaqa_corpus_zh-1.2/efaqa_corpus_zh/
+-rw-rw-rw-   0        0        0     3491 2024-04-29 04:03:33.000000 efaqa_corpus_zh-1.2/efaqa_corpus_zh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:29:03.840176 efaqa_corpus_zh-1.2/efaqa_corpus_zh/data/
+-rw-rw-rw-   0        0        0       13 2023-10-27 09:14:20.000000 efaqa_corpus_zh-1.2/efaqa_corpus_zh/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:29:03.839176 efaqa_corpus_zh-1.2/efaqa_corpus_zh.egg-info/
+-rw-rw-rw-   0        0        0     1805 2024-05-22 11:29:03.000000 efaqa_corpus_zh-1.2/efaqa_corpus_zh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-22 11:29:03.000000 efaqa_corpus_zh-1.2/efaqa_corpus_zh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:29:03.000000 efaqa_corpus_zh-1.2/efaqa_corpus_zh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-22 11:29:03.000000 efaqa_corpus_zh-1.2/efaqa_corpus_zh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-22 11:29:03.000000 efaqa_corpus_zh-1.2/efaqa_corpus_zh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:29:03.841176 efaqa_corpus_zh-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2162 2024-05-22 11:28:40.000000 efaqa_corpus_zh-1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `efaqa_corpus_zh-1.1/README.md` & `efaqa_corpus_zh-1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 <div align=right>
 
 [首页](https://github.com/chatopera/efaqa-corpus-zh)　|　[媒体报道](https://mp.weixin.qq.com/s/AyfWPBRQszKLCvT-YEFxMw)　|　[未来之路](https://zhuanlan.zhihu.com/p/128632328)
 
 </div>
 
+# 心理咨询相关语料库
+
+| 语料库 | 地址 | 描述 |
+| --- | --- | --- |
+| 心理咨询问答语料库（Emotional First Aid Dataset） | [GitHub](https://github.com/chatopera/efaqa-corpus-zh), [Gitee](https://gitee.com/chatopera/efaqa-corpus-zh) | 人工标注的多轮对话 |
+| 心理咨询问答原始语料库（Emotional First Aid Raw Dataset） | [GitHub](https://github.com/chatopera/efaqa-corpus-raw), [Gitee](https://gitee.com/chatopera/efaqa-corpus-raw) | 爬取后未标注的原始语料 |
+
 # Emotional First Aid Dataset
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/efaqa-corpus-zh.svg)](https://pypi.python.org/pypi/efaqa-corpus-zh/) [![PyPI download month](https://img.shields.io/pypi/dm/efaqa-corpus-zh.svg)](https://pypi.python.org/pypi/efaqa-corpus-zh/) [![PyPI version shields.io](https://img.shields.io/pypi/v/efaqa-corpus-zh.svg)](https://pypi.python.org/pypi/efaqa-corpus-zh/)  [![License](https://cdndownload2.chatopera.com/cskefu/licenses/chunsong1.0.svg)](https://www.cskefu.com/licenses/v1.html "开源许可协议")
 
 心理咨询问答语料库，仅限研究用途。
 
 心理咨询问答语料库（以下也称为“**数据集**”，“**语料库**”）是为应用人工智能技术于心理咨询领域制作的语料。据我们所知，这是心理咨询领域首个开放的 QA 语料库，包括 20,000 条心理咨询数据，也是**迄今公开的最大的中文心理咨询对话语料**(发稿日期 2022-04-07)。数据集内容丰富，不但具备多轮对话内容，也有分类等信息，制作过程耗费大量时间和精力，比如标注过程是面向多轮对话，平均每条标记耗时超过 1 分钟。
@@ -31,30 +38,39 @@
 pip install -U efaqa-corpus-zh     # 安装脚本包
 python -c "import efaqa_corpus_zh" # 下载语料文件
 ```
 
 * Windows
 
 ```
+# Set ENV
+## 1/2 Command Prompt
 set EFAQA_DL_LICENSE=YOUR_LICENSE
+## 2/2 PowerShell
+$env:EFAQA_DL_LICENSE='YOUR_LICENSE'
+
+# Download
 pip install -U efaqa-corpus-zh     # 安装脚本包
 python -c "import efaqa_corpus_zh" # 下载语料文件
 ```
 
 `YOUR_LICENSE` 为从[证书商店](https://store.chatopera.com/product/efaqa001)购买的证书的【证书标识】。
 
 ![](https://cdndownload2.chatopera.com/store/imgs/efaqa001_ordering_image.jpg)
 
 假设证书标识为*FOOBAR*，那么，设置如下：
 
 ```
 # Linux / macOS
 export EFAQA_DL_LICENSE=FOOBAR
 # Windows
+## 1/2 Command Prompt
 set EFAQA_DL_LICENSE=FOOBAR
+## 2/2 PowerShell
+$env:EFAQA_DL_LICENSE='FOOBAR'
 ```
 
 ### 演示代码
 
 ```
 import efaqa_corpus_zh
 records = list(efaqa_corpus_zh.load())
```

#### html2text {}

```diff
@@ -1,11 +1,18 @@
     [é¦é¡µ](https://github.com/chatopera/efaqa-corpus-zh)ã|ã[åªä½æ¥é]
 (https://mp.weixin.qq.com/s/AyfWPBRQszKLCvT-YEFxMw)ã|ã[æªæ¥ä¹è·¯](https:
                                               //zhuanlan.zhihu.com/p/128632328)
-# Emotional First Aid Dataset [![PyPI pyversions](https://img.shields.io/pypi/
+# å¿çå¨è¯¢ç¸å³è¯­æåº | è¯­æåº | å°å | æè¿° | | --- | --- | --
+- | | å¿çå¨è¯¢é®ç­è¯­æåºï¼Emotional First Aid Datasetï¼ | [GitHub]
+(https://github.com/chatopera/efaqa-corpus-zh), [Gitee](https://gitee.com/
+chatopera/efaqa-corpus-zh) | äººå·¥æ æ³¨çå¤è½®å¯¹è¯ | |
+å¿çå¨è¯¢é®ç­åå§è¯­æåºï¼Emotional First Aid Raw Datasetï¼ |
+[GitHub](https://github.com/chatopera/efaqa-corpus-raw), [Gitee](https://
+gitee.com/chatopera/efaqa-corpus-raw) | ç¬ååæªæ æ³¨çåå§è¯­æ | #
+Emotional First Aid Dataset [![PyPI pyversions](https://img.shields.io/pypi/
 pyversions/efaqa-corpus-zh.svg)](https://pypi.python.org/pypi/efaqa-corpus-zh/
 ) [![PyPI download month](https://img.shields.io/pypi/dm/efaqa-corpus-zh.svg)]
 (https://pypi.python.org/pypi/efaqa-corpus-zh/) [![PyPI version shields.io]
 (https://img.shields.io/pypi/v/efaqa-corpus-zh.svg)](https://pypi.python.org/
 pypi/efaqa-corpus-zh/) [![License](https://cdndownload2.chatopera.com/cskefu/
 licenses/chunsong1.0.svg)](https://www.cskefu.com/licenses/v1.html
 "å¼æºè®¸å¯åè®®") å¿çå¨è¯¢é®ç­è¯­æåºï¼ä»éç ç©¶ç¨éã
@@ -17,27 +24,30 @@
 1 åéã
 å¿çå¨è¯¢é®ç­è¯­æåºçæºä»£ç æ¯åºäºå¼æºè®¸å¯è¯ååï¼ä½æ¯å®è£ä½¿ç¨è¿ç¨ä¸­ï¼ä¸è½½çè¯­ææä»¶ï¼éè¦ä»
 [è¯ä¹¦ååº](https://store.chatopera.com/product/
 efaqa001)è´­ä¹°è¯ä¹¦ï¼æè½ä¸è½½åä½¿ç¨ï¼å·ä½ä½¿ç¨è¿ç¨æè¿°å¦ä¸ã
 ## å®è£ä½¿ç¨ ä¾èµï¼ * Python: 2.x, 3.x * Pip ###
 å®è£åä¸è½½è¯­ææä»¶ * Linux æ macOS ``` export
 EFAQA_DL_LICENSE=YOUR_LICENSE pip install -U efaqa-corpus-zh # å®è£èæ¬å
-python -c "import efaqa_corpus_zh" # ä¸è½½è¯­ææä»¶ ``` * Windows ``` set
-EFAQA_DL_LICENSE=YOUR_LICENSE pip install -U efaqa-corpus-zh # å®è£èæ¬å
-python -c "import efaqa_corpus_zh" # ä¸è½½è¯­ææä»¶ ``` `YOUR_LICENSE`
-ä¸ºä»[è¯ä¹¦ååº](https://store.chatopera.com/product/
+python -c "import efaqa_corpus_zh" # ä¸è½½è¯­ææä»¶ ``` * Windows ``` # Set
+ENV ## 1/2 Command Prompt set EFAQA_DL_LICENSE=YOUR_LICENSE ## 2/2 PowerShell
+$env:EFAQA_DL_LICENSE='YOUR_LICENSE' # Download pip install -U efaqa-corpus-zh
+# å®è£èæ¬å python -c "import efaqa_corpus_zh" # ä¸è½½è¯­ææä»¶ ```
+`YOUR_LICENSE` ä¸ºä»[è¯ä¹¦ååº](https://store.chatopera.com/product/
 efaqa001)è´­ä¹°çè¯ä¹¦çãè¯ä¹¦æ è¯ãã ![](https://
 cdndownload2.chatopera.com/store/imgs/efaqa001_ordering_image.jpg)
 åè®¾è¯ä¹¦æ è¯ä¸º*FOOBAR*ï¼é£ä¹ï¼è®¾ç½®å¦ä¸ï¼ ``` # Linux / macOS
-export EFAQA_DL_LICENSE=FOOBAR # Windows set EFAQA_DL_LICENSE=FOOBAR ``` ###
-æ¼ç¤ºä»£ç  ``` import efaqa_corpus_zh records = list(efaqa_corpus_zh.load())
-print("size: %s" % len(records)) print(records[0]["title"]) ``` åæ¬¡æ§è¡
-`load` æ¥å£ï¼ä¼ä¸è½½æ°æ®ï¼ä¸è½½éåº¦åå³äºç½ç»è´¨éã ##
-æ°æ®æ ¼å¼ å è½½æ°æ® `records = list(efaqa_corpus_zh.load())`
-ä¸­ï¼æ¯ä¸æ¡ `records` æ°æ®é½éµå¾ªå¦ä¸æ ¼å¼ï¼
+export EFAQA_DL_LICENSE=FOOBAR # Windows ## 1/2 Command Prompt set
+EFAQA_DL_LICENSE=FOOBAR ## 2/2 PowerShell $env:EFAQA_DL_LICENSE='FOOBAR' ```
+### æ¼ç¤ºä»£ç  ``` import efaqa_corpus_zh records = list(efaqa_corpus_zh.load
+()) print("size: %s" % len(records)) print(records[0]["title"]) ```
+åæ¬¡æ§è¡ `load`
+æ¥å£ï¼ä¼ä¸è½½æ°æ®ï¼ä¸è½½éåº¦åå³äºç½ç»è´¨éã ## æ°æ®æ ¼å¼
+å è½½æ°æ® `records = list(efaqa_corpus_zh.load())` ä¸­ï¼æ¯ä¸æ¡ `records`
+æ°æ®é½éµå¾ªå¦ä¸æ ¼å¼ï¼
 ?å?­??æ?®?µ      ?è?¯?´?æ??                        ?ç?±?»?å??
 md5         å¯ä¸æ è¯                  string
 title       æ é¢                        string
 description æè¿°                        string
 owner       å¨è¯¢èï¼è±æåï¼      string
 label       è¯é¢æ ç­¾                  Object
             s3     ç¦æ¼ç±»å           string
```

### Comparing `efaqa_corpus_zh-1.1/efaqa_corpus_zh/__init__.py` & `efaqa_corpus_zh-1.2/efaqa_corpus_zh/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 print("\n Project Sponsored by Chatopera")
 print("\n  deliver your chatbots with Chatopera Cloud Services --> https://bot.chatopera.com\n")
 
 
 print("\n Module file path: %s" % __file__)
 print("\n ************ NOTICE ************")
 print("  Require license to download model package, purchase from https://store.chatopera.com/product/efaqa001")
+print("  Need a larger psychological corpus? 44,000,000+ tokens, check out https://github.com/chatopera/efaqa-corpus-raw")
 print(" ********************************\n")
 
 try:
     from smart_open import smart_open
 except ImportError:
     print(
         "smart_open library not found; falling back to local-filesystem-only")
```

### Comparing `efaqa_corpus_zh-1.1/setup.py` & `efaqa_corpus_zh-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 欢迎任何进一步增加此数据集的想法。
 
 阅读 `详细文档 <https://github.com/chatopera/efaqa-corpus-zh>`__
 
 """
 
 setup(name='efaqa_corpus_zh',
-      version='1.1',
+      version='1.2',
       description='Emotional First Aid Dataset, 心理咨询问答语料库',
       long_description=LONGDOC,
       author='Hai Liang Wang',
       author_email='hain@chatopera.com',
       url='https://github.com/chatopera/efaqa-corpus-zh',
       license="Chunsong Public License, version 1.0",
       classifiers=[
```

