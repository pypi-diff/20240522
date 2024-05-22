# Comparing `tmp/medkit_lib-0.9.1.tar.gz` & `tmp/medkit_lib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medkit_lib-0.9.1.tar", max compression
+gzip compressed data, was "medkit_lib-0.9.2.tar", max compression
```

## Comparing `medkit_lib-0.9.1.tar` & `medkit_lib-0.9.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.9.1/LICENSE
--rw-r--r--   0        0        0     1282 2023-09-12 12:18:25.713016 medkit_lib-0.9.1/README.md
--rw-r--r--   0        0        0      173 2023-04-04 06:31:49.436370 medkit_lib-0.9.1/medkit/__init__.py
--rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.9.1/medkit/audio/__init__.py
--rw-r--r--   0        0        0      248 2023-04-04 06:31:49.436370 medkit_lib-0.9.1/medkit/audio/preprocessing/__init__.py
--rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.9.1/medkit/audio/preprocessing/downmixer.py
--rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.9.1/medkit/audio/preprocessing/power_normalizer.py
--rw-r--r--   0        0        0     2482 2023-04-21 12:33:02.946744 medkit_lib-0.9.1/medkit/audio/preprocessing/resampler.py
--rw-r--r--   0        0        0      250 2023-04-04 06:31:49.440370 medkit_lib-0.9.1/medkit/audio/segmentation/__init__.py
--rw-r--r--   0        0        0     6574 2023-09-25 09:03:10.286242 medkit_lib-0.9.1/medkit/audio/segmentation/pa_speaker_detector.py
--rw-r--r--   0        0        0     7416 2023-04-21 12:33:02.946744 medkit_lib-0.9.1/medkit/audio/segmentation/webrtc_voice_detector.py
--rw-r--r--   0        0        0      554 2023-06-27 14:10:01.377546 medkit_lib-0.9.1/medkit/audio/transcription/__init__.py
--rw-r--r--   0        0        0     7168 2023-06-27 14:10:01.377546 medkit_lib-0.9.1/medkit/audio/transcription/doc_transcriber.py
--rw-r--r--   0        0        0     3821 2023-06-27 14:10:01.377546 medkit_lib-0.9.1/medkit/audio/transcription/hf_transcriber_function.py
--rw-r--r--   0        0        0     4562 2023-06-27 14:10:01.377546 medkit_lib-0.9.1/medkit/audio/transcription/sb_transcriber_function.py
--rw-r--r--   0        0        0     4776 2023-06-27 14:10:01.377546 medkit_lib-0.9.1/medkit/audio/transcription/transcribed_document.py
--rw-r--r--   0        0        0     1549 2023-08-07 09:06:28.578043 medkit_lib-0.9.1/medkit/core/__init__.py
--rw-r--r--   0        0        0     7827 2023-04-20 16:18:05.215523 medkit_lib-0.9.1/medkit/core/_prov_graph.py
--rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/annotation.py
--rw-r--r--   0        0        0     4665 2023-03-28 15:25:00.537196 medkit_lib-0.9.1/medkit/core/annotation_container.py
--rw-r--r--   0        0        0     2969 2023-04-21 08:20:44.049464 medkit_lib-0.9.1/medkit/core/attribute.py
--rw-r--r--   0        0        0     3052 2023-03-28 15:25:00.537196 medkit_lib-0.9.1/medkit/core/attribute_container.py
--rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/audio/__init__.py
--rw-r--r--   0        0        0     3712 2023-07-21 10:01:08.934587 medkit_lib-0.9.1/medkit/core/audio/annotation.py
--rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/audio/annotation_container.py
--rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/audio/audio_buffer.py
--rw-r--r--   0        0        0     3835 2023-08-07 09:06:28.578043 medkit_lib-0.9.1/medkit/core/audio/document.py
--rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/audio/operation.py
--rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/audio/span.py
--rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/collection.py
--rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/conversion.py
--rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/data_item.py
--rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/dict_conv.py
--rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/doc_pipeline.py
--rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/document.py
--rw-r--r--   0        0        0      597 2023-08-07 09:06:28.578043 medkit_lib-0.9.1/medkit/core/id.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/operation.py
--rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/operation_desc.py
--rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/pipeline.py
--rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/prov_store.py
--rw-r--r--   0        0        0    11205 2023-07-21 10:01:08.934587 medkit_lib-0.9.1/medkit/core/prov_tracer.py
--rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.9.1/medkit/core/store.py
--rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/core/text/__init__.py
--rw-r--r--   0        0        0     8728 2023-04-04 06:31:49.484372 medkit_lib-0.9.1/medkit/core/text/annotation.py
--rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/core/text/annotation_container.py
--rw-r--r--   0        0        0     4694 2023-08-07 09:06:28.578043 medkit_lib-0.9.1/medkit/core/text/document.py
--rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/core/text/entity_attribute_container.py
--rw-r--r--   0        0        0     3244 2023-04-21 08:20:44.049464 medkit_lib-0.9.1/medkit/core/text/entity_norm_attribute.py
--rw-r--r--   0        0        0     6827 2023-08-07 11:59:02.944405 medkit_lib-0.9.1/medkit/core/text/operation.py
--rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/core/text/span.py
--rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/core/text/span_utils.py
--rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/core/text/utils.py
--rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/core/utils.py
--rw-r--r--   0        0        0      628 2023-08-07 09:06:28.578043 medkit_lib-0.9.1/medkit/io/__init__.py
--rw-r--r--   0        0        0    16195 2023-09-11 09:09:50.669223 medkit_lib-0.9.1/medkit/io/_brat_utils.py
--rw-r--r--   0        0        0     1657 2023-08-07 09:06:28.578043 medkit_lib-0.9.1/medkit/io/_common.py
--rw-r--r--   0        0        0    20230 2023-09-11 09:09:50.677223 medkit_lib-0.9.1/medkit/io/brat.py
--rw-r--r--   0        0        0    24335 2023-08-07 15:23:23.968742 medkit_lib-0.9.1/medkit/io/doccano.py
--rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/io/medkit_json/__init__.py
--rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/io/medkit_json/_common.py
--rw-r--r--   0        0        0     6402 2023-07-21 10:01:08.934587 medkit_lib-0.9.1/medkit/io/medkit_json/audio.py
--rw-r--r--   0        0        0     6440 2023-09-13 15:34:35.132968 medkit_lib-0.9.1/medkit/io/medkit_json/text.py
--rw-r--r--   0        0        0    12123 2023-06-27 14:10:01.377546 medkit_lib-0.9.1/medkit/io/rttm.py
--rw-r--r--   0        0        0     7750 2023-04-21 12:33:02.950744 medkit_lib-0.9.1/medkit/io/spacy.py
--rw-r--r--   0        0        0      165 2023-07-21 10:01:08.934587 medkit_lib-0.9.1/medkit/text/__init__.py
--rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/text/context/__init__.py
--rw-r--r--   0        0        0     9568 2023-07-21 10:01:08.934587 medkit_lib-0.9.1/medkit/text/context/family_detector.py
--rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.9.1/medkit/text/context/family_detector_default_rules.yml
--rw-r--r--   0        0        0    14492 2023-09-07 14:00:14.374840 medkit_lib-0.9.1/medkit/text/context/hypothesis_detector.py
--rw-r--r--   0        0        0      905 2023-09-07 14:00:14.374840 medkit_lib-0.9.1/medkit/text/context/hypothesis_detector_default_rules.yml
--rw-r--r--   0        0        0   307270 2023-09-07 14:00:14.374840 medkit_lib-0.9.1/medkit/text/context/hypothesis_detector_default_verbs.yml
--rw-r--r--   0        0        0     9097 2023-07-21 10:01:08.934587 medkit_lib-0.9.1/medkit/text/context/negation_detector.py
--rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.9.1/medkit/text/context/negation_detector_default_rules.yml
--rw-r--r--   0        0        0      304 2023-05-23 14:37:42.934717 medkit_lib-0.9.1/medkit/text/metrics/__init__.py
--rw-r--r--   0        0        0     9422 2023-05-23 14:37:42.934717 medkit_lib-0.9.1/medkit/text/metrics/ner.py
--rw-r--r--   0        0        0     1584 2023-07-21 12:04:08.608377 medkit_lib-0.9.1/medkit/text/ner/__init__.py
--rw-r--r--   0        0        0    22325 2023-09-19 09:41:49.174486 medkit_lib-0.9.1/medkit/text/ner/_base_simstring_matcher.py
--rw-r--r--   0        0        0     3795 2023-04-21 08:20:44.049464 medkit_lib-0.9.1/medkit/text/ner/adicap_norm_attribute.py
--rw-r--r--   0        0        0    11470 2023-04-21 08:20:44.049464 medkit_lib-0.9.1/medkit/text/ner/date_attribute.py
--rw-r--r--   0        0        0     5527 2023-04-20 16:18:05.219523 medkit_lib-0.9.1/medkit/text/ner/duckling_matcher.py
--rw-r--r--   0        0        0     4639 2023-07-21 10:01:08.934587 medkit_lib-0.9.1/medkit/text/ner/edsnlp_date_matcher.py
--rw-r--r--   0        0        0     6534 2023-04-21 12:33:02.950744 medkit_lib-0.9.1/medkit/text/ner/hf_entity_matcher.py
--rw-r--r--   0        0        0     8255 2023-08-07 09:06:28.578043 medkit_lib-0.9.1/medkit/text/ner/hf_entity_matcher_trainable.py
--rw-r--r--   0        0        0     7082 2023-05-23 14:37:42.934717 medkit_lib-0.9.1/medkit/text/ner/hf_tokenization_utils.py
--rw-r--r--   0        0        0     5993 2023-05-23 16:01:44.808582 medkit_lib-0.9.1/medkit/text/ner/iamsystem_matcher.py
--rw-r--r--   0        0        0    11902 2023-07-21 12:04:08.608377 medkit_lib-0.9.1/medkit/text/ner/quick_umls_matcher.py
--rw-r--r--   0        0        0    13295 2023-09-19 09:41:49.174486 medkit_lib-0.9.1/medkit/text/ner/regexp_matcher.py
--rw-r--r--   0        0        0    22529 2023-09-19 09:41:49.174486 medkit_lib-0.9.1/medkit/text/ner/regexp_matcher_default_rules.yml
--rw-r--r--   0        0        0     8125 2023-09-19 09:41:49.174486 medkit_lib-0.9.1/medkit/text/ner/simstring_matcher.py
--rw-r--r--   0        0        0     5154 2023-04-21 08:20:44.049464 medkit_lib-0.9.1/medkit/text/ner/tnm_attribute.py
--rw-r--r--   0        0        0    17837 2023-09-11 14:42:57.175151 medkit_lib-0.9.1/medkit/text/ner/umls_coder_normalizer.py
--rw-r--r--   0        0        0    13293 2023-09-19 09:41:49.178486 medkit_lib-0.9.1/medkit/text/ner/umls_matcher.py
--rw-r--r--   0        0        0     2791 2023-04-21 08:20:44.049464 medkit_lib-0.9.1/medkit/text/ner/umls_norm_attribute.py
--rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.9.1/medkit/text/ner/umls_semgroups_v04.txt
--rw-r--r--   0        0        0     9107 2023-07-21 12:04:08.608377 medkit_lib-0.9.1/medkit/text/ner/umls_utils.py
--rw-r--r--   0        0        0      268 2023-08-07 09:06:28.578043 medkit_lib-0.9.1/medkit/text/postprocessing/__init__.py
--rw-r--r--   0        0        0     1742 2023-05-30 15:09:33.847172 medkit_lib-0.9.1/medkit/text/postprocessing/alignment_utils.py
--rw-r--r--   0        0        0     2212 2023-05-30 15:09:33.847172 medkit_lib-0.9.1/medkit/text/postprocessing/attribute_duplicator.py
--rw-r--r--   0        0        0     1500 2023-08-07 09:06:28.582043 medkit_lib-0.9.1/medkit/text/postprocessing/overlapping.py
--rw-r--r--   0        0        0      614 2023-09-07 14:00:14.374840 medkit_lib-0.9.1/medkit/text/preprocessing/__init__.py
--rw-r--r--   0        0        0     3074 2023-06-19 15:44:01.764862 medkit_lib-0.9.1/medkit/text/preprocessing/char_replacer.py
--rw-r--r--   0        0        0     2378 2023-09-07 14:00:14.374840 medkit_lib-0.9.1/medkit/text/preprocessing/char_rules.py
--rw-r--r--   0        0        0    13694 2023-09-18 18:48:20.595419 medkit_lib-0.9.1/medkit/text/preprocessing/duplicate_finder.py
--rw-r--r--   0        0        0     5083 2023-09-14 14:22:43.151824 medkit_lib-0.9.1/medkit/text/preprocessing/eds_cleaner.py
--rw-r--r--   0        0        0     3193 2023-09-07 14:00:14.378841 medkit_lib-0.9.1/medkit/text/preprocessing/regexp_replacer.py
--rw-r--r--   0        0        0      202 2023-04-04 06:31:49.492373 medkit_lib-0.9.1/medkit/text/relations/__init__.py
--rw-r--r--   0        0        0     9562 2023-09-14 14:22:43.151824 medkit_lib-0.9.1/medkit/text/relations/syntactic_relation_extractor.py
--rw-r--r--   0        0        0      475 2023-05-05 09:23:06.369871 medkit_lib-0.9.1/medkit/text/segmentation/__init__.py
--rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.9.1/medkit/text/segmentation/default_section_definition.yml
--rw-r--r--   0        0        0      762 2023-09-21 15:21:47.199672 medkit_lib-0.9.1/medkit/text/segmentation/default_syntagma_definition.yml
--rw-r--r--   0        0        0     4345 2023-09-21 15:47:13.425496 medkit_lib-0.9.1/medkit/text/segmentation/rush_sentence_tokenizer.py
--rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.9.1/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
--rw-r--r--   0        0        0     9439 2023-09-14 14:22:43.151824 medkit_lib-0.9.1/medkit/text/segmentation/section_tokenizer.py
--rw-r--r--   0        0        0     5338 2023-09-21 15:47:13.425496 medkit_lib-0.9.1/medkit/text/segmentation/sentence_tokenizer.py
--rw-r--r--   0        0        0     6691 2023-09-21 15:47:13.425496 medkit_lib-0.9.1/medkit/text/segmentation/syntagma_tokenizer.py
--rw-r--r--   0        0        0     1821 2023-09-11 09:09:50.681223 medkit_lib-0.9.1/medkit/text/segmentation/tokenizer_utils.py
--rw-r--r--   0        0        0      669 2023-04-21 12:33:02.950744 medkit_lib-0.9.1/medkit/text/spacy/__init__.py
--rw-r--r--   0        0        0     4203 2023-03-23 15:19:08.274090 medkit_lib-0.9.1/medkit/text/spacy/displacy_utils.py
--rw-r--r--   0        0        0     5765 2023-04-21 08:20:44.049464 medkit_lib-0.9.1/medkit/text/spacy/doc_pipeline.py
--rw-r--r--   0        0        0    15636 2023-04-21 08:20:44.049464 medkit_lib-0.9.1/medkit/text/spacy/edsnlp.py
--rw-r--r--   0        0        0     5136 2023-04-21 08:20:44.049464 medkit_lib-0.9.1/medkit/text/spacy/pipeline.py
--rw-r--r--   0        0        0    17779 2023-08-07 09:06:28.582043 medkit_lib-0.9.1/medkit/text/spacy/spacy_utils.py
--rw-r--r--   0        0        0      180 2023-04-04 06:31:49.500373 medkit_lib-0.9.1/medkit/text/translation/__init__.py
--rw-r--r--   0        0        0    15174 2023-09-14 14:22:43.155824 medkit_lib-0.9.1/medkit/text/translation/hf_translator.py
--rw-r--r--   0        0        0       23 2023-08-07 09:04:26.059126 medkit_lib-0.9.1/medkit/text/utils/__init__.py
--rw-r--r--   0        0        0     1424 2023-07-21 10:01:08.938588 medkit_lib-0.9.1/medkit/text/utils/decoding.py
--rw-r--r--   0        0        0      232 2023-08-11 08:43:48.061208 medkit_lib-0.9.1/medkit/tools/__init__.py
--rw-r--r--   0        0        0     5450 2023-07-21 10:01:08.938588 medkit_lib-0.9.1/medkit/tools/_save_prov_to_dot.py
--rw-r--r--   0        0        0    10381 2023-08-17 12:56:09.524805 medkit_lib-0.9.1/medkit/tools/e3c_corpus.py
--rw-r--r--   0        0        0     1198 2023-04-21 12:33:02.950744 medkit_lib-0.9.1/medkit/tools/hf_utils.py
--rw-r--r--   0        0        0     3602 2023-07-21 10:01:08.938588 medkit_lib-0.9.1/medkit/tools/mtsamples.py
--rw-r--r--   0        0        0      765 2023-04-21 12:33:02.950744 medkit_lib-0.9.1/medkit/training/__init__.py
--rw-r--r--   0        0        0     3845 2023-09-13 15:22:38.304743 medkit_lib-0.9.1/medkit/training/callbacks.py
--rw-r--r--   0        0        0     1987 2023-07-27 10:50:06.359861 medkit_lib-0.9.1/medkit/training/trainable_component.py
--rw-r--r--   0        0        0    11816 2023-09-13 15:22:38.304743 medkit_lib-0.9.1/medkit/training/trainer.py
--rw-r--r--   0        0        0     1844 2023-09-13 15:22:38.304743 medkit_lib-0.9.1/medkit/training/trainer_config.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.9.1/medkit/training/utils.py
--rw-r--r--   0        0        0     5119 2023-09-25 09:38:17.334296 medkit_lib-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5508 1970-01-01 00:00:00.000000 medkit_lib-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1282 2023-09-12 12:18:25.713016 medkit_lib-0.9.2/README.md
+-rw-r--r--   0        0        0      173 2023-04-04 06:31:49.436370 medkit_lib-0.9.2/medkit/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.9.2/medkit/audio/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-04 06:31:49.436370 medkit_lib-0.9.2/medkit/audio/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.9.2/medkit/audio/preprocessing/downmixer.py
+-rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.9.2/medkit/audio/preprocessing/power_normalizer.py
+-rw-r--r--   0        0        0     2482 2023-04-21 12:33:02.946744 medkit_lib-0.9.2/medkit/audio/preprocessing/resampler.py
+-rw-r--r--   0        0        0      250 2023-04-04 06:31:49.440370 medkit_lib-0.9.2/medkit/audio/segmentation/__init__.py
+-rw-r--r--   0        0        0     6574 2023-09-25 09:03:10.286242 medkit_lib-0.9.2/medkit/audio/segmentation/pa_speaker_detector.py
+-rw-r--r--   0        0        0     7416 2023-04-21 12:33:02.946744 medkit_lib-0.9.2/medkit/audio/segmentation/webrtc_voice_detector.py
+-rw-r--r--   0        0        0      554 2023-06-27 14:10:01.377546 medkit_lib-0.9.2/medkit/audio/transcription/__init__.py
+-rw-r--r--   0        0        0     7168 2023-06-27 14:10:01.377546 medkit_lib-0.9.2/medkit/audio/transcription/doc_transcriber.py
+-rw-r--r--   0        0        0     3821 2023-06-27 14:10:01.377546 medkit_lib-0.9.2/medkit/audio/transcription/hf_transcriber_function.py
+-rw-r--r--   0        0        0     4562 2023-06-27 14:10:01.377546 medkit_lib-0.9.2/medkit/audio/transcription/sb_transcriber_function.py
+-rw-r--r--   0        0        0     4776 2023-06-27 14:10:01.377546 medkit_lib-0.9.2/medkit/audio/transcription/transcribed_document.py
+-rw-r--r--   0        0        0     1549 2023-08-07 09:06:28.578043 medkit_lib-0.9.2/medkit/core/__init__.py
+-rw-r--r--   0        0        0     7827 2023-04-20 16:18:05.215523 medkit_lib-0.9.2/medkit/core/_prov_graph.py
+-rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/annotation.py
+-rw-r--r--   0        0        0     4665 2023-03-28 15:25:00.537196 medkit_lib-0.9.2/medkit/core/annotation_container.py
+-rw-r--r--   0        0        0     2969 2023-04-21 08:20:44.049464 medkit_lib-0.9.2/medkit/core/attribute.py
+-rw-r--r--   0        0        0     3052 2023-03-28 15:25:00.537196 medkit_lib-0.9.2/medkit/core/attribute_container.py
+-rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/audio/__init__.py
+-rw-r--r--   0        0        0     3712 2023-07-21 10:01:08.934587 medkit_lib-0.9.2/medkit/core/audio/annotation.py
+-rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/audio/annotation_container.py
+-rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/audio/audio_buffer.py
+-rw-r--r--   0        0        0     3835 2023-08-07 09:06:28.578043 medkit_lib-0.9.2/medkit/core/audio/document.py
+-rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/audio/operation.py
+-rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/audio/span.py
+-rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/collection.py
+-rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/conversion.py
+-rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/data_item.py
+-rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/dict_conv.py
+-rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/doc_pipeline.py
+-rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/document.py
+-rw-r--r--   0        0        0      597 2023-08-07 09:06:28.578043 medkit_lib-0.9.2/medkit/core/id.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/operation.py
+-rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/operation_desc.py
+-rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/pipeline.py
+-rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/prov_store.py
+-rw-r--r--   0        0        0    11205 2023-07-21 10:01:08.934587 medkit_lib-0.9.2/medkit/core/prov_tracer.py
+-rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.9.2/medkit/core/store.py
+-rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/core/text/__init__.py
+-rw-r--r--   0        0        0     8728 2023-04-04 06:31:49.484372 medkit_lib-0.9.2/medkit/core/text/annotation.py
+-rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/core/text/annotation_container.py
+-rw-r--r--   0        0        0     4694 2023-08-07 09:06:28.578043 medkit_lib-0.9.2/medkit/core/text/document.py
+-rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/core/text/entity_attribute_container.py
+-rw-r--r--   0        0        0     3244 2023-04-21 08:20:44.049464 medkit_lib-0.9.2/medkit/core/text/entity_norm_attribute.py
+-rw-r--r--   0        0        0     6827 2023-08-07 11:59:02.944405 medkit_lib-0.9.2/medkit/core/text/operation.py
+-rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/core/text/span.py
+-rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/core/text/span_utils.py
+-rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/core/text/utils.py
+-rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/core/utils.py
+-rw-r--r--   0        0        0      628 2023-08-07 09:06:28.578043 medkit_lib-0.9.2/medkit/io/__init__.py
+-rw-r--r--   0        0        0    16195 2023-09-11 09:09:50.669223 medkit_lib-0.9.2/medkit/io/_brat_utils.py
+-rw-r--r--   0        0        0     1657 2023-08-07 09:06:28.578043 medkit_lib-0.9.2/medkit/io/_common.py
+-rw-r--r--   0        0        0    20230 2023-09-11 09:09:50.677223 medkit_lib-0.9.2/medkit/io/brat.py
+-rw-r--r--   0        0        0    24335 2023-08-07 15:23:23.968742 medkit_lib-0.9.2/medkit/io/doccano.py
+-rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/io/medkit_json/__init__.py
+-rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/io/medkit_json/_common.py
+-rw-r--r--   0        0        0     6402 2023-07-21 10:01:08.934587 medkit_lib-0.9.2/medkit/io/medkit_json/audio.py
+-rw-r--r--   0        0        0     6440 2023-09-13 15:34:35.132968 medkit_lib-0.9.2/medkit/io/medkit_json/text.py
+-rw-r--r--   0        0        0    12123 2023-06-27 14:10:01.377546 medkit_lib-0.9.2/medkit/io/rttm.py
+-rw-r--r--   0        0        0     7750 2023-04-21 12:33:02.950744 medkit_lib-0.9.2/medkit/io/spacy.py
+-rw-r--r--   0        0        0      165 2023-07-21 10:01:08.934587 medkit_lib-0.9.2/medkit/text/__init__.py
+-rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/text/context/__init__.py
+-rw-r--r--   0        0        0     9568 2023-07-21 10:01:08.934587 medkit_lib-0.9.2/medkit/text/context/family_detector.py
+-rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.9.2/medkit/text/context/family_detector_default_rules.yml
+-rw-r--r--   0        0        0    14492 2023-09-07 14:00:14.374840 medkit_lib-0.9.2/medkit/text/context/hypothesis_detector.py
+-rw-r--r--   0        0        0      905 2023-09-07 14:00:14.374840 medkit_lib-0.9.2/medkit/text/context/hypothesis_detector_default_rules.yml
+-rw-r--r--   0        0        0   307270 2023-09-07 14:00:14.374840 medkit_lib-0.9.2/medkit/text/context/hypothesis_detector_default_verbs.yml
+-rw-r--r--   0        0        0     9097 2023-07-21 10:01:08.934587 medkit_lib-0.9.2/medkit/text/context/negation_detector.py
+-rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.9.2/medkit/text/context/negation_detector_default_rules.yml
+-rw-r--r--   0        0        0      304 2023-05-23 14:37:42.934717 medkit_lib-0.9.2/medkit/text/metrics/__init__.py
+-rw-r--r--   0        0        0     9422 2023-05-23 14:37:42.934717 medkit_lib-0.9.2/medkit/text/metrics/ner.py
+-rw-r--r--   0        0        0     1584 2023-07-21 12:04:08.608377 medkit_lib-0.9.2/medkit/text/ner/__init__.py
+-rw-r--r--   0        0        0    22325 2023-09-19 09:41:49.174486 medkit_lib-0.9.2/medkit/text/ner/_base_simstring_matcher.py
+-rw-r--r--   0        0        0     3795 2023-04-21 08:20:44.049464 medkit_lib-0.9.2/medkit/text/ner/adicap_norm_attribute.py
+-rw-r--r--   0        0        0    11470 2023-04-21 08:20:44.049464 medkit_lib-0.9.2/medkit/text/ner/date_attribute.py
+-rw-r--r--   0        0        0     5527 2023-04-20 16:18:05.219523 medkit_lib-0.9.2/medkit/text/ner/duckling_matcher.py
+-rw-r--r--   0        0        0     4639 2023-07-21 10:01:08.934587 medkit_lib-0.9.2/medkit/text/ner/edsnlp_date_matcher.py
+-rw-r--r--   0        0        0     6534 2023-04-21 12:33:02.950744 medkit_lib-0.9.2/medkit/text/ner/hf_entity_matcher.py
+-rw-r--r--   0        0        0     8255 2023-08-07 09:06:28.578043 medkit_lib-0.9.2/medkit/text/ner/hf_entity_matcher_trainable.py
+-rw-r--r--   0        0        0     7082 2023-05-23 14:37:42.934717 medkit_lib-0.9.2/medkit/text/ner/hf_tokenization_utils.py
+-rw-r--r--   0        0        0     5993 2023-05-23 16:01:44.808582 medkit_lib-0.9.2/medkit/text/ner/iamsystem_matcher.py
+-rw-r--r--   0        0        0    11902 2023-07-21 12:04:08.608377 medkit_lib-0.9.2/medkit/text/ner/quick_umls_matcher.py
+-rw-r--r--   0        0        0    13295 2023-09-19 09:41:49.174486 medkit_lib-0.9.2/medkit/text/ner/regexp_matcher.py
+-rw-r--r--   0        0        0    22529 2023-09-19 09:41:49.174486 medkit_lib-0.9.2/medkit/text/ner/regexp_matcher_default_rules.yml
+-rw-r--r--   0        0        0     8125 2023-09-19 09:41:49.174486 medkit_lib-0.9.2/medkit/text/ner/simstring_matcher.py
+-rw-r--r--   0        0        0     5154 2023-04-21 08:20:44.049464 medkit_lib-0.9.2/medkit/text/ner/tnm_attribute.py
+-rw-r--r--   0        0        0    17837 2023-09-11 14:42:57.175151 medkit_lib-0.9.2/medkit/text/ner/umls_coder_normalizer.py
+-rw-r--r--   0        0        0    13293 2023-09-19 09:41:49.178486 medkit_lib-0.9.2/medkit/text/ner/umls_matcher.py
+-rw-r--r--   0        0        0     2791 2023-04-21 08:20:44.049464 medkit_lib-0.9.2/medkit/text/ner/umls_norm_attribute.py
+-rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.9.2/medkit/text/ner/umls_semgroups_v04.txt
+-rw-r--r--   0        0        0     9107 2023-07-21 12:04:08.608377 medkit_lib-0.9.2/medkit/text/ner/umls_utils.py
+-rw-r--r--   0        0        0      268 2023-08-07 09:06:28.578043 medkit_lib-0.9.2/medkit/text/postprocessing/__init__.py
+-rw-r--r--   0        0        0     1742 2023-05-30 15:09:33.847172 medkit_lib-0.9.2/medkit/text/postprocessing/alignment_utils.py
+-rw-r--r--   0        0        0     2212 2023-05-30 15:09:33.847172 medkit_lib-0.9.2/medkit/text/postprocessing/attribute_duplicator.py
+-rw-r--r--   0        0        0     1500 2023-08-07 09:06:28.582043 medkit_lib-0.9.2/medkit/text/postprocessing/overlapping.py
+-rw-r--r--   0        0        0      614 2023-09-07 14:00:14.374840 medkit_lib-0.9.2/medkit/text/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3074 2023-06-19 15:44:01.764862 medkit_lib-0.9.2/medkit/text/preprocessing/char_replacer.py
+-rw-r--r--   0        0        0     2378 2023-09-07 14:00:14.374840 medkit_lib-0.9.2/medkit/text/preprocessing/char_rules.py
+-rw-r--r--   0        0        0    13694 2023-09-18 18:48:20.595419 medkit_lib-0.9.2/medkit/text/preprocessing/duplicate_finder.py
+-rw-r--r--   0        0        0     5083 2023-09-14 14:22:43.151824 medkit_lib-0.9.2/medkit/text/preprocessing/eds_cleaner.py
+-rw-r--r--   0        0        0     3193 2023-09-07 14:00:14.378841 medkit_lib-0.9.2/medkit/text/preprocessing/regexp_replacer.py
+-rw-r--r--   0        0        0      202 2023-04-04 06:31:49.492373 medkit_lib-0.9.2/medkit/text/relations/__init__.py
+-rw-r--r--   0        0        0     9562 2023-09-14 14:22:43.151824 medkit_lib-0.9.2/medkit/text/relations/syntactic_relation_extractor.py
+-rw-r--r--   0        0        0      475 2023-05-05 09:23:06.369871 medkit_lib-0.9.2/medkit/text/segmentation/__init__.py
+-rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.9.2/medkit/text/segmentation/default_section_definition.yml
+-rw-r--r--   0        0        0      762 2023-09-21 15:21:47.199672 medkit_lib-0.9.2/medkit/text/segmentation/default_syntagma_definition.yml
+-rw-r--r--   0        0        0     4345 2023-09-21 15:47:13.425496 medkit_lib-0.9.2/medkit/text/segmentation/rush_sentence_tokenizer.py
+-rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.9.2/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
+-rw-r--r--   0        0        0     9439 2023-09-14 14:22:43.151824 medkit_lib-0.9.2/medkit/text/segmentation/section_tokenizer.py
+-rw-r--r--   0        0        0     5338 2023-09-21 15:47:13.425496 medkit_lib-0.9.2/medkit/text/segmentation/sentence_tokenizer.py
+-rw-r--r--   0        0        0     6691 2023-09-21 15:47:13.425496 medkit_lib-0.9.2/medkit/text/segmentation/syntagma_tokenizer.py
+-rw-r--r--   0        0        0     1821 2023-09-11 09:09:50.681223 medkit_lib-0.9.2/medkit/text/segmentation/tokenizer_utils.py
+-rw-r--r--   0        0        0      669 2023-04-21 12:33:02.950744 medkit_lib-0.9.2/medkit/text/spacy/__init__.py
+-rw-r--r--   0        0        0     4203 2023-09-25 10:01:12.536215 medkit_lib-0.9.2/medkit/text/spacy/displacy_utils.py
+-rw-r--r--   0        0        0     5765 2023-04-21 08:20:44.049464 medkit_lib-0.9.2/medkit/text/spacy/doc_pipeline.py
+-rw-r--r--   0        0        0    15636 2023-04-21 08:20:44.049464 medkit_lib-0.9.2/medkit/text/spacy/edsnlp.py
+-rw-r--r--   0        0        0     5136 2023-04-21 08:20:44.049464 medkit_lib-0.9.2/medkit/text/spacy/pipeline.py
+-rw-r--r--   0        0        0    17779 2023-08-07 09:06:28.582043 medkit_lib-0.9.2/medkit/text/spacy/spacy_utils.py
+-rw-r--r--   0        0        0      180 2023-04-04 06:31:49.500373 medkit_lib-0.9.2/medkit/text/translation/__init__.py
+-rw-r--r--   0        0        0    15174 2023-09-14 14:22:43.155824 medkit_lib-0.9.2/medkit/text/translation/hf_translator.py
+-rw-r--r--   0        0        0       23 2023-08-07 09:04:26.059126 medkit_lib-0.9.2/medkit/text/utils/__init__.py
+-rw-r--r--   0        0        0     1424 2023-07-21 10:01:08.938588 medkit_lib-0.9.2/medkit/text/utils/decoding.py
+-rw-r--r--   0        0        0      232 2023-08-11 08:43:48.061208 medkit_lib-0.9.2/medkit/tools/__init__.py
+-rw-r--r--   0        0        0     5450 2023-07-21 10:01:08.938588 medkit_lib-0.9.2/medkit/tools/_save_prov_to_dot.py
+-rw-r--r--   0        0        0    10381 2023-08-17 12:56:09.524805 medkit_lib-0.9.2/medkit/tools/e3c_corpus.py
+-rw-r--r--   0        0        0     1198 2023-04-21 12:33:02.950744 medkit_lib-0.9.2/medkit/tools/hf_utils.py
+-rw-r--r--   0        0        0     3602 2023-07-21 10:01:08.938588 medkit_lib-0.9.2/medkit/tools/mtsamples.py
+-rw-r--r--   0        0        0      765 2023-04-21 12:33:02.950744 medkit_lib-0.9.2/medkit/training/__init__.py
+-rw-r--r--   0        0        0     3845 2023-09-13 15:22:38.304743 medkit_lib-0.9.2/medkit/training/callbacks.py
+-rw-r--r--   0        0        0     1987 2023-07-27 10:50:06.359861 medkit_lib-0.9.2/medkit/training/trainable_component.py
+-rw-r--r--   0        0        0    11816 2023-09-13 15:22:38.304743 medkit_lib-0.9.2/medkit/training/trainer.py
+-rw-r--r--   0        0        0     1844 2023-09-13 15:22:38.304743 medkit_lib-0.9.2/medkit/training/trainer_config.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.9.2/medkit/training/utils.py
+-rw-r--r--   0        0        0     5119 2023-09-25 10:17:06.581869 medkit_lib-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5508 1970-01-01 00:00:00.000000 medkit_lib-0.9.2/PKG-INFO
```

### Comparing `medkit_lib-0.9.1/LICENSE` & `medkit_lib-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/README.md` & `medkit_lib-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/preprocessing/downmixer.py` & `medkit_lib-0.9.2/medkit/audio/preprocessing/downmixer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/preprocessing/power_normalizer.py` & `medkit_lib-0.9.2/medkit/audio/preprocessing/power_normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/preprocessing/resampler.py` & `medkit_lib-0.9.2/medkit/audio/preprocessing/resampler.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/segmentation/pa_speaker_detector.py` & `medkit_lib-0.9.2/medkit/audio/segmentation/pa_speaker_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/segmentation/webrtc_voice_detector.py` & `medkit_lib-0.9.2/medkit/audio/segmentation/webrtc_voice_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/transcription/__init__.py` & `medkit_lib-0.9.2/medkit/audio/transcription/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/transcription/doc_transcriber.py` & `medkit_lib-0.9.2/medkit/audio/transcription/doc_transcriber.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/transcription/hf_transcriber_function.py` & `medkit_lib-0.9.2/medkit/audio/transcription/hf_transcriber_function.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/transcription/sb_transcriber_function.py` & `medkit_lib-0.9.2/medkit/audio/transcription/sb_transcriber_function.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/audio/transcription/transcribed_document.py` & `medkit_lib-0.9.2/medkit/audio/transcription/transcribed_document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/__init__.py` & `medkit_lib-0.9.2/medkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/_prov_graph.py` & `medkit_lib-0.9.2/medkit/core/_prov_graph.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/annotation.py` & `medkit_lib-0.9.2/medkit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/annotation_container.py` & `medkit_lib-0.9.2/medkit/core/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/attribute.py` & `medkit_lib-0.9.2/medkit/core/attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/attribute_container.py` & `medkit_lib-0.9.2/medkit/core/attribute_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/audio/__init__.py` & `medkit_lib-0.9.2/medkit/core/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/audio/annotation.py` & `medkit_lib-0.9.2/medkit/core/audio/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/audio/annotation_container.py` & `medkit_lib-0.9.2/medkit/core/audio/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/audio/audio_buffer.py` & `medkit_lib-0.9.2/medkit/core/audio/audio_buffer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/audio/document.py` & `medkit_lib-0.9.2/medkit/core/audio/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/audio/operation.py` & `medkit_lib-0.9.2/medkit/core/audio/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/audio/span.py` & `medkit_lib-0.9.2/medkit/core/audio/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/collection.py` & `medkit_lib-0.9.2/medkit/core/collection.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/conversion.py` & `medkit_lib-0.9.2/medkit/core/conversion.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/dict_conv.py` & `medkit_lib-0.9.2/medkit/core/dict_conv.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/doc_pipeline.py` & `medkit_lib-0.9.2/medkit/core/doc_pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/document.py` & `medkit_lib-0.9.2/medkit/core/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/id.py` & `medkit_lib-0.9.2/medkit/core/id.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/operation.py` & `medkit_lib-0.9.2/medkit/core/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/operation_desc.py` & `medkit_lib-0.9.2/medkit/core/operation_desc.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/pipeline.py` & `medkit_lib-0.9.2/medkit/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/prov_store.py` & `medkit_lib-0.9.2/medkit/core/prov_store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/prov_tracer.py` & `medkit_lib-0.9.2/medkit/core/prov_tracer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/store.py` & `medkit_lib-0.9.2/medkit/core/store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/__init__.py` & `medkit_lib-0.9.2/medkit/core/text/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/annotation.py` & `medkit_lib-0.9.2/medkit/core/text/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/annotation_container.py` & `medkit_lib-0.9.2/medkit/core/text/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/document.py` & `medkit_lib-0.9.2/medkit/core/text/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/entity_attribute_container.py` & `medkit_lib-0.9.2/medkit/core/text/entity_attribute_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/entity_norm_attribute.py` & `medkit_lib-0.9.2/medkit/core/text/entity_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/operation.py` & `medkit_lib-0.9.2/medkit/core/text/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/span.py` & `medkit_lib-0.9.2/medkit/core/text/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/span_utils.py` & `medkit_lib-0.9.2/medkit/core/text/span_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/text/utils.py` & `medkit_lib-0.9.2/medkit/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/core/utils.py` & `medkit_lib-0.9.2/medkit/core/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/__init__.py` & `medkit_lib-0.9.2/medkit/io/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/_brat_utils.py` & `medkit_lib-0.9.2/medkit/io/_brat_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/_common.py` & `medkit_lib-0.9.2/medkit/io/_common.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/brat.py` & `medkit_lib-0.9.2/medkit/io/brat.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/doccano.py` & `medkit_lib-0.9.2/medkit/io/doccano.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/medkit_json/__init__.py` & `medkit_lib-0.9.2/medkit/io/medkit_json/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/medkit_json/_common.py` & `medkit_lib-0.9.2/medkit/io/medkit_json/_common.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/medkit_json/audio.py` & `medkit_lib-0.9.2/medkit/io/medkit_json/audio.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/medkit_json/text.py` & `medkit_lib-0.9.2/medkit/io/medkit_json/text.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/rttm.py` & `medkit_lib-0.9.2/medkit/io/rttm.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/io/spacy.py` & `medkit_lib-0.9.2/medkit/io/spacy.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/context/__init__.py` & `medkit_lib-0.9.2/medkit/text/context/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/context/family_detector.py` & `medkit_lib-0.9.2/medkit/text/context/family_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/context/family_detector_default_rules.yml` & `medkit_lib-0.9.2/medkit/text/context/family_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/context/hypothesis_detector.py` & `medkit_lib-0.9.2/medkit/text/context/hypothesis_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/context/hypothesis_detector_default_rules.yml` & `medkit_lib-0.9.2/medkit/text/context/hypothesis_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/context/hypothesis_detector_default_verbs.yml` & `medkit_lib-0.9.2/medkit/text/context/hypothesis_detector_default_verbs.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/context/negation_detector.py` & `medkit_lib-0.9.2/medkit/text/context/negation_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/context/negation_detector_default_rules.yml` & `medkit_lib-0.9.2/medkit/text/context/negation_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/metrics/ner.py` & `medkit_lib-0.9.2/medkit/text/metrics/ner.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/__init__.py` & `medkit_lib-0.9.2/medkit/text/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/_base_simstring_matcher.py` & `medkit_lib-0.9.2/medkit/text/ner/_base_simstring_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/adicap_norm_attribute.py` & `medkit_lib-0.9.2/medkit/text/ner/adicap_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/date_attribute.py` & `medkit_lib-0.9.2/medkit/text/ner/date_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/duckling_matcher.py` & `medkit_lib-0.9.2/medkit/text/ner/duckling_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/edsnlp_date_matcher.py` & `medkit_lib-0.9.2/medkit/text/ner/edsnlp_date_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/hf_entity_matcher.py` & `medkit_lib-0.9.2/medkit/text/ner/hf_entity_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/hf_entity_matcher_trainable.py` & `medkit_lib-0.9.2/medkit/text/ner/hf_entity_matcher_trainable.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/hf_tokenization_utils.py` & `medkit_lib-0.9.2/medkit/text/ner/hf_tokenization_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/iamsystem_matcher.py` & `medkit_lib-0.9.2/medkit/text/ner/iamsystem_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/quick_umls_matcher.py` & `medkit_lib-0.9.2/medkit/text/ner/quick_umls_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/regexp_matcher.py` & `medkit_lib-0.9.2/medkit/text/ner/regexp_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/regexp_matcher_default_rules.yml` & `medkit_lib-0.9.2/medkit/text/ner/regexp_matcher_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/simstring_matcher.py` & `medkit_lib-0.9.2/medkit/text/ner/simstring_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/tnm_attribute.py` & `medkit_lib-0.9.2/medkit/text/ner/tnm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/umls_coder_normalizer.py` & `medkit_lib-0.9.2/medkit/text/ner/umls_coder_normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/umls_matcher.py` & `medkit_lib-0.9.2/medkit/text/ner/umls_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/umls_norm_attribute.py` & `medkit_lib-0.9.2/medkit/text/ner/umls_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/umls_semgroups_v04.txt` & `medkit_lib-0.9.2/medkit/text/ner/umls_semgroups_v04.txt`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/ner/umls_utils.py` & `medkit_lib-0.9.2/medkit/text/ner/umls_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/postprocessing/alignment_utils.py` & `medkit_lib-0.9.2/medkit/text/postprocessing/alignment_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/postprocessing/attribute_duplicator.py` & `medkit_lib-0.9.2/medkit/text/postprocessing/attribute_duplicator.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/postprocessing/overlapping.py` & `medkit_lib-0.9.2/medkit/text/postprocessing/overlapping.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/preprocessing/__init__.py` & `medkit_lib-0.9.2/medkit/text/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/preprocessing/char_replacer.py` & `medkit_lib-0.9.2/medkit/text/preprocessing/char_replacer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/preprocessing/char_rules.py` & `medkit_lib-0.9.2/medkit/text/preprocessing/char_rules.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/preprocessing/duplicate_finder.py` & `medkit_lib-0.9.2/medkit/text/preprocessing/duplicate_finder.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/preprocessing/eds_cleaner.py` & `medkit_lib-0.9.2/medkit/text/preprocessing/eds_cleaner.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/preprocessing/regexp_replacer.py` & `medkit_lib-0.9.2/medkit/text/preprocessing/regexp_replacer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/relations/syntactic_relation_extractor.py` & `medkit_lib-0.9.2/medkit/text/relations/syntactic_relation_extractor.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/segmentation/default_section_definition.yml` & `medkit_lib-0.9.2/medkit/text/segmentation/default_section_definition.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/segmentation/default_syntagma_definition.yml` & `medkit_lib-0.9.2/medkit/text/segmentation/default_syntagma_definition.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/segmentation/rush_sentence_tokenizer.py` & `medkit_lib-0.9.2/medkit/text/segmentation/rush_sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv` & `medkit_lib-0.9.2/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/segmentation/section_tokenizer.py` & `medkit_lib-0.9.2/medkit/text/segmentation/section_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/segmentation/sentence_tokenizer.py` & `medkit_lib-0.9.2/medkit/text/segmentation/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/segmentation/syntagma_tokenizer.py` & `medkit_lib-0.9.2/medkit/text/segmentation/syntagma_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/segmentation/tokenizer_utils.py` & `medkit_lib-0.9.2/medkit/text/segmentation/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/spacy/__init__.py` & `medkit_lib-0.9.2/medkit/text/spacy/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/spacy/displacy_utils.py` & `medkit_lib-0.9.2/medkit/text/spacy/displacy_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/spacy/doc_pipeline.py` & `medkit_lib-0.9.2/medkit/text/spacy/doc_pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/spacy/edsnlp.py` & `medkit_lib-0.9.2/medkit/text/spacy/edsnlp.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/spacy/pipeline.py` & `medkit_lib-0.9.2/medkit/text/spacy/pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/spacy/spacy_utils.py` & `medkit_lib-0.9.2/medkit/text/spacy/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/translation/hf_translator.py` & `medkit_lib-0.9.2/medkit/text/translation/hf_translator.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/text/utils/decoding.py` & `medkit_lib-0.9.2/medkit/text/utils/decoding.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/tools/_save_prov_to_dot.py` & `medkit_lib-0.9.2/medkit/tools/_save_prov_to_dot.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/tools/e3c_corpus.py` & `medkit_lib-0.9.2/medkit/tools/e3c_corpus.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/tools/hf_utils.py` & `medkit_lib-0.9.2/medkit/tools/hf_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/tools/mtsamples.py` & `medkit_lib-0.9.2/medkit/tools/mtsamples.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/training/__init__.py` & `medkit_lib-0.9.2/medkit/training/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/training/callbacks.py` & `medkit_lib-0.9.2/medkit/training/callbacks.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/training/trainable_component.py` & `medkit_lib-0.9.2/medkit/training/trainable_component.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/training/trainer.py` & `medkit_lib-0.9.2/medkit/training/trainer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/training/trainer_config.py` & `medkit_lib-0.9.2/medkit/training/trainer_config.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/medkit/training/utils.py` & `medkit_lib-0.9.2/medkit/training/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.9.1/pyproject.toml` & `medkit_lib-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medkit-lib"
-version = "0.9.1"
+version = "0.9.2"
 description = "A Python library for a learning health system"
 readme = "README.md"
 repository = "https://gitlab.inria.fr/heka/medkit/"
 documentation = "https://heka.gitlabpages.inria.fr/medkit/"
 authors = ["HeKA Research Team"]
 maintainers = [
     "medkit-maintainers <medkit-maintainers@inria.fr>"
```

### Comparing `medkit_lib-0.9.1/PKG-INFO` & `medkit_lib-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medkit-lib
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python library for a learning health system
 Home-page: https://gitlab.inria.fr/heka/medkit/
 License: MIT
 Author: HeKA Research Team
 Maintainer: medkit-maintainers
 Maintainer-email: medkit-maintainers@inria.fr
 Requires-Python: >=3.8,<4.0
```

