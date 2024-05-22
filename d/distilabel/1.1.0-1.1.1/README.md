# Comparing `tmp/distilabel-1.1.0.tar.gz` & `tmp/distilabel-1.1.1.tar.gz`

## Comparing `distilabel-1.1.0.tar` & `distilabel-1.1.1.tar`

### file list

```diff
@@ -1,307 +1,307 @@
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.1.0/Makefile
--rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 distilabel-1.1.0/mkdocs.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/ISSUE_TEMPLATE/blank-issue-template.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/CNAME
--rw-r--r--   0        0        0     9308 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/index.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/cli.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/anthropic.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/anyscale.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/azure.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/groq.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/huggingface.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/index.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/litellm.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/llamacpp.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/mistral.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/ollama.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/openai.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/together.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/vertexai.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/vllm.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/pipeline/index.md
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/pipeline/routing_batch_function.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/pipeline/typing.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/pipeline/utils.md
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step/decorator.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step/generator_step.md
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step/global_step.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step/index.md
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step_gallery/argilla.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step_gallery/columns.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step_gallery/extra.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/task/generator_task.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/task/index.md
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/task_gallery/index.md
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-badge-dark.png
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-badge-light.png
--rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-black.png
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-icon.svg
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-white.png
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/logo.svg
--rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/distilabel-diagram-dark.svg
--rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/distilabel-diagram.svg
--rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_1.png
--rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_2.png
--rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_3.png
--rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_4.png
--rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/cli/cli_pipe.png
--rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/learn/steps/argilla/preference.png
--rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/learn/steps/argilla/text_generation.png
--rw-r--r--   0        0        0   336223 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/pipeline/pipeline-ctrlc.png
--rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
--rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
--rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/deita/datasets.png
--rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/deita/diversity.png
--rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/deita/overview.png
--rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/deita/results.png
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/scripts/gen_ref_pages.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/faq.md
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/how_to_guide.md
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/installation.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/index.md
--rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/argilla.md
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/caching.md
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/distiset.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/index.md
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/structured_generation.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/index.md
--rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/cli/index.md
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/llm/index.md
--rw-r--r--   0        0        0    21776 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/pipeline/index.md
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/step/generator_step.md
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/step/global_step.md
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/step/index.md
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/task/generator_task.md
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/task/index.md
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/index.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/examples/index.md
--rw-r--r--   0        0        0    21843 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/papers/deita.md
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/papers/index.md
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/papers/instruction_backtranslation.md
--rw-r--r--   0        0        0    10707 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/papers/ultrafeedback.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 distilabel-1.1.0/examples/structured_generation_with_outlines.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/__main__.py
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/distiset.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/app.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/pipeline/app.py
--rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/pipeline/utils.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/anthropic.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/anyscale.py
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/azure.py
--rw-r--r--   0        0        0    11651 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/base.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/chat_templates.py
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/cohere.py
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/groq.py
--rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/litellm.py
--rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/llamacpp.py
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/mistral.py
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/mixins.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/ollama.py
--rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/openai.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/together.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/typing.py
--rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/vertexai.py
--rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/vllm.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/huggingface/__init__.py
--rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/huggingface/inference_endpoints.py
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/huggingface/transformers.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/mixins/__init__.py
--rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/mixins/runtime_parameters.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/__init__.py
--rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/_dag.py
--rw-r--r--   0        0        0    57088 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/base.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/constants.py
--rw-r--r--   0        0        0    39256 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/local.py
--rw-r--r--   0        0        0    13786 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/routing_batch_function.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/typing.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/utils.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/__init__.py
--rw-r--r--   0        0        0    24715 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/base.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/combine.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/decorator.py
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/deita.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/expand.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/keep.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/typing.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/argilla/base.py
--rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/argilla/preference.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/argilla/text_generation.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/formatting/__init__.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/formatting/conversation.py
--rw-r--r--   0        0        0    12377 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/formatting/dpo.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/formatting/sft.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/generators/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/generators/data.py
--rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/generators/huggingface.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/globals/__init__.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/globals/huggingface.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/__init__.py
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/base.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/complexity_scorer.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/generate_embeddings.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/genstruct.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/instruction_backtranslation.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/pair_rm.py
--rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/prometheus_eval.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/quality_scorer.py
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/self_instruct.py
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/text_generation.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/typing.py
--rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/ultrafeedback.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/base.py
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
--rw-r--r--   0        0        0    12983 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/generator.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/base.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/structured_outputs/__init__.py
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/structured_outputs/outlines.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/complexity-scorer.jinja2
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/genstruct.jinja2
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/quality-scorer.jinja2
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/self-instruct.jinja2
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/absolute_with_reference.jinja2
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/absolute_without_reference.jinja2
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/relative_with_reference.jinja2
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/relative_without_reference.jinja2
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/chat.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/dicts.py
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/docstring.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/export_components_info.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/files.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/itertools.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/lists.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/logging.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/notebook.py
--rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/serialization.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/typing_.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/card/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/card/dataset_card.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/card/distilabel_template.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/__init__.py
--rw-r--r--   0        0        0    14542 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/components_gallery.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/components-list.jinja2
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/index.md
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/llm-detail.jinja2
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/step-detail.jinja2
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_branching_missaligmnent.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_dry_run.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_pipe_llms.py
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_pipe_simple.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_routing_batch_function.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/helpers.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/test_distiset.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/test_imports.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/__init__.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/test_pipeline.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/pipeline/test_app.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/__init__.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_anthropic.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_anyscale.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_azure.py
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_cohere.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_groq.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_litellm.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_llamacpp.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_mistral.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_mixins.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_ollama.py
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_openai.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_together.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_vertexai.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/huggingface/__init__.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/huggingface/test_inference_endpoints.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/huggingface/test_transformers.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/mixins/__init__.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/mixins/test_runtime_parameters.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/__init__.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/conftest.py
--rw-r--r--   0        0        0    82348 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/test_base.py
--rw-r--r--   0        0        0    23637 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/test_dag.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/test_local.py
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/test_routing_batch_function.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/__init__.py
--rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_base.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_combine.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_decorator.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_deita.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_expand.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_keep.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/argilla/test_base.py
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/argilla/test_preference.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/argilla/test_text_generation.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/formatting/__init__.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/formatting/test_conversation.py
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/formatting/test_dpo.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/formatting/test_sft.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/generators/test_data.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/generators/test_huggingface.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/__init__.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/conftest.py
--rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_base.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_complexity_scorer.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_generate_embeddings.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_genstruct.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_instruction_backtranslation.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_pair_rm.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_prometheus_eval.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_quality_scorer.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_self_instruct.py
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_text_generation.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_ultrafeedback.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/test_base.py
--rw-r--r--   0        0        0    11637 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/test_generator.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_quality/test_base.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/structured_outputs/__init__.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/structured_outputs/test_outlines.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_chat.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_docstring.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_files.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_lists.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_typing.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.1.0/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.1.0/LICENSE
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.1.0/LICENSE_HEADER
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 distilabel-1.1.0/README.md
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 distilabel-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12566 2020-02-02 00:00:00.000000 distilabel-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.1.1/Makefile
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 distilabel-1.1.1/mkdocs.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.1.1/.github/ISSUE_TEMPLATE/blank-issue-template.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.1.1/.github/ISSUE_TEMPLATE/🆕-feature-request.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.1.1/.github/ISSUE_TEMPLATE/🐛-bug-report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.1.1/.github/ISSUE_TEMPLATE/📚-documentation-update.md
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 distilabel-1.1.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 distilabel-1.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/CNAME
+-rw-r--r--   0        0        0     9308 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/index.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/cli.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/anthropic.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/anyscale.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/azure.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/groq.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/huggingface.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/index.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/litellm.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/llamacpp.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/mistral.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/ollama.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/openai.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/together.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/vertexai.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/llm/vllm.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/pipeline/index.md
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/pipeline/routing_batch_function.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/pipeline/typing.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/pipeline/utils.md
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/step/decorator.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/step/generator_step.md
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/step/global_step.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/step/index.md
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/step_gallery/argilla.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/step_gallery/columns.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/step_gallery/extra.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/task/generator_task.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/task/index.md
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/api/task_gallery/index.md
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/distilabel-badge-dark.png
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/distilabel-badge-light.png
+-rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/distilabel-black.png
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/distilabel-icon.svg
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/distilabel-white.png
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/logo.svg
+-rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/distilabel-diagram-dark.svg
+-rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/distilabel-diagram.svg
+-rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/sections/caching/caching_pipe_1.png
+-rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/sections/caching/caching_pipe_2.png
+-rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/sections/caching/caching_pipe_3.png
+-rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/sections/caching/caching_pipe_4.png
+-rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/sections/cli/cli_pipe.png
+-rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/sections/learn/steps/argilla/preference.png
+-rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/sections/learn/steps/argilla/text_generation.png
+-rw-r--r--   0        0        0   336223 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/images/sections/pipeline/pipeline-ctrlc.png
+-rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
+-rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
+-rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/tutorials-assets/deita/datasets.png
+-rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/tutorials-assets/deita/diversity.png
+-rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/tutorials-assets/deita/overview.png
+-rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/assets/tutorials-assets/deita/results.png
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/scripts/gen_ref_pages.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/faq.md
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/how_to_guide.md
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/installation.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/index.md
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/advanced/argilla.md
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/advanced/caching.md
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/advanced/distiset.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/advanced/index.md
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/advanced/structured_generation.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/tutorial/index.md
+-rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/tutorial/cli/index.md
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/tutorial/llm/index.md
+-rw-r--r--   0        0        0    21776 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/tutorial/pipeline/index.md
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/tutorial/step/generator_step.md
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/tutorial/step/global_step.md
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/tutorial/step/index.md
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/tutorial/task/generator_task.md
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/learn/tutorial/task/index.md
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/pipeline_samples/index.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/pipeline_samples/examples/index.md
+-rw-r--r--   0        0        0    21843 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/pipeline_samples/papers/deita.md
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/pipeline_samples/papers/index.md
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/pipeline_samples/papers/instruction_backtranslation.md
+-rw-r--r--   0        0        0    10707 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/sections/pipeline_samples/papers/ultrafeedback.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.1.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 distilabel-1.1.1/examples/structured_generation_with_outlines.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/__main__.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/distiset.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/cli/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/cli/app.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/cli/pipeline/app.py
+-rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/cli/pipeline/utils.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/anthropic.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/anyscale.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/azure.py
+-rw-r--r--   0        0        0    11651 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/base.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/chat_templates.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/cohere.py
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/groq.py
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/litellm.py
+-rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/llamacpp.py
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/mistral.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/mixins.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/ollama.py
+-rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/openai.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/together.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/typing.py
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/vertexai.py
+-rw-r--r--   0        0        0    10564 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/vllm.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/huggingface/inference_endpoints.py
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/llms/huggingface/transformers.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/mixins/__init__.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/mixins/runtime_parameters.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/pipeline/__init__.py
+-rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/pipeline/_dag.py
+-rw-r--r--   0        0        0    57041 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/pipeline/base.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/pipeline/constants.py
+-rw-r--r--   0        0        0    39256 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/pipeline/local.py
+-rw-r--r--   0        0        0    13786 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/pipeline/routing_batch_function.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/pipeline/typing.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/pipeline/utils.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/__init__.py
+-rw-r--r--   0        0        0    24715 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/base.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/combine.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/decorator.py
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/deita.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/expand.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/keep.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/typing.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/argilla/base.py
+-rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/argilla/preference.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/argilla/text_generation.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/formatting/__init__.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/formatting/conversation.py
+-rw-r--r--   0        0        0    12377 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/formatting/dpo.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/formatting/sft.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/generators/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/generators/data.py
+-rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/generators/huggingface.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/globals/__init__.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/globals/huggingface.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/base.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/complexity_scorer.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/generate_embeddings.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/genstruct.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/instruction_backtranslation.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/pair_rm.py
+-rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/prometheus_eval.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/quality_scorer.py
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/self_instruct.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/text_generation.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/typing.py
+-rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/ultrafeedback.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/base.py
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
+-rw-r--r--   0        0        0    12983 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/generator.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_quality/base.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/evol_quality/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/structured_outputs/__init__.py
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/structured_outputs/outlines.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/complexity-scorer.jinja2
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/genstruct.jinja2
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/quality-scorer.jinja2
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/self-instruct.jinja2
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/prometheus/absolute_with_reference.jinja2
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/prometheus/absolute_without_reference.jinja2
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/prometheus/relative_with_reference.jinja2
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/prometheus/relative_without_reference.jinja2
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/chat.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/dicts.py
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/docstring.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/export_components_info.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/files.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/itertools.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/lists.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/logging.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/notebook.py
+-rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/serialization.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/typing_.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/card/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/card/dataset_card.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/card/distilabel_template.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/mkdocs/__init__.py
+-rw-r--r--   0        0        0    14542 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/mkdocs/components_gallery.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/mkdocs/templates/components-gallery/components-list.jinja2
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/mkdocs/templates/components-gallery/index.md
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/mkdocs/templates/components-gallery/llm-detail.jinja2
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 distilabel-1.1.1/src/distilabel/utils/mkdocs/templates/components-gallery/step-detail.jinja2
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/integration/test_branching_missaligmnent.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/integration/test_dry_run.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/integration/test_pipe_llms.py
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/integration/test_pipe_simple.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/integration/test_routing_batch_function.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/helpers.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/test_distiset.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/test_imports.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/cli/test_pipeline.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/cli/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/cli/pipeline/test_app.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/cli/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/__init__.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_anthropic.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_anyscale.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_azure.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_cohere.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_groq.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_litellm.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_llamacpp.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_mistral.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_mixins.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_ollama.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_openai.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_together.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/test_vertexai.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/huggingface/test_inference_endpoints.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/llms/huggingface/test_transformers.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/mixins/__init__.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/mixins/test_runtime_parameters.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/pipeline/__init__.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/pipeline/conftest.py
+-rw-r--r--   0        0        0    82348 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/pipeline/test_base.py
+-rw-r--r--   0        0        0    23637 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/pipeline/test_dag.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/pipeline/test_local.py
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/pipeline/test_routing_batch_function.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/__init__.py
+-rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/test_base.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/test_combine.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/test_decorator.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/test_deita.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/test_expand.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/test_keep.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/argilla/test_base.py
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/argilla/test_preference.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/argilla/test_text_generation.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/formatting/__init__.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/formatting/test_conversation.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/formatting/test_dpo.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/formatting/test_sft.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/generators/test_data.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/generators/test_huggingface.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/conftest.py
+-rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_base.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_complexity_scorer.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_generate_embeddings.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_genstruct.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_instruction_backtranslation.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_pair_rm.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_prometheus_eval.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_quality_scorer.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_self_instruct.py
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_text_generation.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/test_ultrafeedback.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/test_base.py
+-rw-r--r--   0        0        0    11637 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/test_generator.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/evol_quality/test_base.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/structured_outputs/__init__.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/steps/tasks/structured_outputs/test_outlines.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/utils/test_chat.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/utils/test_docstring.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/utils/test_files.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/utils/test_lists.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.1.1/tests/unit/utils/test_typing.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.1.1/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.1.1/LICENSE
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.1.1/LICENSE_HEADER
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 distilabel-1.1.1/README.md
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 distilabel-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12566 2020-02-02 00:00:00.000000 distilabel-1.1.1/PKG-INFO
```

