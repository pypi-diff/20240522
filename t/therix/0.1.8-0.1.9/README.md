# Comparing `tmp/therix-0.1.8.tar.gz` & `tmp/therix-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "therix-0.1.8.tar", max compression
+gzip compressed data, was "therix-0.1.9.tar", max compression
```

## Comparing `therix-0.1.8.tar` & `therix-0.1.9.tar`

### file list

```diff
@@ -1,119 +1,120 @@
--rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.8/LICENSE
--rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.8/README.md
--rw-r--r--   0        0        0     1202 2024-05-20 05:54:01.079924 therix-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.8/therix/__init__.py
--rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.8/therix/alembic/README
--rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.8/therix/alembic/env.py
--rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.8/therix/alembic/script.py.mako
--rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.8/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
--rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.8/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
--rw-r--r--   0        0        0      880 2024-05-08 11:24:55.867083 therix-0.1.8/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py
--rw-r--r--   0        0        0     2614 2024-05-14 09:23:25.311332 therix-0.1.8/therix/alembic/versions/2024_05_13_1842-f5c4562bcd86_added_config_type_for_system_prompt.py
--rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.8/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
--rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.8/therix/alembic.ini
--rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.8/therix/core/JSONLoader.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.8/therix/core/__init__.py
--rw-r--r--   0        0        0     2737 2024-05-13 10:00:13.299373 therix-0.1.8/therix/core/cache.py
--rw-r--r--   0        0        0     1399 2024-05-13 10:00:13.301278 therix-0.1.8/therix/core/chat_history/base_chat_history.py
--rw-r--r--   0        0        0     1771 2024-05-20 05:38:26.419587 therix-0.1.8/therix/core/constants.py
--rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.8/therix/core/data_sources.py
--rw-r--r--   0        0        0     1854 2024-05-20 05:38:26.420061 therix-0.1.8/therix/core/embedding_models.py
--rw-r--r--   0        0        0     2722 2024-05-20 05:38:26.420176 therix-0.1.8/therix/core/inference_models.py
--rw-r--r--   0        0        0      317 2024-05-13 10:00:13.302010 therix-0.1.8/therix/core/output_parser.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.8/therix/core/output_source.py
--rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.8/therix/core/pii_filter_config.py
--rw-r--r--   0        0        0     6893 2024-05-20 05:38:26.420716 therix-0.1.8/therix/core/pipeline.py
--rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.8/therix/core/pipeline_component.py
--rw-r--r--   0        0        0      238 2024-05-08 11:24:55.868662 therix-0.1.8/therix/core/response.py
--rw-r--r--   0        0        0      594 2024-05-13 10:00:13.302774 therix-0.1.8/therix/core/summarizer_config.py
--rw-r--r--   0        0        0       98 2024-05-13 10:00:13.302847 therix-0.1.8/therix/core/summarizer_output_model.py
--rw-r--r--   0        0        0      328 2024-05-14 09:23:25.312543 therix-0.1.8/therix/core/system_prompt_config.py
--rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.8/therix/core/trace.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.8/therix/db/__init__.py
--rw-r--r--   0        0        0     3757 2024-05-14 09:52:11.737008 therix-0.1.8/therix/db/db_manager.py
--rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.8/therix/db/session.py
--rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.8/therix/db/tests/__init__.py
--rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.8/therix/db/tests/test_db_manager.py
--rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.8/therix/docs/.gitignore
--rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.8/therix/docs/README.md
--rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.8/therix/docs/babel.config.js
--rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.8/therix/docs/blog/2019-05-28-first-blog-post.md
--rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.8/therix/docs/blog/2019-05-29-long-blog-post.md
--rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.8/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
--rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.8/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.8/therix/docs/blog/2021-08-26-welcome/index.md
--rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.8/therix/docs/blog/authors.yml
--rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.8/therix/docs/docs/LLM-Proxy/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.8/therix/docs/docs/LLM-Proxy/index.md
--rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.8/therix/docs/docs/core-components/_category_.json
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/_category_.json
--rw-r--r--   0        0        0     3533 2024-05-08 11:24:55.869158 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/caching.md
--rw-r--r--   0        0        0     1288 2024-05-08 11:24:55.869292 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
--rw-r--r--   0        0        0     3959 2024-05-08 11:24:55.869587 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
--rw-r--r--   0        0        0     5428 2024-05-13 10:00:13.303279 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
--rw-r--r--   0        0        0   101843 2024-05-08 11:24:55.870971 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG
--rw-r--r--   0        0        0    87594 2024-05-08 11:24:55.871966 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG
--rw-r--r--   0        0        0     1474 2024-05-20 05:38:26.421148 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/system-prompt.md
--rw-r--r--   0        0        0     1835 2024-05-08 11:24:55.872168 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/trace.md
--rw-r--r--   0        0        0     1377 2024-05-08 11:24:55.868823 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations.md
--rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.8/therix/docs/docs/core-components/pipeline-templates.md
--rw-r--r--   0        0        0     3488 2024-05-08 11:24:55.872304 therix-0.1.8/therix/docs/docs/core-components/pipeline.md
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.8/therix/docs/docs/introduction/_category_.json
--rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.8/therix/docs/docs/introduction/getting-started.md
--rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.8/therix/docs/docs/introduction/index.md
--rw-r--r--   0        0        0     1813 2024-05-08 11:24:55.872443 therix-0.1.8/therix/docs/docs/introduction/installation.md
--rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.8/therix/docs/docs/observability/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.8/therix/docs/docs/observability/index.md
--rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.8/therix/docs/docs/squad/_category_.json
--rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.8/therix/docs/docs/squad/index.md
--rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.8/therix/docs/docs/usage/_category_.json
--rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.8/therix/docs/docs/usage/index.md
--rw-r--r--   0        0        0     3717 2024-05-13 10:00:13.303378 therix-0.1.8/therix/docs/docs/use-cases/Keyword Search.md
--rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.8/therix/docs/docs/use-cases/_category_.json
--rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.8/therix/docs/docs/use-cases/faq.md
--rw-r--r--   0        0        0     3579 2024-05-13 10:00:13.303497 therix-0.1.8/therix/docs/docs/use-cases/pii_filer.md
--rw-r--r--   0        0        0     4861 2024-05-14 09:23:25.314499 therix-0.1.8/therix/docs/docs/use-cases/summarizer.md
--rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.8/therix/docs/docusaurus.config.js
--rw-r--r--   0        0        0      133 2024-05-13 10:00:13.303753 therix-0.1.8/therix/docs/firebase.json
--rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.8/therix/docs/package-lock.json
--rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.8/therix/docs/package.json
--rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.8/therix/docs/sidebars.js
--rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.8/therix/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.8/therix/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.8/therix/docs/src/css/custom.css
--rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.8/therix/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.8/therix/docs/src/pages/markdown-page.md
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.8/therix/docs/static/.nojekyll
--rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.8/therix/docs/static/img/coditas.png
--rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.8/therix/docs/static/img/coditasLogo.svg
--rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.8/therix/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.8/therix/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.8/therix/docs/static/img/favicon.ico
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.8/therix/docs/static/img/icon.svg
--rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.8/therix/docs/static/img/logo.png
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.8/therix/docs/static/img/logo.svg
--rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.8/therix/docs/static/img/therix-logo.png
--rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.8/therix/docs/static/img/undraw_docusaurus_mountain.svg
--rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.8/therix/docs/static/img/undraw_docusaurus_react.svg
--rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.8/therix/docs/static/img/undraw_docusaurus_tree.svg
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.8/therix/entities/__init__.py
--rw-r--r--   0        0        0     2571 2024-05-20 05:38:26.421434 therix-0.1.8/therix/entities/models.py
--rw-r--r--   0        0        0     2480 2024-05-20 05:38:26.421562 therix-0.1.8/therix/examples/cache_config_example.py
--rw-r--r--   0        0        0     1294 2024-05-20 05:38:26.421625 therix-0.1.8/therix/examples/gemini.rag.py
--rw-r--r--   0        0        0     2748 2024-05-20 05:38:26.421736 therix-0.1.8/therix/examples/keyword_search_examples.py
--rw-r--r--   0        0        0     2475 2024-05-14 09:52:11.737235 therix-0.1.8/therix/examples/main.py
--rw-r--r--   0        0        0     2099 2024-05-20 05:38:26.421832 therix-0.1.8/therix/examples/pii_filter_example.py
--rw-r--r--   0        0        0     6384 2024-05-20 05:38:26.422087 therix-0.1.8/therix/examples/summarizer_example.py
--rw-r--r--   0        0        0     6934 2024-05-14 09:52:11.737539 therix-0.1.8/therix/examples/system_prompt_example.py
--rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.8/therix/pylintrc
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.8/therix/services/__init__.py
--rw-r--r--   0        0        0     7603 2024-05-20 05:38:26.422335 therix-0.1.8/therix/services/pipeline_service.py
--rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.8/therix/services/web_crawling.py
--rw-r--r--   0        0        0     2077 2024-05-13 10:00:13.304865 therix-0.1.8/therix/tests/test_cache.py
--rw-r--r--   0        0        0      602 2024-05-08 11:24:55.874269 therix-0.1.8/therix/tests/test_pii_filter.py
--rw-r--r--   0        0        0     8197 2024-05-13 10:00:13.305133 therix-0.1.8/therix/tests/test_summarizer.py
--rw-r--r--   0        0        0     3591 2024-05-20 05:38:26.422456 therix-0.1.8/therix/utils/keyword_search.py
--rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.8/therix/utils/pii_filter.py
--rw-r--r--   0        0        0    13454 2024-05-20 05:38:26.422650 therix-0.1.8/therix/utils/rag.py
--rw-r--r--   0        0        0     5140 2024-05-20 05:38:26.422883 therix-0.1.8/therix/utils/summarizer.py
--rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 therix-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.9/README.md
+-rw-r--r--   0        0        0     1202 2024-05-22 12:26:19.698854 therix-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.9/therix/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.9/therix/alembic/README
+-rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.9/therix/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.9/therix/alembic/script.py.mako
+-rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.9/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
+-rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.9/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
+-rw-r--r--   0        0        0      880 2024-05-08 11:24:55.867083 therix-0.1.9/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py
+-rw-r--r--   0        0        0     2614 2024-05-14 09:23:25.311332 therix-0.1.9/therix/alembic/versions/2024_05_13_1842-f5c4562bcd86_added_config_type_for_system_prompt.py
+-rw-r--r--   0        0        0      851 2024-05-22 12:25:37.404056 therix-0.1.9/therix/alembic/versions/2024_05_21_1701-3d84bc32c8ee_changes_type_of_session_id.py
+-rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.9/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
+-rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.9/therix/alembic.ini
+-rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.9/therix/core/JSONLoader.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.9/therix/core/__init__.py
+-rw-r--r--   0        0        0     2737 2024-05-13 10:00:13.299373 therix-0.1.9/therix/core/cache.py
+-rw-r--r--   0        0        0     2152 2024-05-22 12:25:37.404872 therix-0.1.9/therix/core/chat_history/base_chat_history.py
+-rw-r--r--   0        0        0     1771 2024-05-20 05:38:26.419587 therix-0.1.9/therix/core/constants.py
+-rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.9/therix/core/data_sources.py
+-rw-r--r--   0        0        0     1854 2024-05-20 05:38:26.420061 therix-0.1.9/therix/core/embedding_models.py
+-rw-r--r--   0        0        0     2722 2024-05-20 05:38:26.420176 therix-0.1.9/therix/core/inference_models.py
+-rw-r--r--   0        0        0      317 2024-05-13 10:00:13.302010 therix-0.1.9/therix/core/output_parser.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.9/therix/core/output_source.py
+-rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.9/therix/core/pii_filter_config.py
+-rw-r--r--   0        0        0     7272 2024-05-22 12:25:37.405438 therix-0.1.9/therix/core/pipeline.py
+-rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.9/therix/core/pipeline_component.py
+-rw-r--r--   0        0        0      238 2024-05-08 11:24:55.868662 therix-0.1.9/therix/core/response.py
+-rw-r--r--   0        0        0      594 2024-05-13 10:00:13.302774 therix-0.1.9/therix/core/summarizer_config.py
+-rw-r--r--   0        0        0       98 2024-05-13 10:00:13.302847 therix-0.1.9/therix/core/summarizer_output_model.py
+-rw-r--r--   0        0        0      328 2024-05-14 09:23:25.312543 therix-0.1.9/therix/core/system_prompt_config.py
+-rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.9/therix/core/trace.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.9/therix/db/__init__.py
+-rw-r--r--   0        0        0     3757 2024-05-14 09:52:11.737008 therix-0.1.9/therix/db/db_manager.py
+-rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.9/therix/db/session.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.9/therix/db/tests/__init__.py
+-rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.9/therix/db/tests/test_db_manager.py
+-rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.9/therix/docs/.gitignore
+-rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.9/therix/docs/README.md
+-rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.9/therix/docs/babel.config.js
+-rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.9/therix/docs/blog/2019-05-28-first-blog-post.md
+-rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.9/therix/docs/blog/2019-05-29-long-blog-post.md
+-rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.9/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
+-rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.9/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.9/therix/docs/blog/2021-08-26-welcome/index.md
+-rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.9/therix/docs/blog/authors.yml
+-rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.9/therix/docs/docs/LLM-Proxy/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.9/therix/docs/docs/LLM-Proxy/index.md
+-rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.9/therix/docs/docs/core-components/_category_.json
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/_category_.json
+-rw-r--r--   0        0        0     3533 2024-05-08 11:24:55.869158 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/caching.md
+-rw-r--r--   0        0        0     1288 2024-05-08 11:24:55.869292 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
+-rw-r--r--   0        0        0     3959 2024-05-08 11:24:55.869587 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
+-rw-r--r--   0        0        0     5428 2024-05-13 10:00:13.303279 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
+-rw-r--r--   0        0        0   101843 2024-05-08 11:24:55.870971 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG
+-rw-r--r--   0        0        0    87594 2024-05-08 11:24:55.871966 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG
+-rw-r--r--   0        0        0     1474 2024-05-20 05:38:26.421148 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/system-prompt.md
+-rw-r--r--   0        0        0     1835 2024-05-08 11:24:55.872168 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/trace.md
+-rw-r--r--   0        0        0     1377 2024-05-08 11:24:55.868823 therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations.md
+-rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.9/therix/docs/docs/core-components/pipeline-templates.md
+-rw-r--r--   0        0        0     3488 2024-05-08 11:24:55.872304 therix-0.1.9/therix/docs/docs/core-components/pipeline.md
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.9/therix/docs/docs/introduction/_category_.json
+-rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.9/therix/docs/docs/introduction/getting-started.md
+-rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.9/therix/docs/docs/introduction/index.md
+-rw-r--r--   0        0        0     1813 2024-05-08 11:24:55.872443 therix-0.1.9/therix/docs/docs/introduction/installation.md
+-rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.9/therix/docs/docs/observability/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.9/therix/docs/docs/observability/index.md
+-rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.9/therix/docs/docs/squad/_category_.json
+-rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.9/therix/docs/docs/squad/index.md
+-rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.9/therix/docs/docs/usage/_category_.json
+-rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.9/therix/docs/docs/usage/index.md
+-rw-r--r--   0        0        0     4242 2024-05-22 12:25:37.405807 therix-0.1.9/therix/docs/docs/use-cases/Keyword Search.md
+-rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.9/therix/docs/docs/use-cases/_category_.json
+-rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.9/therix/docs/docs/use-cases/faq.md
+-rw-r--r--   0        0        0     3579 2024-05-13 10:00:13.303497 therix-0.1.9/therix/docs/docs/use-cases/pii_filer.md
+-rw-r--r--   0        0        0     4861 2024-05-14 09:23:25.314499 therix-0.1.9/therix/docs/docs/use-cases/summarizer.md
+-rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.9/therix/docs/docusaurus.config.js
+-rw-r--r--   0        0        0      133 2024-05-13 10:00:13.303753 therix-0.1.9/therix/docs/firebase.json
+-rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.9/therix/docs/package-lock.json
+-rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.9/therix/docs/package.json
+-rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.9/therix/docs/sidebars.js
+-rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.9/therix/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.9/therix/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.9/therix/docs/src/css/custom.css
+-rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.9/therix/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.9/therix/docs/src/pages/markdown-page.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.9/therix/docs/static/.nojekyll
+-rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.9/therix/docs/static/img/coditas.png
+-rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.9/therix/docs/static/img/coditasLogo.svg
+-rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.9/therix/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.9/therix/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.9/therix/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.9/therix/docs/static/img/icon.svg
+-rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.9/therix/docs/static/img/logo.png
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.9/therix/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.9/therix/docs/static/img/therix-logo.png
+-rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.9/therix/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.9/therix/docs/static/img/undraw_docusaurus_react.svg
+-rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.9/therix/docs/static/img/undraw_docusaurus_tree.svg
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.9/therix/entities/__init__.py
+-rw-r--r--   0        0        0     2571 2024-05-22 12:25:33.460779 therix-0.1.9/therix/entities/models.py
+-rw-r--r--   0        0        0     2480 2024-05-20 05:38:26.421562 therix-0.1.9/therix/examples/cache_config_example.py
+-rw-r--r--   0        0        0     1294 2024-05-20 05:38:26.421625 therix-0.1.9/therix/examples/gemini.rag.py
+-rw-r--r--   0        0        0     2748 2024-05-20 05:38:26.421736 therix-0.1.9/therix/examples/keyword_search_examples.py
+-rw-r--r--   0        0        0     2475 2024-05-14 09:52:11.737235 therix-0.1.9/therix/examples/main.py
+-rw-r--r--   0        0        0     2099 2024-05-20 05:38:26.421832 therix-0.1.9/therix/examples/pii_filter_example.py
+-rw-r--r--   0        0        0     6384 2024-05-20 05:38:26.422087 therix-0.1.9/therix/examples/summarizer_example.py
+-rw-r--r--   0        0        0     6934 2024-05-14 09:52:11.737539 therix-0.1.9/therix/examples/system_prompt_example.py
+-rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.9/therix/pylintrc
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.9/therix/services/__init__.py
+-rw-r--r--   0        0        0     7796 2024-05-22 12:25:37.406177 therix-0.1.9/therix/services/pipeline_service.py
+-rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.9/therix/services/web_crawling.py
+-rw-r--r--   0        0        0     2077 2024-05-13 10:00:13.304865 therix-0.1.9/therix/tests/test_cache.py
+-rw-r--r--   0        0        0      602 2024-05-08 11:24:55.874269 therix-0.1.9/therix/tests/test_pii_filter.py
+-rw-r--r--   0        0        0     8197 2024-05-13 10:00:13.305133 therix-0.1.9/therix/tests/test_summarizer.py
+-rw-r--r--   0        0        0     3591 2024-05-20 05:38:26.422456 therix-0.1.9/therix/utils/keyword_search.py
+-rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.9/therix/utils/pii_filter.py
+-rw-r--r--   0        0        0    13915 2024-05-22 12:25:37.407093 therix-0.1.9/therix/utils/rag.py
+-rw-r--r--   0        0        0     5131 2024-05-22 12:25:37.407493 therix-0.1.9/therix/utils/summarizer.py
+-rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 therix-0.1.9/PKG-INFO
```

### Comparing `therix-0.1.8/LICENSE` & `therix-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/README.md` & `therix-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/pyproject.toml` & `therix-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "therix"
-version = "0.1.8"
+version = "0.1.9"
 description = "Therix is the SDK for langchain based applications."
 authors = ["Ajinath"]
 license = "MIT"
 readme = "README.md"
 include = ["alembic/**/*", "alembic.ini"]
 
 [tool.poetry.dependencies]
