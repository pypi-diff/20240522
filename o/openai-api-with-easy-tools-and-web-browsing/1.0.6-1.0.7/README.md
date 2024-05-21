# Comparing `tmp/openai_api_with_easy_tools_and_web_browsing-1.0.6.tar.gz` & `tmp/openai_api_with_easy_tools_and_web_browsing-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-1.0.6.tar", last modified: Wed May  1 09:12:02 2024, max compression
+gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-1.0.7.tar", last modified: Tue May 21 22:58:20 2024, max compression
```

## Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.6.tar` & `openai_api_with_easy_tools_and_web_browsing-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 09:12:02.827296 openai_api_with_easy_tools_and_web_browsing-1.0.6/
--rw-rw-rw-   0        0        0     1087 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     4973 2024-05-01 09:12:02.826251 openai_api_with_easy_tools_and_web_browsing-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4183 2024-05-01 09:04:23.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/README.md
--rw-rw-rw-   0        0        0      879 2024-05-01 09:08:40.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 09:12:02.828301 openai_api_with_easy_tools_and_web_browsing-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 09:12:02.792275 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 09:12:02.824920 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
--rw-rw-rw-   0        0        0     4973 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11332 2024-05-01 08:42:51.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:12:02.823914 openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/
--rw-rw-rw-   0        0        0     2871 2024-05-01 08:40:45.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/test.py
--rw-rw-rw-   0        0        0     3009 2024-05-01 09:05:30.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/test_fr.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:58:20.434444 openai_api_with_easy_tools_and_web_browsing-1.0.7/
+-rw-rw-rw-   0        0        0     1087 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5338 2024-05-21 22:58:20.433153 openai_api_with_easy_tools_and_web_browsing-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4547 2024-05-21 22:45:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/README.md
+-rw-rw-rw-   0        0        0      880 2024-05-21 21:32:22.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 22:58:20.434444 openai_api_with_easy_tools_and_web_browsing-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 22:58:20.410375 openai_api_with_easy_tools_and_web_browsing-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 22:58:20.433153 openai_api_with_easy_tools_and_web_browsing-1.0.7/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
+-rw-rw-rw-   0        0        0     5338 2024-05-21 22:58:20.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-05-21 22:58:20.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 22:58:20.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-21 22:58:20.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/src/openai_api_with_easy_tools_and_web_browsing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2024-05-21 22:58:20.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12459 2024-05-21 22:49:19.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/src/openai_api_with_easy_tools_and_web_browsing.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:58:20.432152 openai_api_with_easy_tools_and_web_browsing-1.0.7/tests/
+-rw-rw-rw-   0        0        0     3229 2024-05-21 22:45:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/tests/test.py
+-rw-rw-rw-   0        0        0     3366 2024-05-21 22:51:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.7/tests/test_fr.py
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.6/LICENSE` & `openai_api_with_easy_tools_and_web_browsing-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.6/PKG-INFO` & `openai_api_with_easy_tools_and_web_browsing-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openai_api_with_easy_tools_and_web_browsing
-Version: 1.0.6
+Version: 1.0.7
 Summary: An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools
 Author-email: ThomLecha <hamster12@hotmail.fr>
 Project-URL: Homepage, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing
 Project-URL: Issues, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai>=1.3.5
+Requires-Dist: openai>=1.30.1
 Requires-Dist: requests>=2.31.0
 
 # openai-api-with-easy-tools-and-web-browsing
 An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools.
 
 Here is an example of capabilities of this library:
 
@@ -25,19 +25,19 @@
 The response, using a web search and a custom tool to add two numbers, should be something like:
 *The total population of Paris and New York in 2015 was about 31,082,144 inhabitants. If 10,000,000 is added to this number, it becomes 41,082,144.*
 
 **See code below to reproduce this example.**
 
 First, get an API key from OpenAI [here](https://openai.com/blog/openai-api) and get a Bing Custom Search API key, which you can get [here](https://azuremarketplace.microsoft.com/fr/marketplace/apps/Microsoft.BingCustomSearch?tab=Overview) ([free for limited use](https://www.microsoft.com/en-us/bing/apis/pricing))
 
-Then, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
+Then, get the [library](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/) with pip: **pip install openai-api-with-easy-tools-and-web-browsing**
 
 And then, you can use the following code to get started:
 
-```
+```python
 import openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # Enter our API keys
 subscriptionKey = ""
 openAIAPIKey = ""
 
 ### Creation of the Bing search tool ###
@@ -74,23 +74,29 @@
             },
             "required": ["a", "b"]
         }
     }
 }
 
 # Create an instance of the 'OpenaiApiWithEasyToolsAndWebBrowsing' class
-openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
+openaiApiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
 print("PONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+answer = openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual",
+                                                           toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                           temperature=0.9, top_p=1,
+                                                           verbosity=1)
 # The response, using a web search and a custom tool to add two numbers, should be something like:
 # "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
 # If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(None, systemMessage="You are a helpful assistant", model="gpt-4o", mode="continuous",
+                                                  toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                  max_prompt_tokens=4096, max_completion_tokens=2048,
+                                                  verbosity=1)
 ```
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.6/README.md` & `openai_api_with_easy_tools_and_web_browsing-1.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 The response, using a web search and a custom tool to add two numbers, should be something like:
 *The total population of Paris and New York in 2015 was about 31,082,144 inhabitants. If 10,000,000 is added to this number, it becomes 41,082,144.*
 
 **See code below to reproduce this example.**
 
 First, get an API key from OpenAI [here](https://openai.com/blog/openai-api) and get a Bing Custom Search API key, which you can get [here](https://azuremarketplace.microsoft.com/fr/marketplace/apps/Microsoft.BingCustomSearch?tab=Overview) ([free for limited use](https://www.microsoft.com/en-us/bing/apis/pricing))
 
-Then, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
+Then, get the [library](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/) with pip: **pip install openai-api-with-easy-tools-and-web-browsing**
 
 And then, you can use the following code to get started:
 
-```
+```python
 import openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # Enter our API keys
 subscriptionKey = ""
 openAIAPIKey = ""
 
 ### Creation of the Bing search tool ###
@@ -58,23 +58,29 @@
             },
             "required": ["a", "b"]
         }
     }
 }
 
 # Create an instance of the 'OpenaiApiWithEasyToolsAndWebBrowsing' class
-openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
+openaiApiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
 print("PONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+answer = openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual",
+                                                           toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                           temperature=0.9, top_p=1,
+                                                           verbosity=1)
 # The response, using a web search and a custom tool to add two numbers, should be something like:
 # "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
 # If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(None, systemMessage="You are a helpful assistant", model="gpt-4o", mode="continuous",
+                                                  toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                  max_prompt_tokens=4096, max_completion_tokens=2048,
+                                                  verbosity=1)
 ```
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.6/pyproject.toml` & `openai_api_with_easy_tools_and_web_browsing-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "openai_api_with_easy_tools_and_web_browsing"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="ThomLecha", email="hamster12@hotmail.fr" },
 ]
 description = "An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools"
 
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "openai>=1.3.5",
+    "openai>=1.30.1",
     "requests>=2.31.0"
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO` & `openai_api_with_easy_tools_and_web_browsing-1.0.7/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openai_api_with_easy_tools_and_web_browsing
-Version: 1.0.6
+Version: 1.0.7
 Summary: An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools
 Author-email: ThomLecha <hamster12@hotmail.fr>
 Project-URL: Homepage, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing
 Project-URL: Issues, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai>=1.3.5
+Requires-Dist: openai>=1.30.1
 Requires-Dist: requests>=2.31.0
 
 # openai-api-with-easy-tools-and-web-browsing
 An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools.
 
 Here is an example of capabilities of this library:
 
@@ -25,19 +25,19 @@
 The response, using a web search and a custom tool to add two numbers, should be something like:
 *The total population of Paris and New York in 2015 was about 31,082,144 inhabitants. If 10,000,000 is added to this number, it becomes 41,082,144.*
 
 **See code below to reproduce this example.**
 
 First, get an API key from OpenAI [here](https://openai.com/blog/openai-api) and get a Bing Custom Search API key, which you can get [here](https://azuremarketplace.microsoft.com/fr/marketplace/apps/Microsoft.BingCustomSearch?tab=Overview) ([free for limited use](https://www.microsoft.com/en-us/bing/apis/pricing))
 
-Then, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
+Then, get the [library](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/) with pip: **pip install openai-api-with-easy-tools-and-web-browsing**
 
 And then, you can use the following code to get started:
 
-```
+```python
 import openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # Enter our API keys
 subscriptionKey = ""
 openAIAPIKey = ""
 
 ### Creation of the Bing search tool ###
@@ -74,23 +74,29 @@
             },
             "required": ["a", "b"]
         }
     }
 }
 
 # Create an instance of the 'OpenaiApiWithEasyToolsAndWebBrowsing' class
-openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
+openaiApiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
 print("PONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+answer = openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual",
+                                                           toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                           temperature=0.9, top_p=1,
+                                                           verbosity=1)
 # The response, using a web search and a custom tool to add two numbers, should be something like:
 # "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
 # If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(None, systemMessage="You are a helpful assistant", model="gpt-4o", mode="continuous",
+                                                  toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                  max_prompt_tokens=4096, max_completion_tokens=2048,
+                                                  verbosity=1)
 ```
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.7/src/openai_api_with_easy_tools_and_web_browsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,14 +142,20 @@
                 },
             },
         "required": ["userRequest"]
         }
     }
 }
 
