# Comparing `tmp/annobee-0.5.9.tar.gz` & `tmp/annobee-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annobee-0.5.9.tar", last modified: Mon May 20 21:58:18 2024, max compression
+gzip compressed data, was "annobee-0.6.0.tar", last modified: Wed May 22 16:28:19 2024, max compression
```

## Comparing `annobee-0.5.9.tar` & `annobee-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-20 21:58:18.771803 annobee-0.5.9/
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     1074 2024-05-13 19:30:06.000000 annobee-0.5.9/LICENSE
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     7350 2024-05-20 21:58:18.771803 annobee-0.5.9/PKG-INFO
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     6953 2024-05-15 12:36:35.000000 annobee-0.5.9/README.md
-drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-20 21:58:18.767803 annobee-0.5.9/annobee/
--rw-rw-r--   0 kadir     (1001) kadir     (1001)       30 2024-05-15 11:15:27.000000 annobee-0.5.9/annobee/__init__.py
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     2984 2024-05-20 21:54:46.000000 annobee-0.5.9/annobee/cli.py
-drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-20 21:58:18.767803 annobee-0.5.9/annobee.egg-info/
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     7350 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/PKG-INFO
--rw-rw-r--   0 kadir     (1001) kadir     (1001)      249 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/SOURCES.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)        1 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/dependency_links.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)       46 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/entry_points.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)       82 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/requires.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)        8 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/top_level.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)       38 2024-05-20 21:58:18.771803 annobee-0.5.9/setup.cfg
--rw-rw-r--   0 kadir     (1001) kadir     (1001)      937 2024-05-20 21:57:22.000000 annobee-0.5.9/setup.py
+drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-22 16:28:19.608652 annobee-0.6.0/
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     1074 2024-05-13 19:30:06.000000 annobee-0.6.0/LICENSE
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     6514 2024-05-22 16:28:19.608652 annobee-0.6.0/PKG-INFO
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     6117 2024-05-22 16:22:14.000000 annobee-0.6.0/README.md
+drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-22 16:28:19.608652 annobee-0.6.0/annobee/
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)       30 2024-05-15 11:15:27.000000 annobee-0.6.0/annobee/__init__.py
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     2921 2024-05-21 16:37:47.000000 annobee-0.6.0/annobee/cli.py
+drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-22 16:28:19.608652 annobee-0.6.0/annobee.egg-info/
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     6514 2024-05-22 16:28:19.000000 annobee-0.6.0/annobee.egg-info/PKG-INFO
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)      249 2024-05-22 16:28:19.000000 annobee-0.6.0/annobee.egg-info/SOURCES.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)        1 2024-05-22 16:28:19.000000 annobee-0.6.0/annobee.egg-info/dependency_links.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)       46 2024-05-22 16:28:19.000000 annobee-0.6.0/annobee.egg-info/entry_points.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)       82 2024-05-22 16:28:19.000000 annobee-0.6.0/annobee.egg-info/requires.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)        8 2024-05-22 16:28:19.000000 annobee-0.6.0/annobee.egg-info/top_level.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)       38 2024-05-22 16:28:19.608652 annobee-0.6.0/setup.cfg
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)      937 2024-05-22 16:25:07.000000 annobee-0.6.0/setup.py
```

### Comparing `annobee-0.5.9/LICENSE` & `annobee-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `annobee-0.5.9/PKG-INFO` & `annobee-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,160 +1,96 @@
 Metadata-Version: 2.1
 Name: annobee
-Version: 0.5.9
+Version: 0.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/variantAnnotation/annobee-sdk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
-<!--
-*** Thanks for checking out the Best-README-Template. If you have a suggestion
-*** that would make this better, please fork the repo and create a pull request
-*** or simply open an issue with the tag "enhancement".
-*** Don't forget to give the project a star!
-*** Thanks again! Now go create something AMAZING! :D
--->
-
-
-
-<!-- PROJECT SHIELDS -->
-<!--
-*** I'm using markdown "reference style" links for readability.
-*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
-*** See the bottom of this document for the declaration of the reference variables
-*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
-*** https://www.markdownguide.org/basic-syntax/#reference-style-links
--->
 
 <!-- ABOUT THE PROJECT -->
+<h1>Annobee</h1>
 <h2>About The Project</h2>
 <p>
-    <code>annobee-sdk</code> is designed to analyze genetic variants to determine their pathogenicity using multiple established criteria. It integrates several functions to set various genetic criteria based on evolutionary conservation, allele frequency, and ACMG/AMP standards. The main functionality is centralized in the <code>main.py</code>.
+    <code>annobee</code> is designed to analyze genetic variants to determine their pathogenicity using multiple established criteria. It integrates several functions to set various genetic criteria based on evolutionary conservation, allele frequency, and ACMG/AMP standards. The main functionality is centralized in the <code>main.py</code>.
 </p>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <h3>Built With</h3>
-
 <ul>
     <li><a href="https://www.python.org/">Python</a></li>
 </ul>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
 <!-- GETTING STARTED -->
 <h2>Getting Started</h2>
-
 <p>To get a local copy up and running follow these simple example steps.</p>
 
 <h3>Prerequisites</h3>
-
 <ul>
+    <li>MongoDB: You can download it from <a href="https://www.mongodb.com/download-center/community">MongoDB Download Center</a>.</li>
     <li>Python: Download Python <a href="https://www.python.org/downloads/">here</a>.</li>
 </ul>
 
 <h3>Requirements</h3>
-
 <ul>
     <li>flask==2.0.1</li>
     <li>numpy==1.23.5</li>
     <li>pandas==1.5.3</li>
     <li>requests==2.25.1</li>
     <li>tqdm==4.65.0</li>
 </ul>
 
 <h3>Installation</h3>
-
 <ol>
     <li>Clone the repo
-        <pre><code>git clone https://github.com/variantAnnotation/annobee-sdk </code></pre>
+        <pre><code>git clone https://github.com/variantAnnotation/annobee-sdk.git</code></pre>
     </li>
     <li>Follow to directory where you clone the repo:
         <pre><code>cd annobee-sdk</code></pre>
     </li>
     <li>Install requirements and dependencies:
         <pre><code>pip install -r requirements.txt</code></pre>
     </li>
 </ol>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- USAGE EXAMPLES -->
 <h2>Usage</h2>
 
-<h3> Downloading annobee</h3>
-<pre><code>pip install annobee</code></pre>
+<h3>Starting the Flask API</h3>
+<p>To start the Flask API that the SDK communicates with:</p>
+<pre><code>python app.py</code></pre>
 
 <h3>Command-Line Interface</h3>
 
 <p>To use the <code>annobee-sdk</code>, you can execute the CLI tool with various options to evaluate genetic variant criteria.</p>
 
 <h4> </4>
 
 <h4>Example 1: Evaluate Specific Criteria (PS1)</h4>
-<pre><code>annobee 1-14973-A-AG -ps1</code></pre>
-<p> It returns : </p>
-<pre><code>  { "PS1": 0 }</code></pre>
-
-<h4>Example 2: Evaluate Specific Criterias more then One (PS1, BP7, PP2 etc)</h4>
-<pre><code>annobee 1-14973-A-AG -ps1</code></pre>
-<p> It returns : </p>
-<pre><code>   {
-    "PS1": 0,
-    "BP7": 1,
-    "PP2": 0,
-    "BS1": 0,
-    "PP5": 0
-} </code></pre>
-
-<h4>Example 3: Evaluate All Criteria and pathogenicity</h4>
-<pre><code>annobee 1-14973-A-AG -all</code></pre>
-<p> It returns : </p>
-<pre><code>
-    {"PS1": 0,
-    "PM5": 0,
-    "BP7": 1,
-    "PVS1": 1,
-    "BP1": 0,
-    "PP2": 0,
-    "PS4": 0,
-    "BS1": 0,
-    "BS2": 1,
-    "PM2": 0,
-    "PM1": 0,
-    "PP5": 0,
-    "BP6": 0,
-    "BA1": 1,
-    "PP3": 0,
-    "BP4": 1,
-    "PM4": 1,
-    "BP3": 0,
-    "VA_PATHOGENICITY": "Pathogenic"}
-</code></pre>
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+<pre><code>python cli.py 1-14973-A-AG --endpoint http://localhost:5000/api/interpret -ps1</code></pre>
 
-<h2>Usage as python library</h2>
+<h4>Example 2: Evaluate All Criteria</h4>
+<pre><code>python cli.py 1-14973-A-AG --endpoint http://localhost:5000/api/interpret -all</code></pre>
 
-Here's a simple script that evaluates multiple variants using the `annobee` SDK:
+<h3>Using the Annobee Class in a Python Script</h3>
+<p>Here's an example script that evaluates multiple variants using the <code>Annobee</code> class:</p>
 
-```python
-import json
-from annobee import Annobee
+<pre><code>import json
+from cli import Annobee
 
 def evaluate_variant(annobee, variant, criteria):
     variant_info = annobee.get_criteria(variant)
     results = {}
     
     if criteria == 'all':
         results = annobee.get_all(variant_info)