```

### Comparing `therix-0.1.8/therix/alembic/env.py` & `therix-0.1.9/therix/alembic/env.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/alembic/script.py.mako` & `therix-0.1.9/therix/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py` & `therix-0.1.9/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py` & `therix-0.1.9/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py` & `therix-0.1.9/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/alembic/versions/2024_05_13_1842-f5c4562bcd86_added_config_type_for_system_prompt.py` & `therix-0.1.9/therix/alembic/versions/2024_05_13_1842-f5c4562bcd86_added_config_type_for_system_prompt.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py` & `therix-0.1.9/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/alembic.ini` & `therix-0.1.9/therix/alembic.ini`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/core/JSONLoader.py` & `therix-0.1.9/therix/core/JSONLoader.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/core/cache.py` & `therix-0.1.9/therix/core/cache.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/core/constants.py` & `therix-0.1.9/therix/core/constants.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/core/data_sources.py` & `therix-0.1.9/therix/core/data_sources.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/core/embedding_models.py` & `therix-0.1.9/therix/core/embedding_models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/core/inference_models.py` & `therix-0.1.9/therix/core/inference_models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/core/pipeline.py` & `therix-0.1.9/therix/core/pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from uuid import uuid4
+import uuid
 from therix.core.pipeline_component import PipelineComponent
 from .constants import DataSourceMaster, EmbeddingModelMaster, PipelineTypeMaster  # Import your constants
 from ..services.pipeline_service import PipelineService  # Import your service
 from ..entities.models import ConfigType  # Import your ConfigType enum
 from ..services.pipeline_service import PipelineService  # Import your service
 from langchain.globals import set_llm_cache
 from therix.core.response import ModelResponse
@@ -88,56 +89,65 @@
         self.pipeline_data = self.pipeline_service.get_pipeline(pipeline_id)
         self.id = self.pipeline_data.id
         self.name = self.pipeline_data.name
         return self.pipeline_data
 
     def preprocess_data(self):
        return self.pipeline_service.preprocess_data(self.pipeline_data.id)
+    
 
-    def invoke(self, question=None, session_id=None , keyword_search_params=None):
-            cached_response = None
-            therix_cache = TherixCache(engine)
-            inference_model = self.pipeline_service.get_pipeline_configuraitons_by_type(self.pipeline_data.id, ConfigType.INFERENCE_MODEL)
-
-            if session_id is None:
-                session_id = uuid4()
-            add_cache = self.pipeline_service.get_pipeline_configuraitons_by_type(self.pipeline_data.id, ConfigType.CACHE_CONFIG)
-            
-            if(question == None and keyword_search_params == None):
-                return "Please provide the required Parameters to invoke the pipeline"
-
-            pipeline_trace_config = self.pipeline_service.get_pipeline_configuraitons_by_type(
-                self.pipeline_data.id, ConfigType.TRACE_DETAILS
-            )
-            pipeline_system_prompt = self.pipeline_service.get_pipeline_configuraitons_by_type(self.pipeline_data.id, ConfigType.SYSTEM_PROMPT)
-            trace_details = pipeline_trace_config[0].config if pipeline_trace_config else None
-
-            pipeline_type = self.pipeline_service.get_pipeline(self.pipeline_data.id).type.value
-
-            if pipeline_type == PipelineTypeMaster.RAG.value:
-                if add_cache:
-                    cached_response = therix_cache.lookup(question, inference_model[0].name, self.pipeline_data.id)
+    def get_configurations(self,pipeline_id):
+        therix_cache = TherixCache(engine)
+        inference_model = self.pipeline_service.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.INFERENCE_MODEL)
+        add_cache = self.pipeline_service.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.CACHE_CONFIG)
+        pipeline_trace_config = self.pipeline_service.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.TRACE_DETAILS)
+        saved_system_prompt = self.pipeline_service.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.SYSTEM_PROMPT)
+        pipeline_type = self.pipeline_service.get_pipeline(pipeline_id).type.value
+
+        return therix_cache, inference_model, add_cache, pipeline_trace_config, saved_system_prompt, pipeline_type
+
+    def invoke(self, question=None, session_id=None , keyword_search_params=None, dynamic_system_prompt=None):
+         # Check if required parameters are provided
+        if question is None and keyword_search_params is None:
+            return "Please provide the required parameters to invoke the pipeline"
+
+        # Initialize session_id if not provided
+        if session_id is None:
+            session_id = str(uuid.uuid4())
+
+        therix_cache, inference_model, add_cache, pipeline_trace_config, saved_system_prompt, pipeline_type = self.get_configurations(self.pipeline_data.id)
+
+        # Determine system prompt to use
+        pipeline_system_prompt = {"system_prompt": dynamic_system_prompt} if dynamic_system_prompt else (saved_system_prompt[0].config if saved_system_prompt else None)
+        trace_details = pipeline_trace_config[0].config if pipeline_trace_config else None
+
+        # Handle RAG pipeline type
+        if pipeline_type == PipelineTypeMaster.RAG.value:
+            if add_cache:
+                cached_response = therix_cache.lookup(question, inference_model[0].name, self.pipeline_data.id)
                 if cached_response:
                     return ModelResponse(cached_response.response, session_id).create_response()
-                if (keyword_search_params and question == None):
-                    keyword_search_params['pipeline_id'] = self.pipeline_data.id
-                    keyword_search_params['trace_details'] = trace_details
-                    answer = self.pipeline_service.search_keywords(keyword_search_params)
-                else:
-                    if(pipeline_system_prompt):
-                        answer = self.pipeline_service.invoke_pipeline(
-                            self.pipeline_data.id, question, session_id, trace_details, pipeline_system_prompt[0]
-                        )
-                    else:
-                        answer = self.pipeline_service.invoke_pipeline(
-                            self.pipeline_data.id, question, session_id, trace_details
-                        )                        
-                if add_cache:
-                    therix_cache.update(question, inference_model[0].name, answer, self.pipeline_data.id)
-            elif pipeline_type == PipelineTypeMaster.SUMMARIZER.value:
-                if(pipeline_system_prompt):
-                    answer = self.pipeline_service.invoke_summarizer_pipeline(self.pipeline_data.id, text=question, trace_details=trace_details, system_prompt = pipeline_system_prompt[0])
-                else: 
-                    answer = self.pipeline_service.invoke_summarizer_pipeline(self.pipeline_data.id, text=question, trace_details=trace_details)
 
-            return ModelResponse(answer, session_id).create_response()
+            if keyword_search_params and question is None:
+                keyword_search_params['pipeline_id'] = self.pipeline_data.id
+                keyword_search_params['trace_details'] = trace_details
+                answer = self.pipeline_service.search_keywords(keyword_search_params)
+            else:
+                answer = self.pipeline_service.invoke_pipeline(
+                    self.pipeline_data.id, question, session_id, trace_details, pipeline_system_prompt
+                ) if pipeline_system_prompt else self.pipeline_service.invoke_pipeline(
+                    self.pipeline_data.id, question, session_id, trace_details
+                )
+
+            if add_cache:
+                therix_cache.update(question, inference_model[0].name, answer, self.pipeline_data.id)
+
+        # Handle Summarizer pipeline type
+        elif pipeline_type == PipelineTypeMaster.SUMMARIZER.value:
+            answer = self.pipeline_service.invoke_summarizer_pipeline(
+                self.pipeline_data.id, text=question, trace_details=trace_details, system_prompt=pipeline_system_prompt
+            ) if pipeline_system_prompt else self.pipeline_service.invoke_summarizer_pipeline(
+                self.pipeline_data.id, text=question, trace_details=trace_details
+            )
+
+        return ModelResponse(answer, session_id).create_response()
```

