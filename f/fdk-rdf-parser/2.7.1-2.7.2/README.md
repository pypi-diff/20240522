# Comparing `tmp/fdk_rdf_parser-2.7.1.tar.gz` & `tmp/fdk_rdf_parser-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdk_rdf_parser-2.7.1.tar", max compression
+gzip compressed data, was "fdk_rdf_parser-2.7.2.tar", max compression
```

## Comparing `fdk_rdf_parser-2.7.1.tar` & `fdk_rdf_parser-2.7.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0    11357 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/LICENSE
--rw-r--r--   0        0        0     1248 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/pyproject.toml
--rw-r--r--   0        0        0      473 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/__init__.py
--rw-r--r--   0        0        0     1587 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/__init__.py
--rw-r--r--   0        0        0      270 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/address.py
--rw-r--r--   0        0        0      342 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/agent.py
--rw-r--r--   0        0        0      766 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/business_event.py
--rw-r--r--   0        0        0      336 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/catalog.py
--rw-r--r--   0        0        0      610 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/channel.py
--rw-r--r--   0        0        0     2885 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/concept.py
--rw-r--r--   0        0        0      189 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/conforms_to.py
--rw-r--r--   0        0        0      750 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/contactpoint.py
--rw-r--r--   0        0        0      436 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/cost.py
--rw-r--r--   0        0        0     2449 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/cpsvno_service.py
--rw-r--r--   0        0        0      356 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/data_distribution_service.py
--rw-r--r--   0        0        0     1668 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dataservice.py
--rw-r--r--   0        0        0     8657 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dataset.py
--rw-r--r--   0        0        0     1143 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dcat_resource.py
--rw-r--r--   0        0        0      274 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dct_standard.py
--rw-r--r--   0        0        0      924 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/distribution.py
--rw-r--r--   0        0        0      777 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/event.py
--rw-r--r--   0        0        0      758 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/evidence.py
--rw-r--r--   0        0        0      355 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/exceptions.py
--rw-r--r--   0        0        0      349 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/format.py
--rw-r--r--   0        0        0      174 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/harvest_meta_data.py
--rw-r--r--   0        0        0     3478 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/info_model.py
--rw-r--r--   0        0        0      331 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/legal_resource.py
--rw-r--r--   0        0        0      758 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/life_event.py
--rw-r--r--   0        0        0      402 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/media_type.py
--rw-r--r--   0        0        0     1910 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/model_element.py
--rw-r--r--   0        0        0     1147 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/model_property.py
--rw-r--r--   0        0        0      430 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/organization.py
--rw-r--r--   0        0        0      466 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/output.py
--rw-r--r--   0        0        0      376 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/participation.py
--rw-r--r--   0        0        0     1888 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/public_service.py
--rw-r--r--   0        0        0      326 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/publisher.py
--rw-r--r--   0        0        0      206 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/qualified_attribution.py
--rw-r--r--   0        0        0      202 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/quality_annotation.py
--rw-r--r--   0        0        0      227 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/reference_data_code.py
--rw-r--r--   0        0        0      277 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/references.py
--rw-r--r--   0        0        0      412 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/requirement.py
--rw-r--r--   0        0        0      424 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/rule.py
--rw-r--r--   0        0        0      317 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/skos_concept.py
--rw-r--r--   0        0        0      271 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/subject.py
--rw-r--r--   0        0        0      191 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/temporal.py
--rw-r--r--   0        0        0      610 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/theme.py
--rw-r--r--   0        0        0      506 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/types.py
--rw-r--r--   0        0        0     8796 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/fdk_rdf_parser.py
--rw-r--r--   0        0        0     1349 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/__init__.py
--rw-r--r--   0        0        0     1070 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/address.py
--rw-r--r--   0        0        0     2175 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/agent.py
--rw-r--r--   0        0        0     1153 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/catalog.py
--rw-r--r--   0        0        0     1739 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/channel.py
--rw-r--r--   0        0        0    15032 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/concept.py
--rw-r--r--   0        0        0      992 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/conforms_to.py
--rw-r--r--   0        0        0     3172 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/contactpoint.py
--rw-r--r--   0        0        0     1336 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/cost.py
--rw-r--r--   0        0        0     6030 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
--rw-r--r--   0        0        0     1555 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
--rw-r--r--   0        0        0     1671 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dataservice.py
--rw-r--r--   0        0        0     9262 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dataset.py
--rw-r--r--   0        0        0     2928 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dcat_resource.py
--rw-r--r--   0        0        0      979 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dct_standard.py
--rw-r--r--   0        0        0     2051 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/distribution.py
--rw-r--r--   0        0        0     3093 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/event.py
--rw-r--r--   0        0        0     2018 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/evidence.py
--rw-r--r--   0        0        0     1116 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/format.py
--rw-r--r--   0        0        0      422 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
--rw-r--r--   0        0        0     6492 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/info_model.py
--rw-r--r--   0        0        0     1047 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/legal_resource.py
--rw-r--r--   0        0        0     3338 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/media_type.py
--rw-r--r--   0        0        0     4432 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/model_element.py
--rw-r--r--   0        0        0     3439 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/model_property.py
--rw-r--r--   0        0        0     2623 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/organization.py
--rw-r--r--   0        0        0     1247 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/output.py
--rw-r--r--   0        0        0      816 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/participation.py
--rw-r--r--   0        0        0     2155 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/publisher.py
--rw-r--r--   0        0        0      911 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
--rw-r--r--   0        0        0     1451 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/quality_annotation.py
--rw-r--r--   0        0        0     5858 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/reference_data_code.py
--rw-r--r--   0        0        0     1610 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/references.py
--rw-r--r--   0        0        0     1170 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/requirement.py
--rw-r--r--   0        0        0     1251 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/rule.py
--rw-r--r--   0        0        0     1605 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/skos_concept.py
--rw-r--r--   0        0        0     1049 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/spatial.py
--rw-r--r--   0        0        0      965 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/subject.py
--rw-r--r--   0        0        0     2540 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/temporal.py
--rw-r--r--   0        0        0     2891 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/theme.py
--rw-r--r--   0        0        0      831 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/__init__.py
--rw-r--r--   0        0        0     3518 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/ns.py
--rw-r--r--   0        0        0     4675 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/utils.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/LICENSE
+-rw-r--r--   0        0        0     1248 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0      473 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/__init__.py
+-rw-r--r--   0        0        0     1587 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/address.py
+-rw-r--r--   0        0        0      342 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/agent.py
+-rw-r--r--   0        0        0      766 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/business_event.py
+-rw-r--r--   0        0        0      336 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/catalog.py
+-rw-r--r--   0        0        0      610 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/channel.py
+-rw-r--r--   0        0        0     2879 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/concept.py
+-rw-r--r--   0        0        0      189 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/conforms_to.py
+-rw-r--r--   0        0        0      750 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/contactpoint.py
+-rw-r--r--   0        0        0      436 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/cost.py
+-rw-r--r--   0        0        0     2449 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/cpsvno_service.py
+-rw-r--r--   0        0        0      356 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/data_distribution_service.py
+-rw-r--r--   0        0        0     1668 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dataservice.py
+-rw-r--r--   0        0        0     8657 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dataset.py
+-rw-r--r--   0        0        0     1143 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dcat_resource.py
+-rw-r--r--   0        0        0      274 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dct_standard.py
+-rw-r--r--   0        0        0      924 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/distribution.py
+-rw-r--r--   0        0        0      777 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/event.py
+-rw-r--r--   0        0        0      758 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/evidence.py
+-rw-r--r--   0        0        0      355 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/exceptions.py
+-rw-r--r--   0        0        0      349 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/format.py
+-rw-r--r--   0        0        0      174 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/harvest_meta_data.py
+-rw-r--r--   0        0        0     3478 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/info_model.py
+-rw-r--r--   0        0        0      331 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/legal_resource.py
+-rw-r--r--   0        0        0      758 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/life_event.py
+-rw-r--r--   0        0        0      402 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/media_type.py
+-rw-r--r--   0        0        0     1910 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/model_element.py
+-rw-r--r--   0        0        0     1147 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/model_property.py
+-rw-r--r--   0        0        0      430 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/organization.py
+-rw-r--r--   0        0        0      466 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/output.py
+-rw-r--r--   0        0        0      376 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/participation.py
+-rw-r--r--   0        0        0     1888 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/public_service.py
+-rw-r--r--   0        0        0      326 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/publisher.py
+-rw-r--r--   0        0        0      206 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/qualified_attribution.py
+-rw-r--r--   0        0        0      202 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/quality_annotation.py
+-rw-r--r--   0        0        0      227 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/reference_data_code.py
+-rw-r--r--   0        0        0      277 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/references.py
+-rw-r--r--   0        0        0      412 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/requirement.py
+-rw-r--r--   0        0        0      424 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/rule.py
+-rw-r--r--   0        0        0      317 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/skos_concept.py
+-rw-r--r--   0        0        0      271 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/subject.py
+-rw-r--r--   0        0        0      191 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/temporal.py
+-rw-r--r--   0        0        0      610 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/theme.py
+-rw-r--r--   0        0        0      506 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/types.py
+-rw-r--r--   0        0        0     8796 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/fdk_rdf_parser.py
+-rw-r--r--   0        0        0     1349 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/address.py
+-rw-r--r--   0        0        0     2175 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/agent.py
+-rw-r--r--   0        0        0     1153 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/catalog.py
+-rw-r--r--   0        0        0     1739 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/channel.py
+-rw-r--r--   0        0        0    15020 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/concept.py
+-rw-r--r--   0        0        0      992 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/conforms_to.py
+-rw-r--r--   0        0        0     3172 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/contactpoint.py
+-rw-r--r--   0        0        0     1336 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/cost.py
+-rw-r--r--   0        0        0     6030 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
+-rw-r--r--   0        0        0     1555 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
+-rw-r--r--   0        0        0     1671 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dataservice.py
+-rw-r--r--   0        0        0     9262 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dataset.py
+-rw-r--r--   0        0        0     2928 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dcat_resource.py
+-rw-r--r--   0        0        0      979 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dct_standard.py
+-rw-r--r--   0        0        0     2051 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/distribution.py
+-rw-r--r--   0        0        0     3093 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/event.py
+-rw-r--r--   0        0        0     2018 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/evidence.py
+-rw-r--r--   0        0        0     1116 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/format.py
+-rw-r--r--   0        0        0      422 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
+-rw-r--r--   0        0        0     6492 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/info_model.py
+-rw-r--r--   0        0        0     1047 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/legal_resource.py
+-rw-r--r--   0        0        0     3338 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/media_type.py
+-rw-r--r--   0        0        0     4432 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/model_element.py
+-rw-r--r--   0        0        0     3439 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/model_property.py
+-rw-r--r--   0        0        0     2623 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/organization.py
+-rw-r--r--   0        0        0     1247 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/output.py
+-rw-r--r--   0        0        0      816 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/participation.py
+-rw-r--r--   0        0        0     2155 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/publisher.py
+-rw-r--r--   0        0        0      911 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
+-rw-r--r--   0        0        0     1451 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/quality_annotation.py
+-rw-r--r--   0        0        0     5858 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/reference_data_code.py
+-rw-r--r--   0        0        0     1610 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/references.py
+-rw-r--r--   0        0        0     1170 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/requirement.py
+-rw-r--r--   0        0        0     1251 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/rule.py
+-rw-r--r--   0        0        0     1605 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/skos_concept.py
+-rw-r--r--   0        0        0     1049 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/spatial.py
+-rw-r--r--   0        0        0      965 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/subject.py
+-rw-r--r--   0        0        0     2540 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/temporal.py
+-rw-r--r--   0        0        0     2891 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/theme.py
+-rw-r--r--   0        0        0      831 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/__init__.py
+-rw-r--r--   0        0        0     3518 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/ns.py
+-rw-r--r--   0        0        0     4675 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/utils.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.7.2/PKG-INFO
```

### Comparing `fdk_rdf_parser-2.7.1/LICENSE` & `fdk_rdf_parser-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/pyproject.toml` & `fdk_rdf_parser-2.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fdk-rdf-parser"
-version = "2.7.1"
+version = "2.7.2"
 description = ""
 authors = ["NilsOveTen <nils.ove.tendenes@digdir.no>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 rdflib = "^7.0.0"
 isodate = "^0.6.1"
```

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/__init__.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/business_event.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/business_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/channel.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/concept.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/concept.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,10 +88,10 @@
     associativeRelation: Optional[List[AssociativeRelation]] = None
     partitiveRelation: Optional[List[PartitiveRelation]] = None
     genericRelation: Optional[List[GenericRelation]] = None
     created: Optional[str] = None
     exactMatch: Optional[Set[str]] = None
     closeMatch: Optional[Set[str]] = None
     memberOf: Optional[Set[str]] = None
-    remark: Optional[List[Dict[str, str]]] = None
+    remark: Optional[Dict[str, str]] = None
     range: Optional[List[TextAndURI]] = None
     type: str = "concept"  # used by elasticsearch for indexing
```

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/contactpoint.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/cpsvno_service.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dataservice.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dataset.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dcat_resource.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/distribution.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/event.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/evidence.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/info_model.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/life_event.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/life_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/model_element.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/model_property.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/public_service.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/public_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/theme.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/theme.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/fdk_rdf_parser.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/fdk_rdf_parser.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/__init__.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/address.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/address.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/agent.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/agent.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/catalog.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/catalog.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/channel.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/concept.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/concept.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,10 +419,10 @@
         associativeRelation=extract_associative_relations(graph, concept_uri),
         partitiveRelation=extract_partitive_relations(graph, concept_uri),
         genericRelation=extract_generic_relations(graph, concept_uri),
         created=date_value(graph, concept_uri, DCTERMS.created),
         exactMatch=value_set(graph, concept_uri, SKOS.exactMatch),
         closeMatch=value_set(graph, concept_uri, SKOS.closeMatch),
         memberOf=value_set(graph, concept_uri, uneskos_uri("memberOf")),
-        remark=extract_labels(graph, concept_uri, SKOS.scopeNote, SKOS.scopeNote),
+        remark=value_translations(graph, concept_uri, SKOS.scopeNote),
         range=extract_range(graph, concept_uri),
     )
```

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/conforms_to.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/conforms_to.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/contactpoint.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/cost.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/cost.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/cpsvno_service.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/data_distribution_service.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/data_distribution_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dataservice.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dataset.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dataset.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dcat_resource.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dct_standard.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dct_standard.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/distribution.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/event.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/evidence.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/format.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/format.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/info_model.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/legal_resource.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/legal_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/media_type.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/media_type.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/model_element.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/model_property.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/organization.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/organization.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/output.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/output.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/participation.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/participation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/publisher.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/publisher.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/qualified_attribution.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/qualified_attribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/quality_annotation.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/quality_annotation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/reference_data_code.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/reference_data_code.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/references.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/references.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/requirement.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/requirement.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/rule.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/rule.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/skos_concept.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/skos_concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/spatial.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/spatial.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/subject.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/subject.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/temporal.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/temporal.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/theme.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/theme.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/__init__.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/ns.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/ns.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/utils.py` & `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.1/PKG-INFO` & `fdk_rdf_parser-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdk-rdf-parser
-Version: 2.7.1
+Version: 2.7.2
 Summary: 
 Author: NilsOveTen
 Author-email: nils.ove.tendenes@digdir.no
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