@@ -196,55 +132,47 @@
     result_three_criteria = evaluate_variant(annobee, variants[0], ['PS1', 'PM5', 'BP7'])
     print(json.dumps(result_three_criteria, indent=4))
 
     # Evaluate all criteria for one variant
     print("\nEvaluating all criteria for one variant:")
     result_all_criteria = evaluate_variant(annobee, variants[0], 'all')
     print(json.dumps(result_all_criteria, indent=4))
-```
+</code></pre>
 
+<h3>Running the Test Script</h3>
+<p>Ensure your Flask API is running and that the <code>cli.py</code> script with the <code>Annobee</code> class is in the same directory or properly installed. Then run the <code>test.py</code> script:</p>
 
+<pre><code>python test.py</code></pre>
+<p>This will print the results of evaluating both one criterion, three criteria, and all criteria for the first variant in the list using the specified endpoint. Adjust the criteria and variant list as needed for your specific use case.</p>
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- ROADMAP -->
 <h2>Roadmap</h2>
-
 <ul>
-    <li>[ ] Adding testing metrics regarding the performance of the platform</li>
+    <li>Adding testing metrics regarding the performance of the platform</li>
 </ul>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- CONTRIBUTING -->
 <h2>Contributing</h2>
-
 <p>Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are <strong>greatly appreciated</strong>.</p>
 
 <p>If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!</p>
 
 <ol>
     <li>Fork the Project</li>
     <li>Create your Feature Branch (<code>git checkout -b feature/AmazingFeature</code>)</li>
     <li>Commit your Changes (<code>git commit -m 'Add some AmazingFeature'</code>)</li>
     <li>Push to the Branch (<code>git push origin feature/AmazingFeature</code>)</li>
     <li>Open a Pull Request</li>
 </ol>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- LICENSE -->
 <h2>License</h2>
-
 <p>Distributed under the MIT License. See <code>LICENSE.txt</code> for more information.</p>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-<a href="https://www.python.org/">Python</a>
+</body>
+</html>
```