### Comparing `therix-0.1.8/therix/core/pipeline_component.py` & `therix-0.1.9/therix/core/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/core/summarizer_config.py` & `therix-0.1.9/therix/core/summarizer_config.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/db/db_manager.py` & `therix-0.1.9/therix/db/db_manager.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/db/tests/test_db_manager.py` & `therix-0.1.9/therix/db/tests/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/README.md` & `therix-0.1.9/therix/docs/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/blog/2019-05-29-long-blog-post.md` & `therix-0.1.9/therix/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `therix-0.1.9/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/blog/2021-08-26-welcome/index.md` & `therix-0.1.9/therix/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/caching.md` & `therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/caching.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/data-sources.md` & `therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/data-sources.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md` & `therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/inference-model.md` & `therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/inference-model.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG` & `therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG` & `therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/system-prompt.md` & `therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/system-prompt.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/trace.md` & `therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations/trace.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations.md` & `therix-0.1.9/therix/docs/docs/core-components/pipeline-configurations.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/core-components/pipeline.md` & `therix-0.1.9/therix/docs/docs/core-components/pipeline.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/introduction/getting-started.md` & `therix-0.1.9/therix/docs/docs/introduction/getting-started.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/introduction/index.md` & `therix-0.1.9/therix/docs/docs/introduction/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/introduction/installation.md` & `therix-0.1.9/therix/docs/docs/introduction/installation.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/use-cases/Keyword Search.md` & `therix-0.1.9/therix/docs/docs/use-cases/Keyword Search.md`

 * *Files 12% similar despite different names*

