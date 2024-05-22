# Comparing `tmp/athina-1.2.9.tar.gz` & `tmp/athina-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athina-1.2.9.tar", max compression
+gzip compressed data, was "athina-1.3.0.tar", max compression
```

## Comparing `athina-1.2.9.tar` & `athina-1.3.0.tar`

### file list

```diff
@@ -1,133 +1,143 @@
--rw-r--r--   0        0        0     8595 2024-03-19 22:27:57.176555 athina-1.2.9/README.md
--rw-r--r--   0        0        0      169 2024-04-07 23:05:49.900916 athina-1.2.9/athina/__init__.py
--rw-r--r--   0        0        0     2938 2024-03-19 22:27:57.176822 athina-1.2.9/athina/benchmark/eval_performance_calculator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.176900 athina-1.2.9/athina/cli/__init__.py
--rw-r--r--   0        0        0     5390 2024-04-01 04:55:21.103552 athina-1.2.9/athina/cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177123 athina-1.2.9/athina/constants/__init__.py
--rw-r--r--   0        0        0      517 2024-03-19 22:27:57.177236 athina-1.2.9/athina/constants/messages.py
--rw-r--r--   0        0        0       72 2024-04-07 23:05:49.901344 athina-1.2.9/athina/datasets/__init__.py
--rw-r--r--   0        0        0   218970 2024-03-19 22:27:57.177712 athina-1.2.9/athina/datasets/conversations.json
--rw-r--r--   0        0        0     2971 2024-04-07 23:05:49.901583 athina-1.2.9/athina/datasets/dataset.py
--rw-r--r--   0        0        0     3355 2024-03-19 22:27:57.177821 athina-1.2.9/athina/datasets/summarization_sample.py
--rw-r--r--   0        0        0     2675 2024-03-19 22:27:57.177915 athina-1.2.9/athina/datasets/yc_query_mini.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177993 athina-1.2.9/athina/errors/__init__.py
--rw-r--r--   0        0        0      801 2024-03-19 22:27:57.178079 athina-1.2.9/athina/errors/exceptions.py
--rw-r--r--   0        0        0     4069 2024-04-02 05:23:54.521662 athina-1.2.9/athina/evals/__init__.py
--rw-r--r--   0        0        0     7508 2024-03-27 06:24:44.855919 athina-1.2.9/athina/evals/base_evaluator.py
--rw-r--r--   0        0        0     4253 2024-03-20 00:06:17.768963 athina-1.2.9/athina/evals/conversation/conversation_coherence/evaluator.py
--rw-r--r--   0        0        0     1198 2024-03-19 22:27:57.178641 athina-1.2.9/athina/evals/conversation/conversation_coherence/prompt.py
--rw-r--r--   0        0        0     4408 2024-03-19 22:27:57.178765 athina-1.2.9/athina/evals/conversation/conversation_resolution/evaluator.py
--rw-r--r--   0        0        0     1104 2024-03-19 22:27:57.178845 athina-1.2.9/athina/evals/conversation/conversation_resolution/prompt.py
--rw-r--r--   0        0        0     2470 2024-04-07 23:05:49.901880 athina-1.2.9/athina/evals/eval_type.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179006 athina-1.2.9/athina/evals/function/__init__.py
--rw-r--r--   0        0        0     3599 2024-03-27 06:24:44.856062 athina-1.2.9/athina/evals/function/function_evaluator.py
--rw-r--r--   0        0        0    18806 2024-03-27 11:54:50.117642 athina-1.2.9/athina/evals/function/functions.py
--rw-r--r--   0        0        0    10216 2024-03-27 09:12:43.212033 athina-1.2.9/athina/evals/function/wrapper.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179629 athina-1.2.9/athina/evals/grounded/__init__.py
--rw-r--r--   0        0        0     3879 2024-03-20 16:40:39.753015 athina-1.2.9/athina/evals/grounded/grounded_evaluator.py
--rw-r--r--   0        0        0     4178 2024-03-19 22:27:57.179870 athina-1.2.9/athina/evals/grounded/similarity.py
--rw-r--r--   0        0        0     1708 2024-03-19 22:27:57.179950 athina-1.2.9/athina/evals/grounded/wrapper.py
--rw-r--r--   0        0        0     2961 2024-04-02 05:23:01.185679 athina-1.2.9/athina/evals/guardrails/gibberish_text/evaluator.py
--rw-r--r--   0        0        0     3727 2024-04-02 05:23:01.186096 athina-1.2.9/athina/evals/guardrails/sensitive_topics/evaluator.py
--rw-r--r--   0        0        0     2885 2024-04-02 05:23:01.186344 athina-1.2.9/athina/evals/guardrails/sfw/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180226 athina-1.2.9/athina/evals/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180328 athina-1.2.9/athina/evals/llm/context_contains_enough_information/__init__.py
--rw-r--r--   0        0        0     2671 2024-03-27 03:09:24.346838 athina-1.2.9/athina/evals/llm/context_contains_enough_information/evaluator.py
--rw-r--r--   0        0        0     1867 2024-03-19 22:27:57.180505 athina-1.2.9/athina/evals/llm/context_contains_enough_information/examples.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180583 athina-1.2.9/athina/evals/llm/custom_prompt/__init__.py
--rw-r--r--   0        0        0     2362 2024-03-27 06:24:44.857102 athina-1.2.9/athina/evals/llm/custom_prompt/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180792 athina-1.2.9/athina/evals/llm/does_response_answer_query/__init__.py
--rw-r--r--   0        0        0     2632 2024-03-19 22:27:57.180901 athina-1.2.9/athina/evals/llm/does_response_answer_query/evaluator.py
--rw-r--r--   0        0        0     1186 2024-03-19 22:27:57.180970 athina-1.2.9/athina/evals/llm/does_response_answer_query/examples.py
--rw-r--r--   0        0        0     1238 2024-03-19 22:27:57.181044 athina-1.2.9/athina/evals/llm/example.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181120 athina-1.2.9/athina/evals/llm/faithfulness/__init__.py
--rw-r--r--   0        0        0     2599 2024-03-19 22:27:57.181215 athina-1.2.9/athina/evals/llm/faithfulness/evaluator.py
--rw-r--r--   0        0        0     1335 2024-03-19 22:27:57.181288 athina-1.2.9/athina/evals/llm/faithfulness/examples.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181361 athina-1.2.9/athina/evals/llm/grading_criteria/__init__.py
--rw-r--r--   0        0        0     2080 2024-04-01 04:53:12.884603 athina-1.2.9/athina/evals/llm/grading_criteria/evaluator.py
--rw-r--r--   0        0        0     5821 2024-03-20 00:37:57.522908 athina-1.2.9/athina/evals/llm/groundedness/evaluator.py
--rw-r--r--   0        0        0     1601 2024-03-19 22:27:57.181666 athina-1.2.9/athina/evals/llm/groundedness/prompt.py
--rw-r--r--   0        0        0     4982 2024-03-19 22:27:57.181767 athina-1.2.9/athina/evals/llm/llm_evaluator.py
--rw-r--r--   0        0        0    10915 2024-03-20 02:27:27.436310 athina-1.2.9/athina/evals/llm/summary_accuracy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182165 athina-1.2.9/athina/evals/ragas/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182276 athina-1.2.9/athina/evals/ragas/answer_correctness/__init__.py
--rw-r--r--   0        0        0     2383 2024-03-19 22:27:57.182414 athina-1.2.9/athina/evals/ragas/answer_correctness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182502 athina-1.2.9/athina/evals/ragas/answer_relevancy/__init__.py
--rw-r--r--   0        0        0     2441 2024-03-19 22:27:57.182610 athina-1.2.9/athina/evals/ragas/answer_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182699 athina-1.2.9/athina/evals/ragas/answer_semantic_similarity/__init__.py
--rw-r--r--   0        0        0     2440 2024-03-19 22:27:57.182849 athina-1.2.9/athina/evals/ragas/answer_semantic_similarity/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182961 athina-1.2.9/athina/evals/ragas/coherence/__init__.py
--rw-r--r--   0        0        0     2187 2024-04-13 09:11:12.974405 athina-1.2.9/athina/evals/ragas/coherence/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183170 athina-1.2.9/athina/evals/ragas/conciseness/__init__.py
--rw-r--r--   0        0        0     2223 2024-04-13 09:11:12.974616 athina-1.2.9/athina/evals/ragas/conciseness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183377 athina-1.2.9/athina/evals/ragas/context_precision/__init__.py
--rw-r--r--   0        0        0     2521 2024-04-13 09:11:12.975045 athina-1.2.9/athina/evals/ragas/context_precision/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183558 athina-1.2.9/athina/evals/ragas/context_recall/__init__.py
--rw-r--r--   0        0        0     2316 2024-03-19 22:27:57.183641 athina-1.2.9/athina/evals/ragas/context_recall/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183719 athina-1.2.9/athina/evals/ragas/context_relevancy/__init__.py
--rw-r--r--   0        0        0     2159 2024-03-19 22:27:57.183804 athina-1.2.9/athina/evals/ragas/context_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183882 athina-1.2.9/athina/evals/ragas/faithfulness/__init__.py
--rw-r--r--   0        0        0     2370 2024-04-11 02:35:41.526056 athina-1.2.9/athina/evals/ragas/faithfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184050 athina-1.2.9/athina/evals/ragas/harmfulness/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-13 09:11:12.975249 athina-1.2.9/athina/evals/ragas/harmfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184253 athina-1.2.9/athina/evals/ragas/maliciousness/__init__.py
--rw-r--r--   0        0        0     2127 2024-04-13 09:11:12.975444 athina-1.2.9/athina/evals/ragas/maliciousness/evaluator.py
--rw-r--r--   0        0        0     3298 2024-03-19 22:27:57.184435 athina-1.2.9/athina/evals/ragas/ragas_evaluator.py
--rw-r--r--   0        0        0     5154 2024-04-02 05:28:57.223435 athina-1.2.9/athina/evals/safety/content_moderation/evaluator.py
--rw-r--r--   0        0        0     3299 2024-03-27 06:24:44.857314 athina-1.2.9/athina/evals/safety/pii_detection/evaluator.py
--rw-r--r--   0        0        0     4370 2024-03-27 06:24:44.857479 athina-1.2.9/athina/evals/safety/prompt_injection/evaluator.py
--rw-r--r--   0        0        0      106 2024-03-27 06:24:44.857663 athina-1.2.9/athina/guard/exception.py
--rw-r--r--   0        0        0     1404 2024-04-01 04:53:12.917663 athina-1.2.9/athina/guard/guard.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184508 athina-1.2.9/athina/helpers/__init__.py
--rw-r--r--   0        0        0     4446 2024-03-19 22:27:57.184591 athina-1.2.9/athina/helpers/athina_logging_helper.py
--rw-r--r--   0        0        0     1351 2024-03-19 22:27:57.184662 athina-1.2.9/athina/helpers/config.py
--rw-r--r--   0        0        0      122 2024-03-19 22:27:57.184730 athina-1.2.9/athina/helpers/constants.py
--rw-r--r--   0        0        0      172 2024-03-19 22:27:57.184807 athina-1.2.9/athina/helpers/eval_helper.py
--rw-r--r--   0        0        0      642 2024-03-19 22:27:57.184880 athina-1.2.9/athina/helpers/function_eval_util.py
--rw-r--r--   0        0        0     4405 2024-04-01 04:53:12.911568 athina-1.2.9/athina/helpers/get_evaluator.py
--rw-r--r--   0        0        0     1190 2024-03-19 22:27:57.185041 athina-1.2.9/athina/helpers/json.py
--rw-r--r--   0        0        0      403 2024-03-19 22:27:57.185114 athina-1.2.9/athina/helpers/kwparser.py
--rw-r--r--   0        0        0      894 2024-04-01 04:55:21.103741 athina-1.2.9/athina/helpers/loader_helper.py
--rw-r--r--   0        0        0     3051 2024-03-19 22:27:57.185252 athina-1.2.9/athina/helpers/logger.py
--rw-r--r--   0        0        0      265 2024-03-19 22:27:57.185337 athina-1.2.9/athina/helpers/package_helper.py
--rw-r--r--   0        0        0     5296 2024-03-19 22:27:57.185429 athina-1.2.9/athina/helpers/run_helper.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.185498 athina-1.2.9/athina/interfaces/__init__.py
--rw-r--r--   0        0        0     3905 2024-03-19 22:27:57.185587 athina-1.2.9/athina/interfaces/athina.py
--rw-r--r--   0        0        0      132 2024-03-19 22:27:57.185654 athina-1.2.9/athina/interfaces/data.py
--rw-r--r--   0        0        0     1238 2024-03-27 06:24:44.857991 athina-1.2.9/athina/interfaces/model.py
--rw-r--r--   0        0        0      100 2024-03-19 22:27:57.185783 athina-1.2.9/athina/interfaces/openai.py
--rw-r--r--   0        0        0     2944 2024-03-27 06:24:44.858163 athina-1.2.9/athina/interfaces/result.py
--rw-r--r--   0        0        0      126 2024-03-19 22:27:57.185951 athina-1.2.9/athina/keys/__init__.py
--rw-r--r--   0        0        0      322 2024-03-19 22:27:57.186019 athina-1.2.9/athina/keys/athina_api_key.py
--rw-r--r--   0        0        0      236 2024-03-19 22:27:57.186085 athina-1.2.9/athina/keys/openai_api_key.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.186149 athina-1.2.9/athina/llms/__init__.py
--rw-r--r--   0        0        0     1398 2024-03-19 22:27:57.186244 athina-1.2.9/athina/llms/abstract_llm_service.py
--rw-r--r--   0        0        0     3342 2024-03-19 22:27:57.186314 athina-1.2.9/athina/llms/openai_service.py
--rw-r--r--   0        0        0      337 2024-03-19 22:27:57.186378 athina-1.2.9/athina/llms/question_answerer.py
--rw-r--r--   0        0        0     2874 2024-03-19 22:27:57.186451 athina-1.2.9/athina/llms/question_answerer_bulk.py
--rw-r--r--   0        0        0     3675 2024-03-19 22:27:57.186521 athina-1.2.9/athina/llms/question_answerer_cot.py
--rw-r--r--   0        0        0     6674 2024-03-20 01:02:59.337117 athina-1.2.9/athina/llms/question_answerer_with_retrieval.py
--rw-r--r--   0        0        0     2402 2024-03-19 22:27:57.186684 athina-1.2.9/athina/llms/question_generator.py
--rw-r--r--   0        0        0      323 2024-03-27 06:24:44.858328 athina-1.2.9/athina/loaders/__init__.py
--rw-r--r--   0        0        0     2126 2024-03-19 22:27:57.186849 athina-1.2.9/athina/loaders/base_loader.py
--rw-r--r--   0        0        0     2173 2024-03-19 22:27:57.186916 athina-1.2.9/athina/loaders/conversation_loader.py
--rw-r--r--   0        0        0     4355 2024-03-20 04:43:24.983837 athina-1.2.9/athina/loaders/loader.py
--rw-r--r--   0        0        0     3501 2024-03-19 22:27:57.187089 athina-1.2.9/athina/loaders/response_loader.py
--rw-r--r--   0        0        0     2970 2024-03-19 22:27:57.187156 athina-1.2.9/athina/loaders/summary_loader.py
--rw-r--r--   0        0        0     2380 2024-03-27 06:24:44.858458 athina-1.2.9/athina/loaders/text_loader.py
--rw-r--r--   0        0        0     1854 2024-03-19 22:27:57.187257 athina-1.2.9/athina/metrics/agreement_score.py
--rw-r--r--   0        0        0     2448 2024-03-19 22:27:57.187346 athina-1.2.9/athina/metrics/contradiction_score.py
--rw-r--r--   0        0        0     1342 2024-03-19 22:27:57.187416 athina-1.2.9/athina/metrics/groundedness.py
--rw-r--r--   0        0        0     2209 2024-03-19 22:27:57.187494 athina-1.2.9/athina/metrics/hallucination_score.py
--rw-r--r--   0        0        0      246 2024-03-19 22:27:57.187555 athina-1.2.9/athina/metrics/metric.py
--rw-r--r--   0        0        0     3000 2024-03-20 00:48:19.997400 athina-1.2.9/athina/metrics/metric_type.py
--rw-r--r--   0        0        0      393 2024-03-19 22:27:57.187682 athina-1.2.9/athina/metrics/passed.py
--rw-r--r--   0        0        0      275 2024-03-19 22:27:57.187758 athina-1.2.9/athina/metrics/ragas_metric.py
--rw-r--r--   0        0        0      509 2024-03-19 22:27:57.187846 athina-1.2.9/athina/metrics/similarity_score.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.187933 athina-1.2.9/athina/runner/__init__.py
--rw-r--r--   0        0        0     5510 2024-04-13 09:11:12.976052 athina-1.2.9/athina/runner/run.py
--rw-r--r--   0        0        0      341 2024-04-07 23:05:49.902009 athina-1.2.9/athina/runner/run_wrapper.py
--rw-r--r--   0        0        0     1262 2024-04-02 05:23:08.938087 athina-1.2.9/athina/scripts/guardrails.py
--rw-r--r--   0        0        0    12648 2024-04-07 23:05:49.902313 athina-1.2.9/athina/services/athina_api_service.py
--rw-r--r--   0        0        0      935 2024-04-13 09:14:44.263057 athina-1.2.9/pyproject.toml
--rw-r--r--   0        0        0     9634 1970-01-01 00:00:00.000000 athina-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0     8595 2024-05-03 15:41:49.406642 athina-1.3.0/README.md
+-rw-r--r--   0        0        0      169 2024-05-03 15:41:49.406999 athina-1.3.0/athina/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.176900 athina-1.3.0/athina/cli/__init__.py
+-rw-r--r--   0        0        0     5390 2024-05-05 12:00:16.321612 athina-1.3.0/athina/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177123 athina-1.3.0/athina/constants/__init__.py
+-rw-r--r--   0        0        0      517 2024-03-19 22:27:57.177236 athina-1.3.0/athina/constants/messages.py
+-rw-r--r--   0        0        0       72 2024-05-03 15:41:49.407935 athina-1.3.0/athina/datasets/__init__.py
+-rw-r--r--   0        0        0   218970 2024-05-03 15:41:49.408467 athina-1.3.0/athina/datasets/conversations.json
+-rw-r--r--   0        0        0     3230 2024-05-19 14:25:58.792810 athina-1.3.0/athina/datasets/dataset.py
+-rw-r--r--   0        0        0     3355 2024-03-19 22:27:57.177821 athina-1.3.0/athina/datasets/summarization_sample.py
+-rw-r--r--   0        0        0     2675 2024-05-03 15:41:49.409340 athina-1.3.0/athina/datasets/yc_query_mini.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177993 athina-1.3.0/athina/errors/__init__.py
+-rw-r--r--   0        0        0      801 2024-03-19 22:27:57.178079 athina-1.3.0/athina/errors/exceptions.py
+-rw-r--r--   0        0        0     4069 2024-05-03 15:41:49.409717 athina-1.3.0/athina/evals/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-16 19:27:48.886844 athina-1.3.0/athina/evals/base_evaluator.py
+-rw-r--r--   0        0        0     4259 2024-05-16 19:27:48.887245 athina-1.3.0/athina/evals/conversation/conversation_coherence/evaluator.py
+-rw-r--r--   0        0        0     1198 2024-05-03 15:41:49.410542 athina-1.3.0/athina/evals/conversation/conversation_coherence/prompt.py
+-rw-r--r--   0        0        0     4414 2024-05-16 19:27:48.887449 athina-1.3.0/athina/evals/conversation/conversation_resolution/evaluator.py
+-rw-r--r--   0        0        0     1104 2024-05-03 15:41:49.410767 athina-1.3.0/athina/evals/conversation/conversation_resolution/prompt.py
+-rw-r--r--   0        0        0     2579 2024-05-03 15:41:49.411157 athina-1.3.0/athina/evals/eval_type.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179006 athina-1.3.0/athina/evals/function/__init__.py
+-rw-r--r--   0        0        0     3780 2024-05-16 19:27:48.888106 athina-1.3.0/athina/evals/function/function_evaluator.py
+-rw-r--r--   0        0        0    18806 2024-05-03 15:41:49.412956 athina-1.3.0/athina/evals/function/functions.py
+-rw-r--r--   0        0        0    10216 2024-05-03 15:41:49.414039 athina-1.3.0/athina/evals/function/wrapper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179629 athina-1.3.0/athina/evals/grounded/__init__.py
+-rw-r--r--   0        0        0     4298 2024-05-16 19:27:48.888364 athina-1.3.0/athina/evals/grounded/grounded_evaluator.py
+-rw-r--r--   0        0        0     4178 2024-03-19 22:27:57.179870 athina-1.3.0/athina/evals/grounded/similarity.py
+-rw-r--r--   0        0        0     1708 2024-03-19 22:27:57.179950 athina-1.3.0/athina/evals/grounded/wrapper.py
+-rw-r--r--   0        0        0     3041 2024-05-16 19:27:48.889059 athina-1.3.0/athina/evals/guardrails/gibberish_text/evaluator.py
+-rw-r--r--   0        0        0     3797 2024-05-16 19:27:48.889242 athina-1.3.0/athina/evals/guardrails/sensitive_topics/evaluator.py
+-rw-r--r--   0        0        0     2965 2024-05-16 19:27:48.889409 athina-1.3.0/athina/evals/guardrails/sfw/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180226 athina-1.3.0/athina/evals/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180328 athina-1.3.0/athina/evals/llm/context_contains_enough_information/__init__.py
+-rw-r--r--   0        0        0     3004 2024-05-16 19:27:48.889580 athina-1.3.0/athina/evals/llm/context_contains_enough_information/evaluator.py
+-rw-r--r--   0        0        0     1867 2024-03-19 22:27:57.180505 athina-1.3.0/athina/evals/llm/context_contains_enough_information/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180583 athina-1.3.0/athina/evals/llm/custom_prompt/__init__.py
+-rw-r--r--   0        0        0     2483 2024-05-16 19:27:48.889741 athina-1.3.0/athina/evals/llm/custom_prompt/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180792 athina-1.3.0/athina/evals/llm/does_response_answer_query/__init__.py
+-rw-r--r--   0        0        0     2632 2024-05-03 15:41:49.417364 athina-1.3.0/athina/evals/llm/does_response_answer_query/evaluator.py
+-rw-r--r--   0        0        0     1186 2024-03-19 22:27:57.180970 athina-1.3.0/athina/evals/llm/does_response_answer_query/examples.py
+-rw-r--r--   0        0        0     1238 2024-03-19 22:27:57.181044 athina-1.3.0/athina/evals/llm/example.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181120 athina-1.3.0/athina/evals/llm/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2599 2024-05-03 15:41:49.417490 athina-1.3.0/athina/evals/llm/faithfulness/evaluator.py
+-rw-r--r--   0        0        0     1335 2024-03-19 22:27:57.181288 athina-1.3.0/athina/evals/llm/faithfulness/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181361 athina-1.3.0/athina/evals/llm/grading_criteria/__init__.py
+-rw-r--r--   0        0        0     2209 2024-05-16 19:27:48.889913 athina-1.3.0/athina/evals/llm/grading_criteria/evaluator.py
+-rw-r--r--   0        0        0     5821 2024-05-03 15:41:49.418273 athina-1.3.0/athina/evals/llm/groundedness/evaluator.py
+-rw-r--r--   0        0        0     1601 2024-03-19 22:27:57.181666 athina-1.3.0/athina/evals/llm/groundedness/prompt.py
+-rw-r--r--   0        0        0     4982 2024-05-05 09:24:29.466550 athina-1.3.0/athina/evals/llm/llm_evaluator.py
+-rw-r--r--   0        0        0    10915 2024-05-03 15:41:49.418745 athina-1.3.0/athina/evals/llm/summary_accuracy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182165 athina-1.3.0/athina/evals/ragas/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182276 athina-1.3.0/athina/evals/ragas/answer_correctness/__init__.py
+-rw-r--r--   0        0        0     2383 2024-05-03 15:41:49.419035 athina-1.3.0/athina/evals/ragas/answer_correctness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182502 athina-1.3.0/athina/evals/ragas/answer_relevancy/__init__.py
+-rw-r--r--   0        0        0     2441 2024-05-03 15:41:49.419202 athina-1.3.0/athina/evals/ragas/answer_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182699 athina-1.3.0/athina/evals/ragas/answer_semantic_similarity/__init__.py
+-rw-r--r--   0        0        0     2440 2024-05-03 15:41:49.419340 athina-1.3.0/athina/evals/ragas/answer_semantic_similarity/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182961 athina-1.3.0/athina/evals/ragas/coherence/__init__.py
+-rw-r--r--   0        0        0     2187 2024-05-03 15:41:49.419789 athina-1.3.0/athina/evals/ragas/coherence/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183170 athina-1.3.0/athina/evals/ragas/conciseness/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-03 15:41:49.420084 athina-1.3.0/athina/evals/ragas/conciseness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183377 athina-1.3.0/athina/evals/ragas/context_precision/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-03 15:41:49.420494 athina-1.3.0/athina/evals/ragas/context_precision/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183558 athina-1.3.0/athina/evals/ragas/context_recall/__init__.py
+-rw-r--r--   0        0        0     2316 2024-05-03 15:41:49.420634 athina-1.3.0/athina/evals/ragas/context_recall/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183719 athina-1.3.0/athina/evals/ragas/context_relevancy/__init__.py
+-rw-r--r--   0        0        0     2159 2024-05-03 15:41:49.420776 athina-1.3.0/athina/evals/ragas/context_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183882 athina-1.3.0/athina/evals/ragas/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2370 2024-05-03 15:41:49.420918 athina-1.3.0/athina/evals/ragas/faithfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184050 athina-1.3.0/athina/evals/ragas/harmfulness/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-03 15:41:49.421222 athina-1.3.0/athina/evals/ragas/harmfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184253 athina-1.3.0/athina/evals/ragas/maliciousness/__init__.py
+-rw-r--r--   0        0        0     2127 2024-05-03 15:41:49.421640 athina-1.3.0/athina/evals/ragas/maliciousness/evaluator.py
+-rw-r--r--   0        0        0     3298 2024-05-03 15:41:49.421803 athina-1.3.0/athina/evals/ragas/ragas_evaluator.py
+-rw-r--r--   0        0        0     5154 2024-05-03 15:41:49.422152 athina-1.3.0/athina/evals/safety/content_moderation/evaluator.py
+-rw-r--r--   0        0        0     3387 2024-05-03 15:41:49.422800 athina-1.3.0/athina/evals/safety/pii_detection/evaluator.py
+-rw-r--r--   0        0        0     4370 2024-05-03 15:41:49.424028 athina-1.3.0/athina/evals/safety/prompt_injection/evaluator.py
+-rw-r--r--   0        0        0      106 2024-05-03 15:41:49.424321 athina-1.3.0/athina/guard/exception.py
+-rw-r--r--   0        0        0     1404 2024-05-03 15:41:49.424686 athina-1.3.0/athina/guard/guard.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184508 athina-1.3.0/athina/helpers/__init__.py
+-rw-r--r--   0        0        0     5739 2024-05-16 19:27:48.890218 athina-1.3.0/athina/helpers/athina_logging_helper.py
+-rw-r--r--   0        0        0     1351 2024-03-19 22:27:57.184662 athina-1.3.0/athina/helpers/config.py
+-rw-r--r--   0        0        0      122 2024-03-19 22:27:57.184730 athina-1.3.0/athina/helpers/constants.py
+-rw-r--r--   0        0        0      790 2024-05-16 19:27:48.890420 athina-1.3.0/athina/helpers/dataset_helper.py
+-rw-r--r--   0        0        0      172 2024-03-19 22:27:57.184807 athina-1.3.0/athina/helpers/eval_helper.py
+-rw-r--r--   0        0        0      642 2024-03-19 22:27:57.184880 athina-1.3.0/athina/helpers/function_eval_util.py
+-rw-r--r--   0        0        0     4591 2024-05-03 15:41:49.425070 athina-1.3.0/athina/helpers/get_evaluator.py
+-rw-r--r--   0        0        0     2469 2024-05-22 07:52:50.227484 athina-1.3.0/athina/helpers/json.py
+-rw-r--r--   0        0        0      403 2024-03-19 22:27:57.185114 athina-1.3.0/athina/helpers/kwparser.py
+-rw-r--r--   0        0        0      894 2024-05-03 15:41:49.425348 athina-1.3.0/athina/helpers/loader_helper.py
+-rw-r--r--   0        0        0     3051 2024-03-19 22:27:57.185252 athina-1.3.0/athina/helpers/logger.py
+-rw-r--r--   0        0        0      265 2024-03-19 22:27:57.185337 athina-1.3.0/athina/helpers/package_helper.py
+-rw-r--r--   0        0        0     5296 2024-03-19 22:27:57.185429 athina-1.3.0/athina/helpers/run_helper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.185498 athina-1.3.0/athina/interfaces/__init__.py
+-rw-r--r--   0        0        0     3905 2024-05-03 15:41:49.425463 athina-1.3.0/athina/interfaces/athina.py
+-rw-r--r--   0        0        0      132 2024-03-19 22:27:57.185654 athina-1.3.0/athina/interfaces/data.py
+-rw-r--r--   0        0        0     2065 2024-05-14 15:59:10.451321 athina-1.3.0/athina/interfaces/model.py
+-rw-r--r--   0        0        0      100 2024-03-19 22:27:57.185783 athina-1.3.0/athina/interfaces/openai.py
+-rw-r--r--   0        0        0     2944 2024-05-05 12:12:32.954417 athina-1.3.0/athina/interfaces/result.py
+-rw-r--r--   0        0        0      126 2024-03-19 22:27:57.185951 athina-1.3.0/athina/keys/__init__.py
+-rw-r--r--   0        0        0      322 2024-03-19 22:27:57.186019 athina-1.3.0/athina/keys/athina_api_key.py
+-rw-r--r--   0        0        0      236 2024-03-19 22:27:57.186085 athina-1.3.0/athina/keys/openai_api_key.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.186149 athina-1.3.0/athina/llms/__init__.py
+-rw-r--r--   0        0        0     1368 2024-05-22 07:52:50.227988 athina-1.3.0/athina/llms/abstract_llm_service.py
+-rw-r--r--   0        0        0     1524 2024-05-22 07:52:50.228405 athina-1.3.0/athina/llms/litellm_service.py
+-rw-r--r--   0        0        0     3461 2024-05-22 07:52:50.228694 athina-1.3.0/athina/llms/openai_service.py
+-rw-r--r--   0        0        0      337 2024-03-19 22:27:57.186378 athina-1.3.0/athina/llms/question_answerer.py
+-rw-r--r--   0        0        0     2874 2024-05-21 13:33:12.522927 athina-1.3.0/athina/llms/question_answerer_bulk.py
+-rw-r--r--   0        0        0     3675 2024-03-19 22:27:57.186521 athina-1.3.0/athina/llms/question_answerer_cot.py
+-rw-r--r--   0        0        0     6674 2024-05-03 15:41:49.426272 athina-1.3.0/athina/llms/question_answerer_with_retrieval.py
+-rw-r--r--   0        0        0     2402 2024-03-19 22:27:57.186684 athina-1.3.0/athina/llms/question_generator.py
+-rw-r--r--   0        0        0      323 2024-05-03 15:41:49.426530 athina-1.3.0/athina/loaders/__init__.py
+-rw-r--r--   0        0        0     2326 2024-05-16 23:56:49.987467 athina-1.3.0/athina/loaders/base_loader.py
+-rw-r--r--   0        0        0     2179 2024-05-16 19:27:48.890989 athina-1.3.0/athina/loaders/conversation_loader.py
+-rw-r--r--   0        0        0     6507 2024-05-17 01:08:19.006440 athina-1.3.0/athina/loaders/loader.py
+-rw-r--r--   0        0        0     3597 2024-05-16 19:27:48.892946 athina-1.3.0/athina/loaders/response_loader.py
+-rw-r--r--   0        0        0     2970 2024-05-03 17:07:59.624449 athina-1.3.0/athina/loaders/summary_loader.py
+-rw-r--r--   0        0        0     2380 2024-05-03 15:41:49.427400 athina-1.3.0/athina/loaders/text_loader.py
+-rw-r--r--   0        0        0     1854 2024-03-19 22:27:57.187257 athina-1.3.0/athina/metrics/agreement_score.py
+-rw-r--r--   0        0        0     2448 2024-03-19 22:27:57.187346 athina-1.3.0/athina/metrics/contradiction_score.py
+-rw-r--r--   0        0        0     1342 2024-03-19 22:27:57.187416 athina-1.3.0/athina/metrics/groundedness.py
+-rw-r--r--   0        0        0     2209 2024-03-19 22:27:57.187494 athina-1.3.0/athina/metrics/hallucination_score.py
+-rw-r--r--   0        0        0      246 2024-03-19 22:27:57.187555 athina-1.3.0/athina/metrics/metric.py
+-rw-r--r--   0        0        0     3000 2024-05-03 15:41:49.427514 athina-1.3.0/athina/metrics/metric_type.py
+-rw-r--r--   0        0        0      393 2024-03-19 22:27:57.187682 athina-1.3.0/athina/metrics/passed.py
+-rw-r--r--   0        0        0      275 2024-03-19 22:27:57.187758 athina-1.3.0/athina/metrics/ragas_metric.py
+-rw-r--r--   0        0        0      509 2024-03-19 22:27:57.187846 athina-1.3.0/athina/metrics/similarity_score.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.187933 athina-1.3.0/athina/runner/__init__.py
+-rw-r--r--   0        0        0     6940 2024-05-16 19:27:48.893298 athina-1.3.0/athina/runner/run.py
+-rw-r--r--   0        0        0      341 2024-05-03 15:41:49.427983 athina-1.3.0/athina/runner/run_wrapper.py
+-rw-r--r--   0        0        0     1781 2024-05-03 15:41:49.428243 athina-1.3.0/athina/scripts/guardrails.py
+-rw-r--r--   0        0        0    13804 2024-05-19 14:25:58.794110 athina-1.3.0/athina/services/athina_api_service.py
+-rw-r--r--   0        0        0      472 2024-05-22 07:52:50.229087 athina-1.3.0/athina/steps/__init__.py
+-rw-r--r--   0        0        0     1582 2024-05-22 07:52:50.229307 athina-1.3.0/athina/steps/api.py
+-rw-r--r--   0        0        0     4456 2024-05-22 07:52:50.229580 athina-1.3.0/athina/steps/base.py
+-rw-r--r--   0        0        0     1729 2024-05-22 07:52:50.229864 athina-1.3.0/athina/steps/chain.py
+-rw-r--r--   0        0        0     1501 2024-05-22 07:52:50.230002 athina-1.3.0/athina/steps/conditional.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:52:50.230033 athina-1.3.0/athina/steps/debug.py
+-rw-r--r--   0        0        0      646 2024-05-22 07:52:50.230202 athina-1.3.0/athina/steps/iterator.py
+-rw-r--r--   0        0        0     3187 2024-05-22 07:52:50.230415 athina-1.3.0/athina/steps/llm.py
+-rw-r--r--   0        0        0      787 2024-05-22 07:52:50.230543 athina-1.3.0/athina/steps/transform.py
+-rw-r--r--   0        0        0      978 2024-05-22 07:52:50.232786 athina-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9705 1970-01-01 00:00:00.000000 athina-1.3.0/PKG-INFO
```

### Comparing `athina-1.2.9/README.md` & `athina-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/cli/cli.py` & `athina-1.3.0/athina/cli/cli.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/constants/messages.py` & `athina-1.3.0/athina/constants/messages.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/datasets/conversations.json` & `athina-1.3.0/athina/datasets/conversations.json`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/datasets/dataset.py` & `athina-1.3.0/athina/datasets/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,17 @@
                 "name": name,
                 "description": description,
                 "language_model_id": language_model_id,
                 "prompt_template": prompt_template,
                 "dataset_rows": rows or []
             }
         
+        # Remove keys where the value is None
+        dataset_data = {k: v for k, v in dataset_data.items() if v is not None}
+        
         try:
             created_dataset_data = AthinaApiService.create_dataset(dataset_data)
         except Exception as e:
             raise
         dataset = Dataset(id=created_dataset_data['id'], source=created_dataset_data['source'], name=created_dataset_data['name'], description=created_dataset_data['description'], language_model_id=created_dataset_data['language_model_id'], prompt_template=created_dataset_data['prompt_template'])
         return dataset
 
@@ -69,9 +72,13 @@
         for i in range(0, len(rows), batch_size):
             batch = rows[i:i+batch_size]
             try:
                 AthinaApiService.add_dataset_rows(dataset_id, batch)
             except Exception as e:
                 raise
     
+    @staticmethod
+    def dataset_link(dataset_id: str):
+        return f"https://app.athina.ai/datasets/{dataset_id}"
+
```

