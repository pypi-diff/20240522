# Comparing `tmp/swarmauri-0.2.7.tar.gz` & `tmp/swarmauri-0.2.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarmauri-0.2.7.tar", last modified: Wed May 22 01:56:51 2024, max compression
+gzip compressed data, was "swarmauri-0.2.8.dev1.tar", last modified: Wed May 22 02:03:58 2024, max compression
```

## Comparing `swarmauri-0.2.7.tar` & `swarmauri-0.2.8.dev1.tar`

### file list

```diff
@@ -1,520 +1,520 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.864421 swarmauri-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-22 01:56:51.864421 swarmauri-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-22 01:56:39.000000 swarmauri-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:56:51.864421 swarmauri-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-22 01:56:39.000000 swarmauri-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.780421 swarmauri-0.2.7/swarmauri/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.780421 swarmauri-0.2.7/swarmauri/community/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.780421 swarmauri-0.2.7/swarmauri/community/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.780421 swarmauri-0.2.7/swarmauri/community/document_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/document_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.784421 swarmauri-0.2.7/swarmauri/community/document_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/document_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.784421 swarmauri-0.2.7/swarmauri/community/retrievers/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.784421 swarmauri-0.2.7/swarmauri/community/retrievers/base/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/retrievers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.784421 swarmauri-0.2.7/swarmauri/community/retrievers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/retrievers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.784421 swarmauri-0.2.7/swarmauri/community/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.784421 swarmauri-0.2.7/swarmauri/community/tools/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.784421 swarmauri-0.2.7/swarmauri/community/tools/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/concrete/DownloadPdfTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/concrete/EntityRecognitionTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/concrete/GmailReadTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/concrete/GmailSendTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/concrete/PaCMAP.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/concrete/WebScrapingTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/concrete/ZapierHookTool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/community/tools/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.784421 swarmauri-0.2.7/swarmauri/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.784421 swarmauri-0.2.7/swarmauri/core/agent_apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agent_apis/IAgentCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agent_apis/IAgentRouterCRUD.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agent_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.788421 swarmauri-0.2.7/swarmauri/core/agent_factories/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agent_factories/IAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agent_factories/IExportConf.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agent_factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.788421 swarmauri-0.2.7/swarmauri/core/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agents/IAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agents/IAgentConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agents/IAgentName.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agents/IAgentParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agents/IAgentRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agents/IAgentSystemContext.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agents/IAgentToolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agents/IAgentVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.788421 swarmauri-0.2.7/swarmauri/core/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chains/ICallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chains/IChain.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chains/IChainContext.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chains/IChainContextLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chains/IChainDependencyResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chains/IChainFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chains/IChainStep.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.788421 swarmauri-0.2.7/swarmauri/core/chunkers/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chunkers/IChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/chunkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.792421 swarmauri-0.2.7/swarmauri/core/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/conversations/IConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/conversations/IMaxSize.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/conversations/ISystemContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.792421 swarmauri-0.2.7/swarmauri/core/distances/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/distances/IDistanceSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.792421 swarmauri-0.2.7/swarmauri/core/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/document_stores/IDocumentRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/document_stores/IDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.792421 swarmauri-0.2.7/swarmauri/core/documents/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/documents/IDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/documents/IEmbed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/documents/IExperimentDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.792421 swarmauri-0.2.7/swarmauri/core/experiment_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/experiment_stores/IExperimentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/experiment_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.792421 swarmauri-0.2.7/swarmauri/core/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/messages/IMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.792421 swarmauri-0.2.7/swarmauri/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/metrics/IAggMeasurements.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/metrics/ICalculateMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/metrics/IMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/metrics/IThreshold.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.796421 swarmauri-0.2.7/swarmauri/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/models/IFit.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/models/IModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/models/IPredict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.796421 swarmauri-0.2.7/swarmauri/core/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/parsers/IParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.796421 swarmauri-0.2.7/swarmauri/core/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/prompts/IPrompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/prompts/IPromptMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/prompts/ITemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.796421 swarmauri-0.2.7/swarmauri/core/swarm_apis/
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarm_apis/ISwarmAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarm_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.796421 swarmauri-0.2.7/swarmauri/core/swarms/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarms/ISwarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarms/ISwarmAgentRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarms/ISwarmChainCRUD.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarms/ISwarmComponent.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarms/ISwarmConfigurationExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarms/ISwarmFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.796421 swarmauri-0.2.7/swarmauri/core/toolkits/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/toolkits/IToolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/toolkits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.800421 swarmauri-0.2.7/swarmauri/core/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/tools/IParameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/tools/ITool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.800421 swarmauri-0.2.7/swarmauri/core/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/tracing/IChainTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/tracing/ITraceContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/tracing/ITracer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.800421 swarmauri-0.2.7/swarmauri/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/utils/ITransactional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.804421 swarmauri-0.2.7/swarmauri/core/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IAngleBetweenVectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IDecompose.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IDivergence.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IGradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IOrthogonalProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IReflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/ISaveLoadStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/ISimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/ISimiliarityQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorArithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorBasisCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorLinearCombination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorNorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorRotate.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorSpan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.804421 swarmauri-0.2.7/swarmauri/core/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vectorizers/IFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vectorizers/ISaveModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vectorizers/IVectorize.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.804421 swarmauri-0.2.7/swarmauri/core/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vectors/IVector.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vectors/IVectorMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vectors/IVectorProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vectors/IVectorTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/core/vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.804421 swarmauri-0.2.7/swarmauri/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.804421 swarmauri-0.2.7/swarmauri/experimental/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/chains/IChainFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/chains/IChainNotification.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/chains/IChainPersistence.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/chains/IChainScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/chains/TypeAgnosticCallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.808421 swarmauri-0.2.7/swarmauri/experimental/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/conversations/SemanticConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.808421 swarmauri-0.2.7/swarmauri/experimental/distances/
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/CanberraDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/ChebyshevDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/HaversineDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/ManhattanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/MinkowskiDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/SSASimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/SSIVSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/ScannVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/SorensenDiceDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/SquaredEuclideanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.808421 swarmauri-0.2.7/swarmauri/experimental/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/document_stores/TriplesDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/document_stores/Word2VecDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.808421 swarmauri-0.2.7/swarmauri/experimental/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/models/HierarchicalAttentionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/models/SageMaker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.812421 swarmauri-0.2.7/swarmauri/experimental/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/parsers/PDFToTextParser.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.812421 swarmauri-0.2.7/swarmauri/experimental/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/tools/CypherQueryTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/tools/FileDownloaderTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/tools/LinkedInArticleTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/tools/OutlookSendMailTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/tools/SQLite3QueryTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/tools/TwitterPostTool.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.812421 swarmauri-0.2.7/swarmauri/experimental/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/tracing/RemoteTrace.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.812421 swarmauri-0.2.7/swarmauri/experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/utils/ISerializable.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/utils/get_last_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/utils/log_prompt_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/utils/save_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.812421 swarmauri-0.2.7/swarmauri/experimental/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/vector_stores/TriplesDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.812421 swarmauri-0.2.7/swarmauri/experimental/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/vectorizers/DGLVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/experimental/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.812421 swarmauri-0.2.7/swarmauri/standard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.816421 swarmauri-0.2.7/swarmauri/standard/agent_factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agent_factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.816421 swarmauri-0.2.7/swarmauri/standard/agent_factories/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agent_factories/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.816421 swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/AgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/JsonAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.816421 swarmauri-0.2.7/swarmauri/standard/agents/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.816421 swarmauri-0.2.7/swarmauri/standard/agents/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/base/AgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/base/AgentRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/base/ConversationAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/base/NamedAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/base/SystemContextAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/base/ToolAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/base/VectorStoreAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.820421 swarmauri-0.2.7/swarmauri/standard/agents/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/concrete/QAAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/concrete/RagAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/concrete/SimpleConversationAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/concrete/ToolAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/agents/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.820421 swarmauri-0.2.7/swarmauri/standard/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.820421 swarmauri-0.2.7/swarmauri/standard/apis/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/apis/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.820421 swarmauri-0.2.7/swarmauri/standard/apis/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/apis/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.820421 swarmauri-0.2.7/swarmauri/standard/chains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.820421 swarmauri-0.2.7/swarmauri/standard/chains/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/base/ChainBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/base/ChainContextBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/base/ChainStepBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/base/PromptContextChainBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.820421 swarmauri-0.2.7/swarmauri/standard/chains/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/concrete/CallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/concrete/ChainStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/concrete/ContextChain.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/concrete/PromptContextChain.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chains/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.820421 swarmauri-0.2.7/swarmauri/standard/chunkers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chunkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.820421 swarmauri-0.2.7/swarmauri/standard/chunkers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chunkers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.824421 swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.824421 swarmauri-0.2.7/swarmauri/standard/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.824421 swarmauri-0.2.7/swarmauri/standard/conversations/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/base/ConversationBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/base/SystemContextBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.824421 swarmauri-0.2.7/swarmauri/standard/conversations/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/concrete/MaxSizeConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/concrete/SessionCacheConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/concrete/SharedConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/concrete/SimpleConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/conversations/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.824421 swarmauri-0.2.7/swarmauri/standard/distances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.824421 swarmauri-0.2.7/swarmauri/standard/distances/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/distances/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/distances/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/distances/concrete/ChiSquaredDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/distances/concrete/CosineDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/distances/concrete/EuclideanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/distances/concrete/JaccardIndexDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/distances/concrete/LevenshteinDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/distances/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/document_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/document_stores/base/DocumentStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/document_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/document_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/document_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/documents/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/documents/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/documents/base/DocumentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/documents/base/EmbeddedBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/documents/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/documents/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/documents/concrete/Document.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/documents/concrete/EmbeddedDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/documents/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/exceptions/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/exceptions/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/exceptions/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/exceptions/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.828421 swarmauri-0.2.7/swarmauri/standard/messages/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/messages/base/MessageBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/messages/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.832421 swarmauri-0.2.7/swarmauri/standard/messages/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/messages/concrete/AgentMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/messages/concrete/FunctionMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/messages/concrete/HumanMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/messages/concrete/SystemMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/messages/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.832421 swarmauri-0.2.7/swarmauri/standard/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.832421 swarmauri-0.2.7/swarmauri/standard/metrics/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/base/AggregateMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/base/CalculateMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/base/MetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/base/ThresholdMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.832421 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/HitRateAtK.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/ImpressionAtK.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/MeanMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/StaticValueMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/ZeroMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/metrics/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.836421 swarmauri-0.2.7/swarmauri/standard/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.836421 swarmauri-0.2.7/swarmauri/standard/models/base/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/base/ModelBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.836421 swarmauri-0.2.7/swarmauri/standard/models/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/AnthropicModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/AzureGPT.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/CohereModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/GeminiProModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/GroqModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/GroqToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/MistralModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/MistralToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/OpenAIModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/OpenAIToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/models/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.836421 swarmauri-0.2.7/swarmauri/standard/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.836421 swarmauri-0.2.7/swarmauri/standard/parsers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.840421 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/CSVParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/MarkdownParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/PythonParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/RegExParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/TFIDFParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/URLExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/XMLParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/parsers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.840421 swarmauri-0.2.7/swarmauri/standard/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.840421 swarmauri-0.2.7/swarmauri/standard/prompts/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/prompts/base/BasePromptMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/prompts/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.840421 swarmauri-0.2.7/swarmauri/standard/prompts/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/prompts/concrete/Prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/prompts/concrete/PromptGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/prompts/concrete/PromptMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/prompts/concrete/PromptTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/prompts/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.840421 swarmauri-0.2.7/swarmauri/standard/states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.840421 swarmauri-0.2.7/swarmauri/standard/states/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/states/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/states/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/states/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/swarms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/swarms/base/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/swarms/base/SwarmComponentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/swarms/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/swarms/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/swarms/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/toolkits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/toolkits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/toolkits/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/toolkits/base/ToolkitBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/toolkits/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/toolkits/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/toolkits/concrete/Toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/toolkits/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/tools/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/base/ToolBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.844421 swarmauri-0.2.7/swarmauri/standard/tools/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/concrete/AdditionTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/concrete/CalculatorTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/concrete/CodeInterpreterTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/concrete/ImportMemoryModuleTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/concrete/Parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/concrete/TestTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/concrete/WeatherTool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tools/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.848421 swarmauri-0.2.7/swarmauri/standard/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.848421 swarmauri-0.2.7/swarmauri/standard/tracing/base/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tracing/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.848421 swarmauri-0.2.7/swarmauri/standard/tracing/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tracing/concrete/CallableTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tracing/concrete/ChainTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tracing/concrete/SimpleTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tracing/concrete/TracedVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tracing/concrete/VariableTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/tracing/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.848421 swarmauri-0.2.7/swarmauri/standard/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/utils/apply_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/utils/decorate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/utils/get_class_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/utils/json_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/utils/load_documents_from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/utils/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/utils/sql_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.848421 swarmauri-0.2.7/swarmauri/standard/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.848421 swarmauri-0.2.7/swarmauri/standard/vector_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.852421 swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.852421 swarmauri-0.2.7/swarmauri/standard/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.852421 swarmauri-0.2.7/swarmauri/standard/vectorizers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectorizers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.852421 swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.852421 swarmauri-0.2.7/swarmauri/standard/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.852421 swarmauri-0.2.7/swarmauri/standard/vectors/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectors/base/VectorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectors/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.852421 swarmauri-0.2.7/swarmauri/standard/vectors/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectors/concrete/SimpleVector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectors/concrete/VectorProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:56:39.000000 swarmauri-0.2.7/swarmauri/standard/vectors/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:56:51.852421 swarmauri-0.2.7/swarmauri.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-22 01:56:51.000000 swarmauri-0.2.7/swarmauri.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19089 2024-05-22 01:56:51.000000 swarmauri-0.2.7/swarmauri.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:56:51.000000 swarmauri-0.2.7/swarmauri.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-22 01:56:51.000000 swarmauri-0.2.7/swarmauri.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 01:56:51.000000 swarmauri-0.2.7/swarmauri.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.412806 swarmauri-0.2.8.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-22 02:03:58.412806 swarmauri-0.2.8.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:03:58.412806 swarmauri-0.2.8.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/community/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/community/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/community/document_stores/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/document_stores/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/community/document_stores/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/document_stores/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/community/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/community/retrievers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/retrievers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/community/retrievers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/retrievers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/community/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.328804 swarmauri-0.2.8.dev1/swarmauri/community/tools/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.332804 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/DownloadPdfTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/EntityRecognitionTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/GmailReadTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/GmailSendTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/PaCMAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/WebScrapingTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/ZapierHookTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.332804 swarmauri-0.2.8.dev1/swarmauri/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.332804 swarmauri-0.2.8.dev1/swarmauri/core/agent_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agent_apis/IAgentCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agent_apis/IAgentRouterCRUD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agent_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.332804 swarmauri-0.2.8.dev1/swarmauri/core/agent_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agent_factories/IAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agent_factories/IExportConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agent_factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.332804 swarmauri-0.2.8.dev1/swarmauri/core/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agents/IAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agents/IAgentConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agents/IAgentName.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agents/IAgentParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agents/IAgentRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agents/IAgentSystemContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agents/IAgentToolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agents/IAgentVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.336804 swarmauri-0.2.8.dev1/swarmauri/core/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chains/ICallableChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chains/IChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chains/IChainContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chains/IChainContextLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chains/IChainDependencyResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chains/IChainFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chains/IChainStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.336804 swarmauri-0.2.8.dev1/swarmauri/core/chunkers/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chunkers/IChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/chunkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.336804 swarmauri-0.2.8.dev1/swarmauri/core/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/conversations/IConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/conversations/IMaxSize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/conversations/ISystemContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.336804 swarmauri-0.2.8.dev1/swarmauri/core/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/distances/IDistanceSimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/distances/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.336804 swarmauri-0.2.8.dev1/swarmauri/core/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/document_stores/IDocumentRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/document_stores/IDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.340804 swarmauri-0.2.8.dev1/swarmauri/core/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/documents/IDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/documents/IEmbed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/documents/IExperimentDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.340804 swarmauri-0.2.8.dev1/swarmauri/core/experiment_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/experiment_stores/IExperimentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/experiment_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.340804 swarmauri-0.2.8.dev1/swarmauri/core/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/messages/IMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.340804 swarmauri-0.2.8.dev1/swarmauri/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/metrics/IAggMeasurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/metrics/ICalculateMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/metrics/IMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/metrics/IThreshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.340804 swarmauri-0.2.8.dev1/swarmauri/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/models/IFit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/models/IModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/models/IPredict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.340804 swarmauri-0.2.8.dev1/swarmauri/core/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/parsers/IParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.340804 swarmauri-0.2.8.dev1/swarmauri/core/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/prompts/IPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/prompts/IPromptMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/prompts/ITemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/prompts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.344805 swarmauri-0.2.8.dev1/swarmauri/core/swarm_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarm_apis/ISwarmAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarm_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.344805 swarmauri-0.2.8.dev1/swarmauri/core/swarms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarmAgentRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarmChainCRUD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarmComponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarmConfigurationExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarmFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.344805 swarmauri-0.2.8.dev1/swarmauri/core/toolkits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/toolkits/IToolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/toolkits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.344805 swarmauri-0.2.8.dev1/swarmauri/core/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/tools/IParameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/tools/ITool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.344805 swarmauri-0.2.8.dev1/swarmauri/core/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/tracing/IChainTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/tracing/ITraceContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/tracing/ITracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.344805 swarmauri-0.2.8.dev1/swarmauri/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/utils/ITransactional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.348805 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IAngleBetweenVectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IDecompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IDivergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IGradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IOrthogonalProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IReflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/ISaveLoadStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/ISimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/ISimiliarityQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorArithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorBasisCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorLinearCombination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorNorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorRotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorSpan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.352805 swarmauri-0.2.8.dev1/swarmauri/core/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vectorizers/IFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vectorizers/ISaveModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vectorizers/IVectorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vectorizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.352805 swarmauri-0.2.8.dev1/swarmauri/core/vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vectors/IVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vectors/IVectorMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vectors/IVectorProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vectors/IVectorTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/core/vectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.352805 swarmauri-0.2.8.dev1/swarmauri/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.352805 swarmauri-0.2.8.dev1/swarmauri/experimental/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/chains/IChainFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/chains/IChainNotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/chains/IChainPersistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/chains/IChainScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/chains/TypeAgnosticCallableChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.352805 swarmauri-0.2.8.dev1/swarmauri/experimental/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/conversations/SemanticConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.356805 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/CanberraDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/ChebyshevDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/HaversineDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/ManhattanDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/MinkowskiDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/SSASimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/SSIVSimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/ScannVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/SorensenDiceDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/SquaredEuclideanDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/distances/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.356805 swarmauri-0.2.8.dev1/swarmauri/experimental/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/document_stores/TriplesDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/document_stores/Word2VecDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.356805 swarmauri-0.2.8.dev1/swarmauri/experimental/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/models/HierarchicalAttentionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/models/SageMaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.356805 swarmauri-0.2.8.dev1/swarmauri/experimental/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/parsers/PDFToTextParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/experimental/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/tools/CypherQueryTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/tools/FileDownloaderTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/tools/LinkedInArticleTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/tools/OutlookSendMailTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/tools/SQLite3QueryTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/tools/TwitterPostTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/experimental/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/tracing/RemoteTrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/utils/ISerializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/utils/get_last_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/utils/log_prompt_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/utils/save_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/experimental/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/vector_stores/TriplesDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/experimental/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/vectorizers/DGLVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/experimental/vectorizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/AgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/JsonAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.360805 swarmauri-0.2.8.dev1/swarmauri/standard/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.364805 swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/AgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/AgentRetrieveBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/ConversationAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/NamedAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/SystemContextAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/ToolAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/VectorStoreAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.364805 swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/QAAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/RagAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/SimpleConversationAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/ToolAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.364805 swarmauri-0.2.8.dev1/swarmauri/standard/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.364805 swarmauri-0.2.8.dev1/swarmauri/standard/apis/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/apis/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.364805 swarmauri-0.2.8.dev1/swarmauri/standard/apis/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/apis/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.364805 swarmauri-0.2.8.dev1/swarmauri/standard/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.368805 swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/ChainBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/ChainContextBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/ChainStepBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/PromptContextChainBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.368805 swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/CallableChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/ChainStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/ContextChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/PromptContextChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.368805 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.368805 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.368805 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.368805 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.368805 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/base/ConversationBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/base/SystemContextBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.372805 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/MaxSizeConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/SessionCacheConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/SharedConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/SimpleConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.372805 swarmauri-0.2.8.dev1/swarmauri/standard/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/distances/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.372805 swarmauri-0.2.8.dev1/swarmauri/standard/distances/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/distances/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.372805 swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/ChiSquaredDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/CosineDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/EuclideanDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/JaccardIndexDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/LevenshteinDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.372805 swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.372805 swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/base/DocumentStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.372805 swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.372805 swarmauri-0.2.8.dev1/swarmauri/standard/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.376805 swarmauri-0.2.8.dev1/swarmauri/standard/documents/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/documents/base/DocumentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/documents/base/EmbeddedBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/documents/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.376805 swarmauri-0.2.8.dev1/swarmauri/standard/documents/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/documents/concrete/Document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/documents/concrete/EmbeddedDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/documents/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.376805 swarmauri-0.2.8.dev1/swarmauri/standard/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.376805 swarmauri-0.2.8.dev1/swarmauri/standard/exceptions/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/exceptions/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.376805 swarmauri-0.2.8.dev1/swarmauri/standard/exceptions/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/exceptions/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.376805 swarmauri-0.2.8.dev1/swarmauri/standard/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.376805 swarmauri-0.2.8.dev1/swarmauri/standard/messages/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/messages/base/MessageBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/messages/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.376805 swarmauri-0.2.8.dev1/swarmauri/standard/messages/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/messages/concrete/AgentMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/messages/concrete/FunctionMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/messages/concrete/HumanMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/messages/concrete/SystemMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/messages/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.376805 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.380805 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/AggregateMetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/CalculateMetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/MetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/ThresholdMetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.380805 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/HitRateAtK.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/ImpressionAtK.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/MeanMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/StaticValueMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/ZeroMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.380805 swarmauri-0.2.8.dev1/swarmauri/standard/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.380805 swarmauri-0.2.8.dev1/swarmauri/standard/models/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/base/ModelBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.384805 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/AnthropicModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/AzureGPT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/CohereModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/GeminiProModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/GroqModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/GroqToolModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/MistralModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/MistralToolModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/OpenAIModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/OpenAIToolModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.384805 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.384805 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/CSVParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/MarkdownParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/PythonParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/RegExParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/TFIDFParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/URLExtractorParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/XMLParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/base/BasePromptMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/concrete/Prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/concrete/PromptGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/concrete/PromptMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/concrete/PromptTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/prompts/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/states/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/states/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/states/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/states/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/states/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/swarms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/swarms/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/swarms/base/SwarmComponentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/swarms/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/swarms/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/swarms/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.388805 swarmauri-0.2.8.dev1/swarmauri/standard/toolkits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/toolkits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.392805 swarmauri-0.2.8.dev1/swarmauri/standard/toolkits/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/toolkits/base/ToolkitBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/toolkits/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.392805 swarmauri-0.2.8.dev1/swarmauri/standard/toolkits/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/toolkits/concrete/Toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/toolkits/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.392805 swarmauri-0.2.8.dev1/swarmauri/standard/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.392805 swarmauri-0.2.8.dev1/swarmauri/standard/tools/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/base/ToolBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.392805 swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/AdditionTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/CalculatorTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/CodeInterpreterTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/ImportMemoryModuleTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/Parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/TestTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/WeatherTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.392805 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.392805 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.396805 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/CallableTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/ChainTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/SimpleTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/TracedVariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/VariableTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.396805 swarmauri-0.2.8.dev1/swarmauri/standard/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/utils/apply_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/utils/decorate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/utils/get_class_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/utils/json_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/utils/load_documents_from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/utils/sql_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.396805 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.396805 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.400805 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.400805 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.400805 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.400805 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.400805 swarmauri-0.2.8.dev1/swarmauri/standard/vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.400805 swarmauri-0.2.8.dev1/swarmauri/standard/vectors/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectors/base/VectorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectors/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.400805 swarmauri-0.2.8.dev1/swarmauri/standard/vectors/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectors/concrete/SimpleVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectors/concrete/VectorProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:03:44.000000 swarmauri-0.2.8.dev1/swarmauri/standard/vectors/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:03:58.400805 swarmauri-0.2.8.dev1/swarmauri.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-22 02:03:58.000000 swarmauri-0.2.8.dev1/swarmauri.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19089 2024-05-22 02:03:58.000000 swarmauri-0.2.8.dev1/swarmauri.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:03:58.000000 swarmauri-0.2.8.dev1/swarmauri.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-22 02:03:58.000000 swarmauri-0.2.8.dev1/swarmauri.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 02:03:58.000000 swarmauri-0.2.8.dev1/swarmauri.egg-info/top_level.txt
```

### Comparing `swarmauri-0.2.7/PKG-INFO` & `swarmauri-0.2.8.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri
-Version: 0.2.7
+Version: 0.2.8.dev1
 Summary: This repository includes core interfaces, standard ABCs and concrete references, third party plugins, and experimental modules for the swarmaURI framework.
 Home-page: http://github.com/swarmauri/swarmauri-sdk
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri-0.2.7/README.md` & `swarmauri-0.2.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/setup.py` & `swarmauri-0.2.8.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/document_stores/concrete/RedisDocumentStore.py` & `swarmauri-0.2.8.dev1/swarmauri/community/document_stores/concrete/RedisDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py` & `swarmauri-0.2.8.dev1/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/tools/concrete/DownloadPdfTool.py` & `swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/DownloadPdfTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/tools/concrete/EntityRecognitionTool.py` & `swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/EntityRecognitionTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/tools/concrete/GmailReadTool.py` & `swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/GmailReadTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/tools/concrete/GmailSendTool.py` & `swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/GmailSendTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/tools/concrete/PaCMAP.py` & `swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/PaCMAP.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/tools/concrete/SentimentAnalysisTool.py` & `swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/SentimentAnalysisTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/tools/concrete/WebScrapingTool.py` & `swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/WebScrapingTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/community/tools/concrete/ZapierHookTool.py` & `swarmauri-0.2.8.dev1/swarmauri/community/tools/concrete/ZapierHookTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/agent_apis/IAgentCommands.py` & `swarmauri-0.2.8.dev1/swarmauri/core/agent_apis/IAgentCommands.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/agent_apis/IAgentRouterCRUD.py` & `swarmauri-0.2.8.dev1/swarmauri/core/agent_apis/IAgentRouterCRUD.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/agent_factories/IAgentFactory.py` & `swarmauri-0.2.8.dev1/swarmauri/core/agent_factories/IAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/agent_factories/IExportConf.py` & `swarmauri-0.2.8.dev1/swarmauri/core/agent_factories/IExportConf.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/agents/IAgent.py` & `swarmauri-0.2.8.dev1/swarmauri/core/agents/IAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/chains/IChain.py` & `swarmauri-0.2.8.dev1/swarmauri/core/chains/IChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/chains/IChainDependencyResolver.py` & `swarmauri-0.2.8.dev1/swarmauri/core/chains/IChainDependencyResolver.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/chains/IChainFactory.py` & `swarmauri-0.2.8.dev1/swarmauri/core/chains/IChainFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/chains/IChainStep.py` & `swarmauri-0.2.8.dev1/swarmauri/core/chains/IChainStep.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/conversations/IConversation.py` & `swarmauri-0.2.8.dev1/swarmauri/core/conversations/IConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/conversations/ISystemContext.py` & `swarmauri-0.2.8.dev1/swarmauri/core/conversations/ISystemContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/distances/IDistanceSimilarity.py` & `swarmauri-0.2.8.dev1/swarmauri/core/distances/IDistanceSimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/document_stores/IDocumentRetrieve.py` & `swarmauri-0.2.8.dev1/swarmauri/core/document_stores/IDocumentRetrieve.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/document_stores/IDocumentStore.py` & `swarmauri-0.2.8.dev1/swarmauri/core/document_stores/IDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/documents/IDocument.py` & `swarmauri-0.2.8.dev1/swarmauri/core/documents/IDocument.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/documents/IExperimentDocument.py` & `swarmauri-0.2.8.dev1/swarmauri/core/documents/IExperimentDocument.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/experiment_stores/IExperimentStore.py` & `swarmauri-0.2.8.dev1/swarmauri/core/experiment_stores/IExperimentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/experiment_stores/__init__.py` & `swarmauri-0.2.8.dev1/swarmauri/core/experiment_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/messages/IMessage.py` & `swarmauri-0.2.8.dev1/swarmauri/core/messages/IMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/metrics/IAggMeasurements.py` & `swarmauri-0.2.8.dev1/swarmauri/core/metrics/IAggMeasurements.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/metrics/ICalculateMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/core/metrics/ICalculateMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/metrics/IMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/core/metrics/IMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/parsers/IParser.py` & `swarmauri-0.2.8.dev1/swarmauri/core/parsers/IParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/prompts/IPromptMatrix.py` & `swarmauri-0.2.8.dev1/swarmauri/core/prompts/IPromptMatrix.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/prompts/ITemplate.py` & `swarmauri-0.2.8.dev1/swarmauri/core/prompts/ITemplate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py` & `swarmauri-0.2.8.dev1/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/swarm_apis/ISwarmAPI.py` & `swarmauri-0.2.8.dev1/swarmauri/core/swarm_apis/ISwarmAPI.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/swarms/ISwarm.py` & `swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarm.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/swarms/ISwarmAgentRegistration.py` & `swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarmAgentRegistration.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/swarms/ISwarmChainCRUD.py` & `swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarmChainCRUD.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/swarms/ISwarmConfigurationExporter.py` & `swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarmConfigurationExporter.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/swarms/ISwarmFactory.py` & `swarmauri-0.2.8.dev1/swarmauri/core/swarms/ISwarmFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/toolkits/IToolkit.py` & `swarmauri-0.2.8.dev1/swarmauri/core/toolkits/IToolkit.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/tools/IParameter.py` & `swarmauri-0.2.8.dev1/swarmauri/core/tools/IParameter.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/tracing/IChainTracer.py` & `swarmauri-0.2.8.dev1/swarmauri/core/tracing/IChainTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/tracing/ITraceContext.py` & `swarmauri-0.2.8.dev1/swarmauri/core/tracing/ITraceContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/tracing/ITracer.py` & `swarmauri-0.2.8.dev1/swarmauri/core/tracing/ITracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/utils/ITransactional.py` & `swarmauri-0.2.8.dev1/swarmauri/core/utils/ITransactional.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IAngleBetweenVectors.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IAngleBetweenVectors.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IDecompose.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IDecompose.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IDivergence.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IDivergence.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IGradient.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IGradient.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IOrthogonalProject.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IOrthogonalProject.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IProject.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IProject.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IReflect.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IReflect.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/ISaveLoadStore.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/ISaveLoadStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/ISimilarity.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/ISimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/ISimiliarityQuery.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/ISimiliarityQuery.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorArithmetic.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorArithmetic.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorBasisCheck.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorBasisCheck.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorLinearCombination.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorLinearCombination.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorNorm.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorNorm.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorRetrieve.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorRetrieve.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorRotate.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorRotate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorSpan.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorSpan.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vector_stores/IVectorStore.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vector_stores/IVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vectorizers/ISaveModel.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vectorizers/ISaveModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vectorizers/IVectorize.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vectorizers/IVectorize.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vectors/IVector.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vectors/IVector.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vectors/IVectorMeta.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vectors/IVectorMeta.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vectors/IVectorProduct.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vectors/IVectorProduct.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/core/vectors/IVectorTransform.py` & `swarmauri-0.2.8.dev1/swarmauri/core/vectors/IVectorTransform.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/chains/TypeAgnosticCallableChain.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/chains/TypeAgnosticCallableChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/conversations/ConsensusBuildingConversation.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/conversations/ConsensusBuildingConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/conversations/SemanticConversation.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/conversations/SemanticConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/CanberraDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/CanberraDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/ChebyshevDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/ChebyshevDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/HaversineDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/HaversineDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/ManhattanDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/ManhattanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/MinkowskiDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/MinkowskiDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/SSASimilarity.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/SSASimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/SSIVSimilarity.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/SSIVSimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/ScannVectorStore.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/ScannVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/SorensenDiceDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/SorensenDiceDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/distances/SquaredEuclideanDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/distances/SquaredEuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/document_stores/TriplesDocumentStore.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/document_stores/TriplesDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/document_stores/Word2VecDocumentStore.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/document_stores/Word2VecDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/models/HierarchicalAttentionModel.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/models/HierarchicalAttentionModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/models/SageMaker.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/models/SageMaker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/parsers/PDFToTextParser.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/parsers/PDFToTextParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/tools/CypherQueryTool.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/tools/CypherQueryTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/tools/FileDownloaderTool.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/tools/FileDownloaderTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/tools/LinkedInArticleTool.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/tools/LinkedInArticleTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/tools/OutlookSendMailTool.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/tools/OutlookSendMailTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/tools/SQLite3QueryTool.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/tools/SQLite3QueryTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/tools/TwitterPostTool.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/tools/TwitterPostTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/tracing/RemoteTrace.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/tracing/RemoteTrace.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/utils/ISerializable.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/utils/ISerializable.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/utils/get_last_frame.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/utils/get_last_frame.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/utils/log_prompt_response.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/utils/log_prompt_response.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/utils/save_schema.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/utils/save_schema.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/vector_stores/TriplesDocumentStore.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/vector_stores/TriplesDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/experimental/vectorizers/DGLVectorizer.py` & `swarmauri-0.2.8.dev1/swarmauri/experimental/vectorizers/DGLVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/AgentFactory.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/JsonAgentFactory.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/JsonAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agents/base/AgentBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/AgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agents/base/SystemContextAgentBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/SystemContextAgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agents/base/VectorStoreAgentBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agents/base/VectorStoreAgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agents/concrete/ChatSwarmAgent.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/ChatSwarmAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agents/concrete/RagAgent.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/RagAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agents/concrete/SimpleConversationAgent.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/SimpleConversationAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/agents/concrete/ToolAgent.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/agents/concrete/ToolAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chains/base/ChainBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/ChainBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chains/base/ChainContextBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/ChainContextBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chains/base/ChainStepBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/ChainStepBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chains/base/PromptContextChainBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chains/base/PromptContextChainBase.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,38 +21,64 @@
         model_kwargs: Dict[str, Any] = {}):
         ChainContextBase.__init__(self)
         self.prompt_matrix = prompt_matrix
         self.response_matrix = PromptMatrix(matrix=[[None for _ in range(prompt_matrix.shape[1])] for _ in range(prompt_matrix.shape[0])])
         self.agents = agents
         self.context = context 
         self.model_kwargs = model_kwargs