```diff
@@ -22,24 +22,30 @@
 First, you need to add the PDF documents that you want to analyze. Use the `add` method of the Pipeline object to add a PDFDataSource. Provide a list of file paths as the `files` parameter.
 
 Example:
 ```python
 pipeline.add(PDFDataSource(config={'files': ['./test-data/rat.pdf']}))
 ```
 
-### Step 2: Add Embedding Model
+### Step 2: Add Embedding Model and Inference Model
 Next, add an embedding model to convert text into numerical vectors for analysis. In the example, an Azure OpenAI Embedding 3 Large Embedding Model is added.
+Additionally, include an inference model to send the necessary data to the Language Model and obtain the desired output.
 
 Example:
 ```python
  .add(AzureOpenAIEmbedding3SmallEmbeddingModel(config={'azure_api_key':'',
                                                        'azure_endpoint':'',
                                                        'openai_api_version':'',
-                                                       'azure_deployment':''
-                                                          }))
+                                                       'azure_deployment':'',
+                                                          })
+ .add(AzureOpenAIGPT4InferenceModel(config={'azure_api_key':'',
+                                            'openai_api_version':'',
+                                            'azure_endpoint':'',
+                                            'azure_deployment':'',
+                                            'temperature':''}))                                                       
 ```
 
 
 ### Step 3: Define Output Parser
 An output parser is needed to structure the output based on requirements. In the example, a PydanticOutputParser is used.
 
 Example:
```