### Comparing `athina-1.2.9/athina/datasets/summarization_sample.py` & `athina-1.3.0/athina/datasets/summarization_sample.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/datasets/yc_query_mini.py` & `athina-1.3.0/athina/datasets/yc_query_mini.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/errors/exceptions.py` & `athina-1.3.0/athina/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/__init__.py` & `athina-1.3.0/athina/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/base_evaluator.py` & `athina-1.3.0/athina/evals/base_evaluator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor, as_completed
-from typing import List, Optional
+from typing import List, Optional, Dict
 from athina.helpers.logger import logger
 from athina.helpers.athina_logging_helper import AthinaLoggingHelper
-from athina.interfaces.athina import AthinaExperiment
+from athina.helpers.dataset_helper import generate_unique_dataset_name
 from athina.interfaces.data import DataPoint
 from athina.interfaces.result import BatchRunResult, EvalResult, GuardResult
 from athina.services.athina_api_service import AthinaApiService
+from athina.datasets import Dataset
 import traceback
 
 
 class BaseEvaluator(ABC):
-    _experiment: Optional[AthinaExperiment] = None
-
+    
     # Abstract properties
     @property
     @abstractmethod
     def name(self) -> str:
         """A unique name identifier for the evaluator."""
         pass
 
@@ -49,23 +49,22 @@
         """A method to determine if the evaluation failed."""
         pass
 
     @abstractmethod
     def _evaluate(self, **kwargs) -> EvalResult:
         """The method that performs the evaluation."""
         pass