### Comparing `annobee-0.5.9/README.md` & `annobee-0.6.0/annobee.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,146 +1,96 @@
+Metadata-Version: 2.1
+Name: annobee
+Version: 0.6.0
+Summary: UNKNOWN
+Home-page: https://github.com/variantAnnotation/annobee-sdk
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
-<!--
-*** Thanks for checking out the Best-README-Template. If you have a suggestion
-*** that would make this better, please fork the repo and create a pull request
-*** or simply open an issue with the tag "enhancement".
-*** Don't forget to give the project a star!
-*** Thanks again! Now go create something AMAZING! :D
--->
-
-
-
-<!-- PROJECT SHIELDS -->
-<!--
-*** I'm using markdown "reference style" links for readability.
-*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
-*** See the bottom of this document for the declaration of the reference variables
-*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
-*** https://www.markdownguide.org/basic-syntax/#reference-style-links
--->
 
 <!-- ABOUT THE PROJECT -->
+<h1>Annobee</h1>
 <h2>About The Project</h2>
 <p>
-    <code>annobee-sdk</code> is designed to analyze genetic variants to determine their pathogenicity using multiple established criteria. It integrates several functions to set various genetic criteria based on evolutionary conservation, allele frequency, and ACMG/AMP standards. The main functionality is centralized in the <code>main.py</code>.
+    <code>annobee</code> is designed to analyze genetic variants to determine their pathogenicity using multiple established criteria. It integrates several functions to set various genetic criteria based on evolutionary conservation, allele frequency, and ACMG/AMP standards. The main functionality is centralized in the <code>main.py</code>.
 </p>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <h3>Built With</h3>
