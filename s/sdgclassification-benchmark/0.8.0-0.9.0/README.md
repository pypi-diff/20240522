# Comparing `tmp/sdgclassification_benchmark-0.8.0.tar.gz` & `tmp/sdgclassification_benchmark-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdgclassification_benchmark-0.8.0.tar", max compression
+gzip compressed data, was "sdgclassification_benchmark-0.9.0.tar", max compression
```

## Comparing `sdgclassification_benchmark-0.8.0.tar` & `sdgclassification_benchmark-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1088 2024-02-19 17:47:46.223702 sdgclassification_benchmark-0.8.0/LICENSE
--rw-r--r--   0        0        0    16417 2024-05-03 15:11:58.693366 sdgclassification_benchmark-0.8.0/README.md
--rw-r--r--   0        0        0   330110 2024-05-03 08:26:15.076229 sdgclassification_benchmark-0.8.0/benchmark.csv
--rw-r--r--   0        0        0     1283 2024-05-03 15:14:21.370762 sdgclassification_benchmark-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2594 2024-05-02 21:11:59.048952 sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/Benchmark.py
--rw-r--r--   0        0        0     3347 2024-05-02 20:05:29.569481 sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/Metrics.py
--rw-r--r--   0        0        0      675 2024-04-29 19:31:55.820940 sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/Result.py
--rw-r--r--   0        0        0     1508 2024-05-02 21:05:58.945871 sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/ResultSet.py
--rw-r--r--   0        0        0     2806 2024-05-02 20:53:13.678744 sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/Stats.py
--rw-r--r--   0        0        0      286 2024-05-02 20:57:25.741236 sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/__init__.py
--rw-r--r--   0        0        0      600 2024-04-28 19:18:57.409695 sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/load_benchmark_df.py
--rw-r--r--   0        0        0        0 2024-04-28 19:06:16.132705 sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/py.typed
--rw-r--r--   0        0        0        0 2024-04-11 20:38:32.338056 sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/resources/__init__.py
--rw-r--r--   0        0        0    17361 1970-01-01 00:00:00.000000 sdgclassification_benchmark-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-02-19 17:47:46.223702 sdgclassification_benchmark-0.9.0/LICENSE
+-rw-r--r--   0        0        0    16400 2024-05-10 17:58:06.482700 sdgclassification_benchmark-0.9.0/README.md
+-rw-r--r--   0        0        0   373072 2024-05-10 11:33:25.783424 sdgclassification_benchmark-0.9.0/benchmark.csv
+-rw-r--r--   0        0        0     1253 2024-05-10 17:59:27.015288 sdgclassification_benchmark-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2594 2024-05-10 16:48:13.523881 sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/Benchmark.py
+-rw-r--r--   0        0        0     4357 2024-05-08 07:24:14.725904 sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/Metrics.py
+-rw-r--r--   0        0        0      675 2024-04-29 19:31:55.820940 sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/Result.py
+-rw-r--r--   0        0        0     1508 2024-05-02 21:05:58.945871 sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/ResultSet.py
+-rw-r--r--   0        0        0     2806 2024-05-02 20:53:13.678744 sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/Stats.py
+-rw-r--r--   0        0        0      353 2024-05-08 07:08:47.799605 sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-28 19:18:57.409695 sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/load_benchmark_df.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:06:16.132705 sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/py.typed
+-rw-r--r--   0        0        0        0 2024-04-11 20:38:32.338056 sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/resources/__init__.py
+-rw-r--r--   0        0        0    17293 1970-01-01 00:00:00.000000 sdgclassification_benchmark-0.9.0/PKG-INFO
```

### Comparing `sdgclassification_benchmark-0.8.0/LICENSE` & `sdgclassification_benchmark-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdgclassification_benchmark-0.8.0/README.md` & `sdgclassification_benchmark-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,23 @@
 # Benchmark for SDG Classification<!-- omit from toc -->
 
 The SDG Classification Benchmark is an open and public benchmarking dataset for evaluating and comparing SDG classification models. It consists of text snippets (2 - 3 sentences), which have been carefully labeled and verified by a team of human experts.
 