### Comparing `distilabel-1.1.0/.pre-commit-config.yaml` & `distilabel-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/mkdocs.yml` & `distilabel-1.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md` & `distilabel-1.1.1/.github/ISSUE_TEMPLATE/🆕-feature-request.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md` & `distilabel-1.1.1/.github/ISSUE_TEMPLATE/🐛-bug-report.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md` & `distilabel-1.1.1/.github/ISSUE_TEMPLATE/📚-documentation-update.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/.github/workflows/docs.yml` & `distilabel-1.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/.github/workflows/release.yml` & `distilabel-1.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/.github/workflows/test.yml` & `distilabel-1.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/index.md` & `distilabel-1.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/distilabel-badge-dark.png` & `distilabel-1.1.1/docs/assets/distilabel-badge-dark.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/distilabel-badge-light.png` & `distilabel-1.1.1/docs/assets/distilabel-badge-light.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/distilabel-black.png` & `distilabel-1.1.1/docs/assets/distilabel-black.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/distilabel-icon.svg` & `distilabel-1.1.1/docs/assets/distilabel-icon.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/distilabel-white.png` & `distilabel-1.1.1/docs/assets/distilabel-white.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/logo.svg` & `distilabel-1.1.1/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/distilabel-diagram-dark.svg` & `distilabel-1.1.1/docs/assets/images/distilabel-diagram-dark.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/distilabel-diagram.svg` & `distilabel-1.1.1/docs/assets/images/distilabel-diagram.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_1.png` & `distilabel-1.1.1/docs/assets/images/sections/caching/caching_pipe_1.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_2.png` & `distilabel-1.1.1/docs/assets/images/sections/caching/caching_pipe_2.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_3.png` & `distilabel-1.1.1/docs/assets/images/sections/caching/caching_pipe_3.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_4.png` & `distilabel-1.1.1/docs/assets/images/sections/caching/caching_pipe_4.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/sections/cli/cli_pipe.png` & `distilabel-1.1.1/docs/assets/images/sections/cli/cli_pipe.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/sections/learn/steps/argilla/preference.png` & `distilabel-1.1.1/docs/assets/images/sections/learn/steps/argilla/preference.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/sections/learn/steps/argilla/text_generation.png` & `distilabel-1.1.1/docs/assets/images/sections/learn/steps/argilla/text_generation.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/images/sections/pipeline/pipeline-ctrlc.png` & `distilabel-1.1.1/docs/assets/images/sections/pipeline/pipeline-ctrlc.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png` & `distilabel-1.1.1/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png` & `distilabel-1.1.1/docs/assets/tutorials-assets/preference_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/tutorials-assets/deita/datasets.png` & `distilabel-1.1.1/docs/assets/tutorials-assets/deita/datasets.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/tutorials-assets/deita/diversity.png` & `distilabel-1.1.1/docs/assets/tutorials-assets/deita/diversity.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/tutorials-assets/deita/overview.png` & `distilabel-1.1.1/docs/assets/tutorials-assets/deita/overview.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/assets/tutorials-assets/deita/results.png` & `distilabel-1.1.1/docs/assets/tutorials-assets/deita/results.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/scripts/gen_ref_pages.py` & `distilabel-1.1.1/docs/scripts/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/faq.md` & `distilabel-1.1.1/docs/sections/faq.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/how_to_guide.md` & `distilabel-1.1.1/docs/sections/how_to_guide.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/installation.md` & `distilabel-1.1.1/docs/sections/installation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/advanced/argilla.md` & `distilabel-1.1.1/docs/sections/learn/advanced/argilla.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/advanced/caching.md` & `distilabel-1.1.1/docs/sections/learn/advanced/caching.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/advanced/distiset.md` & `distilabel-1.1.1/docs/sections/learn/advanced/distiset.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/advanced/structured_generation.md` & `distilabel-1.1.1/docs/sections/learn/advanced/structured_generation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/tutorial/cli/index.md` & `distilabel-1.1.1/docs/sections/learn/tutorial/cli/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/tutorial/llm/index.md` & `distilabel-1.1.1/docs/sections/learn/tutorial/llm/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/tutorial/pipeline/index.md` & `distilabel-1.1.1/docs/sections/learn/tutorial/pipeline/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/tutorial/step/generator_step.md` & `distilabel-1.1.1/docs/sections/learn/tutorial/step/generator_step.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/tutorial/step/global_step.md` & `distilabel-1.1.1/docs/sections/learn/tutorial/step/global_step.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/tutorial/step/index.md` & `distilabel-1.1.1/docs/sections/learn/tutorial/step/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/tutorial/task/generator_task.md` & `distilabel-1.1.1/docs/sections/learn/tutorial/task/generator_task.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/learn/tutorial/task/index.md` & `distilabel-1.1.1/docs/sections/learn/tutorial/task/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/pipeline_samples/examples/index.md` & `distilabel-1.1.1/docs/sections/pipeline_samples/examples/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/pipeline_samples/papers/deita.md` & `distilabel-1.1.1/docs/sections/pipeline_samples/papers/deita.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/pipeline_samples/papers/instruction_backtranslation.md` & `distilabel-1.1.1/docs/sections/pipeline_samples/papers/instruction_backtranslation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/docs/sections/pipeline_samples/papers/ultrafeedback.md` & `distilabel-1.1.1/docs/sections/pipeline_samples/papers/ultrafeedback.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/examples/structured_generation_with_outlines.py` & `distilabel-1.1.1/examples/structured_generation_with_outlines.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/__init__.py` & `distilabel-1.1.1/src/distilabel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from rich import traceback as rich_traceback
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 rich_traceback.install(show_locals=True)
```

### Comparing `distilabel-1.1.0/src/distilabel/__main__.py` & `distilabel-1.1.1/src/distilabel/__main__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/distiset.py` & `distilabel-1.1.1/src/distilabel/distiset.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/cli/__init__.py` & `distilabel-1.1.1/src/distilabel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/cli/app.py` & `distilabel-1.1.1/src/distilabel/cli/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/cli/pipeline/__init__.py` & `distilabel-1.1.1/src/distilabel/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/cli/pipeline/app.py` & `distilabel-1.1.1/src/distilabel/cli/pipeline/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/cli/pipeline/utils.py` & `distilabel-1.1.1/src/distilabel/cli/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/__init__.py` & `distilabel-1.1.1/src/distilabel/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/anthropic.py` & `distilabel-1.1.1/src/distilabel/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/anyscale.py` & `distilabel-1.1.1/src/distilabel/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/azure.py` & `distilabel-1.1.1/src/distilabel/llms/azure.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/base.py` & `distilabel-1.1.1/src/distilabel/llms/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/chat_templates.py` & `distilabel-1.1.1/src/distilabel/llms/chat_templates.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/cohere.py` & `distilabel-1.1.1/src/distilabel/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/groq.py` & `distilabel-1.1.1/src/distilabel/llms/groq.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/litellm.py` & `distilabel-1.1.1/src/distilabel/llms/litellm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/llamacpp.py` & `distilabel-1.1.1/src/distilabel/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/mistral.py` & `distilabel-1.1.1/src/distilabel/llms/mistral.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/mixins.py` & `distilabel-1.1.1/src/distilabel/llms/mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/ollama.py` & `distilabel-1.1.1/src/distilabel/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/openai.py` & `distilabel-1.1.1/src/distilabel/llms/openai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/together.py` & `distilabel-1.1.1/src/distilabel/llms/together.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/typing.py` & `distilabel-1.1.1/src/distilabel/llms/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/vertexai.py` & `distilabel-1.1.1/src/distilabel/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/vllm.py` & `distilabel-1.1.1/src/distilabel/llms/vllm.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,17 @@
             n=num_generations,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             temperature=temperature,
             top_p=top_p,
             top_k=top_k,
             max_tokens=max_new_tokens,