+    
+    def to_config(self) -> Optional[Dict]:
+        return None
 
     # Common methods
     def _examples_str(self) -> str:
         return "" if self.examples is None else "\n".join(map(str, self.examples))
 
-    def configure_experiment(self, experiment: AthinaExperiment):
-        """Configured metadata parameters to log an experiment to Athina"""
-        self._experiment = experiment
-        return self
 
     def validate_args(self, **kwargs) -> None:
         """
         Validates that all required arguments are present and not None.
         """
         for arg in self.required_args:
             if arg not in kwargs:
@@ -95,28 +94,18 @@
         Logs usage to Athina for analytics and creates an evaluation request.
         """
         eval_request_id = None
         try:
             eval_request_id = AthinaLoggingHelper.create_eval_request(
                 eval_name=self.name, request_data={"data": data}, request_type="batch"
             )
-            self._log_experiment(eval_request_id)
         except Exception as e:
             pass
         return eval_request_id
 
-    def _log_experiment(self, eval_request_id: Optional[str]):
-        """
-        Logs experiment to Athina if there is an ongoing experiment.
-        """
-        if self._experiment and eval_request_id:
-            AthinaLoggingHelper.log_experiment(
-                eval_request_id=eval_request_id,
-                experiment=self._experiment,
-            )
 
     def _log_evaluation_results(
         self, eval_request_id: Optional[str], eval_results: List[EvalResult]
     ):
         """
         Logs the evaluation results to Athina if the eval_request_id is available.
         """
@@ -189,30 +178,69 @@
             try:
                 yield self._evaluate(**entry)
             except Exception as e:
                 logger.error(f"Error evaluating entry {entry}: {e}")
                 traceback.print_exc()
                 yield None
 
+    def _log_dataset_to_athina(self, data: List[DataPoint]) -> Optional[str]:
+        """
+        Logs the dataset to Athina
+        """
+        try: 
+            dataset = Dataset.create(
+                name=generate_unique_dataset_name(),
+                rows=data
+            )
+            return dataset
+        except Exception as e:
+            print(f"Error logging dataset to Athina: {e}")
+            return None
+    
+    def _log_eval_results_to_athina(self, eval_results: List[EvalResult], dataset_id: str):
+        """
+        Logs the batch results to Athina
+        """
+        try:
+            eval_config = self.to_config()
+            llm_engine = getattr(self, "_model", None)
+            AthinaLoggingHelper.log_eval_results_with_config(
+                eval_results_with_config={
+                    "eval_results": eval_results,
+                    "development_eval_config": {
+                        "eval_type_id": self.name,
+                        "eval_display_name": self.display_name,
+                        "eval_config": eval_config,
+                        "llm_engine": llm_engine
+                    }
+                },
+                dataset_id=dataset_id
+            )
+        except Exception as e:
+            print(f"Error logging eval results to Athina: {e}")
+            pass
+    
     def run_batch(
         self, data: List[DataPoint], max_parallel_evals: int = 5
     ) -> BatchRunResult:
         """
         Runs the evaluator on a batch of data.
         """
         # Log usage to Athina for analytics
         AthinaApiService.log_usage(eval_name=self.name, run_type="batch")
-        eval_request_id = self._log_evaluation_request(data)
 
         # Run the evaluations
         if max_parallel_evals > 1:
             eval_results = self._run_batch_generator_async(data, max_parallel_evals)
         else:
             eval_results = list(self._run_batch_generator(data))
 
-        # Log evaluation results to Athina
-        self._log_evaluation_results(eval_request_id, eval_results)
+        # Create the Dataset
+        dataset = self._log_dataset_to_athina(data)
+        if dataset:
+            self._log_eval_results_to_athina(eval_results, dataset.id)
+            print(f"You can view your dataset at: {Dataset.dataset_link(dataset.id)}")
+        
 
         return BatchRunResult(
-            eval_request_id=eval_request_id,
             eval_results=eval_results,
         )
```

### Comparing `athina-1.2.9/athina/evals/conversation/conversation_coherence/evaluator.py` & `athina-1.3.0/athina/evals/conversation/conversation_coherence/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from typing import List, Optional
+from typing import List, Optional, Dict
 
 from athina.helpers import logger
 from athina.interfaces.model import Model
 from athina.interfaces.result import EvalResult, EvalResultMetric
 from athina.evals.llm.llm_evaluator import LlmEvaluator
 from athina.evals.eval_type import ConversationEvalTypeId
 from athina.metrics.metric_type import MetricType
```

### Comparing `athina-1.2.9/athina/evals/conversation/conversation_coherence/prompt.py` & `athina-1.3.0/athina/evals/conversation/conversation_coherence/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/conversation/conversation_resolution/evaluator.py` & `athina-1.3.0/athina/evals/conversation/conversation_resolution/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from typing import List, Optional
+from typing import List, Optional, Dict
 
 from athina.interfaces.model import Model
 from athina.interfaces.result import EvalResult, EvalResultMetric
 from athina.evals.llm.llm_evaluator import LlmEvaluator
 from athina.evals.eval_type import ConversationEvalTypeId
 from athina.metrics.metric_type import MetricType
 from .prompt import SYSTEM_MESSAGE, USER_MESSAGE
```

### Comparing `athina-1.2.9/athina/evals/conversation/conversation_resolution/prompt.py` & `athina-1.3.0/athina/evals/conversation/conversation_resolution/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/eval_type.py` & `athina-1.3.0/athina/evals/eval_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class LlmEvalTypeId(Enum):
     CONTEXT_CONTAINS_ENOUGH_INFORMATION = "Ccei"
     DOES_RESPONSE_ANSWER_QUERY = "Draq"
     FAITHFULNESS = "Irftc"
     GRADING_CRITERIA = "GradingCriteria"
     CUSTOM_PROMPT = "CustomPrompt"
     SUMMARIZATION_HAL = "SummarizationHal"
+    GROUNDEDNESS = "Groundedness"
 
 class RagasEvalTypeId(Enum):
     RAGAS_CONTEXT_RELEVANCY = "RagasContextRelevancy"
     RAGAS_ANSWER_RELEVANCY = "RagasAnswerRelevancy"
     RAGAS_CONTEXT_PRECISION = "RagasContextPrecision"
     RAGAS_FAITHFULNESS = "RagasFaithfulness"
     RAGAS_CONTEXT_RECALL = "RagasContextRecall"
@@ -45,14 +46,16 @@
     LENGTH_LESS_THAN = "LengthLessThan"
     LENGTH_GREATER_THAN = "LengthGreaterThan"
     API_CALL = "ApiCall"
     SAFE_FOR_WORK_TEXT = "SafeForWorkText"
     NOT_GIBBERISH_TEXT = "NotGibberishText"
     CONTAINS_NO_SENSITIVE_TOPICS = "ContainsNoSensitiveTopics"
     OPENAI_CONTENT_MODERATION = "OpenAiContentModeration"
+    PII_DETECTION = "PiiDetection"
+    PROMPT_INJECTION= "PromptInjection"
     
 class GroundedEvalTypeId(Enum):
     ANSWER_SIMILARITY = "AnswerSimilarity"
     CONTEXT_SIMILARITY = "ContextSimilarity"
 
 def is_llm_eval(evaluator_type: str) -> bool:
     return any(evaluator_type == member.value for member in LlmEvalTypeId)
```

### Comparing `athina-1.2.9/athina/evals/function/function_evaluator.py` & `athina-1.3.0/athina/evals/function/function_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, List
 from athina.metrics.metric_type import MetricType
 import time
-from typing import Optional
+from typing import Optional, Dict
 from athina.interfaces.result import EvalResult, EvalResultMetric
 from athina.helpers.logger import logger
 from athina.interfaces.athina import AthinaExperiment
 from ..base_evaluator import BaseEvaluator
 from .functions import operations
 
 
@@ -69,14 +69,20 @@
     def is_failure(self, eval_response) -> Optional[bool]:
         return (
             not eval_response["result"]
             if eval_response is not None and "result" in eval_response
             else None
         )
 
+    def to_config(self) -> Optional[Dict]:
+        if not self._function_arguments:
+            return None
+        else:
+            return self._function_arguments
+        
     def _evaluate(self, **kwargs) -> EvalResult:
         """
         Run the Function evaluator.
         """
         start_time = time.perf_counter()
 
         # Validate that correct args were passed
```

### Comparing `athina-1.2.9/athina/evals/function/functions.py` & `athina-1.3.0/athina/evals/function/functions.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/function/wrapper.py` & `athina-1.3.0/athina/evals/function/wrapper.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/grounded/grounded_evaluator.py` & `athina-1.3.0/athina/evals/grounded/grounded_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from athina.helpers.logger import logger
 from athina.interfaces.athina import AthinaExperiment
 from ..base_evaluator import BaseEvaluator
 
 class GroundedEvaluator(BaseEvaluator):
 
     _comparator: Comparator
+    _failure_threshold = None
 
     """
     This evaluator runs the requested grounded evaluator on the given data.
     """
 
     @property
     def _model(self):
@@ -46,25 +47,37 @@
             raise ValueError(f"comparator is a required argument") 
         else:
             self._comparator = comparator
         if failure_threshold is not None:
             self._failure_threshold = failure_threshold
 
     def _process_kwargs(self, required_args, **kwargs):
-        required_args_map = {key: kwargs[key] for key in required_args}
+        required_args_map = {
+            key: "\n".join(kwargs[key]) if key == "context" and isinstance(kwargs[key], list) else kwargs[key] 
+            for key in required_args
+        }
         if len(required_args_map) == 2:
             values = list(required_args_map.values())
             if all(isinstance(value, str) for value in values):
                 string1, string2 = values
                 return string1, string2
             else:
                 raise ValueError("Both arguments must be strings.")
         else:
             raise ValueError("Exactly two arguments are required.")
 
+    def to_config(self):
+        config = {
+            "similarity_function": self._comparator.__class__.__name__,
+        }
+        if self._failure_threshold is not None:
+            config["failure_threshold"] = self._failure_threshold
+        return config
+    
+    
     def is_failure(self, score) -> Optional[bool]:
         return bool(score < self._failure_threshold) if self._failure_threshold is not None else None
 
     def _evaluate(self, **kwargs) -> EvalResult:
         """
         Run the Function evaluator.
         """
```

### Comparing `athina-1.2.9/athina/evals/grounded/similarity.py` & `athina-1.3.0/athina/evals/grounded/similarity.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/grounded/wrapper.py` & `athina-1.3.0/athina/evals/grounded/wrapper.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/guardrails/gibberish_text/evaluator.py` & `athina-1.3.0/athina/evals/guardrails/gibberish_text/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Guardrails Gibberish Evaluator
 # https://hub.guardrailsai.com/validator/guardrails/gibberish_text
 
 import time
-from typing import List
+from typing import Dict, List, Optional
 from athina.helpers.logger import logger
 from ...base_evaluator import BaseEvaluator
 from athina.metrics.metric_type import MetricType
 from athina.interfaces.result import EvalResult, EvalResultMetric
 
 
 # Passes when the text is sensible, fails when the text is gibberish.
@@ -46,14 +46,17 @@
     def required_args(self) -> List[str]:
         return ["response"]  # TODO: allow running this on user_query OR response
 
     @property
     def examples(self):
         pass
 
+    def to_config(self) -> Optional[Dict]:
+        return None
+
     def is_failure(self, result: bool) -> bool:
         return not(bool(result))
 
     def _evaluate(self, **kwargs) -> EvalResult:
         """
         Run the Guardrails evaluator.
         """
```

### Comparing `athina-1.2.9/athina/evals/guardrails/sensitive_topics/evaluator.py` & `athina-1.3.0/athina/evals/guardrails/sensitive_topics/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Guardrails Sensitive topics Evaluator
 # https://hub.guardrailsai.com/validator/guardrails/sensitive_topics
 
 import os
 import time
-from typing import List, Optional
+from typing import List, Optional, Dict
 from athina.interfaces.result import EvalResult, EvalResultMetric
 from athina.helpers.logger import logger
 from athina.errors.exceptions import NoOpenAiApiKeyException
 from athina.keys import OpenAiApiKey
 from ...base_evaluator import BaseEvaluator
 from athina.metrics.metric_type import MetricType
 
@@ -52,14 +52,17 @@
     def required_args(self) -> List[str]:
         return ["response"]  # TODO: allow running this on user_query OR response
 
     @property
     def examples(self):
         pass
 
+    def to_config(self) -> Optional[Dict]:
+        return None
+
     def is_failure(self, result: bool) -> bool:
         return not(bool(result))
 
     def _evaluate(self, **kwargs) -> EvalResult:
         from guardrails import Guard
         """
         Run the Guardrails evaluator.