-
 <ul>
     <li><a href="https://www.python.org/">Python</a></li>
 </ul>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
 <!-- GETTING STARTED -->
 <h2>Getting Started</h2>
-
 <p>To get a local copy up and running follow these simple example steps.</p>
 
 <h3>Prerequisites</h3>
-
 <ul>
+    <li>MongoDB: You can download it from <a href="https://www.mongodb.com/download-center/community">MongoDB Download Center</a>.</li>
     <li>Python: Download Python <a href="https://www.python.org/downloads/">here</a>.</li>
 </ul>
 
 <h3>Requirements</h3>
-
 <ul>
     <li>flask==2.0.1</li>
     <li>numpy==1.23.5</li>
     <li>pandas==1.5.3</li>
     <li>requests==2.25.1</li>
     <li>tqdm==4.65.0</li>
 </ul>
 
 <h3>Installation</h3>
-
 <ol>
     <li>Clone the repo
-        <pre><code>git clone https://github.com/variantAnnotation/annobee-sdk </code></pre>
+        <pre><code>git clone https://github.com/variantAnnotation/annobee-sdk.git</code></pre>
     </li>
     <li>Follow to directory where you clone the repo:
         <pre><code>cd annobee-sdk</code></pre>
     </li>
     <li>Install requirements and dependencies:
         <pre><code>pip install -r requirements.txt</code></pre>
     </li>
 </ol>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- USAGE EXAMPLES -->
 <h2>Usage</h2>
 
-<h3> Downloading annobee</h3>
-<pre><code>pip install annobee</code></pre>
+<h3>Starting the Flask API</h3>
+<p>To start the Flask API that the SDK communicates with:</p>
+<pre><code>python app.py</code></pre>
 
 <h3>Command-Line Interface</h3>
 
 <p>To use the <code>annobee-sdk</code>, you can execute the CLI tool with various options to evaluate genetic variant criteria.</p>
 
 <h4> </4>
 
 <h4>Example 1: Evaluate Specific Criteria (PS1)</h4>
-<pre><code>annobee 1-14973-A-AG -ps1</code></pre>
-<p> It returns : </p>
-<pre><code>  { "PS1": 0 }</code></pre>
-
-<h4>Example 2: Evaluate Specific Criterias more then One (PS1, BP7, PP2 etc)</h4>
-<pre><code>annobee 1-14973-A-AG -ps1</code></pre>
-<p> It returns : </p>
-<pre><code>   {
-    "PS1": 0,
-    "BP7": 1,
-    "PP2": 0,
-    "BS1": 0,
-    "PP5": 0
-} </code></pre>
-
-<h4>Example 3: Evaluate All Criteria and pathogenicity</h4>
-<pre><code>annobee 1-14973-A-AG -all</code></pre>
-<p> It returns : </p>
-<pre><code>
-    {"PS1": 0,
-    "PM5": 0,
-    "BP7": 1,
-    "PVS1": 1,
-    "BP1": 0,
-    "PP2": 0,
-    "PS4": 0,
-    "BS1": 0,
-    "BS2": 1,
-    "PM2": 0,
-    "PM1": 0,
-    "PP5": 0,
-    "BP6": 0,
-    "BA1": 1,
-    "PP3": 0,
-    "BP4": 1,
-    "PM4": 1,
-    "BP3": 0,
-    "VA_PATHOGENICITY": "Pathogenic"}
-</code></pre>
+<pre><code>python cli.py 1-14973-A-AG --endpoint http://localhost:5000/api/interpret -ps1</code></pre>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-<h2>Usage as python library</h2>
+<h4>Example 2: Evaluate All Criteria</h4>
+<pre><code>python cli.py 1-14973-A-AG --endpoint http://localhost:5000/api/interpret -all</code></pre>
 