-            logits_processors=[self._logits_processor],
+            logits_processors=(
+                [self._logits_processor] if self._logits_processor else None
+            ),
             **extra_sampling_params,
         )
 
         batch_outputs = self._model.generate(  # type: ignore
             prepared_inputs,
             sampling_params,
             use_tqdm=False,  # type: ignore
```

### Comparing `distilabel-1.1.0/src/distilabel/llms/huggingface/__init__.py` & `distilabel-1.1.1/src/distilabel/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/huggingface/inference_endpoints.py` & `distilabel-1.1.1/src/distilabel/llms/huggingface/inference_endpoints.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/llms/huggingface/transformers.py` & `distilabel-1.1.1/src/distilabel/llms/huggingface/transformers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/mixins/__init__.py` & `distilabel-1.1.1/src/distilabel/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/mixins/runtime_parameters.py` & `distilabel-1.1.1/src/distilabel/mixins/runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/pipeline/__init__.py` & `distilabel-1.1.1/src/distilabel/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/pipeline/_dag.py` & `distilabel-1.1.1/src/distilabel/pipeline/_dag.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/pipeline/base.py` & `distilabel-1.1.1/src/distilabel/pipeline/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,21 +264,21 @@
         Returns:
             Will return the `Distiset` as the main run method would do.
         """
         self._dry_run = True
 
         for step_name in self.dag:
             step = self.dag.get_step(step_name)[STEP_ATTR_NAME]
+
             if step.is_generator:
-                if parameters.get(step_name) and parameters[step_name].get(
-                    "batch_size"
-                ):
-                    parameters[step_name]["batch_size"] = batch_size
+                if not parameters:
+                    parameters = {}
+                parameters[step_name] = {"batch_size": batch_size}
 
-        distiset = self.run(parameters, use_cache=False)
+        distiset = self.run(parameters=parameters, use_cache=False)
 
         self._dry_run = False
         return distiset
 
     def get_runtime_parameters_info(self) -> Dict[str, List[Dict[str, Any]]]:
         """Get the runtime parameters for the steps in the pipeline.
```

### Comparing `distilabel-1.1.0/src/distilabel/pipeline/constants.py` & `distilabel-1.1.1/src/distilabel/pipeline/constants.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/pipeline/local.py` & `distilabel-1.1.1/src/distilabel/pipeline/local.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/pipeline/routing_batch_function.py` & `distilabel-1.1.1/src/distilabel/pipeline/routing_batch_function.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/pipeline/typing.py` & `distilabel-1.1.1/src/distilabel/pipeline/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/pipeline/utils.py` & `distilabel-1.1.1/src/distilabel/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/base.py` & `distilabel-1.1.1/src/distilabel/steps/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/combine.py` & `distilabel-1.1.1/src/distilabel/steps/combine.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/decorator.py` & `distilabel-1.1.1/src/distilabel/steps/decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/deita.py` & `distilabel-1.1.1/src/distilabel/steps/deita.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/expand.py` & `distilabel-1.1.1/src/distilabel/steps/expand.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/keep.py` & `distilabel-1.1.1/src/distilabel/steps/keep.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/typing.py` & `distilabel-1.1.1/src/distilabel/steps/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/argilla/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/argilla/base.py` & `distilabel-1.1.1/src/distilabel/steps/argilla/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/argilla/preference.py` & `distilabel-1.1.1/src/distilabel/steps/argilla/preference.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/argilla/text_generation.py` & `distilabel-1.1.1/src/distilabel/steps/argilla/text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/formatting/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/formatting/conversation.py` & `distilabel-1.1.1/src/distilabel/steps/formatting/conversation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/formatting/dpo.py` & `distilabel-1.1.1/src/distilabel/steps/formatting/dpo.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/formatting/sft.py` & `distilabel-1.1.1/src/distilabel/steps/formatting/sft.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/generators/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/generators/data.py` & `distilabel-1.1.1/src/distilabel/steps/generators/data.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/generators/huggingface.py` & `distilabel-1.1.1/src/distilabel/steps/generators/huggingface.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/globals/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/globals/huggingface.py` & `distilabel-1.1.1/src/distilabel/steps/globals/huggingface.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/base.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/complexity_scorer.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/complexity_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/generate_embeddings.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/genstruct.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/genstruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/instruction_backtranslation.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/instruction_backtranslation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/pair_rm.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/pair_rm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/prometheus_eval.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/prometheus_eval.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/quality_scorer.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/quality_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/self_instruct.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/self_instruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/text_generation.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/typing.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/ultrafeedback.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/ultrafeedback.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/base.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/generator.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/utils.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/base.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_quality/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/utils.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/evol_quality/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/structured_outputs/__init__.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/structured_outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/structured_outputs/outlines.py` & `distilabel-1.1.1/src/distilabel/steps/tasks/structured_outputs/outlines.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/quality-scorer.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/quality-scorer.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/absolute_with_reference.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/prometheus/absolute_with_reference.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/absolute_without_reference.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/prometheus/absolute_without_reference.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/relative_with_reference.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/prometheus/relative_with_reference.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/relative_without_reference.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/prometheus/relative_without_reference.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2` & `distilabel-1.1.1/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/__init__.py` & `distilabel-1.1.1/src/distilabel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/chat.py` & `distilabel-1.1.1/src/distilabel/utils/chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/dicts.py` & `distilabel-1.1.1/src/distilabel/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/docstring.py` & `distilabel-1.1.1/src/distilabel/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/export_components_info.py` & `distilabel-1.1.1/src/distilabel/utils/export_components_info.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/files.py` & `distilabel-1.1.1/src/distilabel/utils/files.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/itertools.py` & `distilabel-1.1.1/src/distilabel/utils/itertools.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/lists.py` & `distilabel-1.1.1/src/distilabel/utils/lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/logging.py` & `distilabel-1.1.1/src/distilabel/utils/logging.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/notebook.py` & `distilabel-1.1.1/src/distilabel/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/serialization.py` & `distilabel-1.1.1/src/distilabel/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/typing_.py` & `distilabel-1.1.1/src/distilabel/utils/typing_.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/card/__init__.py` & `distilabel-1.1.1/src/distilabel/utils/card/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/card/dataset_card.py` & `distilabel-1.1.1/src/distilabel/utils/card/dataset_card.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/card/distilabel_template.md` & `distilabel-1.1.1/src/distilabel/utils/card/distilabel_template.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/mkdocs/__init__.py` & `distilabel-1.1.1/src/distilabel/utils/mkdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/mkdocs/components_gallery.py` & `distilabel-1.1.1/src/distilabel/utils/mkdocs/components_gallery.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/index.md` & `distilabel-1.1.1/src/distilabel/utils/mkdocs/templates/components-gallery/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/llm-detail.jinja2` & `distilabel-1.1.1/src/distilabel/utils/mkdocs/templates/components-gallery/llm-detail.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/step-detail.jinja2` & `distilabel-1.1.1/src/distilabel/utils/mkdocs/templates/components-gallery/step-detail.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/__init__.py` & `distilabel-1.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/integration/test_branching_missaligmnent.py` & `distilabel-1.1.1/tests/integration/test_branching_missaligmnent.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/integration/test_pipe_llms.py` & `distilabel-1.1.1/tests/integration/test_pipe_llms.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/integration/test_pipe_simple.py` & `distilabel-1.1.1/tests/integration/test_pipe_simple.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/integration/test_routing_batch_function.py` & `distilabel-1.1.1/tests/integration/test_routing_batch_function.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/__init__.py` & `distilabel-1.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/helpers.py` & `distilabel-1.1.1/tests/unit/helpers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/test_distiset.py` & `distilabel-1.1.1/tests/unit/test_distiset.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/test_imports.py` & `distilabel-1.1.1/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/cli/__init__.py` & `distilabel-1.1.1/tests/unit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/cli/test_pipeline.yaml` & `distilabel-1.1.1/tests/unit/cli/test_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/cli/utils.py` & `distilabel-1.1.1/tests/unit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/cli/pipeline/__init__.py` & `distilabel-1.1.1/tests/unit/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/cli/pipeline/test_app.py` & `distilabel-1.1.1/tests/unit/cli/pipeline/test_app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/cli/pipeline/utils.py` & `distilabel-1.1.1/tests/unit/cli/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/__init__.py` & `distilabel-1.1.1/tests/unit/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_anthropic.py` & `distilabel-1.1.1/tests/unit/llms/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_anyscale.py` & `distilabel-1.1.1/tests/unit/llms/test_anyscale.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_azure.py` & `distilabel-1.1.1/tests/unit/llms/test_azure.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_cohere.py` & `distilabel-1.1.1/tests/unit/llms/test_cohere.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_groq.py` & `distilabel-1.1.1/tests/unit/llms/test_groq.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_litellm.py` & `distilabel-1.1.1/tests/unit/llms/test_litellm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_llamacpp.py` & `distilabel-1.1.1/tests/unit/llms/test_llamacpp.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_mistral.py` & `distilabel-1.1.1/tests/unit/llms/test_mistral.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_mixins.py` & `distilabel-1.1.1/tests/unit/llms/test_mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_ollama.py` & `distilabel-1.1.1/tests/unit/llms/test_ollama.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_openai.py` & `distilabel-1.1.1/tests/unit/llms/test_openai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_together.py` & `distilabel-1.1.1/tests/unit/llms/test_together.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/test_vertexai.py` & `distilabel-1.1.1/tests/unit/llms/test_vertexai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/huggingface/__init__.py` & `distilabel-1.1.1/tests/unit/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/huggingface/test_inference_endpoints.py` & `distilabel-1.1.1/tests/unit/llms/huggingface/test_inference_endpoints.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/llms/huggingface/test_transformers.py` & `distilabel-1.1.1/tests/unit/llms/huggingface/test_transformers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/mixins/__init__.py` & `distilabel-1.1.1/tests/unit/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/mixins/test_runtime_parameters.py` & `distilabel-1.1.1/tests/unit/mixins/test_runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/pipeline/__init__.py` & `distilabel-1.1.1/tests/unit/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/pipeline/conftest.py` & `distilabel-1.1.1/tests/unit/pipeline/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/pipeline/test_base.py` & `distilabel-1.1.1/tests/unit/pipeline/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/pipeline/test_dag.py` & `distilabel-1.1.1/tests/unit/pipeline/test_dag.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/pipeline/test_local.py` & `distilabel-1.1.1/tests/unit/pipeline/test_local.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/pipeline/test_routing_batch_function.py` & `distilabel-1.1.1/tests/unit/pipeline/test_routing_batch_function.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/pipeline/utils.py` & `distilabel-1.1.1/tests/unit/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/__init__.py` & `distilabel-1.1.1/tests/unit/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/test_base.py` & `distilabel-1.1.1/tests/unit/steps/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/test_combine.py` & `distilabel-1.1.1/tests/unit/steps/test_combine.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/test_decorator.py` & `distilabel-1.1.1/tests/unit/steps/test_decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/test_deita.py` & `distilabel-1.1.1/tests/unit/steps/test_deita.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/test_expand.py` & `distilabel-1.1.1/tests/unit/steps/test_expand.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/test_keep.py` & `distilabel-1.1.1/tests/unit/steps/test_keep.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/argilla/__init__.py` & `distilabel-1.1.1/tests/unit/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/argilla/test_base.py` & `distilabel-1.1.1/tests/unit/steps/argilla/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/argilla/test_preference.py` & `distilabel-1.1.1/tests/unit/steps/argilla/test_preference.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/argilla/test_text_generation.py` & `distilabel-1.1.1/tests/unit/steps/argilla/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/formatting/__init__.py` & `distilabel-1.1.1/tests/unit/steps/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/formatting/test_conversation.py` & `distilabel-1.1.1/tests/unit/steps/formatting/test_conversation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/formatting/test_dpo.py` & `distilabel-1.1.1/tests/unit/steps/formatting/test_dpo.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/formatting/test_sft.py` & `distilabel-1.1.1/tests/unit/steps/formatting/test_sft.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/generators/test_data.py` & `distilabel-1.1.1/tests/unit/steps/generators/test_data.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/generators/test_huggingface.py` & `distilabel-1.1.1/tests/unit/steps/generators/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/__init__.py` & `distilabel-1.1.1/tests/unit/steps/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/conftest.py` & `distilabel-1.1.1/tests/unit/steps/tasks/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_base.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_complexity_scorer.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_complexity_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_generate_embeddings.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_genstruct.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_genstruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_instruction_backtranslation.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_instruction_backtranslation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_pair_rm.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_pair_rm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_prometheus_eval.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_prometheus_eval.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_quality_scorer.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_quality_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_self_instruct.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_self_instruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_text_generation.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/test_ultrafeedback.py` & `distilabel-1.1.1/tests/unit/steps/tasks/test_ultrafeedback.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/utils.py` & `distilabel-1.1.1/tests/unit/steps/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/test_base.py` & `distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/test_generator.py` & `distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/test_generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py` & `distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py` & `distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py` & `distilabel-1.1.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/evol_quality/__init__.py` & `distilabel-1.1.1/tests/unit/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/evol_quality/test_base.py` & `distilabel-1.1.1/tests/unit/steps/tasks/evol_quality/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/structured_outputs/__init__.py` & `distilabel-1.1.1/tests/unit/steps/tasks/structured_outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/steps/tasks/structured_outputs/test_outlines.py` & `distilabel-1.1.1/tests/unit/steps/tasks/structured_outputs/test_outlines.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/utils/__init__.py` & `distilabel-1.1.1/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/utils/test_chat.py` & `distilabel-1.1.1/tests/unit/utils/test_chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/utils/test_docstring.py` & `distilabel-1.1.1/tests/unit/utils/test_docstring.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/utils/test_files.py` & `distilabel-1.1.1/tests/unit/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/utils/test_lists.py` & `distilabel-1.1.1/tests/unit/utils/test_lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/tests/unit/utils/test_typing.py` & `distilabel-1.1.1/tests/unit/utils/test_typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/.gitignore` & `distilabel-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/LICENSE` & `distilabel-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/LICENSE_HEADER` & `distilabel-1.1.1/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/README.md` & `distilabel-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/pyproject.toml` & `distilabel-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `distilabel-1.1.0/PKG-INFO` & `distilabel-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: distilabel
-Version: 1.1.0
+Version: 1.1.1
 Summary: Distilabel is an AI Feedback (AIF) framework for building datasets with and for LLMs.
 Project-URL: Documentation, https://distilabel.argilla.io/
 Project-URL: Issues, https://github.com/argilla/distilabel/issues
 Project-URL: Source, https://github.com/argilla/distilabel
 Author-email: Argilla <admin@argilla.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: distilabel Version: 1.1.0 Summary: Distilabel is an
+Metadata-Version: 2.3 Name: distilabel Version: 1.1.1 Summary: Distilabel is an
 AI Feedback (AIF) framework for building datasets with and for LLMs. Project-
 URL: Documentation, https://distilabel.argilla.io/ Project-URL: Issues, https:/
 /github.com/argilla/distilabel/issues Project-URL: Source, https://github.com/
 argilla/distilabel Author-email: Argilla
 argilla.io> License-Expression: Apache-2.0 License-File: LICENSE License-File:
 LICENSE_HEADER Keywords: alignment,annotation,data,llm,rlaif,synthetic
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
```