```

### Comparing `athina-1.2.9/athina/evals/guardrails/sfw/evaluator.py` & `athina-1.3.0/athina/evals/guardrails/sfw/evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Guardrails NSFW Evaluator
 # https://hub.guardrailsai.com/validator/guardrails/nsfw_text
 
 import time
-from typing import List
+from typing import List, Optional, Dict
 from athina.helpers.logger import logger
 from ...base_evaluator import BaseEvaluator
 from athina.metrics.metric_type import MetricType
 from athina.interfaces.result import EvalResult, EvalResultMetric
 
 # Passes when the text is SFW, fails when the text is NSFW.
 class SafeForWorkText(BaseEvaluator):
@@ -44,14 +44,17 @@
     def required_args(self) -> List[str]:
         return ["response"]  # TODO: allow running this on user_query OR response
 
     @property
     def examples(self):
         pass
 
+    def to_config(self) -> Optional[Dict]:
+        return None
+
     def is_failure(self, result: bool) -> bool:
         return not(bool(result))
 
     def _evaluate(self, **kwargs) -> EvalResult:
         """
         Run the Guardrails nsfw evaluator.
         """
```

### Comparing `athina-1.2.9/athina/evals/llm/context_contains_enough_information/evaluator.py` & `athina-1.3.0/athina/evals/llm/context_contains_enough_information/evaluator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Dict
 from ..llm_evaluator import LlmEvaluator
 from .examples import CONTEXT_CONTAINS_ENOUGH_INFORMATION_EXAMPLES
 from athina.evals.eval_type import LlmEvalTypeId
 from athina.metrics.metric_type import MetricType
 
 
 class ContextContainsEnoughInformation(LlmEvaluator):