+class runFailedError(Exception):
+    pass
+
+class runIncompleteError(Exception):
+    pass
+
 class OpenaiApiWithEasyToolsAndWebBrowsing():
     """This class allows interacting with the OpenAI API to get responses from user messages."""
 
     def __init__(self, openAIAPIKey):
         """Initialize the OpenAI client with the provided API key."""
         self.openaiClient = openai.OpenAI(api_key=openAIAPIKey)
 
@@ -162,15 +168,15 @@
 
     def waitForRunCompletion(self, threadId, runId):
         """This function waits for the completion of a thread/conversation run and returns the result"""
         while True:
             # Check the status of the run 10 times per second
             time.sleep(0.1)
             run = self.openaiClient.beta.threads.runs.retrieve(thread_id=threadId, run_id=runId)
-            if run.status in ["completed", "failed", "requires_action"]:
+            if run.status in ["completed", "failed", "incomplete", "requires_action"]:
                 return(run)
             # Lines below are not necessary
             elif run.status == "in_progress" :
                 continue
 
     def getToolReturnList(self, toolsToCall, toolList=[]):
         """This function returns a list of tool returns from a list of tools to call"""
@@ -190,17 +196,29 @@
                     toolReturn = t(**json.loads(functionArgs))
 
             # Add the tool return to the list
             toolReturnList.append({"tool_call_id": toolCallId, "output": toolReturn})
 
         return(toolReturnList)
 