+        self.steps = self.build_dependencies()
+        self.current_step_index = 0  # Track the current step in the steps list
 
     @property
     def context(self) -> Dict[str, Any]:
         return self._context
 
     @context.setter
     def context(self, value: Dict[str, Any]) -> None:
         self._context = value
 
-    def execute(self) -> None:
+    def execute(self, build_dependencies=True) -> None:
         """
         Execute the chain of prompts based on the state of the prompt matrix.
         Iterates through each sequence in the prompt matrix, resolves dependencies, 
         and executes prompts in the resolved order.
         """
-        steps = self.build_dependencies()
-        for step in steps:
+        if build_dependencies:
+            self.steps = self.build_dependencies()
+            self.current_step_index = 0
+
+        if self.current_step_index < len(self.steps):    
+            step = self.steps[self.current_step_index]
+            method = step.method
+            args = step.args
+            ref = step.ref
+            result = method(*args)
+            self.context[ref] = result
+            prompt_index = self._extract_step_number(ref)
+            self._update_response_matrix(args[0], prompt_index, result)
+            self.current_step_index += 1  # Move to the next step
+        else:
+            print("All steps have been executed.")
+
+    def execute_next_step(self):
+        """
+        Execute the next step in the steps list if available.
+        """
+        if self.current_step_index < len(self.steps):
+            step = self.steps[self.current_step_index]
             method = step.method
             args = step.args
             ref = step.ref
             result = method(*args)
             self.context[ref] = result
             prompt_index = self._extract_step_number(ref)
             self._update_response_matrix(args[0], prompt_index, result)