@@ -12,26 +12,28 @@
 
     SYSTEM_MESSAGE_TEMPLATE = """
     You are an expert at evaluating whether a chatbot can answer a user's query using ONLY the information provided to you as context.
     You are not concerned with factual correctness or accuracy. You only care whether the context contains enough information to answer the user's query.
     """
 
     USER_MESSAGE_TEMPLATE = """
-        Let's think step by step:
+    Let's think step by step:
 
-        1. Consider the following: 
-        user's query: {query}.
-        context: {context}.
-        2. Determine if the chatbot can answer the user's query with nothing but the "context" information provided to you.
-        3. Provide a brief explanation of why the context does or does not contain sufficient information, labeled as 'explanation', leading up to a verdict (Pass/Fail) labeled as 'result'.
-        4. Always return a JSON object in the following format: "result": 'result', "explanation": 'explanation'.
-
-        Here's are some examples: 
-        {examples}
-    """
+    1. Consider the following: 
+    user's query: {query}.
+    context: {context}.
+    chat history: {chat_history}
+    2. Determine if the chatbot can answer the user's query with nothing but the "context" and "chat history" information provided to you.
+    3. If the chat history is not provided, consider only the context.
+    4. Provide a brief explanation of why the context and the chat history do or do not contain sufficient information, labeled as 'explanation', leading up to a verdict (Pass/Fail) labeled as 'result'.
+    5. Always return a JSON object in the following format: "result": 'result', "explanation": 'explanation'.
+
+    Here are some examples: 
+    {examples}
+"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @property
     def name(self):
         return LlmEvalTypeId.CONTEXT_CONTAINS_ENOUGH_INFORMATION.value