-**Note**: The benchmarking dataset currently covers SDGs 1, 3 - 7 and 10. We will be expanding the benchmarking dataset to other SDGs in the coming months.
+**Note**: The benchmarking dataset currently covers SDGs 1 - 7 and 10. We will be expanding the benchmarking dataset to other SDGs in the coming months.
 
 ## Table of Contents<!-- omit from toc -->
 
 - [The dataset](#the-dataset)
 - [How to use](#how-to-use)
-  - [With Python](#with-python)
-  - [With other languages](#with-other-languages)
 - [Background](#background)
-  - [Purpose](#purpose)
-  - [Approach](#approach)
-  - [Coverage](#coverage)
-  - [Limitations](#limitations)
-    - [Binary](#binary)
-    - [Non-exhaustive](#non-exhaustive)
-    - [Ignores sentiment](#ignores-sentiment)
-    - [Non-interpretive](#non-interpretive)
 - [Model evaluation](#model-evaluation)
-  - [Disclaimer](#disclaimer)
-  - [Results](#results)
 - [Contributing](#contributing)
-  - [Join the working group](#join-the-working-group)
-  - [Suggestions and feedback](#suggestions-and-feedback)
 - [Credits](#credits)
-  - [Core contributors](#core-contributors)
-  - [List of annotators](#list-of-annotators)
-  - [Text snippets](#text-snippets)
 
-## The dataset
+## The dataset<a id="the-dataset"></a>
 
 You can find the benchmarking dataset here: https://github.com/SDGClassification/benchmark/blob/main/benchmark.csv
 
 The dataset consists of four columns:
 
 - `id`: Unique identifier for every text (MD5 hash)
 - `text`: Text snippet (2 - 3 sentences)
@@ -48,15 +31,15 @@
 03e9759  Not only does this have potentially negative e...    7  False
 04f6c7f  If too much water is stored behind the reservo...    7  False
 b87a4f8  Energy efficiency targets are now in place at ...    7   True
 12e3f54  Data over the last 30 years suggests that, had...    7   True
 135ea60  Large areas of about 500 000 km2 between Mumba...    7  False
 ```
 
-## How to use
+## How to use<a id="how-to-use"></a>
 
 ### With Python
 
 We have created the Python package [sdgclassification-benchmark](https://pypi.org/project/sdgclassification-benchmark/) to make it easy to benchmark SDG classification models written in Python.
 
 First, install the package: `pip install sdgclassification-benchmark`
 
@@ -128,15 +111,15 @@
 df <- read.csv("https://raw.githubusercontent.com/SDGClassification/benchmark/main/benchmark.csv")
 ```
 
 You can then classify the `text` in each row of the dataset and compare your model's predictions with the true label.
 
 You can [find short descriptions about each of the columns in the dataset here](#the-dataset).
 
-## Background
+## Background<a id="background"></a>
 
 ### Purpose
 
 There exist a number of different models and approaches for classifying texts with respect to the Sustainable Development Goals (SDGs). Refer to [this list](https://globalgoals-directory.notion.site/PUBLIC-List-of-AI-driven-SDG-Classification-Initiatives-fe4770a173194e0b980f95b330a8a83b) for a (non-exhaustive) overview of different SDG classifiers and initiatives.
 
 To further advance the field of SDG classification, it is important that we understand the strengths and weaknesses of the available tools.
 
@@ -150,19 +133,20 @@
 
 To ensure a robust benchmarking dataset, the texts for each SDG were independently annotated by several human experts. For most texts, the annotations made by these experts were identical. For some texts, however, there initially were disagreements between the annotations. These disagreements were resolved through discussion between the experts until consensus was reached.
 
 In some cases, consensus was reached by making slight modifications to a text in order to remove ambiguity.
 
 ### Coverage
 
-The dataset currently covers SDGs 1, 3 - 7 and 10.
+The dataset currently covers SDGs 1 - 7 and 10.
 
 | SDG                                | Number of texts | Texts with SDG | Texts without SDG |
 | ---------------------------------- | --------------: | -------------: | ----------------: |
 | SDG 1: No poverty                  |              77 |             27 |                50 |
+| SDG 2: Zero hunger                 |              69 |             45 |                24 |
 | SDG 3: Good health and well-being  |              76 |             28 |                48 |
 | SDG 4: Quality education           |              82 |             43 |                39 |
 | SDG 5: Gender equality             |              69 |             35 |                34 |
 | SDG 6: Clean water and sanitation  |              85 |             48 |                37 |
 | SDG 7: Affordable and clean energy |             100 |             50 |                50 |
 | SDG 10: Reduced inequalities       |              61 |             32 |                29 |
 
@@ -192,63 +176,65 @@
 
 #### Non-interpretive
 
 Texts were only assigned to a given SDG, if the text directly addressed that SDG and/or its targets. "We are subsidizing the costs of silicon" would not qualify for SDG 7, even though silicon is one of the materials for making photovoltaic cells and reduced cost of silicon might have indirect benefits for the expansion of solar energy.
 
 We ignored indirect relevance in texts because correct assessments would require enormous thematic expertise, and even then such interpretations would often remain highly subjective and controversial.
 
-## Model evaluation
+## Model evaluation<a id="model-evaluation"></a>
 
 ### Disclaimer
 
 Several models have been tested against this benchmark. The results can be used as one criterion when evaluating models. Importantly, there are a range of other important aspects to consider that are not tested by this benchmark, such as cost, speed, and coverage of SDG targets. In addition, many models have been developed and optimized for domain-specific use cases (e.g. analyzing policy documents, research articles or websites) and their performance on this benchmark may not be representative of their performance on their domain-specific use case.
 
 ### Results
 
 The table below shows the accuracy (in percent) of models tested against this benchmark. Clicking on one of the models provides additional details, including metadata about the model, F1 score, precision and recall.
 
 <!-- evaluation table begin -->
 
-| Model                                                                                                                  | Average | SDG 1 | SDG 3 | SDG 4 | SDG 5 | SDG 6 | SDG 7 | SDG 10 |
-| :--------------------------------------------------------------------------------------------------------------------- | ------: | ----: | ----: | ----: | ----: | ----: | ----: | -----: |
-| [AFD SDG Prospector](https://github.com/SDGClassification/benchmark/tree/main/evaluations/sdg-prospector/)             |      91 |    95 |    91 |    95 |    81 |    92 |    95 |     87 |
-| [Aurora SDG](https://github.com/SDGClassification/benchmark/tree/main/evaluations/aurora-sdg/)                         |      82 |    74 |    78 |    83 |    90 |    85 |    87 |     77 |
-| [Global Goals Directory](https://github.com/SDGClassification/benchmark/tree/main/evaluations/global-goals-directory/) |      84 |    90 |    90 |    78 |    74 |    87 |    91 |     80 |
-| [JRC SDG Mapper](https://github.com/SDGClassification/benchmark/tree/main/evaluations/sdg-mapper/)                     |      77 |    82 |    84 |    70 |    75 |    73 |    86 |     70 |
-| [Meta Llama 2 70B](https://github.com/SDGClassification/benchmark/tree/main/evaluations/llama-2/)                      |      89 |    88 |    93 |    90 |    93 |    85 |    92 |     79 |
-| [Meta Llama 3 70B](https://github.com/SDGClassification/benchmark/tree/main/evaluations/llama-3/)                      |      88 |    77 |    86 |    85 |    91 |    92 |    91 |     92 |
-| [OpenAI GPT-3.5 Turbo](https://github.com/SDGClassification/benchmark/tree/main/evaluations/openai-gpt-3/)             |      83 |    65 |    82 |    80 |    87 |    91 |    90 |     87 |
-| [OpenAI GPT-4 Turbo](https://github.com/SDGClassification/benchmark/tree/main/evaluations/openai-gpt-4/)               |      87 |    75 |    86 |    84 |    88 |    92 |    92 |     92 |
+| Model                                                                                                                  |   Average |   SDG 1 |   SDG 2 |   SDG 3 |   SDG 4 |   SDG 5 |   SDG 6 |   SDG 7 |   SDG 10 |
+|:-----------------------------------------------------------------------------------------------------------------------|----------:|--------:|--------:|--------:|--------:|--------:|--------:|--------:|---------:|
+| [AFD SDG Prospector](https://github.com/SDGClassification/benchmark/tree/main/evaluations/sdg-prospector/)             |        90 |      95 |      87 |      91 |      95 |      81 |      92 |      95 |       87 |
+| [Aurora SDG](https://github.com/SDGClassification/benchmark/tree/main/evaluations/aurora-sdg/)                         |        82 |      74 |      83 |      78 |      83 |      90 |      85 |      87 |       77 |
+| [Global Goals Directory](https://github.com/SDGClassification/benchmark/tree/main/evaluations/global-goals-directory/) |        84 |      90 |      80 |      90 |      78 |      74 |      87 |      91 |       80 |
+| [JRC SDG Mapper](https://github.com/SDGClassification/benchmark/tree/main/evaluations/sdg-mapper/)                     |        76 |      82 |      71 |      84 |      70 |      75 |      73 |      86 |       70 |
+| [Meta Llama 2 70B](https://github.com/SDGClassification/benchmark/tree/main/evaluations/llama-2/)                      |        88 |      88 |      84 |      93 |      90 |      93 |      85 |      92 |       79 |
+| [Meta Llama 3 70B](https://github.com/SDGClassification/benchmark/tree/main/evaluations/llama-3/)                      |        88 |      77 |      90 |      86 |      85 |      91 |      92 |      91 |       92 |
+| [OpenAI GPT-3.5 Turbo](https://github.com/SDGClassification/benchmark/tree/main/evaluations/openai-gpt-3/)             |        84 |      65 |      93 |      82 |      80 |      87 |      91 |      90 |       87 |
+| [OpenAI GPT-4 Turbo](https://github.com/SDGClassification/benchmark/tree/main/evaluations/openai-gpt-4/)               |        88 |      75 |      93 |      86 |      84 |      88 |      92 |      92 |       92 |
 
 <!-- evaluation table end -->
 
 More models will be added in the future.
 
 Have you benchmarked a model that is not yet in our list? Please open an issue and share the results with us, so that we can add the model to the table above.
 
-## Contributing
+## Contributing<a id="contributing"></a>
 
 ### Join the working group
 
 The [core contributors](#core-contributors) meet regularly to improve and expand this benchmarking dataset. If you want to join us, please reach out to [finn@globalgoals.directory](mailto:finn@globalgoals.directory).
 
 ### Suggestions and feedback
 
 This benchmarking dataset is a living document and we will continue to make adjustments and improvements based on feedback. Please open an issue to share your ideas, suggestions, and feedback.
 
-## Credits
+## Credits<a id="credits"></a>
 
 ### Core contributors
 
 The benchmarking dataset has been created by the Benchmarking Working Group of the [SDG Classification Expert Group](https://sdg-ai.org/). Core contributors are Finn Woelm, Meike Morren, Steve Borchardt, Jean-Baptiste Jacouton and Gib Ravivanpong.
 
 ### List of annotators
 
 We especially thank our annotators for making this project possible.
 
+- **SDG 1**: Steve Borchardt, Meike Morren, Finn Woelm
+- **SDG 2**: Steve Borchardt, Meike Morren, Gib Ravivanpong, Finn Woelm
 - **SDG 3**: Steve Borchardt, Meike Morren, Finn Woelm
 - **SDG 4**: Steve Borchardt, Meike Morren, Finn Woelm
 - **SDG 5**: Steve Borchardt, Meike Morren, Gib Ravivanpong, Finn Woelm
 - **SDG 6**: Steve Borchardt, Meike Morren, Gib Ravivanpong, Finn Woelm
 - **SDG 7**: Steve Borchardt, Jean-Baptiste Jacouton, Gib Ravivanpong, Finn Woelm
 - **SDG 10**: Steve Borchardt, Jean-Baptiste Jacouton, Meike Morren, Gib Ravivanpong, Finn Woelm
```

### Comparing `sdgclassification_benchmark-0.8.0/benchmark.csv` & `sdgclassification_benchmark-0.9.0/benchmark.csv`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,83 @@
 94f2c0b,"For the purposes of the SHI scheme, “formal sector” refers to enterprises that employ more than ten individuals, a definition which excludes a large proportion of the population. Total expenditure increased steadily from ETB 0.1 million in 2012/13 to ETB 47.9 million in 2015/16. Management and administration initially accounted for the majority of expenditure but the system development’s share of spending increased after 2014/15 and accounted for over 57% of total SHI expenditure in 2015/16.",1,False
 57ed03a,"The Innocenti Research Centre (formally known as the International Child Development Centre) generates knowledge and analysis to support policy formulation and advocacy in favour of children, acts as a convener and catalyst for knowledge exchange and strategic reflections on children’s concerns, and supports programme development and capacity-building. The Centre’s publications represent contributions to a global debate on child rights issues, and include a range of opinions. For that reason, the Centre may produce publications that do not necessarily reflect UNICEF policies or approaches on some topics.",1,False
 3d656dc,"They differ from the usual ones employed by trade modellers of developing country policies in that they are based on direct domestic-to-border price comparisons rather than (as with the GTAP dataset) on applied rates of import tariffs and other key border measures. A first attempt to exploit that new database was recently undertaken to assess the relative impacts on national, regional and global poverty as well as inequality of agricultural and non-agricultural trade policies at home and abroad. This chapter summarizes some of the working papers that have emerged from that research project (see www.worldbank.org/ agdistortions).",1,False
 ac71db1,"Rather, what is needed is a set of marketing policies and institutions that connect farmers to markets by reducing their marketing costs and risks (IFPRI, 2007). Similarly, this analysis strongly confirms the importance of better market integration and investment in rural infrastructure to help reduce transport and energy costs thereby better transmitting the opportunities created by market opening to those regions. Today, food and other agricultural products are sourced globally as much as manufactured products and the expanding markets for agro-food products are opening up new opportunities for developing countries (see Box 4). Participation in regional or global agro-food value chains allows developing country producers to overcome the limits imposed by their small domestic markets. It provides them access to more vibrant markets, allowing them to upgrade their production processes and improve the quality and value-added of their products. Although the strong growth performance of recent years has been mainly attributed to Zambia’s booming mining sector (copper is the country’s single largest foreign exchange earner), agriculture is the most dynamic component of Zambia’s export economy and is the main driver of export diversification.",1,False
 fd58c75,"Investments in education help to reduce the intergenerational transmission of poverty. Although the share of the people who are educated varies greatly among the Asia Pacific LDCs, for both women and men, the poorest are less likely to be educated. The gender gap is also considerable. The differences in educational attainment between the ultra poor and the subjacent poor are large, with the poorest the least educated.",1,True
 f85780b,"The stigma attached to transgender people, men who have sex with men, and sex workers has resulted in their social exclusion (Winter, 2012). In South and South-West Asia, transgender people in particular lack recognition. Being held in low esteem, they find it difficult to pursue education, enter a profession or set up a business.",1,False
 f172dff,"Societies will have to adjust to increasing proportions of older persons in their population. In this regard, in developed countries, concerns about rising costs of health care (partially related to ageing) and viability of pension systems are already at the centre of policy debates. In many developing countries, population ageing is occurring in an accelerated fashion and life expectancy has risen considerably.",1,False
+2923a3e,"She would also like to thank the guest bloggers and other contributors to the SWAC @ Expo Milano website who engaged in discussions on the state and prospect of women's empowerment and gender equality in West Africa over several months, sharing their ideas and experiences and raising challenging questions. She has conducted research, co-ordinated policy analysis and published on gender, migration, conflict, peace and security, land reform and regional integration issues. She has also designed and co-ordinated the implementation of human resources and organisational development-related projects and processes in the areas of: job evaluation, organisational design, diversity and change management. Previous roles include: UNV Programme Officer at the UNDP Senegal Office, Policy Analyst at the Sahel and West Africa Club Secretariat of the OECD, and Human Resources Manager and OD Consultant at the International Institute for Environment and Development (IIED).",2,False
+79df6ac,"A gendered approach to environmental assessment also examines the ways environments and environmental relationships shape, create and sustain gender norms. What are the social costs and consequences of differential gendered environmental relationships? And what is the dynamic relationship between environmental conditions and changes and gender inequality?",2,False
+2f2e3ee,"However, line ministries have greater influence in setting NTBs. They are generally more protectionist and influenced by interest groups. Hence trade policy is a continuous battleground, and a change of key ministerial personalities can easily result in a more protectionist trade policy regime. This is the crux of Indonesia’s trade policy challenge: no minister or agency has control over the full array of trade policy instruments, and is able to adopt an economy-wide public interest viewpoint.",2,False
+86db095,"The main change is due to the need to allocate programmes under Inspection Services and Marketing and promotion into new sub-categories. In particular the inspection and control programmes implemented by the inspection agency SENASICA include inspection, pest and diseases and input components. Good budgetary information for the allocation of this expenditure to different sub-categories was not available and allocation was provisionally done in equal amounts. New information is being collected with the view of improving this allocation in the next monitoring cycle.",2,False
+9fcc296,"The ability to monitor progress at the school level in a comparable manner was a major achievement and was very helpful in linking funding with performance improvements of the education system. Another important direction was the substantial increase in conditional cash transfer programme Bolsa Familia (initially, Bolsa Escuola) which created both incentives and the means for poor parents to send their children to school (De Mello and Hoppe, 2005, OECD, 2011). This has recently received much attention, with enrolment in vocational training more than doubling since the early 2000s.",2,False
+65c3ef2,"The regional average dependency ratio (i.e. the ratio of people younger than 15 to the working-age population in the 15-64 year range) totalled 74.7% (UNFPA, 2015). An ever increasing and younger population is a distinctive feature of West Africa: the total population is projected to almost double and approach 600 million by 2050 (OECD/SWAC, 2013). From 1950 to 2010, the percentage of urban dwellers increased from 9% to 41% and this figure is projected to soar to 67% by 2050 (Moriconi-Ebrard, Harre and Heinrigs, 2016, OECD/SWAC, 2013). Urban growth concerns old and new towns, larger cities and smaller and rural centres alike (Ibidem).",2,False
+2d4e1de,"In many developing countries, a significant number of poor families face poverty, hunger, food insecurity and malnutrition, which intensify with adverse biophysical growing conditions and poor socio-economic infrastructure (Wani, etal., Crop production, which is vital to global food security, is already being affected by climate change, more so in impoverished communities. It has been predicted that over the next decades, billions of people, especially those living in developing countries, will face water and food shortages, and greater risks to health and life because of climate change.",2,True
+f932110,"These searchable on-line databases and their annual reporting summaries are valuable tools for federal and state science managers and scientists. In addition, CRIS has been a critical resource for retrospective assessments of the economic impacts of agricultural research. Using data that measure research resource flows to specific subject areas and specific geographic areas, and linking them to subsequent changes in farm productivity, economists have been able to conduct cost-benefit analysis of public investments in agricultural research. A summary of the findings from these studies is given in Chapter 7.",2,True
+993b964,"This is where measures such as compensation and adjustment assistance come into play. This is sometimes interpreted (if not criticised) as an ideological position representing the entrenched philosophy of economic liberalism (or neoliberalism). Yet, there are very good practical reasons behind that principle. Three thoughts are particularly relevant.",2,False
+82328b3,"Such scenarios may constitute “extreme events”, with a low probability but severe consequences if the event happens. A more likely scenario is that a particular trading partner may block or impede trade temporarily, with implications for the prices that an importing country is obliged to pay. For example, India cut off rice exports to Bangladesh in 2007 in order to lower prices on its domestic market (Dorosh and Rashid, 2012).",2,True
+6a26abc,"Obligations to partners within the Council for Mutual Economic Assistance had to be met before product could be sold to the convertible currency area. Imports had to proceed through an extensive system of quotas and licenses. Additionally, Viet Nam faced a trade embargo with the United States that was only lifted in 1994 (McCaig and Pavcnik, 2013). Permission for private as well as SOEs to establish direct links with foreign markets was given in 1991.",2,False
+7b7428c,"These figures most likely underestimate the contribution of off-farm earnings because they capture only the income coming from activities integrated from the accounting standpoint either fully or partly within the farm business. However, studies on rural diversification indicate that the majority of alternative enterprises of agricultural households are financially and structurally independent of the farm business (OECD, 2009e). For example, around 20% of living expenses of those households involved in dairying and sheep and beef farming originate from off-farm income (MAF, 2009e).",2,True
+274111c,"On the other hand, others such as P. Veltz see the territorial result of post-Ford ist regulation modes combining the uncertainty of the economic situation and flexibility of the job market. Californian geographers such as A. Scott or M. Dear insist on relations between functional and social mutations of very large cities and new forms of urban territoriality."" Both are independent of the level of urbanisation of the territory considered. Table 3.2 presents the indices for Togo and Nigeria. In Togo, Lome was the primate city for the years 1950, 1970 and 2010. In Nigeria, Ibadan held this position in 1950 and 1960, and since then Lagos.",2,False
+eacb981,"Binding biofuel mandates also risks to increase price volatility on agricultural world markets. International trade in ethanol is subject to significant import tariffs, and climate-related standards are already in use on some biofuels and may become increasingly important in the future. In order not to act as trade barriers that discriminate between domestic and foreign products the development and application of internationally harmonised standards warrants close attention.",2,True
+51c6511,"The government’s efforts to develop modern large-scale production should be complemented by the efforts to integrate small-scale producers into agricultural markets as well as to diversify rural incomes. Large state agencies operate on the grain, machinery leasing, and agricultural credit markets. Their primary function is to implement support programmes, but they are also empowered to undertake commercial operations and as such enjoy substantial market power.",2,True
+0d27eec,"Credit resources could be re-directed to support long-term investment and increasingly allocated to well-specified innovation, environmental, and infrastructure projects. Consider a gradual downsizing of concessional loans for working capital to commercial producers. Enhance criteria for loan eligibility to better screen out borrowers that would have invested without support.",2,False
+b2a55ca,"However, the CAP 2014-20 offers more flexibility to member states to re-introduce commodity-specific and output-linked measures. A better alternative would be for member states to focus support on measures to improve the long-term productivity, profitability, sustainability and competitiveness of the sector. The ""Plan to Create Vitality for Agricultural, Forestry and Fishery Industries and Local Communities” aims at revitalising the agricultural sector in view of significant drops in output and farming incomes over the past two decades.",2,True
+151c9d9,"Special thanks go to Thomas Chalaux and Clara Garcia for statistical support and Nadine Dufour and Mercedes Burgos for editorial assistance. The scale of the ongoing transition is highlighted by government plans to grant urban residential status to 100 million rural migrants by 2020. This structural adjustment process can deliver substantial opportunities for the rural economy and China as a whole, but entails major challenges calling for continued reform efforts.",2,False
+89fc1ad,"That role includes funding for research and development, but it also includes the design of a balanced system of intellectual property rights. This report shows that across all countries covered in this report expenditures on research and development represent a relatively small share in the transfers to the agricultural sector. Increased public and private investment in research and development, including extension and advisory services, could be targeted to increase productivity growth and address challenges associated with climate change and improved management of soil and water resources.",2,True
+395d84c,"The rebound in growth is expected to be more rapid in the developing countries and initially tepid and fragile in the OECD area and involving a longer transition period. Once the transition to sustainable gains is reached, the EU and US economies are expected to grow by 2% and 2.5% per annum, respectively to 2019, and with faster growth in some other OECD countries such as Korea, Turkey and Australia. Among the developing countries, the leading Asian economies have fared better than most and lead the world economic recovery.",2,False
+dcb3a8d,"In 2011, a federal programme PRONATEC was launched and now covers 8 million students. Since 2013, it includes a component targeted to rural youngsters: PRONATEC Countryside. For example, in university education, the number of agricultural courses for bachelor degrees reached 830 in 2011, a six-fold increase over 1991, which covers only full-time studies, and does not include distance courses or MBAs (Table 5.1).",2,False
+b654de4,"Finally, New Zealand witnessed rising MPS, but from a very low level and almost entirely due to falling poultry world prices in combination with an appreciation of the currency relative to the US dollar. Per cent changes of nominal values expressed in national currency. The statistical data for Israel are supplied by and under the responsibility of the relevant Israeli authorities. The use of such data by the OECD is without prejudice to the status of the Golan Heights, East Jerusalem and Israeli settlements in the West Bank under the terms of international law.",2,False
+bf441ff,"Through increasing market size, suitable infrastructure may also promote competition and the adoption of productivity-enhancing technologies. Given such positive externalities, there is often an argument for government provision. Nevertheless, it is also important that framework conditions are designed in a way that encourages private sector infrastructure investment. Without a sufficient network of roads and ports, improvements in farm productivity could result in lower local prices for a commodity at the same time as there is inadequate supply in other provinces.",2,True
+f700809,"In the model ECIRS payments are then triggered and the representative mixed crop and livestock farm receives the equivalent to the average receipt of ECIRS in 2007-08 (AUD 37 000)l0. On the other hand, the model assumes that ECRP also triggered under the same circumstance, but it is paid to the farmer only if the realized income is below the level set by income test criteria (AUD 62 per fortnight). The level of the ECRP is chosen at the average receipt of ECRP per recipient in 2007-08 (AUD 13 045).",2,True
+2ee7391,"If land owners are not willing to transfer the land and leave it, the investor does not have the right to lease the land and cany out its investment.” It should be noted that although the government discourages slash and burn cultivation, i.e. shifting cultivation, such a system can be sustainable and deliver environmental goods in areas where demographic pressure is relatively low. An approach tailored to the characteristics of each geographical area should thus be taken.",2,True
+db02548,"Promoting niche markets through denomination of origin, eco-labelling, fair trade, organic and slow food initiatives, geographic indication, globally important agricultural heritage systems, and one-village-one-product initiatives may be particularly useful. Therefore, PGRFA include both farmers' varieties/landraces and modern cultivars of staple crops as well as NUS.The development and implementation of policies are a key component in promoting NUS/FSF into agricultural production systems (FAO, 2015a). Following this, the Rome Declaration on Nutrition included the call to ""Promote the diversification of crops including underutilized traditional crops, more production of fruits and vegetables, and appropriate production of animal-source products as needed, applying sustainable food production and natural resource management practices"" (FAO, 2014a). These commitments have become even more compelling with the imperative of achieving the SDGs by 2030. In general, in developing countries, the attainment of this objective even for staple crops, and more so for NUS, remains a seemingly intractable problem.",2,True
+e5db980,"But it suggests that rather than holding national stocks, it would be better to develop regional stocks or make food reserve agreements. And in March 2004, the ASEAN+3, which includes China, Japan, and the Republic of Korea, expanded this as the East Asia Emergency Rice Reserve. This reserve has been used to provide relief to victims of floods in Indonesia and Cambodia, to victims of volcanic eruption and mud slides in the Philippines, and to victims of Cyclone Nargis in Myanmar.",2,True
+7a6aa94,"The main conditions for forming a successful PPP include: common objective, mutual benefits, complementarity of human and financial resources, clear institutional arrangements, good governance, transparency and public leadership. The new legal framework for PPPs in agriculture, to be refined in two circulars that MARD is developing, should thus clearly state the respective roles and responsibilities of the public and private sectors. There are a large number of cases, e.g. in providing financial support to agriculture or in food safety regulatory regime, in which co-ordination between various agencies both at the central government level and between central and local governments is weak.",2,True
+b8f83b7,"In 2014, 85% of procurement funds were used in this manner (CONAB-PAA, 2014). A significant share of PAA procured supplies (34% in 2014) is used for the school meal programme. In 2009 the National School Meal Program (PNAE) required public schools to allocate at least 30% of food expenditures to direct purchases from family farmers. Since 2011 under the Brazil without Extreme Poverty Plan, PAA procurement is specifically targeted to the 16 million persons living in extreme poverty with monthly income below BRL 70. In 2014, nearly 24 000 PAA suppliers, or 47%, fell within this category. The National Program for Biodiesel Production and Use (PNPB), which contains special provisions for family farmers, was launched by the Brazilian Government in 2005.",2,True
+8246dd1,"A broader analysis of the financial sector in Myanmar can be found in Chapter 6 on financial sector development. While agriculture employs up to 61.2% of the workforce, only 1-3% of the volume of formal bank loans is extended to the agricultural sector. Although its lending has increased in recent years, it provides only short-term seasonal loans that cover a limited share of the production costs and continues to prioritise rice farmers. Other formal lenders have been unable to fill the gap.",2,True
+2b9764a,"The basic model also assumes competition in the market for the commodity and the absence of any other market distortions. A general result is that the main effect of a market distortion in this context is to change the distribution of research benefits, with comparatively small effects on the total benefits. Similar results apply to the other types of extensions to the basic model that may be introduced to allow for multiple markets or proprietary technology.",2,False
+b0649f2,"An alternative is that funding could partly derive from subnational governments, but this would need to be coupled with tax reforms that boost subnational government income such as a possession-based rather than a transaction-based property tax (OECD, 2013a). Even if farmers manage to scale up their land holdings through renting in operating rights to farmland and attract suitable labour, poor access to finance may limit farm investment and mechanisation. A large problem for farmers in many developing countries is a lack of collateral.",2,True
+e592751,"Particular attention is often paid to sustainable, or efficient, water use. Because the agriculture sector demands significant amounts of fresh water, a number of policies in both developing and developed countries target the efficient use of irrigation water. A strong call to recognise the importance of improving the efficiency of water and soil use in a sustainable manner by the agricultural sector was made by G20 leaders and G20 Agricultural Vice Ministers in May and June 2012.",2,True
+b937464,"The complexity of agricultural ecosystems makes it difficult to accurately measure, quantify and monitor the biogeochemical and natural resource flows that underlie agriculture. There is a lack of analytical tools and mechanisms readily available to measure, value and account for resource use and loss in agricultural production systems. Several efforts are under way to remedy this situation, for example within the framework of the World Overview of Conservation Approaches and Technology (WOCAT) and the Land Degradation Assessment in Drylands (LADA) project.",2,True
+bc5912d,"Scenarios emphasizing improvements in end-use efficiency tend to meet sustainable development goals, such as ensuring (almost) universal access to electricity, maintaining air quality, and limiting global average temperature increases. However, if efficiency gains turn out to be small, the world will become highly dependent on rapidly improving innovation and increasing the supply of “clean” energy. Another insight is that sustainable development pathways have been devised that exclude nuclear power, and carbon capture and storage (and its bioengineering variants), technologies that face great sociopolitical and technical challenges.",2,False
+034d2ee,"North Cameroon had an estimated 9 306 km of roads in 2010,8% of them paved, and a density of 0.057 km/km2. Unpaved roads link areas of production to urban consumption centres. The dynamics of market creation have determined a spatial configuration that depends on the quality of the road network, unpaved vs. paved roads.",2,False
+33b482e,"Their impacts on nutrition may also vary according to the economic and nutritional context of the country. Agricultural policies that provide appropriate incentives and clear market signals that promote the sustainable intensification and diversification of production will improve nutrition more effectively. On the other hand, the Common Agricultural Policy in European countries actually raises consumer prices of sugar and dairy products relative to prices of fruits and vegetables and thus may have a small positive impact on the overall healthiness of European diets (Capacci eta/., 2012).",2,True
+5d5f9ae,"There are also structural challenges, such as the domination of subsistence-oriented producers in key product sectors, the weak integration of domestic food chains, and difficult access to external markets. Qualified labour is scarce, commercial credit markets are narrow, and much of the credit resources, especially for long-term investment, depend on state provision. Public resources should be shifted to remove significant deficiencies in transport infrastructure, water and land management, plant and animal health and food safety systems, information, research, education, and knowledge dissemination. Policy reform should not only include a stronger emphasis on the provision of public goods, but would also require developing new policies to manage risks in agriculture and promoting sustainable use of agricultural resources.",2,True
+9e9b0c2,"The delegation used sport as a tool to unite and engage with the community. In partnership with the One World Play Project and Chevrolet, it donated over 11,000 footballs and hosted a friendly youth football match and other organized sporting activities. During the trip, the delegation met with representatives of the United States Agency for International Development (USAID), and with the Malawian Ministries of Lands, Housing and Urban Development, Health, Youth and Sports Development, and Agriculture, Irrigation and Water.",2,False
+0c538c4,"While rice fills the stomach, a rice-dominated diet provides only low to zero amounts of protein, amino acids and essential micronutrients, which can be found, for example, in pulses, fruits, nuts, tubers, vegetables, fish, meat and edible insects. The dependency on rice leads to insufficient intake of nutrient-rich foods, which in turn leads to a significant 'nutrition gap'. Dietary diversity is low when there is high consumption of cereals, mainly rice, but relatively low intakes of vegetables, fruits and pulses which are known to be rich in micronutrients and fibre.",2,True
+3f96fe9,"Under these agreements, the centres recognize the authority of the Governing Body of the Treaty to provide policy guidance relating to their ex situ collections (i.e. collections of seeds stored in genebanks). From 1 February 2008, the Centres have been transferring all plant genetic resources for food and agriculture they hold in trust - using the SMTA. They have also helped countries recover from natural disasters such as Hurricane Mitch which struck Honduras and Nicaragua. A recent study showed that of the more than one million seed samples distributed over the past 10 years, the vast majority (80 per cent or more) went to universities and national agricultural research systems where scientists are developing new crop varieties that give higher yields, have improved nutritional value, use less water, need lower amounts of fertilizers, and have natural resistance to pests, diseases and climatic vagaries such as droughts and floods.",2,True
+f12940a,"To feed an additional two billion people by 2050, food production will need to increase by half globally (FAO, SOFI, 2017). Increasing the production of traditional staple crops is unlikely to meet the increasing demand, in major irrigated wheat, rice and maize systems, yields appear to be near 80 percent of the yield potential. The second challenge is the nutrition gap between what foods are grown and available, and what foods are needed for good health. This requires increasing the availability and access to the nutritious foods necessary for a healthy diet.",2,True
+989d7ad,"The recent food crisis and slow progress towards the achievement of the Millennium Development Goal of eradicating hunger have highlighted the wide disparities in technologies used and productivity achieved in different agricultural systems. While input and resource-intensive agriculture is the norm in many developed and middle-income developing countries, many developing countries continue to rely on low-input, low-productivity agriculture. Even as the former group of countries need to shift towards less intensive and more environmentally sound methods, farmers in many developing countries would benefit from greater input use.",2,True
+693fd6c,"Among the most vulnerable will be those who depend on agriculture for their livelihood and income, particularly smallholder producers in developing countries. In the absence of climate change, and with continuing economic progress, most regions are projected to see a decline in the number of people at risk of hunger by 2050. The increase in the number of poor would be biggest in sub-Saharan Africa, partly because its population is more reliant on agriculture.",2,True
+dcda796,"A recent study by the RIO+ Centre and the Food, Agriculture and Natural Resources Policy Analysis Network which looks at the complex relationship between gender and climate-smart agriculture (CSA) emphasizes the need for both gender-smartness and people-smartness in achieving CSA's aims of food security, higher farmer incomes, and low-carbon agricultural practices (Perch 2015). Nevertheless, food security, as the World Health Organization (WHO) points out, is ""a complex sustainable development issue, linked to health through malnutrition, but also to sustainable economic development, environment and trade"" (WHO 2016a). Greater gender equality is essential to achieve global food security (Carliez 2015, FAO and ADB 2013, Sachs 2013). Food sovereignty is ""more fluid and nuanced than the concept of food security"" (Sachs 2013).",2,True
+a5ec28c,"The most recent data compiled by UNICEF (2013) shows that in 82 out of 95 developing countries for which data are available the prevalence of child underweight is higher in rural areas than in urban areas. Guha-Khasnobis and James (2010) found a prevalence of adult underweight of around 23 percent in the slum areas of eight Indian cities, while the prevalence in rural areas in the same states was close to 40 percent. It is technically a form of undernutrition (UNSCN, 2010), but is often referred to separately because it can coexist with adequate or excessive consumption of macronutrients and carries health consequences that are distinct from those associated with stunting.",2,True
+5c8d3f5,"Investment in R&D has resulted in high growth in Brazilian scientific knowledge, particularly within tropical agriculture. Embrapa has provided comprehensive recommendations ranging from how to correct acid soils and low fertility, the development of varieties that are adapted to the low latitudes and higher temperatures of tropical environments, and to pest and disease control and production systems. Universities also produce high level research in areas complementing Embrapa’s activities, such as in nutrition, health and the environment. This mechanism facilitates participation in global or regional agricultural research networks. Embrapa is also actively collaborating on technology transfer and adaptive research with developing economies, with an emphasis on tropical areas in Latin America, the Caribbean and Africa.",2,True
+2f56281,"This argument is supported in the report by a number of case studies that illustrate that, although macro-economic policy reforms have had positive effects on agriculture in some parts of Africa, the overall impact of the reforms has been slower and less dramatic than could have been expected. The main reason for the reforms' restricted impact is that the constraints to achieving sustainable agricultural productivity and increasing yields lie both on and off the farm. Hence, in many cases, transportation, trade, and macroeconomic policies have stronger effects on farmer and trader incentives than do agricultural sector policies, a point that underscores the need for better policy coordination across ministries. Strategies should therefore focus on transforming the weak points along the food system as a whole, and avoid too narrow a focus on farming.",2,True
+f0b6607,"This might be particularly true in Indonesia where large fertiliser subsidies are channelled through fertiliser suppliers and not provided to farmers directly. In light of expressed government objectives, these proposals highlight policy options that are potentially more effective and efficient than some existing policy measures. Food security would be greatly enhanced by making agriculture a more attractive sector for investors.",2,True
+fe37b4a,"Fertiliser subsidies remain by far the most important programme through which the government provides budgetary support to agriculture. This subsidy is received indirectly by farmers as is channelled through fertiliser companies. These companies are responsible for lowering the price of their final product, which in turn benefits farmers (OECD, 2013b). To ensure the success of the programme, beneficiaries also receive technical guidance from a local agriculture extension officer. The giant is based on a proposal prepared by groups of farmers. The Indonesian government, through the Raskin Programme, buys a given percentage of the total output of rice produced by small-scale farmers.",2,True
+50d2fe2,"Fanning units that showed dominance in specific products were combined to form totals for field crop products, horticultural products and animals and animal products. Farmland plus nature conservation land plus forestry land plus other. Source: Development Bank of Southern Africa. Statistics SA, Census of Agriculture 1993, 2002 and 2007, and agricultural survey 1996. Today there are under 40 000 farming units occupying about 67% of total land of the country, around 86 million hectares. On the other hand, approximately 1.3 million smallholders (that may produce for markets or for selfconsumption) are black.",2,True
+1ac3729,"Obesity and the food system transformation in Latin America. Climate change and food security: risks and responses. World Economic and Social Survey 2016 -Climate Change Resilience: An Opportunity for Reducing Inequalities. Contribution of Working Groups I, II and III to the Fifth Assessment Report of the Intergovernmental Panel on Climate Change.",2,True
+f10934e,"Creating such an environment is complementary to the provision of more traditional public goods such as improved infrastructure, animal and plant health, education and information systems, and extension. Improvements in these areas could bring substantial long-term gains to agricultural producers through more transparent markets, improved price formation, and, ultimately, higher agricultural incomes. Benefits would also accrue to other agents of the supply chain, including food consumers for whom more competitive food chains would provide higher quality products. Because these characteristics vary with the product, and the location or size of the farm, the focus is on specific subsectors: wheat, dairy and beef, the three largest sub-sectors of Kazakhstan’s agro-food system.",2,True
+a860adb,"More extreme weather - with intense precipitation, floods and droughts - is predicted across the six SEE economies. Rainfall is predicted to decrease. These changes could reduce crop yields across the six SEE economies, especially for maize, and increase exposure to agricultural pests. Livestock productivity in Albania, Kosovo and Montenegro could fall (Callaway et al.,",2,True
+6394aa3,"However, more detailed assessments are needed in order to properly assess AFOLU's mitigation potential, the impacts on vulnerable production systems and groups, and the costs of implementation. It is a pre-requisite that practices optimized to reduce GHG emissions or sequester carbon should also protect the land tenure rights of small-scale producers and contribute to food security and climate change adaptation, particularly for the most vulnerable groups. On the economic side, options include positive incentives for farmers to provide and maintain carbon sinks, taxation of nitrogen fertilizer in countries where it is being overutilized, a measure which is already applied in some OECD countries to reduce nitrate pollution, and supply-chain initiatives that market food products with a low carbon footprint (Paustian et al., It has been estimated, using previous calculations and data from Bellarby et al. ( These approaches generally account for emissions from pre-chain inputs through to post-farm gate processing by including methane, nitrous oxide and C02 emissions, and fossil fuel use in food systems (e.g. Steinfeld et al., This can be compared with around 5.2 GtC02-eq generated by agriculture and around 4.9 Gt0O2-eq by forestry and land use change.",2,True
+9413693,"The former were local, the latter, international. Together, they contained the seeds of a reshaping of the West African migratory system. The major historical trends were shifting: the polarity of the coast, initiated by the Arab-Islamic and transatlantic slave trades and fully materialised under colonisation, was weakened.",2,False
+ab7c7ce,"Relying on a very small fraction of staple crops for our diet has dire implications for both food security and nutrition. The lack of genetic diversity within the gene pools of the dominant cultivated crops, leaves agricultural systems vulnerable to pests, diseases and other abiotic stresses. Agricultural sustainability relies on a healthy interaction between agriculture and nature.",2,True
+dc42482,"The CCVFV should ask for recommendations from the Ministry of Mining or the MECF if relevant and obtain MIC agreement for foreign projects. Once the application has been approved by the district FAB and the registration fees have been paid (around USD 0.57 per person), the township FAB issues the certificate. Applicants that are cultivating the land should show photos of the cultivated land and the Nay Pyi Taw Council or the region/state department office should approve the issuance of a land use right.",2,True
+3171bfd,"Bt cotton and corn, for example, use less herbicides and pesticides, but if these crop varieties develop resistance to the less toxic chemical herbicides and pesticides, future more toxic inputs may be required. In this case, adoption of transgenic crops could have large negative ecological implications if “GE crops are adopted more widely in developing countries where domesticated crops have wild relatives” (Ervin, Glenna and Jussaume, 2010, p. 7). Innovative mechanisms designed to engage the private sector need to be explored: results-based performance contracts—for the development, for example, of improved seed or crop varieties with higher water-stress tolerance and greater responsiveness to fertilizers—granted on a competitive basis may be one means of stimulating private research.",2,True
+ccb25d7,"Table 10 summarises risk-related policies following this two dimensional approach, which allows one to highlight several general features of New Zealand’s policies. Risk management policies in New Zealand fall predominantly under the efficiency objective. These measures are largely focused on reducing transactions cost (by establishing regulations conducive to competition and adaptation, and creating a stable macroeconomic framework), addressing the problem of asymmetric information (e.g. through research and information), and addressing the problem of externalities (e.g. biosecurity measures).",2,False
+2b0b848,"Allowing for the spillover benefits into other states, state-specific agricultural research investments generated national benefits of between USD 10 and USD 70 per research dollar, averaging USD 32 across the states. The marginal benefit-cost ratio for USDA intramural research was comparable, at USD 18 per dollar invested in research. In fact, however, these ratios are consistent with internal rates of return at the smaller end of the range compared with the general results in the literature as reviewed by Alston et al. ( Some internal rates of return are reported here to facilitate comparisons with other studies.",2,True
+69e26bd,"Agreements to do so can be reached at the bilateral, regional or multilateral levels. The pursuit of food self-sufficiency to mitigate international risks is a costly policy that undermines the function of the international trading system, making markets thinner, more volatile and therefore riskier than if countries were to adopt open trade policies. In the face of both international and domestic risks, such as that of a failed harvest, a country which uses trade barriers to promote self-sufficiency because of the fear of trade interruptions may find itself exposed to greater potential losses than if it had remained open to international trade. At the national level, some developing countries may be vulnerable to imported instability, notably if their consumption is centred around just one or two food staples, and if their imports are sourced from just one or two countries. These risks can be mitigated by promoting more diversified diets (something that happens naturally to a degree as incomes rise) and by diversifying trading partners.",2,True
+4ce8376,"For the projection period, biofuel markets are projected to be highly influenced by mandates and other incentives in countries all over the world, with the US, Brazil and the EU playing major roles, respectively, on ethanol and biodiesel markets. Based on sustained political support for biofuels, the Outlook projects increasing world biofuel prices and these will also be underpinned by rising crude oil and energy prices. The world ethanol price2 should follow an increasing trend to reach USD 54.4 per hi in 2019 supported by demand conditions in the US market where the Conventional Renewable Fuels mandate is assumed to be binding over the entire projection period. These quantities are far above the average 2007-09 base levels.",2,False
+bb006af,"Brazil's cotton production is expected to grow even faster than the world’s largest cotton producer, India, which has a greater potential for higher yield growth as it starts from a low base. During the course of the next ten years, Brazil is expected to draw-down cotton stocks. Changing competition for resources to produce other commodities is also expected to influence the outlook for cotton markets.",2,False
+4860bf8,"In an integrated world, this difference prevents the regional economy from managing at its own pace the gradual transfer of the active population from agricultural activities to modern-type activities, faced with the import of goods from advanced countries. The sudden appearance on the world market of emerging economies draining the entire investment capacity of the advanced economies may mean that Africa remains limited to exporting primary products (agricultural and mined), postponing industrialisation consistent with the growth of its population. This growth is penalising the consumption and saving potential of households, limiting the ability of the regional market to support a change in production.",2,False
+7dcefc9,"Nutrition-sensitive interventions and programmes: how can they help to accelerate progress in improving maternal and child nutrition? The lancet, 382(9891): 536-551. Household dietary diversity and Food expenditures are closely linked in rural Bangladesh, increasing the risk of malnutrition due to the financial crisis. Association of household rice expenditure with child nutritional status indicates a role for macroeconomic food policy in combating malnutrition. The Journal of Nutrition, 133(5): 1320-1325. Higher household expenditure on animal-source and nongrain foods lowers the risk of stunting among children 0-59 months old in Indonesia: implications of rising food prices.",2,True
+72a14ce,"These estimates translate into roughly 605 million, 260 million and 688 million children under age 15, respectively. The relationship between food insecurity and poverty, and well-being varies by region, demonstrating that definitions of food insecurity depend on regional context, and encompass more than monetary poverty alone. Finally, correlations of food insecurity and income per capita between 2006 and 2015, show that some regions were harder hit by the shocks in food prices and the Great Recession than others. In addition, further research on how food insecurity differs between children and adults will be important for future efforts to address and reduce child hunger.",2,True
+dc5ff8b,"A Commodity Levy Act (1990) empowers producers to self-impose levies through a vote in order to finance the “industry good” activities. Once voted, the levy becomes obligatory for all commercial producers of a commodity and is charged on each unit marketed as a type of sales tax. Levies are collected by downstream operators and transferred to industry good bodies.17 The obligatory character of the levy is grounded by the necessity to avoid a “free-rider problem”. However, this compulsory levy is introduced through voting and therefore is self-imposed.",2,False
+b9ad048,"The elimination of most public stocks in OECD countries and the privatization of most State-trading enterprises have concentrated knowledge concerning agricultural commodity availability in the hands of a small number of companies which maintain this information as proprietary. One of the most important elements of the Action Plan on Food Price Volatility, agreed by the G20 Agriculture Ministers at their meeting held in Paris on 22 and 23 June 2011, was the launching of the Agricultural Market Information System (AMIS) to improve market information and transparency of data on current stocks, and promote coordination of policy responses (see Ministerial declaration, para. Second, assuming the role traditionally played by the United States of America and China as stock holders, the international community should maintain a minimum level of world food stock.",2,True
 e0ab386,"The Ministry of Education is charged with the shaping of the education system through the development of curricula, national objectives and guidelines. Within this framework, municipalities and independent providers implement educational activities, organise school services, allocate resources and ensure that educational goals are met. Individual districts and schools are then entrusted with a large degree of autonomy to organise local schooling.",3,False
 9177b53,"Most of the local government institutions lack the capacity required to implement the policy, legislation and associated programmes. Local bodies are not financially independent and they have no autonomy in decision-making. They are financially dependent on grants from the central Government, as locally mobilized resources (mainly from property taxes) are often insufficient even for their basic operation, let alone for public services. Thus, local bodies depend on the centre for policies, plans, financial resources, human resources and even for budgetary decisions, which severely restricts the creativity and innovativeness of local leaders. Moreover, local leaders lack adequate knowledge and proper training to become visionary with regard to the socio-economic development of their locality.",3,False
 8dd268f,"Brisbane: School of Population Health, University of Queensland. The first version of this model was developed to study the impact of type 2 diabetes on the Australian population including health, health expenditures and broader economic impacts, such as changes in employment and productivity. The model was used to test the potential future impact of various policy interventions to reduce the future burden of diabetes for the purpose of improved decision-making regarding population health investment, work-force participation and productivity.",3,True
 9b237c8,"Authorship is usually collective, but principal writers are named. The papers are generally available only in their original language - English or French - with a summary in the other. The opinions expressed and arguments employed are those of the author(s). Comments on Working Papers are welcomed, and may be sent to the Directorate for Employment, Labour and Social Affairs OECD, 2 rue Andre-Pascal, 75775 Paris Cedex 16, France. The author remains responsible for any errors and omissions. The opinions expressed in the paper are the responsibility of the author and do not necessarily reflect those of the OECD or its Member Countries.",3,False
 52f8fc8,"This is a limiting structure, as real-world events occur in continuous time, and more importantly, some decisions/transitions are joint, or occur together. The model also has no labour-supply dimension. There are models for labour-force participation, unemployment and retirement but no model of hours worked and the variables that influence those hours, including the family budget, tax rates, and health. Changes in the macro economy can be entered into the model as a scenario, however, there is no general equilibrium mechanism within the model itself.",3,False
 9c41e3c,"Young people who are proficient in the Sami language and culture enjoy a more liberated and less politicized definition of ""Saminess"" than did the preceding generation. Many adolescent Sami express a complex identity including Norwegian, Swedish or Finnish and Sami culture and language, some identify themselves with another ethnicity as well. Many of the younger Sami are from families where their parents' and grandparents' generations were the targets of force assimilation policies.",3,False
 c45191f,"The review of models in this paper highlights emerging systems of models where different modelling approaches are designed to work together coherently. In this way, techniques w'ith different strengths are amalgamated and a broader range of policy questions may be explored. Examples include the system of models developed by the U.S. Congressional Budget Office and by the University of Canberra and Monash University in Australia.",3,False
```

### Comparing `sdgclassification_benchmark-0.8.0/pyproject.toml` & `sdgclassification_benchmark-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "sdgclassification-benchmark"
-version = "0.8.0"
+version = "0.9.0"
 description = "The SDG Classification Benchmark is an open and public resource for evaluating and comparing SDG classification models."
 authors = ["Finn Woelm <finn@globalgoals.directory>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/SDGClassification/benchmark"
 packages = [{ include="sdgclassification/benchmark", from="src" }, { include="benchmark.csv", to="sdgclassification/benchmark/resources/"}]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.2"
 progress = "^1.6"
-scikit-learn = "^1.4.1.post1"
 tabulate = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 mypy = "^1.9.0"
 pandas-stubs = "^2.2.0.240218"
 types-tabulate = "^0.9.0.20240106"
```

### Comparing `sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/Benchmark.py` & `sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/Benchmark.py`

 * *Files identical despite different names*

### Comparing `sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/Result.py` & `sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/Result.py`

 * *Files identical despite different names*

### Comparing `sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/ResultSet.py` & `sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/ResultSet.py`

 * *Files identical despite different names*

### Comparing `sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/Stats.py` & `sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/Stats.py`

 * *Files identical despite different names*

### Comparing `sdgclassification_benchmark-0.8.0/src/sdgclassification/benchmark/load_benchmark_df.py` & `sdgclassification_benchmark-0.9.0/src/sdgclassification/benchmark/load_benchmark_df.py`

 * *Files identical despite different names*

### Comparing `sdgclassification_benchmark-0.8.0/PKG-INFO` & `sdgclassification_benchmark-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,44 @@
 Metadata-Version: 2.1
 Name: sdgclassification-benchmark
-Version: 0.8.0
+Version: 0.9.0
 Summary: The SDG Classification Benchmark is an open and public resource for evaluating and comparing SDG classification models.
 Home-page: https://github.com/SDGClassification/benchmark
 License: MIT
 Author: Finn Woelm
 Author-email: finn@globalgoals.directory
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: progress (>=1.6,<2.0)
-Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/SDGClassification/benchmark
 Description-Content-Type: text/markdown
 
 # Benchmark for SDG Classification<!-- omit from toc -->
 
 The SDG Classification Benchmark is an open and public benchmarking dataset for evaluating and comparing SDG classification models. It consists of text snippets (2 - 3 sentences), which have been carefully labeled and verified by a team of human experts.
 
-**Note**: The benchmarking dataset currently covers SDGs 1, 3 - 7 and 10. We will be expanding the benchmarking dataset to other SDGs in the coming months.
+**Note**: The benchmarking dataset currently covers SDGs 1 - 7 and 10. We will be expanding the benchmarking dataset to other SDGs in the coming months.
 
 ## Table of Contents<!-- omit from toc -->
 
 - [The dataset](#the-dataset)
 - [How to use](#how-to-use)
-  - [With Python](#with-python)
-  - [With other languages](#with-other-languages)
 - [Background](#background)
-  - [Purpose](#purpose)
-  - [Approach](#approach)
-  - [Coverage](#coverage)
-  - [Limitations](#limitations)
-    - [Binary](#binary)
-    - [Non-exhaustive](#non-exhaustive)
-    - [Ignores sentiment](#ignores-sentiment)
-    - [Non-interpretive](#non-interpretive)
 - [Model evaluation](#model-evaluation)
-  - [Disclaimer](#disclaimer)
-  - [Results](#results)
 - [Contributing](#contributing)
-  - [Join the working group](#join-the-working-group)
-  - [Suggestions and feedback](#suggestions-and-feedback)
 - [Credits](#credits)
-  - [Core contributors](#core-contributors)
-  - [List of annotators](#list-of-annotators)
-  - [Text snippets](#text-snippets)
 
-## The dataset
+## The dataset<a id="the-dataset"></a>
 
 You can find the benchmarking dataset here: https://github.com/SDGClassification/benchmark/blob/main/benchmark.csv
 
 The dataset consists of four columns:
 
 - `id`: Unique identifier for every text (MD5 hash)
 - `text`: Text snippet (2 - 3 sentences)
@@ -70,15 +52,15 @@
 03e9759  Not only does this have potentially negative e...    7  False
 04f6c7f  If too much water is stored behind the reservo...    7  False
 b87a4f8  Energy efficiency targets are now in place at ...    7   True
 12e3f54  Data over the last 30 years suggests that, had...    7   True
 135ea60  Large areas of about 500 000 km2 between Mumba...    7  False
 ```
 
-## How to use
+## How to use<a id="how-to-use"></a>
 
 ### With Python
 
 We have created the Python package [sdgclassification-benchmark](https://pypi.org/project/sdgclassification-benchmark/) to make it easy to benchmark SDG classification models written in Python.
 
 First, install the package: `pip install sdgclassification-benchmark`
 
@@ -150,15 +132,15 @@
 df <- read.csv("https://raw.githubusercontent.com/SDGClassification/benchmark/main/benchmark.csv")
 ```
 
 You can then classify the `text` in each row of the dataset and compare your model's predictions with the true label.
 
 You can [find short descriptions about each of the columns in the dataset here](#the-dataset).
 
-## Background
+## Background<a id="background"></a>
 
 ### Purpose
 
 There exist a number of different models and approaches for classifying texts with respect to the Sustainable Development Goals (SDGs). Refer to [this list](https://globalgoals-directory.notion.site/PUBLIC-List-of-AI-driven-SDG-Classification-Initiatives-fe4770a173194e0b980f95b330a8a83b) for a (non-exhaustive) overview of different SDG classifiers and initiatives.
 
 To further advance the field of SDG classification, it is important that we understand the strengths and weaknesses of the available tools.
 
@@ -172,19 +154,20 @@
 
 To ensure a robust benchmarking dataset, the texts for each SDG were independently annotated by several human experts. For most texts, the annotations made by these experts were identical. For some texts, however, there initially were disagreements between the annotations. These disagreements were resolved through discussion between the experts until consensus was reached.
 
 In some cases, consensus was reached by making slight modifications to a text in order to remove ambiguity.
 
 ### Coverage
 
-The dataset currently covers SDGs 1, 3 - 7 and 10.
+The dataset currently covers SDGs 1 - 7 and 10.
 
 | SDG                                | Number of texts | Texts with SDG | Texts without SDG |
 | ---------------------------------- | --------------: | -------------: | ----------------: |
 | SDG 1: No poverty                  |              77 |             27 |                50 |
+| SDG 2: Zero hunger                 |              69 |             45 |                24 |
 | SDG 3: Good health and well-being  |              76 |             28 |                48 |
 | SDG 4: Quality education           |              82 |             43 |                39 |
 | SDG 5: Gender equality             |              69 |             35 |                34 |
 | SDG 6: Clean water and sanitation  |              85 |             48 |                37 |
 | SDG 7: Affordable and clean energy |             100 |             50 |                50 |
 | SDG 10: Reduced inequalities       |              61 |             32 |                29 |
 
@@ -214,63 +197,65 @@
 
 #### Non-interpretive
 
 Texts were only assigned to a given SDG, if the text directly addressed that SDG and/or its targets. "We are subsidizing the costs of silicon" would not qualify for SDG 7, even though silicon is one of the materials for making photovoltaic cells and reduced cost of silicon might have indirect benefits for the expansion of solar energy.
 
 We ignored indirect relevance in texts because correct assessments would require enormous thematic expertise, and even then such interpretations would often remain highly subjective and controversial.
 
-## Model evaluation
+## Model evaluation<a id="model-evaluation"></a>
 
 ### Disclaimer
 
 Several models have been tested against this benchmark. The results can be used as one criterion when evaluating models. Importantly, there are a range of other important aspects to consider that are not tested by this benchmark, such as cost, speed, and coverage of SDG targets. In addition, many models have been developed and optimized for domain-specific use cases (e.g. analyzing policy documents, research articles or websites) and their performance on this benchmark may not be representative of their performance on their domain-specific use case.
 
 ### Results
 
 The table below shows the accuracy (in percent) of models tested against this benchmark. Clicking on one of the models provides additional details, including metadata about the model, F1 score, precision and recall.
 
 <!-- evaluation table begin -->
 
-| Model                                                                                                                  | Average | SDG 1 | SDG 3 | SDG 4 | SDG 5 | SDG 6 | SDG 7 | SDG 10 |
-| :--------------------------------------------------------------------------------------------------------------------- | ------: | ----: | ----: | ----: | ----: | ----: | ----: | -----: |
-| [AFD SDG Prospector](https://github.com/SDGClassification/benchmark/tree/main/evaluations/sdg-prospector/)             |      91 |    95 |    91 |    95 |    81 |    92 |    95 |     87 |
-| [Aurora SDG](https://github.com/SDGClassification/benchmark/tree/main/evaluations/aurora-sdg/)                         |      82 |    74 |    78 |    83 |    90 |    85 |    87 |     77 |
-| [Global Goals Directory](https://github.com/SDGClassification/benchmark/tree/main/evaluations/global-goals-directory/) |      84 |    90 |    90 |    78 |    74 |    87 |    91 |     80 |
-| [JRC SDG Mapper](https://github.com/SDGClassification/benchmark/tree/main/evaluations/sdg-mapper/)                     |      77 |    82 |    84 |    70 |    75 |    73 |    86 |     70 |
-| [Meta Llama 2 70B](https://github.com/SDGClassification/benchmark/tree/main/evaluations/llama-2/)                      |      89 |    88 |    93 |    90 |    93 |    85 |    92 |     79 |
-| [Meta Llama 3 70B](https://github.com/SDGClassification/benchmark/tree/main/evaluations/llama-3/)                      |      88 |    77 |    86 |    85 |    91 |    92 |    91 |     92 |
-| [OpenAI GPT-3.5 Turbo](https://github.com/SDGClassification/benchmark/tree/main/evaluations/openai-gpt-3/)             |      83 |    65 |    82 |    80 |    87 |    91 |    90 |     87 |
-| [OpenAI GPT-4 Turbo](https://github.com/SDGClassification/benchmark/tree/main/evaluations/openai-gpt-4/)               |      87 |    75 |    86 |    84 |    88 |    92 |    92 |     92 |
+| Model                                                                                                                  |   Average |   SDG 1 |   SDG 2 |   SDG 3 |   SDG 4 |   SDG 5 |   SDG 6 |   SDG 7 |   SDG 10 |
+|:-----------------------------------------------------------------------------------------------------------------------|----------:|--------:|--------:|--------:|--------:|--------:|--------:|--------:|---------:|
+| [AFD SDG Prospector](https://github.com/SDGClassification/benchmark/tree/main/evaluations/sdg-prospector/)             |        90 |      95 |      87 |      91 |      95 |      81 |      92 |      95 |       87 |
+| [Aurora SDG](https://github.com/SDGClassification/benchmark/tree/main/evaluations/aurora-sdg/)                         |        82 |      74 |      83 |      78 |      83 |      90 |      85 |      87 |       77 |
+| [Global Goals Directory](https://github.com/SDGClassification/benchmark/tree/main/evaluations/global-goals-directory/) |        84 |      90 |      80 |      90 |      78 |      74 |      87 |      91 |       80 |
+| [JRC SDG Mapper](https://github.com/SDGClassification/benchmark/tree/main/evaluations/sdg-mapper/)                     |        76 |      82 |      71 |      84 |      70 |      75 |      73 |      86 |       70 |
+| [Meta Llama 2 70B](https://github.com/SDGClassification/benchmark/tree/main/evaluations/llama-2/)                      |        88 |      88 |      84 |      93 |      90 |      93 |      85 |      92 |       79 |
+| [Meta Llama 3 70B](https://github.com/SDGClassification/benchmark/tree/main/evaluations/llama-3/)                      |        88 |      77 |      90 |      86 |      85 |      91 |      92 |      91 |       92 |
+| [OpenAI GPT-3.5 Turbo](https://github.com/SDGClassification/benchmark/tree/main/evaluations/openai-gpt-3/)             |        84 |      65 |      93 |      82 |      80 |      87 |      91 |      90 |       87 |
+| [OpenAI GPT-4 Turbo](https://github.com/SDGClassification/benchmark/tree/main/evaluations/openai-gpt-4/)               |        88 |      75 |      93 |      86 |      84 |      88 |      92 |      92 |       92 |
 
 <!-- evaluation table end -->
 
 More models will be added in the future.
 
 Have you benchmarked a model that is not yet in our list? Please open an issue and share the results with us, so that we can add the model to the table above.
 
-## Contributing
+## Contributing<a id="contributing"></a>
 
 ### Join the working group
 
 The [core contributors](#core-contributors) meet regularly to improve and expand this benchmarking dataset. If you want to join us, please reach out to [finn@globalgoals.directory](mailto:finn@globalgoals.directory).
 
 ### Suggestions and feedback
 
 This benchmarking dataset is a living document and we will continue to make adjustments and improvements based on feedback. Please open an issue to share your ideas, suggestions, and feedback.
 
-## Credits
+## Credits<a id="credits"></a>
 
 ### Core contributors
 
 The benchmarking dataset has been created by the Benchmarking Working Group of the [SDG Classification Expert Group](https://sdg-ai.org/). Core contributors are Finn Woelm, Meike Morren, Steve Borchardt, Jean-Baptiste Jacouton and Gib Ravivanpong.
 
 ### List of annotators
 
 We especially thank our annotators for making this project possible.
 
+- **SDG 1**: Steve Borchardt, Meike Morren, Finn Woelm
+- **SDG 2**: Steve Borchardt, Meike Morren, Gib Ravivanpong, Finn Woelm
 - **SDG 3**: Steve Borchardt, Meike Morren, Finn Woelm
 - **SDG 4**: Steve Borchardt, Meike Morren, Finn Woelm
 - **SDG 5**: Steve Borchardt, Meike Morren, Gib Ravivanpong, Finn Woelm
 - **SDG 6**: Steve Borchardt, Meike Morren, Gib Ravivanpong, Finn Woelm
 - **SDG 7**: Steve Borchardt, Jean-Baptiste Jacouton, Gib Ravivanpong, Finn Woelm
 - **SDG 10**: Steve Borchardt, Jean-Baptiste Jacouton, Meike Morren, Gib Ravivanpong, Finn Woelm
```