+            self.current_step_index += 1  # Move to the next step
+        else:
+            print("All steps have been executed.")
 
     def _execute_prompt(self, agent_index: int, prompt: str, ref: str):
         """
         Executes a given prompt using the specified agent and updates the response.
         """
         formatted_prompt = prompt.format(**self.context)  # Using context for f-string formatting
```

### Comparing `swarmauri-0.2.7/swarmauri/standard/chains/concrete/CallableChain.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/CallableChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chains/concrete/ChainStep.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/ChainStep.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chains/concrete/ContextChain.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/ContextChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chains/concrete/PromptContextChain.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chains/concrete/PromptContextChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/conversations/base/ConversationBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/conversations/base/ConversationBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/conversations/base/SystemContextBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/conversations/base/SystemContextBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/conversations/concrete/MaxSizeConversation.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/MaxSizeConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/conversations/concrete/SessionCacheConversation.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/SessionCacheConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/conversations/concrete/SharedConversation.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/conversations/concrete/SharedConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/distances/concrete/ChiSquaredDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/ChiSquaredDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/distances/concrete/CosineDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/CosineDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/distances/concrete/EuclideanDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/EuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/distances/concrete/JaccardIndexDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/JaccardIndexDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/distances/concrete/LevenshteinDistance.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/distances/concrete/LevenshteinDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/document_stores/base/DocumentStoreBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/base/DocumentStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/documents/base/DocumentBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/documents/base/DocumentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/documents/base/EmbeddedBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/documents/base/EmbeddedBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/messages/base/MessageBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/messages/base/MessageBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/messages/concrete/FunctionMessage.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/messages/concrete/FunctionMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/messages/concrete/HumanMessage.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/messages/concrete/HumanMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/messages/concrete/SystemMessage.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/messages/concrete/SystemMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/base/AggregateMetricBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/AggregateMetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/base/CalculateMetricBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/CalculateMetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/base/MetricBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/MetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/base/ThresholdMetricBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/base/ThresholdMetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/HitRateAtK.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/HitRateAtK.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/ImpressionAtK.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/ImpressionAtK.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/MeanMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/MeanMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/StaticValueMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/StaticValueMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/metrics/concrete/ZeroMetric.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/metrics/concrete/ZeroMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/base/ModelBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/base/ModelBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/AnthropicModel.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/AnthropicModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/AzureGPT.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/AzureGPT.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/CohereModel.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/CohereModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/GeminiProModel.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/GeminiProModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/GroqModel.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/GroqModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/GroqToolModel.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/GroqToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/MistralModel.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/MistralModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/MistralToolModel.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/MistralToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/OpenAIImageGenerator.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/OpenAIImageGenerator.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/OpenAIModel.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/OpenAIModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/models/concrete/OpenAIToolModel.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/models/concrete/OpenAIToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/CSVParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/CSVParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/MarkdownParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/MarkdownParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/PythonParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/PythonParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/RegExParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/RegExParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/TFIDFParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/TFIDFParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/TextBlobNounParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/TextBlobNounParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/URLExtractorParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/URLExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/parsers/concrete/XMLParser.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/parsers/concrete/XMLParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/prompts/base/BasePromptMatrix.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/prompts/base/BasePromptMatrix.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/prompts/concrete/Prompt.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/prompts/concrete/Prompt.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/prompts/concrete/PromptGenerator.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/prompts/concrete/PromptGenerator.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/prompts/concrete/PromptTemplate.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/prompts/concrete/PromptTemplate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/swarms/base/SwarmComponentBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/swarms/base/SwarmComponentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/toolkits/base/ToolkitBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/toolkits/base/ToolkitBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tools/base/ToolBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tools/base/ToolBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tools/concrete/AdditionTool.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/AdditionTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tools/concrete/CalculatorTool.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/CalculatorTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tools/concrete/CodeInterpreterTool.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/CodeInterpreterTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tools/concrete/ImportMemoryModuleTool.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/ImportMemoryModuleTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tools/concrete/Parameter.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/Parameter.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tools/concrete/TestTool.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/TestTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tools/concrete/WeatherTool.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tools/concrete/WeatherTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tracing/concrete/CallableTracer.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/CallableTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tracing/concrete/ChainTracer.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/ChainTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tracing/concrete/SimpleTraceContext.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/SimpleTraceContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tracing/concrete/SimpleTracer.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/SimpleTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tracing/concrete/TracedVariable.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/TracedVariable.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/tracing/concrete/VariableTracer.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/tracing/concrete/VariableTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/utils/decorate.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/utils/decorate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/utils/get_class_hash.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/utils/get_class_hash.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/utils/json_validator.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/utils/json_validator.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/utils/load_documents_from_json.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/utils/load_documents_from_json.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/utils/sql_log.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/utils/sql_log.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vectors/base/VectorBase.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vectors/base/VectorBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri/standard/vectors/concrete/VectorProduct.py` & `swarmauri-0.2.8.dev1/swarmauri/standard/vectors/concrete/VectorProduct.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri.egg-info/PKG-INFO` & `swarmauri-0.2.8.dev1/swarmauri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri
-Version: 0.2.7
+Version: 0.2.8.dev1
 Summary: This repository includes core interfaces, standard ABCs and concrete references, third party plugins, and experimental modules for the swarmaURI framework.
 Home-page: http://github.com/swarmauri/swarmauri-sdk
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri-0.2.7/swarmauri.egg-info/SOURCES.txt` & `swarmauri-0.2.8.dev1/swarmauri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.7/swarmauri.egg-info/requires.txt` & `swarmauri-0.2.8.dev1/swarmauri.egg-info/requires.txt`

 * *Files identical despite different names*