@@ -55,26 +57,26 @@
     @property
     def examples(self):
         return CONTEXT_CONTAINS_ENOUGH_INFORMATION_EXAMPLES
 
     def is_failure(self, result) -> Optional[bool]:
         return bool(result == "Fail")
 
-    def _user_message(
-        self,
-        query: str,
-        context: str,
-        **kwargs,
-    ) -> str:
+    def _user_message(self, query: str, context: str, **kwargs) -> str:
         """
         Generates data for evaluation.
 
         :param query: user query
         :param context: list of strings of retrieved context
         :return: A dictionary with formatted data for evaluation
         """
         joined_context = "\n".join(context)
+        # Check if chat_history is provided and format it
+        chat_history = kwargs.get('chat_history', [])
+        formatted_chat_history = "\n".join(chat_history) if chat_history else "No chat history provided."
+
         return self.USER_MESSAGE_TEMPLATE.format(
             query=query,
             context=joined_context,
+            chat_history=formatted_chat_history,
             examples=self.examples,
         )
```

### Comparing `athina-1.2.9/athina/evals/llm/context_contains_enough_information/examples.py` & `athina-1.3.0/athina/evals/llm/context_contains_enough_information/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/llm/custom_prompt/evaluator.py` & `athina-1.3.0/athina/evals/llm/custom_prompt/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,19 @@
     @property
     def required_args(self):
         return self._required_args
 
     @property
     def examples(self):
         return self._examples
