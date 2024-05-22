# Comparing `tmp/esanalyzer-1.0.6-py3-none-any.whl.zip` & `tmp/esanalyzer-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7909 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    23279 b- defN 24-Apr-30 12:17 esanalyzer.py
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-30 12:18 esanalyzer-1.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1744 b- defN 24-Apr-30 12:18 esanalyzer-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-30 12:18 esanalyzer-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-30 12:18 esanalyzer-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      472 b- defN 24-Apr-30 12:18 esanalyzer-1.0.6.dist-info/RECORD
-6 files, 26672 bytes uncompressed, 7057 bytes compressed:  73.5%
+Zip file size: 7959 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    23353 b- defN 24-May-22 12:18 esanalyzer.py
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1806 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      472 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/RECORD
+6 files, 26808 bytes uncompressed, 7107 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: esanalyzer.py
 Comment: 
 
-Filename: esanalyzer-1.0.6.dist-info/LICENSE
+Filename: esanalyzer-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: esanalyzer-1.0.6.dist-info/METADATA
+Filename: esanalyzer-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: esanalyzer-1.0.6.dist-info/WHEEL
+Filename: esanalyzer-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: esanalyzer-1.0.6.dist-info/top_level.txt
+Filename: esanalyzer-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: esanalyzer-1.0.6.dist-info/RECORD
+Filename: esanalyzer-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## esanalyzer.py

```diff
@@ -351,14 +351,17 @@
         # Retrieve the text input from the command line
     #    new_text = sys.argv[1]
     #else:
         # Provide a default text if no command-line argument is provided
     #    new_text = "Empty Text"
     #sentiment_analyzer = SentimentAnalyzer(new_text)
     #sentiment, sentiment_score = sentiment_analyzer.analyze_sentiment()
+    
+    if len(new_text) == 0:
+        new_text="Wow, I am so happy."
    
     #TRANSALTE TEXT INTO ENGLISH
     #APPLY GOOGLE TRANSLATE ONLY WHEN IT IS True
     if config.get('googleTranslate', True):
         translated = translator.translate(new_text, dest='en')
         new_text = translated.text
```

## Comparing `esanalyzer-1.0.6.dist-info/LICENSE` & `esanalyzer-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `esanalyzer-1.0.6.dist-info/METADATA` & `esanalyzer-1.0.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: esanalyzer
-Version: 1.0.6
+Version: 1.0.7
 Summary: Emotion("fear", "anger", "surprise", "sadness", "disgust", "joy") and Sentiment("Positive","Negative") Analysis
-Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer/version/1.0.6
+Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer/version/1.0.7
 Author: Ajay Singh Rajput
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nrclex ==3.0.0
 Requires-Dist: datasets ==2.16.1
 Requires-Dist: scikit-learn ==1.3.2
@@ -14,20 +14,23 @@
 Requires-Dist: numpy ==1.26.3
 Requires-Dist: googletrans ==4.0.0-rc1
 Requires-Dist: transformers ==4.36.2
 Requires-Dist: nltk ==3.8.1
 
 # esanalyzer
 
-    The Python Emotion and Sentiment Analysis library you've been looking for.
+    The Python Emotion Analysis and Sentiment Analysis library you've been looking for.
 
     ## Services
     - Emotion Analysis("fear", "anger", "surprise", "sadness", "disgust", "joy")
     - Sentiment Analysis("Positive","Negative")
     - Multi Language Support
+    
+    ## Supported Python Version
+    - 3.12.3
 
     ## Usage
     - Install using `pip install esanalyzer`
 
     ```python
     from esanalyzer import EmotionAnalyzer
```

