# Comparing `tmp/insuranceqa_data-2.5.2.tar.gz` & `tmp/insuranceqa_data-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\insuranceqa_data-2.5.2.tar", last modified: Wed Nov 15 01:46:03 2023, max compression
+gzip compressed data, was "insuranceqa_data-2.5.3.tar", last modified: Wed May 22 11:21:49 2024, max compression
```

## Comparing `insuranceqa_data-2.5.2.tar` & `insuranceqa_data-2.5.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/
--rw-rw-rw-   0        0        0     3478 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     9338 2023-11-15 01:45:32.000000 insuranceqa_data-2.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/insuranceqa_data/
--rw-rw-rw-   0        0        0      636 2023-10-28 04:41:41.000000 insuranceqa_data-2.5.2/insuranceqa_data/LICENSE
--rw-rw-rw-   0        0        0     6961 2023-11-01 23:47:20.000000 insuranceqa_data-2.5.2/insuranceqa_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/insuranceqa_data.egg-info/
--rw-rw-rw-   0        0        0     3478 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/insuranceqa_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/insuranceqa_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/insuranceqa_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/insuranceqa_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/insuranceqa_data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-11-15 01:46:03.000000 insuranceqa_data-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0     3514 2023-11-15 01:44:38.000000 insuranceqa_data-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:21:49.505935 insuranceqa_data-2.5.3/
+-rw-rw-rw-   0        0        0      636 2023-10-28 03:58:42.000000 insuranceqa_data-2.5.3/LICENSE
+-rw-rw-rw-   0        0        0     3093 2024-05-22 11:21:49.506935 insuranceqa_data-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9338 2024-05-22 11:19:32.000000 insuranceqa_data-2.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 11:21:49.502941 insuranceqa_data-2.5.3/insuranceqa_data/
+-rw-rw-rw-   0        0        0      636 2023-10-28 04:41:41.000000 insuranceqa_data-2.5.3/insuranceqa_data/LICENSE
+-rw-rw-rw-   0        0        0     6957 2024-05-22 11:17:49.000000 insuranceqa_data-2.5.3/insuranceqa_data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:21:49.505935 insuranceqa_data-2.5.3/insuranceqa_data.egg-info/
+-rw-rw-rw-   0        0        0     3093 2024-05-22 11:21:49.000000 insuranceqa_data-2.5.3/insuranceqa_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-05-22 11:21:49.000000 insuranceqa_data-2.5.3/insuranceqa_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:21:49.000000 insuranceqa_data-2.5.3/insuranceqa_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-22 11:21:49.000000 insuranceqa_data-2.5.3/insuranceqa_data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 11:21:49.000000 insuranceqa_data-2.5.3/insuranceqa_data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-22 11:21:49.506935 insuranceqa_data-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     3514 2024-05-22 11:19:52.000000 insuranceqa_data-2.5.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `insuranceqa_data-2.5.2/PKG-INFO` & `insuranceqa_data-2.5.3/insuranceqa_data.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-Metadata-Version: 1.1
-Name: insuranceqa_data
-Version: 2.5.2
+Metadata-Version: 2.1
+Name: insuranceqa-data
+Version: 2.5.3
 Summary: Insuranceqa Corpus in Chinese for Machine Learning
 Home-page: https://github.com/chatopera/insuranceqa-corpus-zh
 Author: Hai Liang Wang
 Author-email: hailiang.hl.wang@gmail.com
 License: Chunsong Public License, version 1.0
-Description: 
-        insuranceqa-corpus-zh
-        =====================
-        
-        保险行业语料库
-        
-        Welcome
-        -------
-        
-        该语料库包含从网站\ `Insurance
-        Library <http://www.insurancelibrary.com/>`__ 收集的问题和答案。
-        
-        据我们所知，这是保险领域首个开放的QA语料库：
-        
-        -  该语料库的内容由现实世界的用户提出，高质量的答案由具有深度领域知识的专业人士提供。
-           所以这是一个具有真正价值的语料，而不是玩具。
-        
-        -  在上述论文中，语料库用于答复选择任务。
-           另一方面，这种语料库的其他用法也是可能的。
-           例如，通过阅读理解答案，观察学习等自主学习，使系统能够最终拿出自己的看不见的问题的答案。
-        
-        欢迎任何进一步增加此数据集的想法。
-        
-        阅读 `详细文档 <https://github.com/chatopera/insuranceqa-corpus-zh>`__
-        
-        声明
-        ----
-        
-        声明1 :
-        `insuranceqa-corpus-zh <https://github.com/chatopera/insuranceqa-corpus-zh>`__
-        
-        本数据集使用翻译
-        `insuranceQA <https://github.com/shuzi/insuranceQA>`__\ 而生成，代码发布证书
-        `Chunsong Public License, version 1.0<https://docs.cskefu.com/licenses/v1.html>`。数据仅限于研究用途，如果在发布的任何媒体、期刊、杂志或博客等内容时，必须注明引用和地址。
-        
-        ::
-        
-            InsuranceQA Corpus, Hai Liang Wang, https://github.com/chatopera/insuranceqa-corpus-zh, 07 27, 2017
-        
-        任何基于\ `insuranceqa-corpus <https://github.com/chatopera/insuranceqa-corpus-zh>`__\ 衍生的数据也需要开放并需要声明和“声明1”和“声明2”一致的内容。
-        
-        声明2 : `insuranceQA <https://github.com/shuzi/insuranceQA>`__
-        
-        此数据集仅作为研究目的提供。如果您使用这些数据发表任何内容，请引用我们的论文：\ `Applying
-        Deep Learning to Answer Selection: A Study and An Open
-        Task <https://arxiv.org/abs/1508.01585>`__\ 。Minwei Feng, Bing Xiang,
-        Michael R. Glass, Lidan Wang, Bowen Zhou @ 2015
-        
 Keywords: corpus,machine-learning,deep-learning,NLP,question-answering
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Text Processing :: Linguistic
+License-File: LICENSE
+
+
+insuranceqa-corpus-zh
+=====================
+
+保险行业语料库
+
+Welcome
+-------
+
+该语料库包含从网站\ `Insurance
+Library <http://www.insurancelibrary.com/>`__ 收集的问题和答案。
+
+据我们所知，这是保险领域首个开放的QA语料库：
+
+-  该语料库的内容由现实世界的用户提出，高质量的答案由具有深度领域知识的专业人士提供。
+   所以这是一个具有真正价值的语料，而不是玩具。
+
+-  在上述论文中，语料库用于答复选择任务。
+   另一方面，这种语料库的其他用法也是可能的。
+   例如，通过阅读理解答案，观察学习等自主学习，使系统能够最终拿出自己的看不见的问题的答案。
+
+欢迎任何进一步增加此数据集的想法。
+
+阅读 `详细文档 <https://github.com/chatopera/insuranceqa-corpus-zh>`__
+
+声明
+----
+
+声明1 :
+`insuranceqa-corpus-zh <https://github.com/chatopera/insuranceqa-corpus-zh>`__
+
+本数据集使用翻译
+`insuranceQA <https://github.com/shuzi/insuranceQA>`__\ 而生成，代码发布证书
+`Chunsong Public License, version 1.0<https://docs.cskefu.com/licenses/v1.html>`。数据仅限于研究用途，如果在发布的任何媒体、期刊、杂志或博客等内容时，必须注明引用和地址。
+
+::
+
+    InsuranceQA Corpus, Hai Liang Wang, https://github.com/chatopera/insuranceqa-corpus-zh, 07 27, 2017
+
+任何基于\ `insuranceqa-corpus <https://github.com/chatopera/insuranceqa-corpus-zh>`__\ 衍生的数据也需要开放并需要声明和“声明1”和“声明2”一致的内容。
+
+声明2 : `insuranceQA <https://github.com/shuzi/insuranceQA>`__
+
+此数据集仅作为研究目的提供。如果您使用这些数据发表任何内容，请引用我们的论文：\ `Applying
+Deep Learning to Answer Selection: A Study and An Open
+Task <https://arxiv.org/abs/1508.01585>`__\ 。Minwei Feng, Bing Xiang,
+Michael R. Glass, Lidan Wang, Bowen Zhou @ 2015
```

### Comparing `insuranceqa_data-2.5.2/README.md` & `insuranceqa_data-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `insuranceqa_data-2.5.2/insuranceqa_data/LICENSE` & `insuranceqa_data-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `insuranceqa_data-2.5.2/insuranceqa_data/__init__.py` & `insuranceqa_data-2.5.3/insuranceqa_data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 def load_pool_train(data_path=None):
     download = False
     if data_path is None:
         POOL_TRAIN_DATA = os.path.join(CORPUS_FOLDER_PATH, 'pool', 'train.json.gz')
         download = True
     else:
         POOL_TRAIN_DATA = os.path.join(data_path, 'pool', 'train.json.gz')