-Here's a simple script that evaluates multiple variants using the `annobee` SDK:
+<h3>Using the Annobee Class in a Python Script</h3>
+<p>Here's an example script that evaluates multiple variants using the <code>Annobee</code> class:</p>
 
-```python
-import json
-from annobee import Annobee
+<pre><code>import json
+from cli import Annobee
 
 def evaluate_variant(annobee, variant, criteria):
     variant_info = annobee.get_criteria(variant)
     results = {}
     
     if criteria == 'all':
         results = annobee.get_all(variant_info)
@@ -182,53 +132,47 @@
     result_three_criteria = evaluate_variant(annobee, variants[0], ['PS1', 'PM5', 'BP7'])
     print(json.dumps(result_three_criteria, indent=4))
 
     # Evaluate all criteria for one variant
     print("\nEvaluating all criteria for one variant:")
     result_all_criteria = evaluate_variant(annobee, variants[0], 'all')
     print(json.dumps(result_all_criteria, indent=4))
-```
+</code></pre>
 
+<h3>Running the Test Script</h3>
+<p>Ensure your Flask API is running and that the <code>cli.py</code> script with the <code>Annobee</code> class is in the same directory or properly installed. Then run the <code>test.py</code> script:</p>
 
+<pre><code>python test.py</code></pre>
+<p>This will print the results of evaluating both one criterion, three criteria, and all criteria for the first variant in the list using the specified endpoint. Adjust the criteria and variant list as needed for your specific use case.</p>
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- ROADMAP -->
 <h2>Roadmap</h2>
-
 <ul>
-    <li>[ ] Adding testing metrics regarding the performance of the platform</li>
+    <li>Adding testing metrics regarding the performance of the platform</li>
 </ul>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- CONTRIBUTING -->
 <h2>Contributing</h2>
-
 <p>Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are <strong>greatly appreciated</strong>.</p>
 
 <p>If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!</p>
 
 <ol>
     <li>Fork the Project</li>
     <li>Create your Feature Branch (<code>git checkout -b feature/AmazingFeature</code>)</li>
     <li>Commit your Changes (<code>git commit -m 'Add some AmazingFeature'</code>)</li>
     <li>Push to the Branch (<code>git push origin feature/AmazingFeature</code>)</li>
     <li>Open a Pull Request</li>
 </ol>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- LICENSE -->
 <h2>License</h2>
-
 <p>Distributed under the MIT License. See <code>LICENSE.txt</code> for more information.</p>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-<a href="https://www.python.org/">Python</a>
+</body>
+</html>
+
+
```

### Comparing `annobee-0.5.9/annobee/cli.py` & `annobee-0.6.0/annobee/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,66 @@
 import argparse
 import requests
 import json
 
 class Annobee:
     def __init__(self, endpoint='http://localhost:5000/api/interpret'):
         self.endpoint = endpoint
-
-    def get_criteria(self, variant):
-        """ Sends a POST request to the Flask API with the variant details. """
+    def get_criteria(self, variant, criteria=None):
+        """ Sends a POST request to the Flask API with the variant details and optional criteria. """
+        payload = {
+            'variant': variant,
+            'genome_build': 'hg38',  # default genome build
+            'adjustments': {}        # default adjustments if any
+        }
+        if criteria:
+            payload['criteria'] = criteria
         try:
-            response = requests.post(self.endpoint, json={
-                'variant': variant,
-                'genome_build': 'hg38',  # default genome build
-                'adjustments': {}        # default adjustments if any
-            })
+            response = requests.post(self.endpoint, json=payload)
             response.raise_for_status()
             return response.json()
         except requests.RequestException as e:
             return {"error": str(e)}
 
 def main():
     parser = argparse.ArgumentParser(description='Genetic Variant Analysis CLI')
-    parser.add_argument('variant', type=str, help='Variant in the format chr-pos-ref-alt, e.g., 1-12345-A-G')
+#    parser.add_argument('variant', type=str, help='Variant in the format chr-pos-ref-alt, e.g., 1-12345-A-G')
+    parser.add_argument('variant', type=str, nargs='?', default="2-199308957-C-T", help='Variant in the format chr-pos-ref-alt, e.g., 1-12345-A-G')
     parser.add_argument('--endpoint', type=str, default='http://localhost:5000/api/interpret', help='API endpoint to use')
-
-    # Add argument options for all individual and aggregate criteria
-    criteria_keys = [
+    
+    # Add arguments for all individual criteria
+    criteria = [
         'functional_consequence', 'hgvsp', 'aa_change', 'transcript_id', 'ucsc_trans_id',
         'exon_number', 'start', 'end', 'rmsk', 'clinvar_clnsig', 'clinvar_clnrevstat',
         'af_esp', 'af_exac', 'af_tgp', 'dbscsnv_rf_score', 'dbscsnv_ada_score', 'gerp_rs_score',
         'metasvm_score', 'sift_score', 'af_vep', 'va_pathogenicity', 'interpro_domain',
         'gene', 'ensembl_gene_id', 'vep_gene_id', 'max_af', 'hgnc_id', 'hgnc_src',
-        'pvs1', 'ba1'
+        'pvs1', 'ba1', 'ps', 'pm', 'pp', 'bs', 'bp', "all"
     ]
-
-    # Add arguments for aggregate criteria
-    aggregate_criteria = ['ps', 'pm', 'pp', 'bs', 'bp']
-    for key in criteria_keys + aggregate_criteria:
-        parser.add_argument(f'-{key}', action='store_true', help=f'Return {key.upper()} criteria')
-
+    for crit in criteria:
+        parser.add_argument(f'-{crit}', action='store_true', help=f'Return {crit.replace("_", " ").upper()} information')
     args = parser.parse_args()
-
-    # Extract variant details from command-line arguments
     try:
         chrom, pos, ref, alt = args.variant.split('-')
         variant = {
-            'CHROM': 'chr' + chrom,
+            'CHROM': str(chrom),
             'POS': int(pos),
             'REF': ref,
             'ALT': alt
         }
     except ValueError:
         print("Error: Variant must be in the format 'chr-pos-ref-alt'. Example: chr1-12345-A-G")
         return
-
     annobee = Annobee(endpoint=args.endpoint)
-    variant_info = annobee.get_criteria(variant)
-
-    if 'error' in variant_info:
-        print(variant_info['error'])
-    else:
-        results = {}
-        info = variant_info.get('INFO', {})
-        # Process and display requested information
-        for key in criteria_keys + aggregate_criteria:
-            if getattr(args, key):  # If the specific criteria flag is set
-                if key in aggregate_criteria:
-                    results[key.upper()] = info.get(key, [])
-                else:
-                    results[key.upper()] = info.get(key, 'Not available')
-
-        print(json.dumps(results, indent=4))
+    results = {}
+    info_requested = False
+    for crit in criteria:
+        if getattr(args, crit):
+            info_requested = True
+            response = annobee.get_criteria(variant, crit)
+            results[crit] = response.get('INFO', {}).get(crit, 'Not available')
+    if not info_requested:
+        response = annobee.get_criteria(variant)  # Get all info if no specific criteria requested
+    print("Client : ",json.dumps(response, indent=4))
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `annobee-0.5.9/annobee.egg-info/PKG-INFO` & `annobee-0.6.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,160 +1,82 @@
-Metadata-Version: 2.1
-Name: annobee
-Version: 0.5.9
-Summary: UNKNOWN
-Home-page: https://github.com/variantAnnotation/annobee-sdk
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
-<!--
-*** Thanks for checking out the Best-README-Template. If you have a suggestion
-*** that would make this better, please fork the repo and create a pull request
-*** or simply open an issue with the tag "enhancement".
-*** Don't forget to give the project a star!
-*** Thanks again! Now go create something AMAZING! :D
--->
-
-
-
-<!-- PROJECT SHIELDS -->
-<!--
-*** I'm using markdown "reference style" links for readability.
-*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
-*** See the bottom of this document for the declaration of the reference variables
-*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
-*** https://www.markdownguide.org/basic-syntax/#reference-style-links
--->
 
 <!-- ABOUT THE PROJECT -->
+<h1>Annobee</h1>
 <h2>About The Project</h2>
 <p>
-    <code>annobee-sdk</code> is designed to analyze genetic variants to determine their pathogenicity using multiple established criteria. It integrates several functions to set various genetic criteria based on evolutionary conservation, allele frequency, and ACMG/AMP standards. The main functionality is centralized in the <code>main.py</code>.
+    <code>annobee</code> is designed to analyze genetic variants to determine their pathogenicity using multiple established criteria. It integrates several functions to set various genetic criteria based on evolutionary conservation, allele frequency, and ACMG/AMP standards. The main functionality is centralized in the <code>main.py</code>.
 </p>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <h3>Built With</h3>
-
 <ul>
     <li><a href="https://www.python.org/">Python</a></li>
 </ul>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
 <!-- GETTING STARTED -->
 <h2>Getting Started</h2>
-
 <p>To get a local copy up and running follow these simple example steps.</p>
 
 <h3>Prerequisites</h3>
-
 <ul>
+    <li>MongoDB: You can download it from <a href="https://www.mongodb.com/download-center/community">MongoDB Download Center</a>.</li>
     <li>Python: Download Python <a href="https://www.python.org/downloads/">here</a>.</li>
 </ul>
 
 <h3>Requirements</h3>
-
 <ul>
     <li>flask==2.0.1</li>
     <li>numpy==1.23.5</li>
     <li>pandas==1.5.3</li>
     <li>requests==2.25.1</li>
     <li>tqdm==4.65.0</li>
 </ul>
 
 <h3>Installation</h3>
-
 <ol>
     <li>Clone the repo
-        <pre><code>git clone https://github.com/variantAnnotation/annobee-sdk </code></pre>
+        <pre><code>git clone https://github.com/variantAnnotation/annobee-sdk.git</code></pre>
     </li>
     <li>Follow to directory where you clone the repo:
         <pre><code>cd annobee-sdk</code></pre>
     </li>
     <li>Install requirements and dependencies:
         <pre><code>pip install -r requirements.txt</code></pre>
     </li>
 </ol>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- USAGE EXAMPLES -->
 <h2>Usage</h2>
 
-<h3> Downloading annobee</h3>
-<pre><code>pip install annobee</code></pre>
+<h3>Starting the Flask API</h3>
+<p>To start the Flask API that the SDK communicates with:</p>
+<pre><code>python app.py</code></pre>
 
 <h3>Command-Line Interface</h3>
 
 <p>To use the <code>annobee-sdk</code>, you can execute the CLI tool with various options to evaluate genetic variant criteria.</p>
 
 <h4> </4>
 
 <h4>Example 1: Evaluate Specific Criteria (PS1)</h4>
-<pre><code>annobee 1-14973-A-AG -ps1</code></pre>
-<p> It returns : </p>
-<pre><code>  { "PS1": 0 }</code></pre>
-
-<h4>Example 2: Evaluate Specific Criterias more then One (PS1, BP7, PP2 etc)</h4>
-<pre><code>annobee 1-14973-A-AG -ps1</code></pre>
-<p> It returns : </p>
-<pre><code>   {
-    "PS1": 0,
-    "BP7": 1,
-    "PP2": 0,
-    "BS1": 0,
-    "PP5": 0
-} </code></pre>
-
-<h4>Example 3: Evaluate All Criteria and pathogenicity</h4>
-<pre><code>annobee 1-14973-A-AG -all</code></pre>
-<p> It returns : </p>
-<pre><code>
-    {"PS1": 0,
-    "PM5": 0,
-    "BP7": 1,
-    "PVS1": 1,
-    "BP1": 0,
-    "PP2": 0,
-    "PS4": 0,
-    "BS1": 0,
-    "BS2": 1,
-    "PM2": 0,
-    "PM1": 0,
-    "PP5": 0,
-    "BP6": 0,
-    "BA1": 1,
-    "PP3": 0,
-    "BP4": 1,
-    "PM4": 1,
-    "BP3": 0,
-    "VA_PATHOGENICITY": "Pathogenic"}
-</code></pre>
+<pre><code>python cli.py 1-14973-A-AG --endpoint http://localhost:5000/api/interpret -ps1</code></pre>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-<h2>Usage as python library</h2>
+<h4>Example 2: Evaluate All Criteria</h4>
+<pre><code>python cli.py 1-14973-A-AG --endpoint http://localhost:5000/api/interpret -all</code></pre>
 
-Here's a simple script that evaluates multiple variants using the `annobee` SDK:
+<h3>Using the Annobee Class in a Python Script</h3>
+<p>Here's an example script that evaluates multiple variants using the <code>Annobee</code> class:</p>
 
-```python
-import json
-from annobee import Annobee
+<pre><code>import json
+from cli import Annobee
 
 def evaluate_variant(annobee, variant, criteria):
     variant_info = annobee.get_criteria(variant)
     results = {}
     
     if criteria == 'all':
         results = annobee.get_all(variant_info)
@@ -196,55 +118,45 @@
     result_three_criteria = evaluate_variant(annobee, variants[0], ['PS1', 'PM5', 'BP7'])
     print(json.dumps(result_three_criteria, indent=4))
 
     # Evaluate all criteria for one variant
     print("\nEvaluating all criteria for one variant:")
     result_all_criteria = evaluate_variant(annobee, variants[0], 'all')
     print(json.dumps(result_all_criteria, indent=4))
-```
+</code></pre>
 
+<h3>Running the Test Script</h3>
+<p>Ensure your Flask API is running and that the <code>cli.py</code> script with the <code>Annobee</code> class is in the same directory or properly installed. Then run the <code>test.py</code> script:</p>
 
+<pre><code>python test.py</code></pre>
+<p>This will print the results of evaluating both one criterion, three criteria, and all criteria for the first variant in the list using the specified endpoint. Adjust the criteria and variant list as needed for your specific use case.</p>
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- ROADMAP -->
 <h2>Roadmap</h2>
-
 <ul>
-    <li>[ ] Adding testing metrics regarding the performance of the platform</li>
+    <li>Adding testing metrics regarding the performance of the platform</li>
 </ul>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- CONTRIBUTING -->
 <h2>Contributing</h2>
-
 <p>Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are <strong>greatly appreciated</strong>.</p>
 
 <p>If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!</p>
 
 <ol>
     <li>Fork the Project</li>
     <li>Create your Feature Branch (<code>git checkout -b feature/AmazingFeature</code>)</li>
     <li>Commit your Changes (<code>git commit -m 'Add some AmazingFeature'</code>)</li>
     <li>Push to the Branch (<code>git push origin feature/AmazingFeature</code>)</li>
     <li>Open a Pull Request</li>
 </ol>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- LICENSE -->
 <h2>License</h2>
-
 <p>Distributed under the MIT License. See <code>LICENSE.txt</code> for more information.</p>
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-<a href="https://www.python.org/">Python</a>
-
-
+</body>
+</html>
```

### Comparing `annobee-0.5.9/setup.py` & `annobee-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 
 setup(
     name='annobee',
-    version='0.5.9',
+    version='0.6.0',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'annobee=annobee.cli:main',
         ],
     },
     install_requires=[
```