### Comparing `therix-0.1.8/therix/docs/docs/use-cases/pii_filer.md` & `therix-0.1.9/therix/docs/docs/use-cases/pii_filer.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docs/use-cases/summarizer.md` & `therix-0.1.9/therix/docs/docs/use-cases/summarizer.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/docusaurus.config.js` & `therix-0.1.9/therix/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/package-lock.json` & `therix-0.1.9/therix/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/package.json` & `therix-0.1.9/therix/docs/package.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/sidebars.js` & `therix-0.1.9/therix/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/src/components/HomepageFeatures/index.js` & `therix-0.1.9/therix/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/src/css/custom.css` & `therix-0.1.9/therix/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/coditas.png` & `therix-0.1.9/therix/docs/static/img/coditas.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/coditasLogo.svg` & `therix-0.1.9/therix/docs/static/img/coditasLogo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/docusaurus-social-card.jpg` & `therix-0.1.9/therix/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/docusaurus.png` & `therix-0.1.9/therix/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/favicon.ico` & `therix-0.1.9/therix/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/icon.svg` & `therix-0.1.9/therix/docs/static/img/icon.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/logo.png` & `therix-0.1.9/therix/docs/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/logo.svg` & `therix-0.1.9/therix/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/therix-logo.png` & `therix-0.1.9/therix/docs/static/img/therix-logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/undraw_docusaurus_mountain.svg` & `therix-0.1.9/therix/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/undraw_docusaurus_react.svg` & `therix-0.1.9/therix/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/docs/static/img/undraw_docusaurus_tree.svg` & `therix-0.1.9/therix/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/entities/models.py` & `therix-0.1.9/therix/entities/models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/examples/cache_config_example.py` & `therix-0.1.9/therix/examples/cache_config_example.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/examples/gemini.rag.py` & `therix-0.1.9/therix/examples/gemini.rag.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/examples/keyword_search_examples.py` & `therix-0.1.9/therix/examples/keyword_search_examples.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/examples/main.py` & `therix-0.1.9/therix/examples/main.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/examples/pii_filter_example.py` & `therix-0.1.9/therix/examples/pii_filter_example.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/examples/summarizer_example.py` & `therix-0.1.9/therix/examples/summarizer_example.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/examples/system_prompt_example.py` & `therix-0.1.9/therix/examples/system_prompt_example.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/pylintrc` & `therix-0.1.9/therix/pylintrc`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/services/pipeline_service.py` & `therix-0.1.9/therix/services/pipeline_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,17 @@
         new_pipeline = Pipeline(**pipeline_data)
         self.db_session.add(new_pipeline)
         self.db_session.flush()  # Flush to assign an ID to the new_pipeline
 
         for config_data in configurations_data:
             config_data["pipeline_id"] = new_pipeline.id
             new_config = PipelineConfiguration(**config_data)