-    def getLLMAnswerWithWebBrowsingAndTools(self, userMessage, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[], toolDescriptionList=[], verbosity=0):
+    def getLLMAnswer(self,
+                     userMessage,
+                     systemMessage="You are a helpful assistant",
+                     model="gpt-3.5-turbo",
+                     mode="ponctual",
+                     toolList=[],
+                     toolDescriptionList=[],
+                     temperature=1,
+                     top_p=1,
+                     max_prompt_tokens=32768,
+                     max_completion_tokens=32768,
+                     verbosity=0):
         """This function interacts with an LLM to get a response from a user message.
-        There is 'ponctual' mode for a single response or 'continuous' mode for continuous conversation with user input (then set userMessage=None)."""
+        There is 'ponctual' mode for a single response or 'continuous' mode for
+        continuous conversation with user input (then set userMessage=None)."""
 
         # Initialize the assistant with the list of tools
         assistant = self.openaiClient.beta.assistants.create(instructions=systemMessage, model=model, tools=toolDescriptionList)
 
         # Create a discussion thread
         thread = self.openaiClient.beta.threads.create()
 
@@ -210,33 +228,43 @@
                 print("\nYour request (Type 'exit' to exit the program) : ")
                 userMessage = input()
                 if userMessage.lower() == "exit":
                     break
 
             # Create a message and a run
             self.openaiClient.beta.threads.messages.create(thread_id=thread.id, role="user", content=userMessage)
-            run = self.openaiClient.beta.threads.runs.create(thread_id=thread.id, assistant_id=assistant.id)
+            run = self.openaiClient.beta.threads.runs.create(thread_id=thread.id,
+                                                             assistant_id=assistant.id,
+                                                             temperature=temperature,
+                                                             top_p=top_p,
+                                                             max_prompt_tokens=max_prompt_tokens,
+                                                             max_completion_tokens=max_completion_tokens
+                                                             )
             # Wait for the end of the run
             run = self.waitForRunCompletion(thread.id, run.id)
 
             # If (and as long as) the discussion run returns a tool to be called, call it
             while run.status == "requires_action":
                 # Retrieve the tools to be called
                 toolsToCall = run.required_action.submit_tool_outputs.tool_calls
                 if verbosity >= 1:
-                    print("Tools to call :")
+                    print("Tool(s) called:")
                     [print("   " + str(t)) for t in toolsToCall]
                 toolReturnList = self.getToolReturnList(toolsToCall, toolList=toolList)
                 run = self.openaiClient.beta.threads.runs.submit_tool_outputs(thread_id=thread.id, run_id=run.id, tool_outputs=toolReturnList)
                 # Wait for the end of the run
                 run = self.waitForRunCompletion(thread.id, run.id)
 
-            # If the discussion run returns a failure, display it
+            # If the discussion run returns a failure, raise an exception
             if run.status == "failed":
-                print(run.error)
+                raise runFailedError(run.last_error)
+
+            # If the discussion run returns "incomplete", raise an exception
+            if run.status == "incomplete":
+                raise runIncompleteError(run.incomplete_details)
 
             # If in punctual mode, display the messages and exit the loop
             if mode == "ponctual":
                 return(self.getMessageListFromThread(thread.id)[0])
 
             # Display the messages and restart the loop to continue the conversation
             print("\nAssistant response:\n" + self.getMessageListFromThread(thread.id)[0])
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/test.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.7/tests/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,22 +38,28 @@
             },
             "required": ["a", "b"]
         }
     }
 }
 
 # Create an instance of the 'OpenaiApiWithEasyToolsAndWebBrowsing' class
-openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
+openaiApiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
 print("PONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+answer = openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual",
+                                                           toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                           temperature=0.9, top_p=1,
+                                                           verbosity=1)
 # The response, using a web search and a custom tool to add two numbers, should be something like:
 # "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
 # If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(None, systemMessage="You are a helpful assistant", model="gpt-4o", mode="continuous",
+                                                  toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                  max_prompt_tokens=4096, max_completion_tokens=2048,
+                                                  verbosity=1)
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/test_fr.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.7/tests/test_fr.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,22 +38,28 @@
             },
             "required": ["a", "b"]
         }
     }
 }
 
 # On crée une instance de la classe 'OpenaiApiWithEasyToolsAndWebBrowsing'
-openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
+openaiApiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Renvoie d'une réponse à un prompt en mode 'ponctual' ###
 print("MODE PONCTUEL\n")
 prompt = "Tu peux chercher sur internet la population de Paris et de New York en l'année 2015, puis additionner les 2 valeurs et me dire le résultat, et enfin ensuite ajouter 10 000 000 à ce résultat"
 # On utilise la fonction 'getLLMAnswerWithWebBrowsingAndTools' pour obtenir une réponse à partir d'un message utilisateur
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+answer = openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual",
+                                                           toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                           temperature=0.9, top_p=1,
+                                                           verbosity=1)
 # La réponse, en utilisant l'outil de web browsing et l'additionneur doit être quelque chose du genre :
 # "La population totale de Paris et de New York en 2015 était d'environ 31 082 144 habitants.
 # Si l'on ajoute 10 000 000 à ce nombre, on obtient 41 082 144."
 print(answer)
 
-### Discussion en mode 'continuous' ###s
+### Discussion en mode 'continuous' ###
 print("\n\n\nMODE CONTINUE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
+openaiApiWithEasyToolsAndWebBrowsing.getLLMAnswer(None, systemMessage="You are a helpful assistant", model="gpt-4o", mode="continuous",
+                                                  toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription],
+                                                  max_prompt_tokens=4096, max_completion_tokens=2048,
+                                                  verbosity=1)
```