-        return load(POOL_TRAIN_DATA, download=download)
+    return load(POOL_TRAIN_DATA, download=download)
 
 def load_pool_answers(data_path=None):
     download = False
     if data_path is None:
         POOL_ANS_DATA = os.path.join(CORPUS_FOLDER_PATH, 'pool', 'answers.json.gz')
         download = True
     else:
```

### Comparing `insuranceqa_data-2.5.2/insuranceqa_data.egg-info/PKG-INFO` & `insuranceqa_data-2.5.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-Metadata-Version: 1.1
-Name: insuranceqa-data
-Version: 2.5.2
+Metadata-Version: 2.1
+Name: insuranceqa_data
+Version: 2.5.3
 Summary: Insuranceqa Corpus in Chinese for Machine Learning
 Home-page: https://github.com/chatopera/insuranceqa-corpus-zh
 Author: Hai Liang Wang
 Author-email: hailiang.hl.wang@gmail.com
 License: Chunsong Public License, version 1.0
-Description: 
-        insuranceqa-corpus-zh
-        =====================
-        
-        保险行业语料库
-        
-        Welcome
-        -------
-        
-        该语料库包含从网站\ `Insurance
-        Library <http://www.insurancelibrary.com/>`__ 收集的问题和答案。
-        
-        据我们所知，这是保险领域首个开放的QA语料库：
-        
-        -  该语料库的内容由现实世界的用户提出，高质量的答案由具有深度领域知识的专业人士提供。
-           所以这是一个具有真正价值的语料，而不是玩具。
-        
-        -  在上述论文中，语料库用于答复选择任务。
-           另一方面，这种语料库的其他用法也是可能的。
-           例如，通过阅读理解答案，观察学习等自主学习，使系统能够最终拿出自己的看不见的问题的答案。
-        
-        欢迎任何进一步增加此数据集的想法。
-        
-        阅读 `详细文档 <https://github.com/chatopera/insuranceqa-corpus-zh>`__
-        
-        声明
-        ----
-        
-        声明1 :
-        `insuranceqa-corpus-zh <https://github.com/chatopera/insuranceqa-corpus-zh>`__
-        
-        本数据集使用翻译
-        `insuranceQA <https://github.com/shuzi/insuranceQA>`__\ 而生成，代码发布证书
-        `Chunsong Public License, version 1.0<https://docs.cskefu.com/licenses/v1.html>`。数据仅限于研究用途，如果在发布的任何媒体、期刊、杂志或博客等内容时，必须注明引用和地址。
-        
-        ::
-        
-            InsuranceQA Corpus, Hai Liang Wang, https://github.com/chatopera/insuranceqa-corpus-zh, 07 27, 2017
-        
-        任何基于\ `insuranceqa-corpus <https://github.com/chatopera/insuranceqa-corpus-zh>`__\ 衍生的数据也需要开放并需要声明和“声明1”和“声明2”一致的内容。
-        
-        声明2 : `insuranceQA <https://github.com/shuzi/insuranceQA>`__
-        
-        此数据集仅作为研究目的提供。如果您使用这些数据发表任何内容，请引用我们的论文：\ `Applying
-        Deep Learning to Answer Selection: A Study and An Open
-        Task <https://arxiv.org/abs/1508.01585>`__\ 。Minwei Feng, Bing Xiang,
-        Michael R. Glass, Lidan Wang, Bowen Zhou @ 2015
-        
 Keywords: corpus,machine-learning,deep-learning,NLP,question-answering
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Text Processing :: Linguistic
+License-File: LICENSE
+
+
+insuranceqa-corpus-zh
+=====================
+
+保险行业语料库
+
+Welcome
+-------
+
+该语料库包含从网站\ `Insurance
+Library <http://www.insurancelibrary.com/>`__ 收集的问题和答案。
+
+据我们所知，这是保险领域首个开放的QA语料库：
+
+-  该语料库的内容由现实世界的用户提出，高质量的答案由具有深度领域知识的专业人士提供。
+   所以这是一个具有真正价值的语料，而不是玩具。
+
+-  在上述论文中，语料库用于答复选择任务。
+   另一方面，这种语料库的其他用法也是可能的。
+   例如，通过阅读理解答案，观察学习等自主学习，使系统能够最终拿出自己的看不见的问题的答案。
+
+欢迎任何进一步增加此数据集的想法。
+
+阅读 `详细文档 <https://github.com/chatopera/insuranceqa-corpus-zh>`__
+
+声明
+----
+
+声明1 :
+`insuranceqa-corpus-zh <https://github.com/chatopera/insuranceqa-corpus-zh>`__
+
+本数据集使用翻译
+`insuranceQA <https://github.com/shuzi/insuranceQA>`__\ 而生成，代码发布证书
+`Chunsong Public License, version 1.0<https://docs.cskefu.com/licenses/v1.html>`。数据仅限于研究用途，如果在发布的任何媒体、期刊、杂志或博客等内容时，必须注明引用和地址。
+
+::
+
+    InsuranceQA Corpus, Hai Liang Wang, https://github.com/chatopera/insuranceqa-corpus-zh, 07 27, 2017
+
+任何基于\ `insuranceqa-corpus <https://github.com/chatopera/insuranceqa-corpus-zh>`__\ 衍生的数据也需要开放并需要声明和“声明1”和“声明2”一致的内容。
+
+声明2 : `insuranceQA <https://github.com/shuzi/insuranceQA>`__
+
+此数据集仅作为研究目的提供。如果您使用这些数据发表任何内容，请引用我们的论文：\ `Applying
+Deep Learning to Answer Selection: A Study and An Open
+Task <https://arxiv.org/abs/1508.01585>`__\ 。Minwei Feng, Bing Xiang,
+Michael R. Glass, Lidan Wang, Bowen Zhou @ 2015
```

### Comparing `insuranceqa_data-2.5.2/setup.py` & `insuranceqa_data-2.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 此数据集仅作为研究目的提供。如果您使用这些数据发表任何内容，请引用我们的论文：\ `Applying
 Deep Learning to Answer Selection: A Study and An Open
 Task <https://arxiv.org/abs/1508.01585>`__\ 。Minwei Feng, Bing Xiang,
 Michael R. Glass, Lidan Wang, Bowen Zhou @ 2015
 """
 
 setup(name='insuranceqa_data',
-      version='2.5.2',
+      version='2.5.3',
       description='Insuranceqa Corpus in Chinese for Machine Learning',
       long_description=LONGDOC,
       author='Hai Liang Wang',
       author_email='hailiang.hl.wang@gmail.com',
       url='https://github.com/chatopera/insuranceqa-corpus-zh',
       license="Chunsong Public License, version 1.0",
       classifiers=[
```