+            if new_config.config_type == "INFERENCE_MODEL":
+                if("temperature" not in new_config.config) : 
+                    new_config.config["temperature"] = 0.5            
             self.db_session.add(new_config)
 
         self.db_session.commit()
         return new_pipeline
 
     def publish_pipeline(self, pipeline_data):
         pipeline = (
@@ -144,15 +147,15 @@
         embed_config=embedding_model.config
 
         llm = AzureChatOpenAI(
             deployment_name=keyword_search_params["infer_config"].get("azure_deployment"),
             azure_endpoint=keyword_search_params["infer_config"].get("azure_endpoint"),
             api_version=keyword_search_params["infer_config"].get("openai_api_version"),
             api_key=keyword_search_params["infer_config"].get("azure_api_key"),
-            temperature=keyword_search_params["infer_config"].get("temperature") or 0.7
+            temperature=keyword_search_params["infer_config"].get("temperature") or 0.5
         )
 
         keyword_search_dict = {
             "pipeline_id" : keyword_search_params.get("pipeline_id"),
             "config_id" : keyword_search_params.get("config_id"),
             "keywords": keyword_search_params.get("keywords"),
             "output_parser": keyword_search_params.get("output_parser"),
```

### Comparing `therix-0.1.8/therix/services/web_crawling.py` & `therix-0.1.9/therix/services/web_crawling.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/tests/test_cache.py` & `therix-0.1.9/therix/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/tests/test_pii_filter.py` & `therix-0.1.9/therix/tests/test_pii_filter.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/tests/test_summarizer.py` & `therix-0.1.9/therix/tests/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/utils/keyword_search.py` & `therix-0.1.9/therix/utils/keyword_search.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/utils/pii_filter.py` & `therix-0.1.9/therix/utils/pii_filter.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.8/therix/utils/rag.py` & `therix-0.1.9/therix/utils/rag.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.messages import get_buffer_string
 from langchain_core.prompts import format_document
 from langchain_core.runnables import RunnableParallel
 from langchain_text_splitters import  RecursiveCharacterTextSplitter
 from operator import itemgetter
 from langchain_experimental.data_anonymizer import PresidioReversibleAnonymizer
-
+from langchain_core.messages.chat import ChatMessage
 
 def sanitize_text(text):
     # Remove null characters (0x00) from the text
     sanitized_text = text.replace("\x00", "")
     return sanitized_text
 
 
@@ -135,48 +135,51 @@
     ) and ("azure_api_key" in config):
         return AzureChatOpenAI(
             api_key=config["azure_api_key"],
             model=inference_model_name,
             deployment_name=config["azure_deployment"],
             azure_endpoint=config["azure_endpoint"],
             api_version=config["openai_api_version"],
+            temperature=config["temperature"],
         )
     elif (
         inference_model_name == InferenceModelMaster.GROQ_LLM_MIXTRAL_8_7_B
         or inference_model_name == InferenceModelMaster.GROQ_LLM_LLAMA3_70B
         or inference_model_name == InferenceModelMaster.GROQ_LLM_GEMMA7B
     ) and ("groq_api_key" in config):
-        return ChatGroq(groq_api_key=config["groq_api_key"], model=inference_model_name)
+         return ChatGroq(groq_api_key=config["groq_api_key"], model=inference_model_name, temperature=config["temperature"])
 
     elif (
         inference_model_name == InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1
         or inference_model_name == InferenceModelMaster.BEDROCK_TEXT_LITE_G1
     ) and ("bedrock_aws_session_token" in config):
         bedrock_client = boto3.client(
             service_name="bedrock-runtime",
             aws_access_key_id=config["bedrock_aws_access_key_id"],
             aws_secret_access_key=config["bedrock_aws_secret_access_key"],
             aws_session_token=config["bedrock_aws_session_token"],
             region_name=config["bedrock_region_name"],
+            temperature=config["temperature"], 
         )
         return Bedrock(
             credentials_profile_name="bedrock-admin",
             model_id=inference_model_name,
             client=bedrock_client,
             region_name=config["bedrock_region_name"],
+            temperature=config["temperature"]
         )
     
     elif(
         inference_model_name == InferenceModelMaster.GOOGLE_GEMINI_PRO
         or inference_model_name == InferenceModelMaster.GOOGLE_GEMINI_1_5_PRO
     ) and ("google_api_key" in config):
         return ChatGoogleGenerativeAI(
             model=inference_model_name,
             google_api_key=config["google_api_key"],
-            temperature=0.7, 
+            temperature=config["temperature"], 
             top_p=0.85,
             metadata= {'language': 'en'}
           
 
         )
     else:
         raise ValueError(f"Unknown inference model: {inference_model_name}")
@@ -244,18 +247,24 @@
 
     history = TherixChatMessageHistory(
         str(session_id),
         str(pipeline_id),
         SQLALCHEMY_DATABASE_URL,
         table_name="chat_history",
     )
-    chat_history = history.messages
+    message_history = history.get_message_history(str(session_id))
+    chat_history=[]
+    for message in message_history:
+        chat_history.append(
+            ChatMessage(role=message["message_role"], content=message["message"])
+            
+        )
 
     if(system_prompt):
-        template = system_prompt.config.get("system_prompt")
+        template = system_prompt.get("system_prompt")
     else : 
         template = """
         Answer the question based only on the following context:
 
 {context}
 
 Answer the question based on the above context: {question}
```

### Comparing `therix-0.1.8/therix/utils/summarizer.py` & `therix-0.1.9/therix/utils/summarizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         Please structure your response in the following JSON format:
         {response_schema_json}
         """,
     "ABSTRACTIVE": "Provide a concise summary for the following text using abstractive summarization:\n\n{context}."
 }
         
 def summarizer(summarizer_config,inference_model_details,text, trace_details, system_prompt=None):
-    
+  
     chain_callbacks = []
     if trace_details is not None:
         langfuse_handler = CallbackHandler(
             secret_key=trace_details["secret_key"],
             public_key=trace_details["public_key"],
             host=trace_details["host"],
             trace_name=trace_details["identifier"],
@@ -107,15 +107,15 @@
     # Run the chain
     summary = map_reduce_chain.run(split_docs)
     
     parser = JsonOutputParser()
 
     if(system_prompt and summarization_type=="EXTRACTIVE"):
         prompt = PromptTemplate(
-            template=system_prompt.config.get("system_prompt"),
+            template=system_prompt.get("system_prompt"),
             input_variables=["context"],
             partial_variables={"response_schema_json": pydantic_prompt},
     )
     else: 
         prompt = PromptTemplate(
             template=PROMPT_TEMPLATE[summarization_type],
             input_variables=["context"],
```

### Comparing `therix-0.1.8/PKG-INFO` & `therix-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: therix
-Version: 0.1.8
+Version: 0.1.9
 Summary: Therix is the SDK for langchain based applications.
 License: MIT
 Author: Ajinath
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