+    
+    def to_config(self) -> Optional[Dict]:
+        return {
+            "eval_prompt": self._eval_prompt,
+        }
 
     def is_failure(self, result) -> Optional[bool]:
         return bool(result == "Fail")
 
     def _user_message(self, **kwargs) -> str:
         return self._user_message_template.format(
             **kwargs,
```

### Comparing `athina-1.2.9/athina/evals/llm/does_response_answer_query/evaluator.py` & `athina-1.3.0/athina/evals/llm/does_response_answer_query/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/llm/does_response_answer_query/examples.py` & `athina-1.3.0/athina/evals/llm/does_response_answer_query/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/llm/example.py` & `athina-1.3.0/athina/evals/llm/example.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/llm/faithfulness/evaluator.py` & `athina-1.3.0/athina/evals/llm/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/llm/faithfulness/examples.py` & `athina-1.3.0/athina/evals/llm/faithfulness/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/llm/grading_criteria/evaluator.py` & `athina-1.3.0/athina/evals/llm/grading_criteria/evaluator.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,14 +56,19 @@
     def required_args(self):
         return ["response"]
 
     @property
     def examples(self):
         return self._examples
     
+    def to_config(self) -> Optional[dict]:
+        return {
+            "grading_criteria": self.grading_criteria
+        }
+    
     def is_failure(self, result) -> Optional[bool]:
         return bool(result == "Fail") 
 
     def _user_message(self, response, **kwargs) -> str:
         """
         Generates data for evaluation.
```

### Comparing `athina-1.2.9/athina/evals/llm/groundedness/evaluator.py` & `athina-1.3.0/athina/evals/llm/groundedness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/llm/groundedness/prompt.py` & `athina-1.3.0/athina/evals/llm/groundedness/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/llm/llm_evaluator.py` & `athina-1.3.0/athina/evals/llm/llm_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/llm/summary_accuracy/evaluator.py` & `athina-1.3.0/athina/evals/llm/summary_accuracy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/answer_correctness/evaluator.py` & `athina-1.3.0/athina/evals/ragas/answer_correctness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/answer_relevancy/evaluator.py` & `athina-1.3.0/athina/evals/ragas/answer_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/answer_semantic_similarity/evaluator.py` & `athina-1.3.0/athina/evals/ragas/answer_semantic_similarity/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/coherence/evaluator.py` & `athina-1.3.0/athina/evals/ragas/coherence/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/conciseness/evaluator.py` & `athina-1.3.0/athina/evals/ragas/conciseness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/context_precision/evaluator.py` & `athina-1.3.0/athina/evals/ragas/context_precision/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/context_recall/evaluator.py` & `athina-1.3.0/athina/evals/ragas/context_recall/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/context_relevancy/evaluator.py` & `athina-1.3.0/athina/evals/ragas/context_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/faithfulness/evaluator.py` & `athina-1.3.0/athina/evals/ragas/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/harmfulness/evaluator.py` & `athina-1.3.0/athina/evals/ragas/harmfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/maliciousness/evaluator.py` & `athina-1.3.0/athina/evals/ragas/maliciousness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/ragas/ragas_evaluator.py` & `athina-1.3.0/athina/evals/ragas/ragas_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/safety/content_moderation/evaluator.py` & `athina-1.3.0/athina/evals/safety/content_moderation/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/evals/safety/pii_detection/evaluator.py` & `athina-1.3.0/athina/evals/safety/pii_detection/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,8 +106,10 @@
                 result["reason"] = [
                     f"{entity['entity_group']} detected: {entity['word'].strip()}"
                     for entity in pii_entities
                 ]
         else:
             raise Exception(f"Error occurred during PII detection: {response.text}")
 
+        if not result["pii_detected"]:
+            result["reason"] = "No PII detected"
         return result
```

### Comparing `athina-1.2.9/athina/evals/safety/prompt_injection/evaluator.py` & `athina-1.3.0/athina/evals/safety/prompt_injection/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/guard/guard.py` & `athina-1.3.0/athina/guard/guard.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/helpers/config.py` & `athina-1.3.0/athina/helpers/config.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/helpers/function_eval_util.py` & `athina-1.3.0/athina/helpers/function_eval_util.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/helpers/get_evaluator.py` & `athina-1.3.0/athina/helpers/get_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from athina.evals import Regex, ContainsAny, ContainsAll, Contains, ContainsNone, ContainsJson, ContainsEmail, IsJson, IsEmail, NoInvalidLinks, ContainsLink, ContainsValidLink, Equals, StartsWith, EndsWith, LengthLessThan, LengthGreaterThan, ApiCall, DoesResponseAnswerQuery, Faithfulness, BaseEvaluator, ContextContainsEnoughInformation, SummaryAccuracy, Groundedness, GradingCriteria, CustomPrompt, RagasContextRelevancy, RagasAnswerRelevancy, RagasAnswerCorrectness, RagasAnswerSemanticSimilarity, RagasCoherence, RagasConciseness, RagasContextPrecision, RagasContextRecall, RagasFaithfulness, RagasHarmfulness, RagasMaliciousness, NotGibberishText, SafeForWorkText, ContainsNoSensitiveTopics
+from athina.evals import Regex, ContainsAny, ContainsAll, Contains, ContainsNone, ContainsJson, ContainsEmail, IsJson, IsEmail, NoInvalidLinks, ContainsLink, ContainsValidLink, Equals, StartsWith, EndsWith, LengthLessThan, LengthGreaterThan, ApiCall, DoesResponseAnswerQuery, Faithfulness, BaseEvaluator, ContextContainsEnoughInformation, SummaryAccuracy, Groundedness, GradingCriteria, CustomPrompt, RagasContextRelevancy, RagasAnswerRelevancy, RagasAnswerCorrectness, RagasAnswerSemanticSimilarity, RagasCoherence, RagasConciseness, RagasContextPrecision, RagasContextRecall, RagasFaithfulness, RagasHarmfulness, RagasMaliciousness, NotGibberishText, SafeForWorkText, ContainsNoSensitiveTopics, OpenAiContentModeration, PiiDetection, PromptInjection
 from athina.evals.grounded.similarity import CosineSimilarity, JaccardSimilarity, JaroWincklerSimilarity, NormalisedLevenshteinSimilarity, SorensenDiceSimilarity
 from athina.evals.grounded.wrapper import AnswerSimilarity, ContextSimilarity
 
 grounded_operations = {
     "AnswerSimilarity": AnswerSimilarity,
     "ContextSimilarity": ContextSimilarity,
 }
@@ -28,14 +28,17 @@
     "ApiCall": ApiCall,
 }
 
 safety_operations = {
     "SafeForWorkText": SafeForWorkText,
     "NotGibberishText": NotGibberishText,
     "ContainsNoSensitiveTopics": ContainsNoSensitiveTopics,
+    "OpenAiContentModeration" : OpenAiContentModeration,
+    "PiiDetection": PiiDetection,
+    "PromptInjection": PromptInjection
 }
 
 llm_operations = {
     "Draq": DoesResponseAnswerQuery,
     "Irftc": Faithfulness,
     "BaseEvaluator": BaseEvaluator,
     "Ccei": ContextContainsEnoughInformation,
```

### Comparing `athina-1.2.9/athina/helpers/loader_helper.py` & `athina-1.3.0/athina/helpers/loader_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/helpers/logger.py` & `athina-1.3.0/athina/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/helpers/run_helper.py` & `athina-1.3.0/athina/helpers/run_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/interfaces/athina.py` & `athina-1.3.0/athina/interfaces/athina.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/interfaces/model.py` & `athina-1.3.0/athina/interfaces/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,27 +5,45 @@
     """
     Supported models for evaluations.
     """
 
     GPT35_TURBO = "gpt-3.5-turbo"
     GPT35_TURBO_1106 = "gpt-3.5-turbo-1106"
     GPT4 = "gpt-4"
+    GPT4_O = "gpt-4o"
+    GPT4_32K = "gpt-4-32k"
     GPT4_1106_PREVIEW = "gpt-4-1106-preview"
     GPT4_TURBO_PREVIEW = "gpt-4-turbo-preview"
+    GPT4_TURBO = "gpt-4-turbo"
+    GPT35_TURBO_0125 = "gpt-3.5-turbo-0125"
     GPT35_TURBO_16K = "gpt-3.5-turbo-16k"
     COMMAND_LIGHT = "command-light"
     COMMAND = "command"
+    COMMAND_R = 'command-r'
+    COMMAND_R_PLUS = 'command-r-plus'
     AZURE_GPT35_TURBO = "azure/gpt-3.5-turbo"
     AZURE_GPT35_TURBO_1106 = "azure/gpt-3.5-turbo-1106"
     AZURE_GPT4 = "azure/gpt-4"
     AZURE_GPT4_1106_PREVIEW = "azure/gpt-4-1106-preview"
     GEMINI_PROD = "gemini/gemini-prod"
+    GEMINI_PRO = "gemini/gemini-pro"
+    GEMINI_15_PRO_LATEST = "gemini/gemini-1.5-pro-latest"
     CLAUDE_2 = "claude-2"
+    CLAUDE_21 = "claude-2.1"
+    CLAUDE_3_HAIKU_20240307 = "claude-3-haiku-20240307"
+    CLAUDE_3_SONNET_20240229 = "claude-3-sonnet-20240229"
+    CLAUDE_3_OPUS_20240229 = "claude-3-opus-20240229"
     MISTRAL_TINY = "mistral/mistral-tiny"
     MISTRAL_SMALL = "mistral/mistral-small"
+    MISTRAL_MEDIUM = "mistral/mistral-medium"
+    MISTRAL_LARGE = "mistral/mistral-large-latest"
+    GROQ_LLAMA3_8B_8192 = 'groq/llama3-8b-8192'
+    GROQ_LLAMA3_70B_8192 = 'groq/llama3-70b-8192'
+    HUGGINGFACE_META_LLAMA_3_8B ='huggingface/meta-llama/meta-llama-3-8b'
+    HUGGINGFACE_META_LLAMA_3_70B ='huggingface/meta-llama/meta-llama-3-70b'
 
     @staticmethod
     def is_supported(model_name: str) -> bool:
         """
         Checks if the model is supported.
         """
         return model_name in [model.value for model in Model]
```

### Comparing `athina-1.2.9/athina/interfaces/result.py` & `athina-1.3.0/athina/interfaces/result.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/llms/abstract_llm_service.py` & `athina-1.3.0/athina/llms/abstract_llm_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,29 +10,29 @@
         """
         Fetches embeddings for the given text. This method should be implemented by subclasses 
         to use the specific LLM provider's embeddings API.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def chat_completion(self, messages, model, temperature = None) -> str:
+    def chat_completion(self, messages, model, **kwargs) -> str:
         """
         Fetches a chat completion response. This method should be implemented by subclasses 
         to interact with the specific LLM provider's chat completion API.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def chat_completion_json(self, messages, model, temperature = None) -> str:
+    def chat_completion_json(self, messages, model, **kwargs) -> str:
         """
         Fetches a chat completion response in JSON format. This method should be implemented 
         by subclasses to interact with the specific LLM provider's chat completion API using JSON mode.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def json_completion(self, messages, model, temperature = None):
+    def json_completion(self, messages, model, **kwargs):
         """
         Helper method to be implemented by subclasses. This method should call either chat_completion or chat_completion_json.
         
         """
         raise NotImplementedError
```

### Comparing `athina-1.2.9/athina/llms/openai_service.py` & `athina-1.3.0/athina/llms/openai_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,71 +26,75 @@
 
     def embeddings(self, text: str) -> list:
         """
         Fetches response from OpenAI's Embeddings API.
         """
         try:
             response = self.openai.embeddings.create(
-                model="text-embedding-ada-002",
-                input=text,
-                encoding_format="float"
+                model="text-embedding-ada-002", input=text, encoding_format="float"
             )
             return response.data[0].embedding
         except Exception as e:
             print(f"Error in Embeddings: {e}")
             raise e
 
     @retry(stop_max_attempt_number=3, wait_fixed=2000)
-    def chat_completion(self, messages, model, temperature=DEFAULT_TEMPERATURE) -> str:
+    def chat_completion(self, messages, model, **kwargs) -> str:
         """
         Fetches response from OpenAI's ChatCompletion API.
         """
+        if 'temperature' not in kwargs:
+            kwargs['temperature'] = DEFAULT_TEMPERATURE
         try:
             response = self.openai.chat.completions.create(
-                model=model, messages=messages, temperature=temperature
+                model=model, messages=messages, **kwargs
             )
             return response.choices[0].message.content
         except Exception as e:
             print(f"Error in ChatCompletion: {e}")
             raise e
 
     @retry(stop_max_attempt_number=3, wait_fixed=2000)
-    def chat_completion_json(self, messages, model, temperature=DEFAULT_TEMPERATURE) -> str:
+    def chat_completion_json(self, messages, model, **kwargs) -> str:
         """
         Fetches response from OpenAI's ChatCompletion API using JSON mode.
         """
+        if 'temperature' not in kwargs:
+            kwargs['temperature'] = DEFAULT_TEMPERATURE
         try:
             response = self.openai.chat.completions.create(
                 model=model,
                 messages=messages,
-                temperature=temperature,
                 response_format={"type": "json_object"},
+                **kwargs
             )
             return response.choices[0].message.content
         except Exception as e:
             print(f"Error in ChatCompletion: {e}")
             raise e
 
-    def json_completion(self, messages, model, temperature=DEFAULT_TEMPERATURE):
+    def json_completion(self, messages, model, **kwargs):
         """
         Fetches response from OpenAI's ChatCompletion API using JSON mode.
         """
+        if 'temperature' not in kwargs:
+            kwargs['temperature'] = DEFAULT_TEMPERATURE
         try:
             if Model.supports_json_mode(model):
                 chat_completion_response = self.chat_completion_json(
                     model=model,
                     messages=messages,
-                    temperature=temperature,
+                    **kwargs,
                 )
             else:
                 chat_completion_response = self.chat_completion(
                     model=model,
                     messages=messages,
-                    temperature=temperature,
+                    **kwargs,
                 )
 
             # Extract JSON object from LLM response
             return JsonHelper.extract_json_from_text(chat_completion_response)
-        
+
         except Exception as e:
             print(f"Error in ChatCompletion: {e}")
-            raise e
+            raise e
```

### Comparing `athina-1.2.9/athina/llms/question_answerer_bulk.py` & `athina-1.3.0/athina/llms/question_answerer_bulk.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/llms/question_answerer_cot.py` & `athina-1.3.0/athina/llms/question_answerer_cot.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/llms/question_answerer_with_retrieval.py` & `athina-1.3.0/athina/llms/question_answerer_with_retrieval.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/llms/question_generator.py` & `athina-1.3.0/athina/llms/question_generator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/loaders/base_loader.py` & `athina-1.3.0/athina/loaders/base_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,7 +67,14 @@
     def load_dict(self, data: list) -> List[DataPoint]:
         """
         Loads and processes data from a list of dictionaries.
         """
         self._raw_dataset = data
         self.process()
         return self._processed_dataset
+
+    @abstractmethod
+    def load_athina_inferences(self, data: dict) -> List[DataPoint]:
+        """
+        Loads and processes data from a dictionary of Athina inferences.
+        """
+        pass
```

### Comparing `athina-1.2.9/athina/loaders/conversation_loader.py` & `athina-1.3.0/athina/loaders/conversation_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Dict
 from athina.interfaces.athina import AthinaFilters
 from athina.interfaces.data import DataPoint as BaseDataPoint
 from .base_loader import BaseLoader
 from dataclasses import asdict
 from athina.services.athina_api_service import AthinaApiService
```

### Comparing `athina-1.2.9/athina/loaders/loader.py` & `athina-1.3.0/athina/loaders/loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import List, Optional
 from athina.interfaces.athina import AthinaFilters
 from athina.interfaces.data import DataPoint as BaseDataPoint
 from .base_loader import BaseLoader
 from dataclasses import asdict
 from athina.services.athina_api_service import AthinaApiService
+from llama_index.indices.query.base import BaseQueryEngine
+
 
 class DataPoint(BaseDataPoint):
     """Data point for a single inference."""
 
     query: Optional[str]
-    context: Optional[str]
+    context: Optional[List[str]]
     response: Optional[str]
     expected_response: Optional[str]
 
 
 class Loader(BaseLoader):
     """
     This class is a generic data loader for evals
@@ -72,15 +74,14 @@
             self._processed_dataset.append(processed_instance)
         
 
     def load_athina_inferences(
         self,
         filters: Optional[AthinaFilters] = None,
         limit: int = 10,
-        context_key: Optional[str] = None,
     ):
         """
         Load data from Athina API.
         By default, this will fetch the last 10 inferences from the API.
         """
         self._raw_dataset = AthinaApiService.fetch_inferences(
             filters=filters, limit=limit
@@ -92,8 +93,52 @@
             processed_instance = {
                 "query": raw_dataset_dict['user_query'],
                 "context": context,
                 "response": raw_dataset_dict['prompt_response'],
                 "expected_response": raw_dataset_dict['expected_response']
             }
             self._processed_dataset.append(processed_instance)
+        return self._processed_dataset
+    
+    def _fetch_context_and_response_for_llama_index(self, query: str, query_engine: BaseQueryEngine):
+        """
+        Fetches the context and response from the llama index query engine.
+        """
+        contexts = []
+        query_engine_response = query_engine.query(query)
+        response = query_engine_response.response
+        for c in query_engine_response.source_nodes:
+            text = c.node.get_content()
+            contexts.append(text)
+
+        return contexts, response
+    
+    def _generate_processed_instance_for_llama_index(self, raw_instance: dict, query_engine: BaseQueryEngine) -> DataPoint:
+        """
+        Generates a processed instance for the llama index query engine.
+        """
+        if self.col_query not in raw_instance:
+            raise ValueError(f"'{self.col_query}' not found in provided data.")
+        if self.col_query in raw_instance and not isinstance(raw_instance.get(self.col_query), str):
+            raise TypeError(f"'{self.col_query}' is not of type string.")
+        if self.col_expected_response in raw_instance and not isinstance(raw_instance.get(self.col_expected_response), str):
+            raise TypeError(f"'{self.col_expected_response}' is not of type string.")
+
+        contexts, response = self._fetch_context_and_response_for_llama_index(raw_instance.get(self.col_query), query_engine)
+        processed_instance = {
+            "query": raw_instance.get(self.col_query),
+            "context": contexts,
+            "response": response,
+            "expected_response": raw_instance.get(self.col_expected_response, None)
+        }
+        return processed_instance
+
+    def load_from_llama_index(self, data: list, query_engine: BaseQueryEngine):
+        """
+        Load data from Llama Index.
+        """
+        if query_engine is None:
+            raise ValueError("Query engine is not provided.")
+        for raw_instance in data:
+            processed_instance = self._generate_processed_instance_for_llama_index(raw_instance, query_engine)
+            self._processed_dataset.append(processed_instance)
         return self._processed_dataset
```

### Comparing `athina-1.2.9/athina/loaders/response_loader.py` & `athina-1.3.0/athina/loaders/response_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from typing import List, Optional
 from athina.interfaces.athina import AthinaFilters
 from athina.interfaces.data import DataPoint
 from .base_loader import BaseLoader
+from athina.services.athina_api_service import AthinaApiService
+from dataclasses import asdict
+
 
 
 class ResponseLoader(BaseLoader):
     """
     This class is a data loader for evals that only evaluate the response.
 
     Attributes:
```

### Comparing `athina-1.2.9/athina/loaders/summary_loader.py` & `athina-1.3.0/athina/loaders/summary_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/loaders/text_loader.py` & `athina-1.3.0/athina/loaders/text_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/metrics/agreement_score.py` & `athina-1.3.0/athina/metrics/agreement_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/metrics/contradiction_score.py` & `athina-1.3.0/athina/metrics/contradiction_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/metrics/groundedness.py` & `athina-1.3.0/athina/metrics/groundedness.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/metrics/hallucination_score.py` & `athina-1.3.0/athina/metrics/hallucination_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/metrics/metric_type.py` & `athina-1.3.0/athina/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.9/athina/services/athina_api_service.py` & `athina-1.3.0/athina/services/athina_api_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -301,7 +301,31 @@
             return response.json()
         except Exception as e:
             print(
                 f"An error occurred while posting experiment metadata",
                 str(e),
             )
             raise
+    
+    @staticmethod
+    def log_eval_results_with_config(eval_results_with_config: dict):
+        try:
+            endpoint = f"{API_BASE_URL}/api/v1/eval_run/log-eval-results-sdk"
+            response = requests.post(
+                endpoint,
+                headers=AthinaApiService._headers(),
+                json=eval_results_with_config,
+            )
+            if response.status_code == 401:
+                response_json = response.json()
+                error_message = response_json.get('error', 'Unknown Error')
+                details_message = 'please check your athina api key and try again'
+                raise CustomException(error_message, details_message)
+            elif response.status_code != 200 and response.status_code != 201:
+                response_json = response.json()
+                error_message = response_json.get('error', 'Unknown Error')
+                details_message = response_json.get(
+                    'details', {}).get('message', 'No Details')
+                raise CustomException(error_message, details_message)
+            return response.json()
+        except Exception as e:
+            raise
```

### Comparing `athina-1.2.9/pyproject.toml` & `athina-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athina"
-version = "1.2.9"
+version = "1.3.0"
 description = "Python SDK to configure and run evaluations for your LLM-based application"
 authors = ["Shiv Sakhuja <shiv@athina.ai>", "Akshat Gupta <akshat@athina.ai>", "Vivek Aditya <vivek@athina.ai>", "Akhil Bisht <akhil@athina.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 retrying = "^1.3.4"
@@ -16,14 +16,16 @@
 pandas = "*"
 langchain = ">=0.0.350"
 datasets = "^2.16.0"
 python-dotenv = "^1.0.0"
 requests = "^2.31.0"
 langchain-openai = "^0.0.3"
 llama-index = "^0.9.40"
+pydantic = ">=2.0,<3.0"
+litellm = "1.35.6"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `athina-1.2.9/PKG-INFO` & `athina-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: athina
-Version: 1.2.9
+Version: 1.3.0
 Summary: Python SDK to configure and run evaluations for your LLM-based application
 Author: Shiv Sakhuja
 Author-email: shiv@athina.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: datasets (>=2.16.0,<3.0.0)
 Requires-Dist: langchain (>=0.0.350)
 Requires-Dist: langchain-openai (>=0.0.3,<0.0.4)
+Requires-Dist: litellm (==1.35.6)
 Requires-Dist: llama-index (>=0.9.40,<0.10.0)
 Requires-Dist: openai (>=1.3.4,<2.0.0)
 Requires-Dist: pandas
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: ragas (>=0.0.22,<0.0.23)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: retrying (>=1.3.4,<2.0.0)
 Requires-Dist: timeout-decorator (>=0.5.0,<0.6.0)
 Description-Content-Type: text/markdown
```

